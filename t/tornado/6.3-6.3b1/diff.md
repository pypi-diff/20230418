# Comparing `tmp/tornado-6.3.tar.gz` & `tmp/tornado-6.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tornado-6.3.tar", last modified: Tue Apr 18 01:19:46 2023, max compression
+gzip compressed data, was "tornado-6.3b1.tar", last modified: Sun Apr  9 20:54:13 2023, max compression
```

## Comparing `tornado-6.3.tar` & `tornado-6.3b1.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 01:19:45.000000 tornado-6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 01:19:45.000000 tornado-6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-18 01:19:46.489099 tornado-6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-18 01:19:45.000000 tornado-6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/blog/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/README
--rwxr-xr-x   0 runner    (1001) docker     (123)    10383 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/blog/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/static/blog.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/blog/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/archive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/compose.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/create_author.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/entry.html
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/feed.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/blog/templates/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-18 01:19:45.000000 tornado-6.3/demos/blog/templates/modules/entry.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/chat/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4120 2023-04-18 01:19:45.000000 tornado-6.3/demos/chat/chatdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/chat/static/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-18 01:19:45.000000 tornado-6.3/demos/chat/static/chat.css
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 01:19:45.000000 tornado-6.3/demos/chat/static/chat.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/chat/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-18 01:19:45.000000 tornado-6.3/demos/chat/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 01:19:45.000000 tornado-6.3/demos/chat/templates/message.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/demos/facebook/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/README
--rwxr-xr-x   0 runner    (1001) docker     (123)     4146 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/facebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/facebook/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/static/facebook.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/static/facebook.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/facebook/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/facebook/templates/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/templates/modules/post.html
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-18 01:19:45.000000 tornado-6.3/demos/facebook/templates/stream.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/file_upload/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-04-18 01:19:45.000000 tornado-6.3/demos/file_upload/file_receiver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3429 2023-04-18 01:19:45.000000 tornado-6.3/demos/file_upload/file_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/helloworld/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-04-18 01:19:45.000000 tornado-6.3/demos/helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/s3server/
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-18 01:19:45.000000 tornado-6.3/demos/s3server/s3server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/tcpecho/
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-04-18 01:19:45.000000 tornado-6.3/demos/tcpecho/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-04-18 01:19:45.000000 tornado-6.3/demos/tcpecho/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-18 01:19:45.000000 tornado-6.3/demos/twitter/home.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-04-18 01:19:45.000000 tornado-6.3/demos/twitter/twitterdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/websocket/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3013 2023-04-18 01:19:45.000000 tornado-6.3/demos/websocket/chatdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/websocket/static/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-18 01:19:45.000000 tornado-6.3/demos/websocket/static/chat.css
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-18 01:19:45.000000 tornado-6.3/demos/websocket/static/chat.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/websocket/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 01:19:45.000000 tornado-6.3/demos/websocket/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 01:19:45.000000 tornado-6.3/demos/websocket/templates/message.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.469099 tornado-6.3/demos/webspider/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-04-18 01:19:45.000000 tornado-6.3/demos/webspider/webspider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.473099 tornado-6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-18 01:19:45.000000 tornado-6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 01:19:45.000000 tornado-6.3/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-18 01:19:45.000000 tornado-6.3/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-18 01:19:45.000000 tornado-6.3/docs/autoreload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-18 01:19:45.000000 tornado-6.3/docs/caresresolver.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-18 01:19:45.000000 tornado-6.3/docs/concurrent.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-18 01:19:45.000000 tornado-6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 01:19:45.000000 tornado-6.3/docs/coroutine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-18 01:19:45.000000 tornado-6.3/docs/escape.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-18 01:19:45.000000 tornado-6.3/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 01:19:45.000000 tornado-6.3/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-18 01:19:45.000000 tornado-6.3/docs/gen.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.473099 tornado-6.3/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/coroutines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/queues.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/security.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 01:19:45.000000 tornado-6.3/docs/guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 01:19:45.000000 tornado-6.3/docs/http.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 01:19:45.000000 tornado-6.3/docs/http1connection.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-18 01:19:45.000000 tornado-6.3/docs/httpclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 01:19:45.000000 tornado-6.3/docs/httpserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 01:19:45.000000 tornado-6.3/docs/httputil.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-18 01:19:45.000000 tornado-6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 01:19:45.000000 tornado-6.3/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 01:19:45.000000 tornado-6.3/docs/ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-18 01:19:45.000000 tornado-6.3/docs/iostream.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-18 01:19:45.000000 tornado-6.3/docs/locale.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-18 01:19:45.000000 tornado-6.3/docs/locks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-18 01:19:45.000000 tornado-6.3/docs/log.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-18 01:19:45.000000 tornado-6.3/docs/netutil.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 01:19:45.000000 tornado-6.3/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 01:19:45.000000 tornado-6.3/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 01:19:45.000000 tornado-6.3/docs/process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 01:19:45.000000 tornado-6.3/docs/queues.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.477099 tornado-6.3/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v1.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v2.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21093 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v3.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.5.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v4.5.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v5.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v5.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v5.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v5.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v5.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.0.4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases/v6.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 01:19:45.000000 tornado-6.3/docs/releases.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 01:19:45.000000 tornado-6.3/docs/routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 01:19:45.000000 tornado-6.3/docs/tcpclient.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 01:19:45.000000 tornado-6.3/docs/tcpserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-18 01:19:45.000000 tornado-6.3/docs/template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 01:19:45.000000 tornado-6.3/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-18 01:19:45.000000 tornado-6.3/docs/tornado.png
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-18 01:19:45.000000 tornado-6.3/docs/twisted.rst
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-18 01:19:45.000000 tornado-6.3/docs/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 01:19:45.000000 tornado-6.3/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-04-18 01:19:45.000000 tornado-6.3/docs/web.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 01:19:45.000000 tornado-6.3/docs/webframework.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 01:19:45.000000 tornado-6.3/docs/websocket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 01:19:45.000000 tornado-6.3/docs/wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 01:19:45.000000 tornado-6.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-04-18 01:19:45.000000 tornado-6.3/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 01:19:46.489099 tornado-6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-18 01:19:45.000000 tornado-6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.481099 tornado-6.3/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-18 01:19:45.000000 tornado-6.3/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-18 01:19:45.000000 tornado-6.3/tornado/_locale_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    46806 2023-04-18 01:19:45.000000 tornado-6.3/tornado/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-04-18 01:19:45.000000 tornado-6.3/tornado/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-18 01:19:45.000000 tornado-6.3/tornado/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24660 2023-04-18 01:19:45.000000 tornado-6.3/tornado/curl_httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-04-18 01:19:45.000000 tornado-6.3/tornado/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)    31447 2023-04-18 01:19:45.000000 tornado-6.3/tornado/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    36191 2023-04-18 01:19:45.000000 tornado-6.3/tornado/http1connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-04-18 01:19:45.000000 tornado-6.3/tornado/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-18 01:19:45.000000 tornado-6.3/tornado/httpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    36001 2023-04-18 01:19:45.000000 tornado-6.3/tornado/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35832 2023-04-18 01:19:45.000000 tornado-6.3/tornado/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    65497 2023-04-18 01:19:45.000000 tornado-6.3/tornado/iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-04-18 01:19:45.000000 tornado-6.3/tornado/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-18 01:19:45.000000 tornado-6.3/tornado/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-04-18 01:19:45.000000 tornado-6.3/tornado/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-04-18 01:19:45.000000 tornado-6.3/tornado/netutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    26254 2023-04-18 01:19:45.000000 tornado-6.3/tornado/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.481099 tornado-6.3/tornado/platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:45.000000 tornado-6.3/tornado/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25088 2023-04-18 01:19:45.000000 tornado-6.3/tornado/platform/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-18 01:19:45.000000 tornado-6.3/tornado/platform/caresresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-18 01:19:45.000000 tornado-6.3/tornado/platform/twisted.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-18 01:19:45.000000 tornado-6.3/tornado/process.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:45.000000 tornado-6.3/tornado/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-18 01:19:45.000000 tornado-6.3/tornado/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-04-18 01:19:45.000000 tornado-6.3/tornado/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-04-18 01:19:45.000000 tornado-6.3/tornado/simple_httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-18 01:19:45.000000 tornado-6.3/tornado/speedups.c
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-04-18 01:19:45.000000 tornado-6.3/tornado/tcpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-18 01:19:45.000000 tornado-6.3/tornado/tcpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-04-18 01:19:45.000000 tornado-6.3/tornado/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23418 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/autoreload_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/concurrent_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/csv_translations/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/csv_translations/fr_FR.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/curl_httpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/escape_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/gen_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/tornado/test/gettext_translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.465098 tornado-6.3/tornado/test/gettext_translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/http1connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/httpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    47084 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/httpserver_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/httputil_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27405 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/ioloop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    47311 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/iostream_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/locale_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/locks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/log_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/netutil_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/options_test.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/options_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/options_test_types.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/options_test_types_str.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/queues_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/resolve_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/routing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)    31109 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/simple_httpclient_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/static/dir/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static/dir/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static/sample.xml.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static/sample.xml.gz
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/static_foo.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/tcpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/tcpserver_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.489099 tornado-6.3/tornado/test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/templates/utf8.html
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/test.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/test.key
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/testing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/twisted_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   119034 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/web_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28703 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 01:19:45.000000 tornado-6.3/tornado/test/wsgi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33341 2023-04-18 01:19:45.000000 tornado-6.3/tornado/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-18 01:19:45.000000 tornado-6.3/tornado/util.py
--rw-r--r--   0 runner    (1001) docker     (123)   141587 2023-04-18 01:19:45.000000 tornado-6.3/tornado/web.py
--rw-r--r--   0 runner    (1001) docker     (123)    61175 2023-04-18 01:19:45.000000 tornado-6.3/tornado/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-18 01:19:45.000000 tornado-6.3/tornado/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:19:46.481099 tornado-6.3/tornado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-18 01:19:46.000000 tornado-6.3/tornado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-18 01:19:46.000000 tornado-6.3/tornado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:19:46.000000 tornado-6.3/tornado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 01:19:46.000000 tornado-6.3/tornado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-09 20:54:12.000000 tornado-6.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-09 20:54:12.000000 tornado-6.3b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-09 20:54:13.769427 tornado-6.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-04-09 20:54:12.000000 tornado-6.3b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/demos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/README
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10383 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/blog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/static/blog.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/archive.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/compose.html
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/create_author.html
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/entry.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/feed.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/templates/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/modules/entry.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4120 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/chatdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/static/chat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/static/chat.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/templates/message.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/README
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4146 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/facebook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/static/facebook.css
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/static/facebook.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/templates/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/templates/modules/post.html
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/templates/stream.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/file_upload/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1562 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/file_upload/file_receiver.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3429 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/file_upload/file_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/helloworld/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1155 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/s3server/
+-rw-r--r--   0 runner    (1001) docker     (122)    10014 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/s3server/s3server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/tcpecho/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      696 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/tcpecho/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1118 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/tcpecho/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/twitter/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/twitter/home.html
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3477 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/twitter/twitterdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3013 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/chatdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/static/chat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/static/chat.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/templates/message.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/webspider/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2705 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/webspider/webspider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.745426 tornado-6.3b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/autoreload.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/caresresolver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/concurrent.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4119 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/coroutine.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/escape.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/gen.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.745426 tornado-6.3b1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/coroutines.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/queues.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10932 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/running.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12712 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/security.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14248 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12553 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/http.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/http1connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httpclient.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httpserver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httputil.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/iostream.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/locale.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/locks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/log.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/netutil.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/process.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/queues.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.753426 tornado-6.3b1/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7576 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2885 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    21093 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10631 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14923 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8800 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6985 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7147 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7840 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4223 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tcpclient.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tcpserver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7101 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tornado.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/twisted.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/util.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/web.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/webframework.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/websocket.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-09 20:54:12.000000 tornado-6.3b1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      511 2023-04-09 20:54:12.000000 tornado-6.3b1/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-09 20:54:13.769427 tornado-6.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-04-09 20:54:12.000000 tornado-6.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.753426 tornado-6.3b1/tornado/
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4503 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/_locale_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46806 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13585 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24660 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/curl_httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13266 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/escape.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31447 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36191 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/http1connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31919 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16126 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36001 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35832 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65497 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/iostream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20890 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/locale.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17356 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/locks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25303 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/netutil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26254 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.757426 tornado-6.3b1/tornado/platform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25088 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/caresresolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12789 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/queues.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25082 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27796 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/simple_httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (122)    12152 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/tcpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15022 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/tcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37793 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8345 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23418 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/autoreload_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6049 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/concurrent_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/csv_translations/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/csv_translations/fr_FR.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/curl_httpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12295 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/escape_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34093 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gen_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/tornado/test/gettext_translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1964 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/http1connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34788 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47084 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httpserver_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19045 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httputil_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/ioloop_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47311 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/iostream_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/locale_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17010 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/locks_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9473 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8334 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/netutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11932 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test_types.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test_types_str.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13981 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/queues_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/resolve_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8827 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/routing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8348 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31109 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/simple_httpclient_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/static/dir/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/dir/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml.bz2
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml.gz
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    16847 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/tcpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7720 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/tcpserver_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18657 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/templates/utf8.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/test.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/test.key
+-rw-r--r--   0 runner    (1001) docker     (122)    10317 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/testing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/twisted_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)   119034 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/web_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28703 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3918 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/wsgi_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33341 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16249 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)   141587 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/web.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61175 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10817 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.757426 tornado-6.3b1/tornado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/top_level.txt
```

### Comparing `tornado-6.3/LICENSE` & `tornado-6.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tornado-6.3/MANIFEST.in` & `tornado-6.3b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tornado-6.3/PKG-INFO` & `tornado-6.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tornado
-Version: 6.3
+Version: 6.3b1
 Summary: Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed.
 Home-page: http://www.tornadoweb.org/
 Author: Facebook
 Author-email: python-tornado@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/tornadoweb/tornado
 Platform: UNKNOWN
