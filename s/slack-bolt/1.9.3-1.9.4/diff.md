# Comparing `tmp/slack_bolt-1.9.3.tar.gz` & `tmp/slack_bolt-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_bolt-1.9.3.tar", last modified: Wed Oct 13 08:19:40 2021, max compression
+gzip compressed data, was "slack_bolt-1.9.4.tar", last modified: Fri Oct 29 15:13:36 2021, max compression
```

## Comparing `slack_bolt-1.9.3.tar` & `slack_bolt-1.9.4.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.770007 slack_bolt-1.9.3/
--rw-r--r--   0 ksera      (502) staff       (20)     1091 2021-08-26 02:24:29.000000 slack_bolt-1.9.3/LICENSE
--rw-r--r--   0 ksera      (502) staff       (20)       45 2020-08-06 04:03:27.000000 slack_bolt-1.9.3/MANIFEST.in
--rw-r--r--   0 ksera      (502) staff       (20)    10102 2021-10-13 08:19:40.770368 slack_bolt-1.9.3/PKG-INFO
--rw-r--r--   0 ksera      (502) staff       (20)     9332 2021-07-02 01:23:16.000000 slack_bolt-1.9.3/README.md
--rw-r--r--   0 ksera      (502) staff       (20)       92 2021-10-13 08:19:40.771707 slack_bolt-1.9.3/setup.cfg
--rwxr-xr-x   0 ksera      (502) staff       (20)     3115 2021-09-28 06:08:51.000000 slack_bolt-1.9.3/setup.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.589230 slack_bolt-1.9.3/slack_bolt/
--rw-r--r--   0 ksera      (502) staff       (20)      928 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.593763 slack_bolt-1.9.3/slack_bolt/adapter/
--rw-r--r--   0 ksera      (502) staff       (20)       87 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/adapter/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.594801 slack_bolt-1.9.3/slack_bolt/adapter/aiohttp/
--rw-r--r--   0 ksera      (502) staff       (20)     1255 2021-01-27 04:33:11.000000 slack_bolt-1.9.3/slack_bolt/adapter/aiohttp/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.601867 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     4317 2021-05-02 07:22:32.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/chalice_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     1530 2021-05-02 07:22:32.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/chalice_lazy_listener_runner.py
--rw-r--r--   0 ksera      (502) staff       (20)     4143 2021-08-28 00:49:30.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/handler.py
--rw-r--r--   0 ksera      (502) staff       (20)      260 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     3232 2021-07-15 23:00:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/lambda_s3_oauth_flow.py
--rw-r--r--   0 ksera      (502) staff       (20)     1116 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/lazy_listener_runner.py
--rw-r--r--   0 ksera      (502) staff       (20)      940 2021-08-07 13:23:58.000000 slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/local_lambda_client.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.608113 slack_bolt-1.9.3/slack_bolt/adapter/bottle/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/bottle/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1696 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/bottle/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.610198 slack_bolt-1.9.3/slack_bolt/adapter/cherrypy/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/cherrypy/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     3207 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/cherrypy/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.612067 slack_bolt-1.9.3/slack_bolt/adapter/django/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/django/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     5981 2021-04-10 01:18:37.000000 slack_bolt-1.9.3/slack_bolt/adapter/django/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.613808 slack_bolt-1.9.3/slack_bolt/adapter/falcon/
--rw-r--r--   0 ksera      (502) staff       (20)       39 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/falcon/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2623 2021-03-19 04:59:22.000000 slack_bolt-1.9.3/slack_bolt/adapter/falcon/resource.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.615538 slack_bolt-1.9.3/slack_bolt/adapter/fastapi/
--rw-r--r--   0 ksera      (502) staff       (20)       98 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/fastapi/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)       71 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/fastapi/async_handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.617407 slack_bolt-1.9.3/slack_bolt/adapter/flask/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/flask/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1617 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/flask/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.618958 slack_bolt-1.9.3/slack_bolt/adapter/pyramid/
--rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/pyramid/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1901 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/pyramid/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.620586 slack_bolt-1.9.3/slack_bolt/adapter/sanic/
--rw-r--r--   0 ksera      (502) staff       (20)       52 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/sanic/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2511 2021-08-10 12:00:46.000000 slack_bolt-1.9.3/slack_bolt/adapter/sanic/async_handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.625187 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/
--rw-r--r--   0 ksera      (502) staff       (20)      470 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.625847 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/aiohttp/
--rw-r--r--   0 ksera      (502) staff       (20)     3372 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/aiohttp/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1803 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/async_base_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)      107 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/async_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     1966 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/async_internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     1908 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/base_handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.626532 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/builtin/
--rw-r--r--   0 ksera      (502) staff       (20)     3280 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/builtin/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1827 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/internals.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.627138 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websocket_client/
--rw-r--r--   0 ksera      (502) staff       (20)     2777 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websocket_client/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.627755 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websockets/
--rw-r--r--   0 ksera      (502) staff       (20)     3467 2021-03-29 09:01:39.000000 slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websockets/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.629623 slack_bolt-1.9.3/slack_bolt/adapter/starlette/
--rw-r--r--   0 ksera      (502) staff       (20)       79 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/starlette/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2242 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/starlette/async_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     2059 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/starlette/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.630844 slack_bolt-1.9.3/slack_bolt/adapter/tornado/
--rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/adapter/tornado/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2369 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/adapter/tornado/handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.635136 slack_bolt-1.9.3/slack_bolt/app/
--rw-r--r--   0 ksera      (502) staff       (20)      319 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/app/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)    62858 2021-10-13 08:18:52.000000 slack_bolt-1.9.3/slack_bolt/app/app.py
--rw-r--r--   0 ksera      (502) staff       (20)    60999 2021-10-13 08:18:52.000000 slack_bolt-1.9.3/slack_bolt/app/async_app.py
--rw-r--r--   0 ksera      (502) staff       (20)     3016 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/app/async_server.py
--rw-r--r--   0 ksera      (502) staff       (20)     2312 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/async_app.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.640405 slack_bolt-1.9.3/slack_bolt/authorization/
--rw-r--r--   0 ksera      (502) staff       (20)      259 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/authorization/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)    12109 2021-09-28 06:08:03.000000 slack_bolt-1.9.3/slack_bolt/authorization/async_authorize.py
--rw-r--r--   0 ksera      (502) staff       (20)     1091 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/authorization/async_authorize_args.py
--rw-r--r--   0 ksera      (502) staff       (20)    11608 2021-09-28 06:08:03.000000 slack_bolt-1.9.3/slack_bolt/authorization/authorize.py
--rw-r--r--   0 ksera      (502) staff       (20)     1042 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/authorization/authorize_args.py
--rw-r--r--   0 ksera      (502) staff       (20)     2530 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/authorization/authorize_result.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.643265 slack_bolt-1.9.3/slack_bolt/context/
--rw-r--r--   0 ksera      (502) staff       (20)      406 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/context/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.646941 slack_bolt-1.9.3/slack_bolt/context/ack/
--rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/context/ack/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1717 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/ack/ack.py
--rw-r--r--   0 ksera      (502) staff       (20)     1728 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/ack/async_ack.py
--rw-r--r--   0 ksera      (502) staff       (20)     4753 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/ack/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     3175 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/context/async_context.py
--rw-r--r--   0 ksera      (502) staff       (20)     3144 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/context/base_context.py
--rw-r--r--   0 ksera      (502) staff       (20)     2949 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/context/context.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.650188 slack_bolt-1.9.3/slack_bolt/context/respond/
--rw-r--r--   0 ksera      (502) staff       (20)       67 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/context/respond/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2049 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/respond/async_respond.py
--rw-r--r--   0 ksera      (502) staff       (20)     1310 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/respond/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     2051 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/respond/respond.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.653332 slack_bolt-1.9.3/slack_bolt/context/say/
--rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/context/say/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2144 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/say/async_say.py
--rw-r--r--   0 ksera      (502) staff       (20)      229 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/context/say/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     2059 2021-06-03 07:52:16.000000 slack_bolt-1.9.3/slack_bolt/context/say/say.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.654198 slack_bolt-1.9.3/slack_bolt/error/
--rw-r--r--   0 ksera      (502) staff       (20)      834 2021-04-20 05:51:01.000000 slack_bolt-1.9.3/slack_bolt/error/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.658457 slack_bolt-1.9.3/slack_bolt/kwargs_injection/
--rw-r--r--   0 ksera      (502) staff       (20)      397 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/kwargs_injection/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     4782 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/kwargs_injection/args.py
--rw-r--r--   0 ksera      (502) staff       (20)     4880 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/kwargs_injection/async_args.py
--rw-r--r--   0 ksera      (502) staff       (20)     3822 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/kwargs_injection/async_utils.py
--rw-r--r--   0 ksera      (502) staff       (20)     3777 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/kwargs_injection/utils.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.664368 slack_bolt-1.9.3/slack_bolt/lazy_listener/
--rw-r--r--   0 ksera      (502) staff       (20)      985 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      994 2021-01-27 04:33:11.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/async_internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     1242 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/async_runner.py
--rw-r--r--   0 ksera      (502) staff       (20)      775 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/asyncio_runner.py
--rw-r--r--   0 ksera      (502) staff       (20)      888 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     1068 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/runner.py
--rw-r--r--   0 ksera      (502) staff       (20)      774 2021-08-30 08:32:04.000000 slack_bolt-1.9.3/slack_bolt/lazy_listener/thread_runner.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.674323 slack_bolt-1.9.3/slack_bolt/listener/
--rw-r--r--   0 ksera      (502) staff       (20)      495 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/listener/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1412 2021-04-16 05:22:52.000000 slack_bolt-1.9.3/slack_bolt/listener/async_builtins.py
--rw-r--r--   0 ksera      (502) staff       (20)     4415 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/listener/async_listener.py
--rw-r--r--   0 ksera      (502) staff       (20)     1717 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/listener/async_listener_completion_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     2218 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/listener/async_listener_error_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     8420 2021-04-10 01:18:37.000000 slack_bolt-1.9.3/slack_bolt/listener/asyncio_runner.py
--rw-r--r--   0 ksera      (502) staff       (20)     1341 2021-04-16 05:22:52.000000 slack_bolt-1.9.3/slack_bolt/listener/builtins.py
--rw-r--r--   0 ksera      (502) staff       (20)     1898 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/listener/custom_listener.py
--rw-r--r--   0 ksera      (502) staff       (20)     2072 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/listener/listener.py
--rw-r--r--   0 ksera      (502) staff       (20)     1556 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/listener/listener_completion_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     2084 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/listener/listener_error_handler.py
--rw-r--r--   0 ksera      (502) staff       (20)     8409 2021-08-30 08:32:04.000000 slack_bolt-1.9.3/slack_bolt/listener/thread_runner.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.680207 slack_bolt-1.9.3/slack_bolt/listener_matcher/
--rw-r--r--   0 ksera      (502) staff       (20)      564 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      752 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/async_builtins.py
--rw-r--r--   0 ksera      (502) staff       (20)     1841 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/async_listener_matcher.py
--rw-r--r--   0 ksera      (502) staff       (20)    16177 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/builtins.py
--rw-r--r--   0 ksera      (502) staff       (20)     1067 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/custom_listener_matcher.py
--rw-r--r--   0 ksera      (502) staff       (20)      500 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/listener_matcher/listener_matcher.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.683813 slack_bolt-1.9.3/slack_bolt/logger/
--rw-r--r--   0 ksera      (502) staff       (20)      790 2021-07-21 07:57:05.000000 slack_bolt-1.9.3/slack_bolt/logger/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)    11806 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/logger/messages.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.690723 slack_bolt-1.9.3/slack_bolt/middleware/
--rw-r--r--   0 ksera      (502) staff       (20)      905 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/middleware/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      462 2020-09-21 06:30:41.000000 slack_bolt-1.9.3/slack_bolt/middleware/async_builtins.py
--rw-r--r--   0 ksera      (502) staff       (20)     1813 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/async_custom_middleware.py
--rw-r--r--   0 ksera      (502) staff       (20)     1822 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/async_middleware.py
--rw-r--r--   0 ksera      (502) staff       (20)     2232 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/middleware/async_middleware_error_handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.699109 slack_bolt-1.9.3/slack_bolt/middleware/authorization/
--rw-r--r--   0 ksera      (502) staff       (20)      205 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      147 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)      790 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     3160 2021-09-28 06:08:03.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_multi_teams_authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)     2512 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_single_team_authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)       80 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)     2668 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     2876 2021-09-28 06:08:03.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/multi_teams_authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)     2462 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/authorization/single_team_authorization.py
--rw-r--r--   0 ksera      (502) staff       (20)     1518 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/custom_middleware.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.701518 slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/
--rw-r--r--   0 ksera      (502) staff       (20)       61 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      780 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/async_ignoring_self_events.py
--rw-r--r--   0 ksera      (502) staff       (20)     1821 2021-03-19 04:59:22.000000 slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/ignoring_self_events.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.704158 slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/
--rw-r--r--   0 ksera      (502) staff       (20)       69 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1294 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/async_message_listener_matches.py
--rw-r--r--   0 ksera      (502) staff       (20)     1225 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/message_listener_matches.py
--rw-r--r--   0 ksera      (502) staff       (20)     1729 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/middleware.py
--rw-r--r--   0 ksera      (502) staff       (20)     2106 2021-07-14 12:23:14.000000 slack_bolt-1.9.3/slack_bolt/middleware/middleware_error_handler.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.706366 slack_bolt-1.9.3/slack_bolt/middleware/request_verification/
--rw-r--r--   0 ksera      (502) staff       (20)       62 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/request_verification/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1418 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/request_verification/async_request_verification.py
--rw-r--r--   0 ksera      (502) staff       (20)     2249 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/request_verification/request_verification.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.710396 slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/
--rw-r--r--   0 ksera      (502) staff       (20)       40 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      918 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/async_ssl_check.py
--rw-r--r--   0 ksera      (502) staff       (20)     2067 2021-08-07 13:23:58.000000 slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/ssl_check.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.713187 slack_bolt-1.9.3/slack_bolt/middleware/url_verification/
--rw-r--r--   0 ksera      (502) staff       (20)       54 2020-09-04 11:56:35.000000 slack_bolt-1.9.3/slack_bolt/middleware/url_verification/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      804 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/middleware/url_verification/async_url_verification.py
--rw-r--r--   0 ksera      (502) staff       (20)     1347 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/middleware/url_verification/url_verification.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.726242 slack_bolt-1.9.3/slack_bolt/oauth/
--rw-r--r--   0 ksera      (502) staff       (20)      255 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/oauth/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     3818 2021-05-02 07:22:32.000000 slack_bolt-1.9.3/slack_bolt/oauth/async_callback_options.py
--rw-r--r--   0 ksera      (502) staff       (20)     1582 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/oauth/async_internals.py
--rw-r--r--   0 ksera      (502) staff       (20)    15456 2021-09-27 00:38:01.000000 slack_bolt-1.9.3/slack_bolt/oauth/async_oauth_flow.py
--rw-r--r--   0 ksera      (502) staff       (20)     9070 2021-09-21 07:19:22.000000 slack_bolt-1.9.3/slack_bolt/oauth/async_oauth_settings.py
--rw-r--r--   0 ksera      (502) staff       (20)     3639 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/oauth/callback_options.py
--rw-r--r--   0 ksera      (502) staff       (20)     5334 2021-09-28 06:08:03.000000 slack_bolt-1.9.3/slack_bolt/oauth/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)    14793 2021-09-27 00:38:05.000000 slack_bolt-1.9.3/slack_bolt/oauth/oauth_flow.py
--rw-r--r--   0 ksera      (502) staff       (20)     8795 2021-09-21 07:19:00.000000 slack_bolt-1.9.3/slack_bolt/oauth/oauth_settings.py
--rw-r--r--   0 ksera      (502) staff       (20)        0 2020-08-06 04:03:28.000000 slack_bolt-1.9.3/slack_bolt/py.typed
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.735065 slack_bolt-1.9.3/slack_bolt/request/
--rw-r--r--   0 ksera      (502) staff       (20)      304 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/request/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1307 2021-04-16 05:22:52.000000 slack_bolt-1.9.3/slack_bolt/request/async_internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     2771 2021-05-12 03:16:25.000000 slack_bolt-1.9.3/slack_bolt/request/async_request.py
--rw-r--r--   0 ksera      (502) staff       (20)     7181 2021-05-12 03:16:25.000000 slack_bolt-1.9.3/slack_bolt/request/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)     5608 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/request/payload_utils.py
--rw-r--r--   0 ksera      (502) staff       (20)     2668 2021-05-12 03:16:25.000000 slack_bolt-1.9.3/slack_bolt/request/request.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.737932 slack_bolt-1.9.3/slack_bolt/response/
--rw-r--r--   0 ksera      (502) staff       (20)      344 2021-03-26 08:32:05.000000 slack_bolt-1.9.3/slack_bolt/response/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     2061 2021-09-07 08:54:21.000000 slack_bolt-1.9.3/slack_bolt/response/response.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.742790 slack_bolt-1.9.3/slack_bolt/util/
--rw-r--r--   0 ksera      (502) staff       (20)       49 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/util/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)      420 2021-03-19 04:57:51.000000 slack_bolt-1.9.3/slack_bolt/util/async_utils.py
--rw-r--r--   0 ksera      (502) staff       (20)     3061 2021-05-02 07:22:32.000000 slack_bolt-1.9.3/slack_bolt/util/utils.py
--rw-r--r--   0 ksera      (502) staff       (20)       93 2021-10-13 08:19:04.000000 slack_bolt-1.9.3/slack_bolt/version.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.744522 slack_bolt-1.9.3/slack_bolt/workflows/
--rw-r--r--   0 ksera      (502) staff       (20)      351 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/__init__.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.755368 slack_bolt-1.9.3/slack_bolt/workflows/step/
--rw-r--r--   0 ksera      (502) staff       (20)      237 2020-10-01 04:13:34.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)    16210 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/async_step.py
--rw-r--r--   0 ksera      (502) staff       (20)     2109 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/async_step_middleware.py
--rw-r--r--   0 ksera      (502) staff       (20)      232 2021-03-26 08:32:06.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/internals.py
--rw-r--r--   0 ksera      (502) staff       (20)    15250 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/step.py
--rw-r--r--   0 ksera      (502) staff       (20)     2055 2021-07-10 07:34:36.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/step_middleware.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.768822 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/
--rw-r--r--   0 ksera      (502) staff       (20)      627 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/__init__.py
--rw-r--r--   0 ksera      (502) staff       (20)     1227 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_complete.py
--rw-r--r--   0 ksera      (502) staff       (20)     1638 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_configure.py
--rw-r--r--   0 ksera      (502) staff       (20)     1126 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_fail.py
--rw-r--r--   0 ksera      (502) staff       (20)     1668 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_update.py
--rw-r--r--   0 ksera      (502) staff       (20)     1170 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/complete.py
--rw-r--r--   0 ksera      (502) staff       (20)     1594 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/configure.py
--rw-r--r--   0 ksera      (502) staff       (20)     1069 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/fail.py
--rw-r--r--   0 ksera      (502) staff       (20)     1605 2021-04-02 02:43:41.000000 slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/update.py
-drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-13 08:19:40.593010 slack_bolt-1.9.3/slack_bolt.egg-info/
--rw-r--r--   0 ksera      (502) staff       (20)    10102 2021-10-13 08:19:40.000000 slack_bolt-1.9.3/slack_bolt.egg-info/PKG-INFO
--rw-r--r--   0 ksera      (502) staff       (20)     7571 2021-10-13 08:19:40.000000 slack_bolt-1.9.3/slack_bolt.egg-info/SOURCES.txt
--rw-r--r--   0 ksera      (502) staff       (20)        1 2021-10-13 08:19:40.000000 slack_bolt-1.9.3/slack_bolt.egg-info/dependency_links.txt
--rw-r--r--   0 ksera      (502) staff       (20)      492 2021-10-13 08:19:40.000000 slack_bolt-1.9.3/slack_bolt.egg-info/requires.txt
--rw-r--r--   0 ksera      (502) staff       (20)       11 2021-10-13 08:19:40.000000 slack_bolt-1.9.3/slack_bolt.egg-info/top_level.txt
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.700909 slack_bolt-1.9.4/
+-rw-r--r--   0 ksera      (502) staff       (20)     1091 2021-08-26 02:24:29.000000 slack_bolt-1.9.4/LICENSE
+-rw-r--r--   0 ksera      (502) staff       (20)       45 2020-08-06 04:03:27.000000 slack_bolt-1.9.4/MANIFEST.in
+-rw-r--r--   0 ksera      (502) staff       (20)    10193 2021-10-29 15:13:36.701488 slack_bolt-1.9.4/PKG-INFO
+-rw-r--r--   0 ksera      (502) staff       (20)     9332 2021-07-02 01:23:16.000000 slack_bolt-1.9.4/README.md
+-rw-r--r--   0 ksera      (502) staff       (20)       92 2021-10-29 15:13:36.703329 slack_bolt-1.9.4/setup.cfg
+-rwxr-xr-x   0 ksera      (502) staff       (20)     3349 2021-10-29 15:12:20.000000 slack_bolt-1.9.4/setup.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.340022 slack_bolt-1.9.4/slack_bolt/
+-rw-r--r--   0 ksera      (502) staff       (20)      928 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.400569 slack_bolt-1.9.4/slack_bolt/adapter/
+-rw-r--r--   0 ksera      (502) staff       (20)       87 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/adapter/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.401912 slack_bolt-1.9.4/slack_bolt/adapter/aiohttp/
+-rw-r--r--   0 ksera      (502) staff       (20)     1255 2021-01-27 04:33:11.000000 slack_bolt-1.9.4/slack_bolt/adapter/aiohttp/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.443270 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4317 2021-05-02 07:22:32.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/chalice_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1530 2021-05-02 07:22:32.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/chalice_lazy_listener_runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4143 2021-08-28 00:49:30.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)      260 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3232 2021-07-15 23:00:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/lambda_s3_oauth_flow.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1116 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/lazy_listener_runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)      940 2021-08-07 13:23:58.000000 slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/local_lambda_client.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.446095 slack_bolt-1.9.4/slack_bolt/adapter/bottle/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/bottle/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1696 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/bottle/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.448335 slack_bolt-1.9.4/slack_bolt/adapter/cherrypy/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/cherrypy/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3207 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/cherrypy/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.450465 slack_bolt-1.9.4/slack_bolt/adapter/django/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/django/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     5981 2021-04-10 01:18:37.000000 slack_bolt-1.9.4/slack_bolt/adapter/django/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.453055 slack_bolt-1.9.4/slack_bolt/adapter/falcon/
+-rw-r--r--   0 ksera      (502) staff       (20)       39 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/falcon/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2623 2021-03-19 04:59:22.000000 slack_bolt-1.9.4/slack_bolt/adapter/falcon/resource.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.455219 slack_bolt-1.9.4/slack_bolt/adapter/fastapi/
+-rw-r--r--   0 ksera      (502) staff       (20)       98 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/fastapi/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)       71 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/fastapi/async_handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.456354 slack_bolt-1.9.4/slack_bolt/adapter/flask/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/flask/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1617 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/flask/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.457722 slack_bolt-1.9.4/slack_bolt/adapter/pyramid/
+-rw-r--r--   0 ksera      (502) staff       (20)       41 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/pyramid/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1901 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/pyramid/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.458353 slack_bolt-1.9.4/slack_bolt/adapter/sanic/
+-rw-r--r--   0 ksera      (502) staff       (20)       52 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/sanic/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2511 2021-08-10 12:00:46.000000 slack_bolt-1.9.4/slack_bolt/adapter/sanic/async_handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.461085 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/
+-rw-r--r--   0 ksera      (502) staff       (20)      470 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.462234 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/aiohttp/
+-rw-r--r--   0 ksera      (502) staff       (20)     3372 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/aiohttp/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1803 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/async_base_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)      107 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/async_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1966 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/async_internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1908 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/base_handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.463304 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/builtin/
+-rw-r--r--   0 ksera      (502) staff       (20)     3280 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/builtin/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1827 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/internals.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.464310 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websocket_client/
+-rw-r--r--   0 ksera      (502) staff       (20)     2777 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websocket_client/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.465355 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websockets/
+-rw-r--r--   0 ksera      (502) staff       (20)     3467 2021-03-29 09:01:39.000000 slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websockets/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.468491 slack_bolt-1.9.4/slack_bolt/adapter/starlette/
+-rw-r--r--   0 ksera      (502) staff       (20)       79 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/starlette/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2242 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/starlette/async_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2059 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/starlette/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.470441 slack_bolt-1.9.4/slack_bolt/adapter/tornado/
+-rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/adapter/tornado/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2369 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/adapter/tornado/handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.476484 slack_bolt-1.9.4/slack_bolt/app/
+-rw-r--r--   0 ksera      (502) staff       (20)      319 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/app/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)    62907 2021-10-29 14:31:44.000000 slack_bolt-1.9.4/slack_bolt/app/app.py
+-rw-r--r--   0 ksera      (502) staff       (20)    61053 2021-10-29 14:31:44.000000 slack_bolt-1.9.4/slack_bolt/app/async_app.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3032 2021-10-29 14:31:44.000000 slack_bolt-1.9.4/slack_bolt/app/async_server.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2312 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/async_app.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.489149 slack_bolt-1.9.4/slack_bolt/authorization/
+-rw-r--r--   0 ksera      (502) staff       (20)      259 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/authorization/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)    12101 2021-10-29 14:31:44.000000 slack_bolt-1.9.4/slack_bolt/authorization/async_authorize.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1091 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/authorization/async_authorize_args.py
+-rw-r--r--   0 ksera      (502) staff       (20)    11608 2021-09-28 06:08:03.000000 slack_bolt-1.9.4/slack_bolt/authorization/authorize.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1042 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/authorization/authorize_args.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2530 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/authorization/authorize_result.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.497160 slack_bolt-1.9.4/slack_bolt/context/
+-rw-r--r--   0 ksera      (502) staff       (20)      406 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/context/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.504139 slack_bolt-1.9.4/slack_bolt/context/ack/
+-rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/context/ack/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1717 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/ack/ack.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1728 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/ack/async_ack.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4753 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/ack/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3175 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/context/async_context.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3144 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/context/base_context.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2949 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/context/context.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.510824 slack_bolt-1.9.4/slack_bolt/context/respond/
+-rw-r--r--   0 ksera      (502) staff       (20)       67 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/context/respond/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2049 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/respond/async_respond.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1310 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/respond/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2051 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/respond/respond.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.519012 slack_bolt-1.9.4/slack_bolt/context/say/
+-rw-r--r--   0 ksera      (502) staff       (20)       59 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/context/say/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2144 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/say/async_say.py
+-rw-r--r--   0 ksera      (502) staff       (20)      229 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/context/say/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2059 2021-06-03 07:52:16.000000 slack_bolt-1.9.4/slack_bolt/context/say/say.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.522547 slack_bolt-1.9.4/slack_bolt/error/
+-rw-r--r--   0 ksera      (502) staff       (20)      834 2021-04-20 05:51:01.000000 slack_bolt-1.9.4/slack_bolt/error/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.534548 slack_bolt-1.9.4/slack_bolt/kwargs_injection/
+-rw-r--r--   0 ksera      (502) staff       (20)      397 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/kwargs_injection/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4782 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/kwargs_injection/args.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4880 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/kwargs_injection/async_args.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3822 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/kwargs_injection/async_utils.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3777 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/kwargs_injection/utils.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.547366 slack_bolt-1.9.4/slack_bolt/lazy_listener/
+-rw-r--r--   0 ksera      (502) staff       (20)      985 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      994 2021-01-27 04:33:11.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/async_internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1242 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/async_runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)      775 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/asyncio_runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)      888 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1068 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)      774 2021-08-30 08:32:04.000000 slack_bolt-1.9.4/slack_bolt/lazy_listener/thread_runner.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.566412 slack_bolt-1.9.4/slack_bolt/listener/
+-rw-r--r--   0 ksera      (502) staff       (20)      495 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/listener/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1412 2021-04-16 05:22:52.000000 slack_bolt-1.9.4/slack_bolt/listener/async_builtins.py
+-rw-r--r--   0 ksera      (502) staff       (20)     4415 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/listener/async_listener.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1717 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/listener/async_listener_completion_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2218 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/listener/async_listener_error_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     8420 2021-04-10 01:18:37.000000 slack_bolt-1.9.4/slack_bolt/listener/asyncio_runner.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1341 2021-04-16 05:22:52.000000 slack_bolt-1.9.4/slack_bolt/listener/builtins.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1898 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/listener/custom_listener.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2072 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/listener/listener.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1556 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/listener/listener_completion_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2084 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/listener/listener_error_handler.py
+-rw-r--r--   0 ksera      (502) staff       (20)     8409 2021-08-30 08:32:04.000000 slack_bolt-1.9.4/slack_bolt/listener/thread_runner.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.574176 slack_bolt-1.9.4/slack_bolt/listener_matcher/
+-rw-r--r--   0 ksera      (502) staff       (20)      564 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      752 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/async_builtins.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1841 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/async_listener_matcher.py
+-rw-r--r--   0 ksera      (502) staff       (20)    16177 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/builtins.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1067 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/custom_listener_matcher.py
+-rw-r--r--   0 ksera      (502) staff       (20)      500 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/listener_matcher/listener_matcher.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.576580 slack_bolt-1.9.4/slack_bolt/logger/
+-rw-r--r--   0 ksera      (502) staff       (20)      790 2021-07-21 07:57:05.000000 slack_bolt-1.9.4/slack_bolt/logger/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)    11806 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/logger/messages.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.587357 slack_bolt-1.9.4/slack_bolt/middleware/
+-rw-r--r--   0 ksera      (502) staff       (20)      905 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/middleware/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      462 2020-09-21 06:30:41.000000 slack_bolt-1.9.4/slack_bolt/middleware/async_builtins.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1813 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/async_custom_middleware.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1822 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/async_middleware.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2232 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/middleware/async_middleware_error_handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.598645 slack_bolt-1.9.4/slack_bolt/middleware/authorization/
+-rw-r--r--   0 ksera      (502) staff       (20)      205 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      147 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)      790 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3160 2021-09-28 06:08:03.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_multi_teams_authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2512 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_single_team_authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)       80 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2668 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2876 2021-09-28 06:08:03.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/multi_teams_authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2462 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/authorization/single_team_authorization.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1518 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/custom_middleware.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.602028 slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/
+-rw-r--r--   0 ksera      (502) staff       (20)       61 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      780 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/async_ignoring_self_events.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1821 2021-03-19 04:59:22.000000 slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/ignoring_self_events.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.605120 slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/
+-rw-r--r--   0 ksera      (502) staff       (20)       69 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1294 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/async_message_listener_matches.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1225 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/message_listener_matches.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1729 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/middleware.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2106 2021-07-14 12:23:14.000000 slack_bolt-1.9.4/slack_bolt/middleware/middleware_error_handler.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.608019 slack_bolt-1.9.4/slack_bolt/middleware/request_verification/
+-rw-r--r--   0 ksera      (502) staff       (20)       62 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/request_verification/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1418 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/request_verification/async_request_verification.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2249 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/request_verification/request_verification.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.611484 slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/
+-rw-r--r--   0 ksera      (502) staff       (20)       40 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      918 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/async_ssl_check.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2067 2021-08-07 13:23:58.000000 slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/ssl_check.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.616025 slack_bolt-1.9.4/slack_bolt/middleware/url_verification/
+-rw-r--r--   0 ksera      (502) staff       (20)       54 2020-09-04 11:56:35.000000 slack_bolt-1.9.4/slack_bolt/middleware/url_verification/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      804 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/middleware/url_verification/async_url_verification.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1347 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/middleware/url_verification/url_verification.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.635116 slack_bolt-1.9.4/slack_bolt/oauth/
+-rw-r--r--   0 ksera      (502) staff       (20)      255 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/oauth/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3818 2021-05-02 07:22:32.000000 slack_bolt-1.9.4/slack_bolt/oauth/async_callback_options.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1582 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/oauth/async_internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)    15456 2021-09-27 00:38:01.000000 slack_bolt-1.9.4/slack_bolt/oauth/async_oauth_flow.py
+-rw-r--r--   0 ksera      (502) staff       (20)     9070 2021-09-21 07:19:22.000000 slack_bolt-1.9.4/slack_bolt/oauth/async_oauth_settings.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3639 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/oauth/callback_options.py
+-rw-r--r--   0 ksera      (502) staff       (20)     5334 2021-09-28 06:08:03.000000 slack_bolt-1.9.4/slack_bolt/oauth/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)    14793 2021-09-27 00:38:05.000000 slack_bolt-1.9.4/slack_bolt/oauth/oauth_flow.py
+-rw-r--r--   0 ksera      (502) staff       (20)     8795 2021-09-21 07:19:00.000000 slack_bolt-1.9.4/slack_bolt/oauth/oauth_settings.py
+-rw-r--r--   0 ksera      (502) staff       (20)        0 2020-08-06 04:03:28.000000 slack_bolt-1.9.4/slack_bolt/py.typed
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.647733 slack_bolt-1.9.4/slack_bolt/request/
+-rw-r--r--   0 ksera      (502) staff       (20)      304 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/request/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1307 2021-04-16 05:22:52.000000 slack_bolt-1.9.4/slack_bolt/request/async_internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2771 2021-05-12 03:16:25.000000 slack_bolt-1.9.4/slack_bolt/request/async_request.py
+-rw-r--r--   0 ksera      (502) staff       (20)     7181 2021-05-12 03:16:25.000000 slack_bolt-1.9.4/slack_bolt/request/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)     5608 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/request/payload_utils.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2668 2021-05-12 03:16:25.000000 slack_bolt-1.9.4/slack_bolt/request/request.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.652102 slack_bolt-1.9.4/slack_bolt/response/
+-rw-r--r--   0 ksera      (502) staff       (20)      344 2021-03-26 08:32:05.000000 slack_bolt-1.9.4/slack_bolt/response/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2061 2021-09-07 08:54:21.000000 slack_bolt-1.9.4/slack_bolt/response/response.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.660022 slack_bolt-1.9.4/slack_bolt/util/
+-rw-r--r--   0 ksera      (502) staff       (20)       49 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/util/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)      420 2021-03-19 04:57:51.000000 slack_bolt-1.9.4/slack_bolt/util/async_utils.py
+-rw-r--r--   0 ksera      (502) staff       (20)     3061 2021-05-02 07:22:32.000000 slack_bolt-1.9.4/slack_bolt/util/utils.py
+-rw-r--r--   0 ksera      (502) staff       (20)       93 2021-10-29 15:12:47.000000 slack_bolt-1.9.4/slack_bolt/version.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.663670 slack_bolt-1.9.4/slack_bolt/workflows/
+-rw-r--r--   0 ksera      (502) staff       (20)      351 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/__init__.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.677150 slack_bolt-1.9.4/slack_bolt/workflows/step/
+-rw-r--r--   0 ksera      (502) staff       (20)      237 2020-10-01 04:13:34.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)    16210 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/async_step.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2109 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/async_step_middleware.py
+-rw-r--r--   0 ksera      (502) staff       (20)      232 2021-03-26 08:32:06.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/internals.py
+-rw-r--r--   0 ksera      (502) staff       (20)    15250 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/step.py
+-rw-r--r--   0 ksera      (502) staff       (20)     2055 2021-07-10 07:34:36.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/step_middleware.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.699513 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/
+-rw-r--r--   0 ksera      (502) staff       (20)      627 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/__init__.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1227 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_complete.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1638 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_configure.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1126 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_fail.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1668 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_update.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1170 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/complete.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1594 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/configure.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1069 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/fail.py
+-rw-r--r--   0 ksera      (502) staff       (20)     1605 2021-04-02 02:43:41.000000 slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/update.py
+drwxr-xr-x   0 ksera      (502) staff       (20)        0 2021-10-29 15:13:36.346619 slack_bolt-1.9.4/slack_bolt.egg-info/
+-rw-r--r--   0 ksera      (502) staff       (20)    10193 2021-10-29 15:13:36.000000 slack_bolt-1.9.4/slack_bolt.egg-info/PKG-INFO
+-rw-r--r--   0 ksera      (502) staff       (20)     7571 2021-10-29 15:13:36.000000 slack_bolt-1.9.4/slack_bolt.egg-info/SOURCES.txt
+-rw-r--r--   0 ksera      (502) staff       (20)        1 2021-10-29 15:13:36.000000 slack_bolt-1.9.4/slack_bolt.egg-info/dependency_links.txt
+-rw-r--r--   0 ksera      (502) staff       (20)      613 2021-10-29 15:13:36.000000 slack_bolt-1.9.4/slack_bolt.egg-info/requires.txt
+-rw-r--r--   0 ksera      (502) staff       (20)       11 2021-10-29 15:13:36.000000 slack_bolt-1.9.4/slack_bolt.egg-info/top_level.txt
```

### Comparing `slack_bolt-1.9.3/LICENSE` & `slack_bolt-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/PKG-INFO` & `slack_bolt-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: slack_bolt
-Version: 1.9.3
+Version: 1.9.4
 Summary: The Bolt Framework for Python
 Home-page: https://github.com/slackapi/bolt-python
 Author: Slack Technologies, LLC
 Author-email: opensource@slack.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: adapter
+Provides-Extra: testing_without_asyncio
 Provides-Extra: testing
 License-File: LICENSE
 
 # Bolt ![Bolt logo](docs/assets/bolt-logo.svg) for Python
 
 [![Python Version][python-version]][pypi-url]
 [![pypi package][pypi-image]][pypi-url]
```

### Comparing `slack_bolt-1.9.3/README.md` & `slack_bolt-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/setup.py` & `slack_bolt-1.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 __version__ = None
 exec(open(f"{here}/slack_bolt/version.py").read())
 
 with open(f"{here}/README.md", "r") as fh:
     long_description = fh.read()
 
 test_dependencies = [
-    "pytest>=5,<6",
-    "pytest-cov>=2,<3",
-    "pytest-asyncio<1",  # for async
-    "aiohttp>=3,<4",  # for async
+    "pytest>=6.2.5,<7",
+    "pytest-cov>=3,<4",
     "Flask-Sockets>=0.2,<1",
     "Werkzeug<2",  # TODO: support Flask 2.x
     "black==21.9b0",
 ]
 
+async_test_dependencies = test_dependencies + [
+    "pytest-asyncio<1",  # for async
+    "aiohttp>=3,<4",  # for async
+]
+
 setuptools.setup(
     name="slack_bolt",
     version=__version__,
     license="MIT",
     author="Slack Technologies, LLC",
     author_email="opensource@slack.com",
     description="The Bolt Framework for Python",
@@ -41,15 +44,15 @@
         ]
     ),
     include_package_data=True,  # MANIFEST.in
     install_requires=[
         "slack_sdk>=3.9.0,<4",
     ],
     setup_requires=["pytest-runner==5.2"],