```

### Comparing `tornado-6.3/README.rst` & `tornado-6.3b1/README.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/README` & `tornado-6.3b1/demos/blog/README`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/blog.py` & `tornado-6.3b1/demos/blog/blog.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/schema.sql` & `tornado-6.3b1/demos/blog/schema.sql`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/static/blog.css` & `tornado-6.3b1/demos/blog/static/blog.css`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/templates/archive.html` & `tornado-6.3b1/demos/blog/templates/archive.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/templates/base.html` & `tornado-6.3b1/demos/blog/templates/base.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/templates/compose.html` & `tornado-6.3b1/demos/blog/templates/compose.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/blog/templates/feed.xml` & `tornado-6.3b1/demos/blog/templates/feed.xml`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/chat/chatdemo.py` & `tornado-6.3b1/demos/chat/chatdemo.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/chat/static/chat.css` & `tornado-6.3b1/demos/chat/static/chat.css`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/chat/static/chat.js` & `tornado-6.3b1/demos/chat/static/chat.js`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/chat/templates/index.html` & `tornado-6.3b1/demos/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/facebook/facebook.py` & `tornado-6.3b1/demos/facebook/facebook.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/facebook/static/facebook.css` & `tornado-6.3b1/demos/facebook/static/facebook.css`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/facebook/templates/modules/post.html` & `tornado-6.3b1/demos/facebook/templates/modules/post.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/facebook/templates/stream.html` & `tornado-6.3b1/demos/facebook/templates/stream.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/file_upload/file_receiver.py` & `tornado-6.3b1/demos/file_upload/file_receiver.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/file_upload/file_uploader.py` & `tornado-6.3b1/demos/file_upload/file_uploader.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/helloworld/helloworld.py` & `tornado-6.3b1/demos/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/s3server/s3server.py` & `tornado-6.3b1/demos/s3server/s3server.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/tcpecho/client.py` & `tornado-6.3b1/demos/tcpecho/client.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/tcpecho/server.py` & `tornado-6.3b1/demos/tcpecho/server.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/twitter/twitterdemo.py` & `tornado-6.3b1/demos/twitter/twitterdemo.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/websocket/chatdemo.py` & `tornado-6.3b1/demos/websocket/chatdemo.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/websocket/static/chat.css` & `tornado-6.3b1/demos/websocket/static/chat.css`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/websocket/static/chat.js` & `tornado-6.3b1/demos/websocket/static/chat.js`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/websocket/templates/index.html` & `tornado-6.3b1/demos/websocket/templates/index.html`

 * *Files identical despite different names*