-    tests_require=test_dependencies,
+    tests_require=async_test_dependencies,
     test_suite="tests",
     extras_require={
         # pip install -e ".[async]"
         "async": [
             # async features heavily depends on aiohttp
             "aiohttp>=3,<4",
             # Socket Mode 3rd party implementation
@@ -60,41 +63,44 @@
         "adapter": [
             # used only under src/slack_bolt/adapter
             "boto3<=2",
             # TODO: Upgrade to v2
             "moto<2",  # For AWS tests
             "bottle>=0.12,<1",
             "boddle>=0.2,<0.3",  # For Bottle app tests
-            "chalice>=1.22.4,<2",
+            "chalice>=1.26.1,<2",
             "click>=7,<8",  # for chalice
             "CherryPy>=18,<19",
             "Django>=3,<4",
             "falcon>=2,<3",
-            "fastapi<1",
+            "fastapi>=0.70.0,<1",
             "Flask>=1,<2",
             "Werkzeug<2",  # TODO: support Flask 2.x
             "pyramid>=1,<2",
             "sanic>=21,<22" if sys.version_info.minor > 6 else "sanic>=20,<21",
-            "sanic-testing>=0.6" if sys.version_info.minor > 6 else "",
-            "starlette>=0.13,<1",
+            "sanic-testing>=0.7" if sys.version_info.minor > 6 else "",
+            "starlette>=0.14,<1",
             "requests>=2,<3",  # For starlette's TestClient
             "tornado>=6,<7",
             # server
             "uvicorn<1",
             "gunicorn>=20,<21",
             # Socket Mode 3rd party implementation
             "websocket_client>=1,<2",
         ],
+        # pip install -e ".[testing_without_asyncio]"
+        "testing_without_asyncio": test_dependencies,
         # pip install -e ".[testing]"
-        "testing": test_dependencies,
+        "testing": async_test_dependencies,
     },
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `slack_bolt-1.9.3/slack_bolt/__init__.py` & `slack_bolt-1.9.4/slack_bolt/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aiohttp/__init__.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/chalice_handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/chalice_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/chalice_lazy_listener_runner.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/chalice_lazy_listener_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/lambda_s3_oauth_flow.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/lambda_s3_oauth_flow.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/lazy_listener_runner.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/lazy_listener_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/aws_lambda/local_lambda_client.py` & `slack_bolt-1.9.4/slack_bolt/adapter/aws_lambda/local_lambda_client.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/bottle/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/bottle/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/cherrypy/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/cherrypy/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/django/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/django/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/falcon/resource.py` & `slack_bolt-1.9.4/slack_bolt/adapter/falcon/resource.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/flask/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/flask/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/pyramid/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/pyramid/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/sanic/async_handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/sanic/async_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/aiohttp/__init__.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/async_base_handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/async_base_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/async_internals.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/async_internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/base_handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/base_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/builtin/__init__.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/internals.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websocket_client/__init__.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websocket_client/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/socket_mode/websockets/__init__.py` & `slack_bolt-1.9.4/slack_bolt/adapter/socket_mode/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/starlette/async_handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/starlette/async_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/starlette/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/starlette/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/adapter/tornado/handler.py` & `slack_bolt-1.9.4/slack_bolt/adapter/tornado/handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/app/app.py` & `slack_bolt-1.9.4/slack_bolt/app/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 `SslCheck` is a built-in middleware that handles ssl_check requests from Slack.
             oauth_settings: The settings related to Slack app installation flow (OAuth flow)
             oauth_flow: Instantiated `slack_bolt.oauth.OAuthFlow`. This is always prioritized over oauth_settings.
             verification_token: Deprecated verification mechanism. This can used only for ssl_check requests.
             listener_executor: Custom executor to run background tasks. If absent, the default `ThreadPoolExecutor` will
                 be used.
         """
-        signing_secret = signing_secret or os.environ.get("SLACK_SIGNING_SECRET")
+        signing_secret = signing_secret or os.environ.get("SLACK_SIGNING_SECRET", "")
         token = token or os.environ.get("SLACK_BOT_TOKEN")
 
         self._name: str = name or inspect.stack()[1].filename.split(os.path.sep)[-1]
         self._signing_secret: str = signing_secret
 
         self._verification_token: Optional[str] = verification_token or os.environ.get(
             "SLACK_VERIFICATION_TOKEN", None
@@ -300,15 +300,15 @@
                 self._installation_store
             )
 
         # --------------------------------------
         # Middleware Initialization
         # --------------------------------------
 
-        self._middleware_list: List[Union[Callable, Middleware]] = []
+        self._middleware_list: List[Middleware] = []
         self._listeners: List[Listener] = []
 
         if listener_executor is None:
             listener_executor = ThreadPoolExecutor(max_workers=5)
 
         self._process_before_response = process_before_response
         self._listener_runner = ThreadListenerRunner(
@@ -465,15 +465,15 @@
 
         Returns:
             The response generated by this Bolt app
         """
         starting_time = time.time()
         self._init_context(req)
 
-        resp: BoltResponse = BoltResponse(status=200, body="")
+        resp: Optional[BoltResponse] = BoltResponse(status=200, body="")
         middleware_state = {"next_called": False}
 
         def middleware_next():
             middleware_state["next_called"] = True
 
         try:
             for middleware in self._middleware_list:
@@ -603,15 +603,16 @@
 
         Args:
             *args: A function that works as a global middleware.
         """
         if len(args) > 0:
             middleware_or_callable = args[0]
             if isinstance(middleware_or_callable, Middleware):
-                self._middleware_list.append(middleware_or_callable)
+                middleware: Middleware = middleware_or_callable
+                self._middleware_list.append(middleware)
             elif isinstance(middleware_or_callable, Callable):
                 self._middleware_list.append(
                     CustomMiddleware(app_name=self.name, func=middleware_or_callable)
                 )
                 return middleware_or_callable
             else:
                 raise BoltError(
```

### Comparing `slack_bolt-1.9.3/slack_bolt/app/async_app.py` & `slack_bolt-1.9.4/slack_bolt/app/async_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                 that verify the endpoint for Events API in HTTP Mode requests.
             ssl_check_enabled: bool = False if you would like to disable the built-in middleware (Default: True).
                 `AsyncSslCheck` is a built-in middleware that handles ssl_check requests from Slack.
             oauth_settings: The settings related to Slack app installation flow (OAuth flow)
             oauth_flow: Instantiated `slack_bolt.oauth.AsyncOAuthFlow`. This is always prioritized over oauth_settings.
             verification_token: Deprecated verification mechanism. This can used only for ssl_check requests.
         """
-        signing_secret = signing_secret or os.environ.get("SLACK_SIGNING_SECRET")
+        signing_secret = signing_secret or os.environ.get("SLACK_SIGNING_SECRET", "")
         token = token or os.environ.get("SLACK_BOT_TOKEN")
 
         self._name: str = name or inspect.stack()[1].filename.split(os.path.sep)[-1]
         self._signing_secret: str = signing_secret
         self._verification_token: Optional[str] = verification_token or os.environ.get(
             "SLACK_VERIFICATION_TOKEN", None
         )
@@ -323,15 +323,15 @@
                 self._async_installation_store
             )
 
         # --------------------------------------
         # Middleware Initialization
         # --------------------------------------
 
-        self._async_middleware_list: List[Union[Callable, AsyncMiddleware]] = []
+        self._async_middleware_list: List[AsyncMiddleware] = []
         self._async_listeners: List[AsyncListener] = []
 
         self._process_before_response = process_before_response
         self._async_listener_runner = AsyncioListenerRunner(
             logger=self._framework_logger,
             process_before_response=process_before_response,
             listener_error_handler=AsyncDefaultListenerErrorHandler(
@@ -502,15 +502,15 @@
 
         Returns:
             The response generated by this Bolt app.
         """
         starting_time = time.time()
         self._init_context(req)
 
-        resp: BoltResponse = BoltResponse(status=200, body="")
+        resp: Optional[BoltResponse] = BoltResponse(status=200, body="")
         middleware_state = {"next_called": False}
 
         async def async_middleware_next():
             middleware_state["next_called"] = True
 
         try:
             for middleware in self._async_middleware_list:
@@ -638,15 +638,16 @@
 
         Args:
             *args: A function that works as a global middleware.
         """
         if len(args) > 0:
             middleware_or_callable = args[0]
             if isinstance(middleware_or_callable, AsyncMiddleware):
-                self._async_middleware_list.append(middleware_or_callable)
+                middleware: AsyncMiddleware = middleware_or_callable
+                self._async_middleware_list.append(middleware)
             elif isinstance(middleware_or_callable, Callable):
                 self._async_middleware_list.append(
                     AsyncCustomMiddleware(
                         app_name=self.name, func=middleware_or_callable
                     )
                 )
                 return middleware_or_callable
```

### Comparing `slack_bolt-1.9.3/slack_bolt/app/async_server.py` & `slack_bolt-1.9.4/slack_bolt/app/async_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Args:
             port: The port to listen on
             path: The path to receive incoming requests from Slack
             app: The `AsyncApp` instance that is used for processing requests
         """
         self.port = port
         self.path = path
-        self.bolt_app: "AsyncApp" = app
+        self.bolt_app: "AsyncApp" = app  # type: ignore
         self.web_app = web.Application()
         self._bolt_oauth_flow = self.bolt_app.oauth_flow
         if self._bolt_oauth_flow:
             self.web_app.add_routes(
                 [
                     web.get(
                         self._bolt_oauth_flow.install_path, self.handle_get_requests
```

### Comparing `slack_bolt-1.9.3/slack_bolt/async_app.py` & `slack_bolt-1.9.4/slack_bolt/async_app.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/authorization/async_authorize.py` & `slack_bolt-1.9.4/slack_bolt/authorization/async_authorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                         installation.user_refresh_token is not None
                         or installation.bot_refresh_token is not None
                     ):
                         if self.token_rotator is None:
                             raise BoltError(self._config_error_message)
                         refreshed = await self.token_rotator.perform_token_rotation(
                             installation=installation,
-                            token_rotation_expiration_minutes=self.token_rotation_expiration_minutes,
+                            minutes_before_expiration=self.token_rotation_expiration_minutes,
                         )
                         if refreshed is not None:
                             await self.installation_store.async_save(refreshed)
                             bot_token, user_token = (
                                 refreshed.bot_token,
                                 refreshed.user_token,
                             )
```

### Comparing `slack_bolt-1.9.3/slack_bolt/authorization/async_authorize_args.py` & `slack_bolt-1.9.4/slack_bolt/authorization/async_authorize_args.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/authorization/authorize.py` & `slack_bolt-1.9.4/slack_bolt/authorization/authorize.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/authorization/authorize_args.py` & `slack_bolt-1.9.4/slack_bolt/authorization/authorize_args.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/authorization/authorize_result.py` & `slack_bolt-1.9.4/slack_bolt/authorization/authorize_result.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/ack/ack.py` & `slack_bolt-1.9.4/slack_bolt/context/ack/ack.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/ack/async_ack.py` & `slack_bolt-1.9.4/slack_bolt/context/ack/async_ack.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/ack/internals.py` & `slack_bolt-1.9.4/slack_bolt/context/ack/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/async_context.py` & `slack_bolt-1.9.4/slack_bolt/context/async_context.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/base_context.py` & `slack_bolt-1.9.4/slack_bolt/context/base_context.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/context.py` & `slack_bolt-1.9.4/slack_bolt/context/context.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/respond/async_respond.py` & `slack_bolt-1.9.4/slack_bolt/context/respond/async_respond.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/respond/internals.py` & `slack_bolt-1.9.4/slack_bolt/context/respond/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/respond/respond.py` & `slack_bolt-1.9.4/slack_bolt/context/respond/respond.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/say/async_say.py` & `slack_bolt-1.9.4/slack_bolt/context/say/async_say.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/context/say/say.py` & `slack_bolt-1.9.4/slack_bolt/context/say/say.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/error/__init__.py` & `slack_bolt-1.9.4/slack_bolt/error/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/kwargs_injection/args.py` & `slack_bolt-1.9.4/slack_bolt/kwargs_injection/args.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/kwargs_injection/async_args.py` & `slack_bolt-1.9.4/slack_bolt/kwargs_injection/async_args.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/kwargs_injection/async_utils.py` & `slack_bolt-1.9.4/slack_bolt/kwargs_injection/async_utils.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/kwargs_injection/utils.py` & `slack_bolt-1.9.4/slack_bolt/kwargs_injection/utils.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/__init__.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/async_internals.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/async_internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/async_runner.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/async_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/asyncio_runner.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/internals.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/runner.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/lazy_listener/thread_runner.py` & `slack_bolt-1.9.4/slack_bolt/lazy_listener/thread_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/async_builtins.py` & `slack_bolt-1.9.4/slack_bolt/listener/async_builtins.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/async_listener.py` & `slack_bolt-1.9.4/slack_bolt/listener/async_listener.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/async_listener_completion_handler.py` & `slack_bolt-1.9.4/slack_bolt/listener/async_listener_completion_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/async_listener_error_handler.py` & `slack_bolt-1.9.4/slack_bolt/listener/async_listener_error_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/asyncio_runner.py` & `slack_bolt-1.9.4/slack_bolt/listener/asyncio_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/builtins.py` & `slack_bolt-1.9.4/slack_bolt/listener/builtins.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/custom_listener.py` & `slack_bolt-1.9.4/slack_bolt/listener/custom_listener.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/listener.py` & `slack_bolt-1.9.4/slack_bolt/listener/listener.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/listener_completion_handler.py` & `slack_bolt-1.9.4/slack_bolt/listener/listener_completion_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/listener_error_handler.py` & `slack_bolt-1.9.4/slack_bolt/listener/listener_error_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener/thread_runner.py` & `slack_bolt-1.9.4/slack_bolt/listener/thread_runner.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener_matcher/__init__.py` & `slack_bolt-1.9.4/slack_bolt/listener_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener_matcher/async_builtins.py` & `slack_bolt-1.9.4/slack_bolt/listener_matcher/async_builtins.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener_matcher/async_listener_matcher.py` & `slack_bolt-1.9.4/slack_bolt/listener_matcher/async_listener_matcher.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener_matcher/builtins.py` & `slack_bolt-1.9.4/slack_bolt/listener_matcher/builtins.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/listener_matcher/custom_listener_matcher.py` & `slack_bolt-1.9.4/slack_bolt/listener_matcher/custom_listener_matcher.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/logger/__init__.py` & `slack_bolt-1.9.4/slack_bolt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/logger/messages.py` & `slack_bolt-1.9.4/slack_bolt/logger/messages.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/__init__.py` & `slack_bolt-1.9.4/slack_bolt/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/async_custom_middleware.py` & `slack_bolt-1.9.4/slack_bolt/middleware/async_custom_middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/async_middleware.py` & `slack_bolt-1.9.4/slack_bolt/middleware/async_middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/async_middleware_error_handler.py` & `slack_bolt-1.9.4/slack_bolt/middleware/async_middleware_error_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_internals.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_multi_teams_authorization.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_multi_teams_authorization.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/async_single_team_authorization.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/async_single_team_authorization.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/internals.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/multi_teams_authorization.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/multi_teams_authorization.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/authorization/single_team_authorization.py` & `slack_bolt-1.9.4/slack_bolt/middleware/authorization/single_team_authorization.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/custom_middleware.py` & `slack_bolt-1.9.4/slack_bolt/middleware/custom_middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/async_ignoring_self_events.py` & `slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/async_ignoring_self_events.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/ignoring_self_events/ignoring_self_events.py` & `slack_bolt-1.9.4/slack_bolt/middleware/ignoring_self_events/ignoring_self_events.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/async_message_listener_matches.py` & `slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/async_message_listener_matches.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/message_listener_matches/message_listener_matches.py` & `slack_bolt-1.9.4/slack_bolt/middleware/message_listener_matches/message_listener_matches.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/middleware.py` & `slack_bolt-1.9.4/slack_bolt/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/middleware_error_handler.py` & `slack_bolt-1.9.4/slack_bolt/middleware/middleware_error_handler.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/request_verification/async_request_verification.py` & `slack_bolt-1.9.4/slack_bolt/middleware/request_verification/async_request_verification.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/request_verification/request_verification.py` & `slack_bolt-1.9.4/slack_bolt/middleware/request_verification/request_verification.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/async_ssl_check.py` & `slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/async_ssl_check.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/ssl_check/ssl_check.py` & `slack_bolt-1.9.4/slack_bolt/middleware/ssl_check/ssl_check.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/url_verification/async_url_verification.py` & `slack_bolt-1.9.4/slack_bolt/middleware/url_verification/async_url_verification.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/middleware/url_verification/url_verification.py` & `slack_bolt-1.9.4/slack_bolt/middleware/url_verification/url_verification.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/async_callback_options.py` & `slack_bolt-1.9.4/slack_bolt/oauth/async_callback_options.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/async_internals.py` & `slack_bolt-1.9.4/slack_bolt/oauth/async_internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/async_oauth_flow.py` & `slack_bolt-1.9.4/slack_bolt/oauth/async_oauth_flow.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/async_oauth_settings.py` & `slack_bolt-1.9.4/slack_bolt/oauth/async_oauth_settings.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/callback_options.py` & `slack_bolt-1.9.4/slack_bolt/oauth/callback_options.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/internals.py` & `slack_bolt-1.9.4/slack_bolt/oauth/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/oauth_flow.py` & `slack_bolt-1.9.4/slack_bolt/oauth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/oauth/oauth_settings.py` & `slack_bolt-1.9.4/slack_bolt/oauth/oauth_settings.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/request/async_internals.py` & `slack_bolt-1.9.4/slack_bolt/request/async_internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/request/async_request.py` & `slack_bolt-1.9.4/slack_bolt/request/async_request.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/request/internals.py` & `slack_bolt-1.9.4/slack_bolt/request/internals.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/request/payload_utils.py` & `slack_bolt-1.9.4/slack_bolt/request/payload_utils.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/request/request.py` & `slack_bolt-1.9.4/slack_bolt/request/request.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/response/response.py` & `slack_bolt-1.9.4/slack_bolt/response/response.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/util/utils.py` & `slack_bolt-1.9.4/slack_bolt/util/utils.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/async_step.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/async_step.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/async_step_middleware.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/async_step_middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/step.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/step.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/step_middleware.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/step_middleware.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/__init__.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_complete.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_complete.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_configure.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_configure.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_fail.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_fail.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/async_update.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/async_update.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/complete.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/complete.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/configure.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/configure.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/fail.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/fail.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt/workflows/step/utilities/update.py` & `slack_bolt-1.9.4/slack_bolt/workflows/step/utilities/update.py`

 * *Files identical despite different names*

### Comparing `slack_bolt-1.9.3/slack_bolt.egg-info/PKG-INFO` & `slack_bolt-1.9.4/slack_bolt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: slack-bolt
-Version: 1.9.3
+Version: 1.9.4
 Summary: The Bolt Framework for Python
 Home-page: https://github.com/slackapi/bolt-python
 Author: Slack Technologies, LLC
 Author-email: opensource@slack.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: adapter
+Provides-Extra: testing_without_asyncio
 Provides-Extra: testing
 License-File: LICENSE
 
 # Bolt ![Bolt logo](docs/assets/bolt-logo.svg) for Python
 
 [![Python Version][python-version]][pypi-url]
 [![pypi package][pypi-image]][pypi-url]
```

### Comparing `slack_bolt-1.9.3/slack_bolt.egg-info/SOURCES.txt` & `slack_bolt-1.9.4/slack_bolt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