### Comparing `tornado-6.3/demos/webspider/webspider.py` & `tornado-6.3b1/demos/webspider/webspider.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/Makefile` & `tornado-6.3b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/auth.rst` & `tornado-6.3b1/docs/auth.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/caresresolver.rst` & `tornado-6.3b1/docs/caresresolver.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/concurrent.rst` & `tornado-6.3b1/docs/concurrent.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/conf.py` & `tornado-6.3b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/escape.rst` & `tornado-6.3b1/docs/escape.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/faq.rst` & `tornado-6.3b1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/favicon.ico` & `tornado-6.3b1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/gen.rst` & `tornado-6.3b1/docs/gen.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/async.rst` & `tornado-6.3b1/docs/guide/async.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/coroutines.rst` & `tornado-6.3b1/docs/guide/coroutines.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/intro.rst` & `tornado-6.3b1/docs/guide/intro.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/queues.rst` & `tornado-6.3b1/docs/guide/queues.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/running.rst` & `tornado-6.3b1/docs/guide/running.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/security.rst` & `tornado-6.3b1/docs/guide/security.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/structure.rst` & `tornado-6.3b1/docs/guide/structure.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/guide/templates.rst` & `tornado-6.3b1/docs/guide/templates.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/httpclient.rst` & `tornado-6.3b1/docs/httpclient.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/httpserver.rst` & `tornado-6.3b1/docs/httpserver.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/index.rst` & `tornado-6.3b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/ioloop.rst` & `tornado-6.3b1/docs/ioloop.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/iostream.rst` & `tornado-6.3b1/docs/iostream.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/locks.rst` & `tornado-6.3b1/docs/locks.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/options.rst` & `tornado-6.3b1/docs/options.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/queues.rst` & `tornado-6.3b1/docs/queues.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v1.0.0.rst` & `tornado-6.3b1/docs/releases/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v1.1.0.rst` & `tornado-6.3b1/docs/releases/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v1.1.1.rst` & `tornado-6.3b1/docs/releases/v1.1.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v1.2.0.rst` & `tornado-6.3b1/docs/releases/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v1.2.1.rst` & `tornado-6.3b1/docs/releases/v1.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.0.0.rst` & `tornado-6.3b1/docs/releases/v2.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.1.0.rst` & `tornado-6.3b1/docs/releases/v2.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.1.1.rst` & `tornado-6.3b1/docs/releases/v2.1.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.2.0.rst` & `tornado-6.3b1/docs/releases/v2.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.2.1.rst` & `tornado-6.3b1/docs/releases/v2.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.3.0.rst` & `tornado-6.3b1/docs/releases/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v2.4.0.rst` & `tornado-6.3b1/docs/releases/v2.4.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.0.0.rst` & `tornado-6.3b1/docs/releases/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.0.1.rst` & `tornado-6.3b1/docs/releases/v3.0.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.1.0.rst` & `tornado-6.3b1/docs/releases/v3.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.2.0.rst` & `tornado-6.3b1/docs/releases/v3.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.2.1.rst` & `tornado-6.3b1/docs/releases/v3.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v3.2.2.rst` & `tornado-6.3b1/docs/releases/v3.2.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.0.0.rst` & `tornado-6.3b1/docs/releases/v4.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.0.1.rst` & `tornado-6.3b1/docs/releases/v4.0.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.0.2.rst` & `tornado-6.3b1/docs/releases/v4.0.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.1.0.rst` & `tornado-6.3b1/docs/releases/v4.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.2.0.rst` & `tornado-6.3b1/docs/releases/v4.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.3.0.rst` & `tornado-6.3b1/docs/releases/v4.3.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.4.0.rst` & `tornado-6.3b1/docs/releases/v4.4.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.4.2.rst` & `tornado-6.3b1/docs/releases/v4.4.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.5.0.rst` & `tornado-6.3b1/docs/releases/v4.5.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v4.5.3.rst` & `tornado-6.3b1/docs/releases/v4.5.3.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v5.0.0.rst` & `tornado-6.3b1/docs/releases/v5.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v5.0.2.rst` & `tornado-6.3b1/docs/releases/v5.0.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v5.1.0.rst` & `tornado-6.3b1/docs/releases/v5.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v6.0.0.rst` & `tornado-6.3b1/docs/releases/v6.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v6.0.4.rst` & `tornado-6.3b1/docs/releases/v6.0.4.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v6.1.0.rst` & `tornado-6.3b1/docs/releases/v6.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v6.2.0.rst` & `tornado-6.3b1/docs/releases/v6.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/releases/v6.3.0.rst` & `tornado-6.3b1/docs/releases/v6.3.0.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 What's new in Tornado 6.3.0
 ===========================
 
-Apr 17, 2023
-------------
+In progress
+-----------
 
 Highlights
 ~~~~~~~~~~
 
 - The new `.Application` setting ``xsrf_cookie_name`` can now be used to
   take advantage of the ``__Host`` cookie prefix for improved security.
   To use it, add ``{"xsrf_cookie_name": "__Host-xsrf", "xsrf_cookie_kwargs":
```

### Comparing `tornado-6.3/docs/releases.rst` & `tornado-6.3b1/docs/releases.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/template.rst` & `tornado-6.3b1/docs/template.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/testing.rst` & `tornado-6.3b1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/tornado.png` & `tornado-6.3b1/docs/tornado.png`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/twisted.rst` & `tornado-6.3b1/docs/twisted.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/util.rst` & `tornado-6.3b1/docs/util.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/web.rst` & `tornado-6.3b1/docs/web.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/docs/websocket.rst` & `tornado-6.3b1/docs/websocket.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.3/pyproject.toml` & `tornado-6.3b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.cibuildwheel]
-build = "cp3[89]* cp310* cp311* cp312*"
+build = "cp3[89]* cp310* cp311*"
 test-command = "python -m tornado.test"
 
 [tool.cibuildwheel.macos]
 archs = "x86_64 universal2"
 # The arm portion of a universal wheel is a cross-compile and cannot
 # be tested on an x86 host. This must be configured explicitly to silence
 # a warning.
```

### Comparing `tornado-6.3/setup.py` & `tornado-6.3b1/setup.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/__init__.py` & `tornado-6.3b1/tornado/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number.  The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-version = "6.3"
-version_info = (6, 3, 0, 0)
+version = "6.3b1"
+version_info = (6, 3, 0, -99)
 
 import importlib
 import typing
 
 __all__ = [
     "auth",
     "autoreload",
```

### Comparing `tornado-6.3/tornado/_locale_data.py` & `tornado-6.3b1/tornado/_locale_data.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/auth.py` & `tornado-6.3b1/tornado/auth.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/autoreload.py` & `tornado-6.3b1/tornado/autoreload.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/concurrent.py` & `tornado-6.3b1/tornado/concurrent.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/curl_httpclient.py` & `tornado-6.3b1/tornado/curl_httpclient.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/escape.py` & `tornado-6.3b1/tornado/escape.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/gen.py` & `tornado-6.3b1/tornado/gen.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/http1connection.py` & `tornado-6.3b1/tornado/http1connection.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/httpclient.py` & `tornado-6.3b1/tornado/httpclient.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/httpserver.py` & `tornado-6.3b1/tornado/httpserver.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/httputil.py` & `tornado-6.3b1/tornado/httputil.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/ioloop.py` & `tornado-6.3b1/tornado/ioloop.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/iostream.py` & `tornado-6.3b1/tornado/iostream.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/locale.py` & `tornado-6.3b1/tornado/locale.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/locks.py` & `tornado-6.3b1/tornado/locks.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/log.py` & `tornado-6.3b1/tornado/log.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/netutil.py` & `tornado-6.3b1/tornado/netutil.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/options.py` & `tornado-6.3b1/tornado/options.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/platform/asyncio.py` & `tornado-6.3b1/tornado/platform/asyncio.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/platform/caresresolver.py` & `tornado-6.3b1/tornado/platform/caresresolver.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/platform/twisted.py` & `tornado-6.3b1/tornado/platform/twisted.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/process.py` & `tornado-6.3b1/tornado/process.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/queues.py` & `tornado-6.3b1/tornado/queues.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/routing.py` & `tornado-6.3b1/tornado/routing.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/simple_httpclient.py` & `tornado-6.3b1/tornado/simple_httpclient.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/speedups.c` & `tornado-6.3b1/tornado/speedups.c`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/tcpclient.py` & `tornado-6.3b1/tornado/tcpclient.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/tcpserver.py` & `tornado-6.3b1/tornado/tcpserver.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/template.py` & `tornado-6.3b1/tornado/template.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/asyncio_test.py` & `tornado-6.3b1/tornado/test/asyncio_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/auth_test.py` & `tornado-6.3b1/tornado/test/auth_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/autoreload_test.py` & `tornado-6.3b1/tornado/test/autoreload_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/concurrent_test.py` & `tornado-6.3b1/tornado/test/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/curl_httpclient_test.py` & `tornado-6.3b1/tornado/test/curl_httpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/escape_test.py` & `tornado-6.3b1/tornado/test/escape_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/gen_test.py` & `tornado-6.3b1/tornado/test/gen_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo` & `tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po` & `tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/http1connection_test.py` & `tornado-6.3b1/tornado/test/http1connection_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/httpclient_test.py` & `tornado-6.3b1/tornado/test/httpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/httpserver_test.py` & `tornado-6.3b1/tornado/test/httpserver_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/httputil_test.py` & `tornado-6.3b1/tornado/test/httputil_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/import_test.py` & `tornado-6.3b1/tornado/test/import_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/ioloop_test.py` & `tornado-6.3b1/tornado/test/ioloop_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/iostream_test.py` & `tornado-6.3b1/tornado/test/iostream_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/locale_test.py` & `tornado-6.3b1/tornado/test/locale_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/locks_test.py` & `tornado-6.3b1/tornado/test/locks_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/log_test.py` & `tornado-6.3b1/tornado/test/log_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/netutil_test.py` & `tornado-6.3b1/tornado/test/netutil_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/options_test.py` & `tornado-6.3b1/tornado/test/options_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/process_test.py` & `tornado-6.3b1/tornado/test/process_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/queues_test.py` & `tornado-6.3b1/tornado/test/queues_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/routing_test.py` & `tornado-6.3b1/tornado/test/routing_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/runtests.py` & `tornado-6.3b1/tornado/test/runtests.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/simple_httpclient_test.py` & `tornado-6.3b1/tornado/test/simple_httpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/static/sample.xml` & `tornado-6.3b1/tornado/test/static/sample.xml`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/tcpclient_test.py` & `tornado-6.3b1/tornado/test/tcpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/tcpserver_test.py` & `tornado-6.3b1/tornado/test/tcpserver_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/template_test.py` & `tornado-6.3b1/tornado/test/template_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/test.crt` & `tornado-6.3b1/tornado/test/test.crt`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/test.key` & `tornado-6.3b1/tornado/test/test.key`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/testing_test.py` & `tornado-6.3b1/tornado/test/testing_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/twisted_test.py` & `tornado-6.3b1/tornado/test/twisted_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/util.py` & `tornado-6.3b1/tornado/test/util.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/util_test.py` & `tornado-6.3b1/tornado/test/util_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/web_test.py` & `tornado-6.3b1/tornado/test/web_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/websocket_test.py` & `tornado-6.3b1/tornado/test/websocket_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/test/wsgi_test.py` & `tornado-6.3b1/tornado/test/wsgi_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/testing.py` & `tornado-6.3b1/tornado/testing.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/util.py` & `tornado-6.3b1/tornado/util.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/web.py` & `tornado-6.3b1/tornado/web.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/websocket.py` & `tornado-6.3b1/tornado/websocket.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado/wsgi.py` & `tornado-6.3b1/tornado/wsgi.py`

 * *Files identical despite different names*

### Comparing `tornado-6.3/tornado.egg-info/PKG-INFO` & `tornado-6.3b1/tornado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tornado
-Version: 6.3
+Version: 6.3b1
 Summary: Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed.
 Home-page: http://www.tornadoweb.org/
 Author: Facebook
 Author-email: python-tornado@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/tornadoweb/tornado
 Platform: UNKNOWN
```

### Comparing `tornado-6.3/tornado.egg-info/SOURCES.txt` & `tornado-6.3b1/tornado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

