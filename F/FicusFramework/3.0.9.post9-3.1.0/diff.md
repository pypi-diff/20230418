# Comparing `tmp/FicusFramework-3.0.9.post9.tar.gz` & `tmp/FicusFramework-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FicusFramework-3.0.9.post9.tar", last modified: Wed Mar 24 03:16:58 2021, max compression
+gzip compressed data, was "dist/FicusFramework-3.1.0.tar", last modified: Tue Apr 18 02:40:39 2023, max compression
```

## Comparing `FicusFramework-3.0.9.post9.tar` & `FicusFramework-3.1.0.tar`

### file list

```diff
@@ -1,282 +1,293 @@
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/
--rw-r--r--   0 sun        (501) admin       (80)     2942 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/PKG-INFO
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/test/
--rw-r--r--   0 sun        (501) admin       (80)     1535 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/test/test_factDatasourceChangeListener.py
--rw-r--r--   0 sun        (501) admin       (80)     2748 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/test/test_abstractSimpleScripCrawlTestSuite.py
--rw-r--r--   0 sun        (501) admin       (80)      984 2019-08-02 08:53:21.000000 FicusFramework-3.0.9.post9/test/test_utils.py
--rw-r--r--   0 sun        (501) admin       (80)     1701 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/test/test_customerDaoContextHolder.py
--rw-r--r--   0 sun        (501) admin       (80)     1765 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/test/test_cryptography.py
--rw-r--r--   0 sun        (501) admin       (80)     1168 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/test/test_distributedFactDatasourceProxy.py
--rw-r--r--   0 sun        (501) admin       (80)     3131 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/test/test_abstractBatchCETestSuite.py
--rw-r--r--   0 sun        (501) admin       (80)     1266 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/test/test_factDatasourceService.py
--rw-r--r--   0 sun        (501) admin       (80)     3169 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/test/test_abstractSimpleScriptCETestSuite.py
--rw-r--r--   0 sun        (501) admin       (80)     2742 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/test/test_abstractSimpleCrawlTestSuite.py
--rw-r--r--   0 sun        (501) admin       (80)     2926 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/test/test_abstractBatchCrawlTestSuite.py
--rw-r--r--   0 sun        (501) admin       (80)     1259 2021-03-24 03:16:06.000000 FicusFramework-3.0.9.post9/setup.py
--rw-r--r--   0 sun        (501) admin       (80)      100 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/setup.cfg
--rw-r--r--   0 sun        (501) admin       (80)     2346 2018-06-15 02:07:44.000000 FicusFramework-3.0.9.post9/README.rst
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/init/
--rw-r--r--   0 sun        (501) admin       (80)        0 2020-10-27 11:51:51.000000 FicusFramework-3.0.9.post9/src/init/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5195 2020-10-19 02:45:22.000000 FicusFramework-3.0.9.post9/src/init/app.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/schedule/
--rw-r--r--   0 sun        (501) admin       (80)     3436 2020-12-11 02:26:37.000000 FicusFramework-3.0.9.post9/src/schedule/TaskThreadHolder.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/schedule/test/
--rw-r--r--   0 sun        (501) admin       (80)       88 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/schedule/test/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/schedule/test/suite/
--rw-r--r--   0 sun        (501) admin       (80)    14502 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/schedule/test/suite/crawl.py
--rw-r--r--   0 sun        (501) admin       (80)     6057 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/src/schedule/test/suite/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    10791 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/schedule/test/suite/ce.py
--rw-r--r--   0 sun        (501) admin       (80)       28 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    16133 2020-03-24 09:32:14.000000 FicusFramework-3.0.9.post9/src/schedule/TaskThread.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/schedule/utils/
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/utils/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/
--rw-r--r--   0 sun        (501) admin       (80)     4438 2020-08-18 09:18:52.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogFileAppender.py
--rw-r--r--   0 sun        (501) admin       (80)     2428 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogCleanScheduler.py
--rw-r--r--   0 sun        (501) admin       (80)     2284 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogger.py
--rw-r--r--   0 sun        (501) admin       (80)     2981 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/FrameworkHandlerLogger.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/utils/log/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3905 2020-10-28 06:03:01.000000 FicusFramework-3.0.9.post9/src/schedule/TriggerActor.py
--rw-r--r--   0 sun        (501) admin       (80)      484 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/ShardContext.py
--rw-r--r--   0 sun        (501) admin       (80)      245 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/schedule/TaskHandlerContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/cloudcelery/
--rw-r--r--   0 sun        (501) admin       (80)     3452 2021-01-27 02:59:31.000000 FicusFramework-3.0.9.post9/src/cloudcelery/CeleryOnRequest.py
--rw-r--r--   0 sun        (501) admin       (80)     3529 2020-04-29 11:59:19.000000 FicusFramework-3.0.9.post9/src/cloudcelery/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      887 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/cloudcelery/celery_config.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/config/
--rw-r--r--   0 sun        (501) admin       (80)     9841 2020-07-25 08:30:32.000000 FicusFramework-3.0.9.post9/src/config/BootstrapPropertyLoader.py
--rw-r--r--   0 sun        (501) admin       (80)     4093 2020-04-29 12:42:45.000000 FicusFramework-3.0.9.post9/src/config/annotation.py
--rw-r--r--   0 sun        (501) admin       (80)     1722 2021-02-02 06:32:45.000000 FicusFramework-3.0.9.post9/src/config/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/discovery/
--rw-r--r--   0 sun        (501) admin       (80)    14209 2020-07-25 08:30:32.000000 FicusFramework-3.0.9.post9/src/discovery/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/
--rw-r--r--   0 sun        (501) admin       (80)    28003 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceProxyService.py
--rw-r--r--   0 sun        (501) admin       (80)    10882 2021-02-03 08:54:08.000000 FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceContextHolder.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/
--rw-r--r--   0 sun        (501) admin       (80)      718 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/ChineseToNumberTransformer.py
--rw-r--r--   0 sun        (501) admin       (80)     2338 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/TransformerContext.py
--rw-r--r--   0 sun        (501) admin       (80)      762 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/ITransformer.py
--rw-r--r--   0 sun        (501) admin       (80)      579 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/CompleteGB32100Transformer.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     1001 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/FixItemTransformer.py
--rw-r--r--   0 sun        (501) admin       (80)      991 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/ParseDateTimeTransformer.py
--rw-r--r--   0 sun        (501) admin       (80)     3677 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/DefaultValueTransformer.py
--rw-r--r--   0 sun        (501) admin       (80)      881 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/CompleteStringTransformer.py
--rw-r--r--   0 sun        (501) admin       (80)      900 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/transformer/NumberToChineseTransformer.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/
--rw-r--r--   0 sun        (501) admin       (80)     1877 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/MultipleDatasourceHolder.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      643 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/RedisDatasourceDao.py
--rw-r--r--   0 sun        (501) admin       (80)     7186 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/MultipleRedisDatasource.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/graph/
--rw-r--r--   0 sun        (501) admin       (80)     8390 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/graph/GraphDatasourceDao.py
--rw-r--r--   0 sun        (501) admin       (80)     1093 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/graph/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5258 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)     1778 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/AmqpDatasourceDao.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/
--rw-r--r--   0 sun        (501) admin       (80)     3174 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py
--rw-r--r--   0 sun        (501) admin       (80)    12634 2021-02-03 08:54:08.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/
--rw-r--r--   0 sun        (501) admin       (80)     5501 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      926 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/KafkaDatasourceDao.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5132 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/MultipleStompDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)     1035 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/StompDatasourceDao.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3567 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/MongoDatasourceDao.py
--rw-r--r--   0 sun        (501) admin       (80)     5867 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/MultipleMongoDatasource.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/es/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/es/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3287 2020-06-17 11:00:50.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/es/EsDatasourceDao.py
--rw-r--r--   0 sun        (501) admin       (80)     4484 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/es/MultipleEsDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)     4600 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/dao/FactDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)     1603 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/message/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/message/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    10633 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/message/FactDatasourceMessageHanlder.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/file/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/file/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3186 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/file/FileFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/redis/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/redis/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    12650 2020-12-09 07:31:39.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/amqp/
--rw-r--r--   0 sun        (501) admin       (80)     5276 2020-12-09 07:28:30.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/amqp/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    12086 2020-12-09 07:23:42.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/AbstractFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/algorithm/
--rw-r--r--   0 sun        (501) admin       (80)        0 2020-07-27 11:07:37.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/algorithm/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     8030 2020-07-27 11:07:37.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/
--rw-r--r--   0 sun        (501) admin       (80)      534 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    15075 2020-12-09 07:29:32.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/
--rw-r--r--   0 sun        (501) admin       (80)      740 2021-02-03 08:54:08.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     3436 2020-12-09 07:30:40.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     3703 2020-12-09 07:30:49.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      532 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     3801 2020-12-09 07:30:13.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)      283 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/VernoxJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     3291 2020-12-09 07:29:54.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/kafka/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/kafka/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5513 2021-01-27 02:59:31.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/stomp/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/stomp/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5325 2020-12-09 07:31:55.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/mongo/
--rw-r--r--   0 sun        (501) admin       (80)    13093 2020-12-09 07:31:21.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/mongo/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/sobeyhive/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/sobeyhive/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    15917 2020-12-09 07:31:49.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/es/
--rw-r--r--   0 sun        (501) admin       (80)    14150 2020-12-09 07:29:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/es/EsFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/es/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/custom/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/custom/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     2913 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     6093 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/SqlableDeleteCondition.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/graphdb/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/graphdb/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    11260 2020-12-09 07:29:19.000000 FicusFramework-3.0.9.post9/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)     4175 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceContext.py
--rw-r--r--   0 sun        (501) admin       (80)      609 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/factdatasource/execptions.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/libs/
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/libs/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     6659 2021-02-03 08:54:08.000000 FicusFramework-3.0.9.post9/src/libs/utils.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/
--rw-r--r--   0 sun        (501) admin       (80)     3118 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/__urlopen_proxy__.py
--rw-r--r--   0 sun        (501) admin       (80)     4398 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/http_client.py
--rw-r--r--   0 sun        (501) admin       (80)       25 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    51693 2020-09-15 02:23:43.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/eureka_client.py
--rw-r--r--   0 sun        (501) admin       (80)      951 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/py_eureka_client/__logger__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/registry/
--rw-r--r--   0 sun        (501) admin       (80)    12712 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/registry/LoadOnRegistryLoader.py
--rw-r--r--   0 sun        (501) admin       (80)     7749 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/registry/LoadOnAlgorithmLoader.py
--rw-r--r--   0 sun        (501) admin       (80)     2681 2020-07-20 06:12:53.000000 FicusFramework-3.0.9.post9/src/registry/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/
--rw-r--r--   0 sun        (501) admin       (80)      114 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/api/handler/IKillable.py
--rw-r--r--   0 sun        (501) admin       (80)     6313 2020-11-19 08:33:18.000000 FicusFramework-3.0.9.post9/src/api/handler/ICacheAbleHandler.py
--rw-r--r--   0 sun        (501) admin       (80)      160 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/api/handler/IHandler.py
--rw-r--r--   0 sun        (501) admin       (80)      530 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/IProgressAble.py
--rw-r--r--   0 sun        (501) admin       (80)       77 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/api/handler/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/message/
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/message/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     1075 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/api/handler/message/IMessageHandler.py
--rw-r--r--   0 sun        (501) admin       (80)      990 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/ITaskHandler.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/script/
--rw-r--r--   0 sun        (501) admin       (80)      134 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/script/ScriptHandlerHolder.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/script/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3433 2019-11-22 03:45:56.000000 FicusFramework-3.0.9.post9/src/api/handler/script/ScriptPythonFactory.py
--rw-r--r--   0 sun        (501) admin       (80)     1759 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/script/ICacheAbleScript.py
--rw-r--r--   0 sun        (501) admin       (80)     9657 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/handler/script/ScriptPythonTaskHandler.py
--rw-r--r--   0 sun        (501) admin       (80)      301 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/script/IProgressAbleScript.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/
--rw-r--r--   0 sun        (501) admin       (80)      638 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/ISampleScriptCrawl.py
--rw-r--r--   0 sun        (501) admin       (80)     6027 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/AbstractBatchCrawl.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     5242 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/AbstractSimpleCrawl.py
--rw-r--r--   0 sun        (501) admin       (80)      888 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/crawl/ISimpleScriptCrawl.py
--rw-r--r--   0 sun        (501) admin       (80)      428 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/ILogAbleHandler.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/outputer/
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/outputer/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      813 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/outputer/ISimpleOutputer.py
--rw-r--r--   0 sun        (501) admin       (80)     3748 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/handler/outputer/IBatchOutputer.py
--rw-r--r--   0 sun        (501) admin       (80)     5212 2020-08-18 09:18:52.000000 FicusFramework-3.0.9.post9/src/api/handler/outputer/IBaseOutputer.py
--rw-r--r--   0 sun        (501) admin       (80)     1203 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/ICacheAble.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/
--rw-r--r--   0 sun        (501) admin       (80)     7537 2021-03-19 02:01:16.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/IMessageCE.py
--rw-r--r--   0 sun        (501) admin       (80)    12057 2021-03-24 03:15:23.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractAsyncServiceBatchCE.py
--rw-r--r--   0 sun        (501) admin       (80)     6216 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractBatchCE.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      765 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/ISampleScriptCE.py
--rw-r--r--   0 sun        (501) admin       (80)     1045 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/ISimpleScriptCE.py
--rw-r--r--   0 sun        (501) admin       (80)     5626 2020-12-16 03:26:18.000000 FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractMessageCE.py
--rw-r--r--   0 sun        (501) admin       (80)      421 2020-07-06 10:53:29.000000 FicusFramework-3.0.9.post9/src/api/handler/IAsyncAble.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/annotation/
--rw-r--r--   0 sun        (501) admin       (80)      396 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/annotation/annotation.py
--rw-r--r--   0 sun        (501) admin       (80)        0 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/annotation/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/api/model/
--rw-r--r--   0 sun        (501) admin       (80)     2026 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/model/OutputWrapper.py
--rw-r--r--   0 sun        (501) admin       (80)     1123 2020-07-06 10:53:29.000000 FicusFramework-3.0.9.post9/src/api/model/AsyncServiceRequest.py
--rw-r--r--   0 sun        (501) admin       (80)     3653 2020-12-11 02:26:37.000000 FicusFramework-3.0.9.post9/src/api/model/AlgorithmFdInputWrapper.py
--rw-r--r--   0 sun        (501) admin       (80)     1182 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/GraphNode.py
--rw-r--r--   0 sun        (501) admin       (80)     1128 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/ReadWriteLock.py
--rw-r--r--   0 sun        (501) admin       (80)     2088 2021-01-27 02:59:31.000000 FicusFramework-3.0.9.post9/src/api/model/MetaModel.py
--rw-r--r--   0 sun        (501) admin       (80)      679 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/ResultVO.py
--rw-r--r--   0 sun        (501) admin       (80)     1777 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/GraphRelation.py
--rw-r--r--   0 sun        (501) admin       (80)      640 2020-07-06 10:53:29.000000 FicusFramework-3.0.9.post9/src/api/model/AsyncServiceResponse.py
--rw-r--r--   0 sun        (501) admin       (80)     1791 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3225 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/api/model/BatchOutputPipe.py
--rw-r--r--   0 sun        (501) admin       (80)     1879 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/api/model/Page.py
--rw-r--r--   0 sun        (501) admin       (80)     1793 2021-01-27 02:59:31.000000 FicusFramework-3.0.9.post9/src/api/model/MetaModelField.py
--rw-r--r--   0 sun        (501) admin       (80)     2046 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/api/model/MetaModelTransform.py
--rw-r--r--   0 sun        (501) admin       (80)      952 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/api/model/Condition.py
--rw-r--r--   0 sun        (501) admin       (80)      855 2020-07-27 11:07:37.000000 FicusFramework-3.0.9.post9/src/api/model/AlgoOutWrapper.py
--rw-r--r--   0 sun        (501) admin       (80)     1139 2020-07-27 11:07:37.000000 FicusFramework-3.0.9.post9/src/api/model/FdInputPipe.py
--rw-r--r--   0 sun        (501) admin       (80)     6733 2019-02-27 06:21:54.000000 FicusFramework-3.0.9.post9/src/api/model/OtherTargetOutputPipe.py
--rw-r--r--   0 sun        (501) admin       (80)     2436 2020-12-11 02:26:37.000000 FicusFramework-3.0.9.post9/src/api/model/FdInputWrapper.py
--rw-r--r--   0 sun        (501) admin       (80)     5416 2021-02-03 08:54:08.000000 FicusFramework-3.0.9.post9/src/api/model/FactDatasource.py
--rw-r--r--   0 sun        (501) admin       (80)      245 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/api/exceptions.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/rule_engine/
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/rule_engine/operation/
--rw-r--r--   0 sun        (501) admin       (80)     4529 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/operation/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)    13749 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/RuleEngineInitialize.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/
--rw-r--r--   0 sun        (501) admin       (80)     3330 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/SimpleValueProvider.py
--rw-r--r--   0 sun        (501) admin       (80)     1201 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     3576 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/SimpleRuleGroupSession.py
--rw-r--r--   0 sun        (501) admin       (80)     2784 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/DefaultAgenda.py
--rw-r--r--   0 sun        (501) admin       (80)     3489 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/core/PattenMatcher.py
--rw-r--r--   0 sun        (501) admin       (80)     2061 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/RuleEngine.py
--rw-r--r--   0 sun        (501) admin       (80)    11736 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/__init__.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/rule_engine/action/
--rw-r--r--   0 sun        (501) admin       (80)     1347 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/action/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     1678 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/rule_engine/RuleEngineCustomScriptFactory.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/service/
--rw-r--r--   0 sun        (501) admin       (80)     1613 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/service/FactDatasourceService.py
--rw-r--r--   0 sun        (501) admin       (80)       89 2019-05-13 10:28:04.000000 FicusFramework-3.0.9.post9/src/service/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     2256 2020-04-29 11:49:46.000000 FicusFramework-3.0.9.post9/src/service/TaskQueueService.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/
--rw-r--r--   0 sun        (501) admin       (80)     2942 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/PKG-INFO
--rw-r--r--   0 sun        (501) admin       (80)        1 2019-02-27 06:22:29.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/not-zip-safe
--rw-r--r--   0 sun        (501) admin       (80)     9238 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/SOURCES.txt
--rw-r--r--   0 sun        (501) admin       (80)      239 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/requires.txt
--rw-r--r--   0 sun        (501) admin       (80)      127 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/top_level.txt
--rw-r--r--   0 sun        (501) admin       (80)        1 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/dependency_links.txt
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/client/
--rw-r--r--   0 sun        (501) admin       (80)     3234 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/client/ComputeExecutionClient.py
--rw-r--r--   0 sun        (501) admin       (80)     1035 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/client/FactDatasourceManageClient.py
--rw-r--r--   0 sun        (501) admin       (80)     6932 2019-12-13 09:21:10.000000 FicusFramework-3.0.9.post9/src/client/ScheduleJobTaskLogClient.py
--rw-r--r--   0 sun        (501) admin       (80)     1173 2020-04-29 13:07:29.000000 FicusFramework-3.0.9.post9/src/client/ScheduleCloudClient.py
--rw-r--r--   0 sun        (501) admin       (80)     2158 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/client/HandlerLogClient.py
--rw-r--r--   0 sun        (501) admin       (80)     1019 2020-09-28 07:42:31.000000 FicusFramework-3.0.9.post9/src/client/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)     8802 2019-04-15 11:08:40.000000 FicusFramework-3.0.9.post9/src/client/JobScheduleClient.py
--rw-r--r--   0 sun        (501) admin       (80)     4296 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/client/DataCrawlClient.py
--rw-r--r--   0 sun        (501) admin       (80)     3656 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/client/ClientAuth.py
--rw-r--r--   0 sun        (501) admin       (80)     3815 2020-07-24 11:47:04.000000 FicusFramework-3.0.9.post9/src/client/DataAlgorithmClient.py
--rw-r--r--   0 sun        (501) admin       (80)     2728 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/client/AuthClient.py
--rw-r--r--   0 sun        (501) admin       (80)     2079 2020-09-28 06:27:10.000000 FicusFramework-3.0.9.post9/src/client/FactDatasourceClient.py
--rw-r--r--   0 sun        (501) admin       (80)     3905 2019-04-15 11:08:07.000000 FicusFramework-3.0.9.post9/src/client/ScheduleCacheClient.py
-drwxr-xr-x   0 sun        (501) admin       (80)        0 2021-03-24 03:16:58.000000 FicusFramework-3.0.9.post9/src/remote/
--rw-r--r--   0 sun        (501) admin       (80)     1453 2020-03-23 08:49:50.000000 FicusFramework-3.0.9.post9/src/remote/TriggerRemoteActor.py
--rw-r--r--   0 sun        (501) admin       (80)      591 2020-06-15 12:21:33.000000 FicusFramework-3.0.9.post9/src/remote/__init__.py
--rw-r--r--   0 sun        (501) admin       (80)      795 2020-03-24 09:55:45.000000 FicusFramework-3.0.9.post9/src/remote/PrometheusMetricsRemoteService.py
--rw-r--r--   0 sun        (501) admin       (80)      375 2020-10-27 11:51:17.000000 FicusFramework-3.0.9.post9/src/remote/ActuatorRemote.py
--rw-r--r--   0 sun        (501) admin       (80)      914 2019-06-25 08:47:51.000000 FicusFramework-3.0.9.post9/src/remote/LogReadRemoteService.py
--rw-r--r--   0 sun        (501) admin       (80)     7060 2020-12-11 02:26:37.000000 FicusFramework-3.0.9.post9/src/remote/AsyncResponseRestService.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/
+-rw-r--r--   0 sun        (501) wheel        (0)     2936 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/PKG-INFO
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/test/
+-rw-r--r--   0 sun        (501) wheel        (0)     1535 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/test/test_factDatasourceChangeListener.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2748 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractSimpleScripCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)      984 2019-08-02 08:53:21.000000 FicusFramework-3.1.0/test/test_utils.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1701 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/test/test_customerDaoContextHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1765 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/test/test_cryptography.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1192 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/test/test_distributedFactDatasourceProxy.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3242 2022-10-13 03:25:59.000000 FicusFramework-3.1.0/test/test_abstractBatchCETestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1302 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/test/test_factDatasourceService.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3280 2022-10-13 03:25:59.000000 FicusFramework-3.1.0/test/test_abstractSimpleScriptCETestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2742 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractSimpleCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2926 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractBatchCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1263 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/setup.py
+-rw-r--r--   0 sun        (501) wheel        (0)      100 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/setup.cfg
+-rw-r--r--   0 sun        (501) wheel        (0)     2346 2018-06-15 02:07:44.000000 FicusFramework-3.1.0/README.rst
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/init/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2020-10-27 11:51:51.000000 FicusFramework-3.1.0/src/init/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5199 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/init/app.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/
+-rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-11 02:26:37.000000 FicusFramework-3.1.0/src/schedule/TaskThreadHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/test/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/schedule/test/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/test/suite/
+-rw-r--r--   0 sun        (501) wheel        (0)    14543 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/crawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6427 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    10984 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/ce.py
+-rw-r--r--   0 sun        (501) wheel        (0)       28 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    16977 2021-07-22 02:54:07.000000 FicusFramework-3.1.0/src/schedule/TaskThread.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/utils/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/utils/log/
+-rw-r--r--   0 sun        (501) wheel        (0)     4438 2020-08-18 09:18:52.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogFileAppender.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogCleanScheduler.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2284 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogger.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2981 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/FrameworkHandlerLogger.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4190 2021-05-08 09:50:08.000000 FicusFramework-3.1.0/src/schedule/TriggerActor.py
+-rw-r--r--   0 sun        (501) wheel        (0)      484 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/ShardContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      245 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/TaskHandlerContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/cloudcelery/
+-rw-r--r--   0 sun        (501) wheel        (0)     4930 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/cloudcelery/CeleryOnRequest.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4780 2023-01-06 10:44:05.000000 FicusFramework-3.1.0/src/cloudcelery/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1096 2021-07-22 02:42:02.000000 FicusFramework-3.1.0/src/cloudcelery/celery_config.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/config/
+-rw-r--r--   0 sun        (501) wheel        (0)    10997 2021-07-16 06:13:02.000000 FicusFramework-3.1.0/src/config/BootstrapPropertyLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4953 2023-03-16 07:22:14.000000 FicusFramework-3.1.0/src/config/annotation.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2302 2021-07-16 06:12:10.000000 FicusFramework-3.1.0/src/config/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/discovery/
+-rw-r--r--   0 sun        (501) wheel        (0)    14413 2021-07-07 07:23:16.000000 FicusFramework-3.1.0/src/discovery/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/
+-rw-r--r--   0 sun        (501) wheel        (0)    33598 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyService.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12673 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceContextHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/transformer/
+-rw-r--r--   0 sun        (501) wheel        (0)      718 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ChineseToNumberTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2338 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/TransformerContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      762 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ITransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      579 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/CompleteGB32100Transformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1001 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/FixItemTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      991 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ParseDateTimeTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3749 2021-03-25 11:30:40.000000 FicusFramework-3.1.0/src/factdatasource/transformer/DefaultValueTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      881 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/CompleteStringTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      900 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/NumberToChineseTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)    34157 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyServiceV2.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/
+-rw-r--r--   0 sun        (501) wheel        (0)     2095 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/MultipleDatasourceHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      643 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/RedisDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7237 2021-12-10 03:38:55.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/MultipleRedisDatasource.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/
+-rw-r--r--   0 sun        (501) wheel        (0)     8390 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/GraphDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1093 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5310 2021-12-10 03:28:59.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1778 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/AmqpDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/
+-rw-r--r--   0 sun        (501) wheel        (0)     3174 2020-09-28 06:27:10.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12694 2021-12-10 03:36:30.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/
+-rw-r--r--   0 sun        (501) wheel        (0)     5501 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      926 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/KafkaDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5132 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/MultipleStompDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1035 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/StompDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5137 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)      564 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3567 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/MongoDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5894 2021-12-10 03:37:48.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/MultipleMongoDatasource.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3287 2020-06-17 11:00:50.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/EsDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4484 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/MultipleEsDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4600 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/FactDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1603 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/message/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/message/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    10913 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/message/FactDatasourceMessageHanlder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3186 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/FileFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12650 2020-12-09 07:31:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/
+-rw-r--r--   0 sun        (501) wheel        (0)     5276 2020-12-09 07:28:30.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12086 2020-12-09 07:23:42.000000 FicusFramework-3.1.0/src/factdatasource/persistence/AbstractFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     8030 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/
+-rw-r--r--   0 sun        (501) wheel        (0)      534 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    15075 2020-12-09 07:29:32.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/
+-rw-r--r--   0 sun        (501) wheel        (0)      740 2021-02-03 08:54:08.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-09 07:30:40.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3703 2020-12-09 07:30:49.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      532 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3801 2020-12-09 07:30:13.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      283 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3291 2020-12-09 07:29:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5513 2021-01-27 02:59:31.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5325 2020-12-09 07:31:55.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    29851 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/
+-rw-r--r--   0 sun        (501) wheel        (0)    13093 2021-05-18 02:18:14.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    15917 2020-12-09 07:31:49.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/
+-rw-r--r--   0 sun        (501) wheel        (0)    14150 2020-12-09 07:29:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/EsFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2913 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6093 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/SqlableDeleteCondition.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11260 2020-12-09 07:29:19.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4175 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      609 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/execptions.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/libs/
+-rw-r--r--   0 sun        (501) wheel        (0)     1008 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/libs/HeaderHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2023-04-14 11:35:27.000000 FicusFramework-3.1.0/src/libs/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6659 2021-02-03 08:54:08.000000 FicusFramework-3.1.0/src/libs/utils.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/py_eureka_client/
+-rw-r--r--   0 sun        (501) wheel        (0)     3118 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__urlopen_proxy__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4398 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/http_client.py
+-rw-r--r--   0 sun        (501) wheel        (0)       25 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    52699 2021-07-07 06:44:45.000000 FicusFramework-3.1.0/src/py_eureka_client/eureka_client.py
+-rw-r--r--   0 sun        (501) wheel        (0)      951 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__logger__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/registry/
+-rw-r--r--   0 sun        (501) wheel        (0)    12773 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/registry/LoadOnRegistryLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7749 2020-09-28 06:27:10.000000 FicusFramework-3.1.0/src/registry/LoadOnAlgorithmLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2681 2020-07-20 06:12:53.000000 FicusFramework-3.1.0/src/registry/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/
+-rw-r--r--   0 sun        (501) wheel        (0)      114 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/IKillable.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6935 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ICacheAbleHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      160 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/IHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      530 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/IProgressAble.py
+-rw-r--r--   0 sun        (501) wheel        (0)       77 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/message/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/message/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1075 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/message/IMessageHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1039 2021-05-28 02:02:59.000000 FicusFramework-3.1.0/src/api/handler/ITaskHandler.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/script/
+-rw-r--r--   0 sun        (501) wheel        (0)      134 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptHandlerHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/script/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3686 2023-03-16 07:29:04.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptPythonFactory.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1759 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/script/ICacheAbleScript.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11195 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptPythonTaskHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      301 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/script/IProgressAbleScript.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/crawl/
+-rw-r--r--   0 sun        (501) wheel        (0)      638 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/crawl/ISampleScriptCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6190 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/AbstractBatchCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/crawl/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5522 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/AbstractSimpleCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)      937 2021-05-28 02:29:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/ISimpleScriptCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)      428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ILogAbleHandler.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/outputer/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/outputer/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      923 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/ISimpleOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3929 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/IBatchOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5490 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/IBaseOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      199 2021-05-28 02:09:19.000000 FicusFramework-3.1.0/src/api/handler/IRevoke.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1203 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ICacheAble.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/ce/
+-rw-r--r--   0 sun        (501) wheel        (0)     7827 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/IMessageCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)    13379 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractAsyncServiceBatchCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6467 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractBatchCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ce/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      765 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ce/ISampleScriptCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1094 2021-05-28 02:28:47.000000 FicusFramework-3.1.0/src/api/handler/ce/ISimpleScriptCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5919 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractMessageCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)      421 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/handler/IAsyncAble.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/annotation/
+-rw-r--r--   0 sun        (501) wheel        (0)      396 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/api/annotation/annotation.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/annotation/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/model/
+-rw-r--r--   0 sun        (501) wheel        (0)     2026 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/model/OutputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1123 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/model/AsyncServiceRequest.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3853 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/AlgorithmFdInputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1182 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/GraphNode.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1128 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/ReadWriteLock.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2088 2021-01-27 02:59:31.000000 FicusFramework-3.1.0/src/api/model/MetaModel.py
+-rw-r--r--   0 sun        (501) wheel        (0)      679 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/ResultVO.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1777 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/GraphRelation.py
+-rw-r--r--   0 sun        (501) wheel        (0)      640 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/model/AsyncServiceResponse.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1791 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3225 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/model/BatchOutputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1879 2021-03-25 11:31:25.000000 FicusFramework-3.1.0/src/api/model/Page.py
+-rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FactDatasourceQueryParameter.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1857 2021-03-25 10:50:10.000000 FicusFramework-3.1.0/src/api/model/MetaModelField.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2046 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/api/model/MetaModelTransform.py
+-rw-r--r--   0 sun        (501) wheel        (0)      952 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/api/model/Condition.py
+-rw-r--r--   0 sun        (501) wheel        (0)      855 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/api/model/AlgoOutWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1572 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FdInputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6733 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/OtherTargetOutputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4423 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FdInputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5501 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/api/model/FactDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)      245 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/exceptions.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/operation/
+-rw-r--r--   0 sun        (501) wheel        (0)     4529 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/operation/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    13749 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngineInitialize.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/core/
+-rw-r--r--   0 sun        (501) wheel        (0)     3330 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/SimpleValueProvider.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1201 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3576 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/SimpleRuleGroupSession.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2784 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/DefaultAgenda.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3489 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/PattenMatcher.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2061 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngine.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11736 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/action/
+-rw-r--r--   0 sun        (501) wheel        (0)     1347 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/action/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1678 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngineCustomScriptFactory.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/service/
+-rw-r--r--   0 sun        (501) wheel        (0)     1809 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/service/FactDatasourceService.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/service/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2256 2020-04-29 11:49:46.000000 FicusFramework-3.1.0/src/service/TaskQueueService.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/
+-rw-r--r--   0 sun        (501) wheel        (0)     2936 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/PKG-INFO
+-rw-r--r--   0 sun        (501) wheel        (0)        1 2019-02-27 06:22:29.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/not-zip-safe
+-rw-r--r--   0 sun        (501) wheel        (0)     9687 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 sun        (501) wheel        (0)      247 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/requires.txt
+-rw-r--r--   0 sun        (501) wheel        (0)      127 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/top_level.txt
+-rw-r--r--   0 sun        (501) wheel        (0)        1 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/dependency_links.txt
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/client/
+-rw-r--r--   0 sun        (501) wheel        (0)     3234 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/ComputeExecutionClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1035 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/client/FactDatasourceManageClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6946 2021-08-13 06:23:01.000000 FicusFramework-3.1.0/src/client/ScheduleJobTaskLogClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1173 2020-04-29 13:07:29.000000 FicusFramework-3.1.0/src/client/ScheduleCloudClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2158 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/HandlerLogClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1791 2021-06-04 07:35:30.000000 FicusFramework-3.1.0/src/client/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     8802 2019-04-15 11:08:40.000000 FicusFramework-3.1.0/src/client/JobScheduleClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4296 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/DataCrawlClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3996 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/ClientAuth.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3815 2020-07-24 11:47:04.000000 FicusFramework-3.1.0/src/client/DataAlgorithmClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2850 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/AuthClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2254 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/FactDatasourceClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3905 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/ScheduleCacheClient.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/remote/
+-rw-r--r--   0 sun        (501) wheel        (0)     1453 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/remote/TriggerRemoteActor.py
+-rw-r--r--   0 sun        (501) wheel        (0)      591 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/remote/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      795 2020-03-24 09:55:45.000000 FicusFramework-3.1.0/src/remote/PrometheusMetricsRemoteService.py
+-rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/remote/ActuatorRemote.py
+-rw-r--r--   0 sun        (501) wheel        (0)      914 2019-06-25 08:47:51.000000 FicusFramework-3.1.0/src/remote/LogReadRemoteService.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7060 2020-12-11 02:26:37.000000 FicusFramework-3.1.0/src/remote/AsyncResponseRestService.py
```

### Comparing `FicusFramework-3.0.9.post9/PKG-INFO` & `FicusFramework-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: FicusFramework
-Version: 3.0.9.post9
+Version: 3.1.0
 Summary: A framework for Ficus by Python3.
 Home-page: https://git.sobey.com/SobeyHive/FicusFramework4Py
 Author: sunxiang0918
 Author-email: sunxiang0918@gmail.com
 License: MIT
 Description: \u0023\u0020\u0046\u0069\u0063\u0075\u0073\u0020\u0050\u0079\u0074\u0068\u006f\u006e\u0020\u5f00\u53d1\u5957\u4ef6\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u5f00\u53d1\u6b65\u9aa4\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u5fc5\u987b\u8981\u6709\u4e00\u4e2a\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u6587\u4ef6\u002c\u7528\u4e8e\u53d1\u5e03\u0060\u0066\u006c\u0061\u0073\u006b\u0060\u7684\u0072\u0065\u0073\u0074\u0066\u0075\u006c\u0020\u0041\u0070\u0069\u000d\u000a\u0032\u002e\u0020\u5728\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u4e2d\u6267\u884c\u0060\u0061\u0070\u0070\u0020\u003d\u0020\u0046\u006c\u0061\u0073\u006b\u0028\u005f\u005f\u006e\u0061\u006d\u0065\u005f\u005f\u0029\u0060\u7528\u4e8e\u542f\u52a8\u0046\u006c\u0061\u0073\u006b\u670d\u52a1\u000d\u000a\u0033\u002e\u0020\u4f7f\u7528\u0060\u0066\u0072\u006f\u006d\u0020\u0072\u0065\u006d\u006f\u0074\u0065\u0020\u0069\u006d\u0070\u006f\u0072\u0074\u0020\u002a\u0060\u0020\u5bfc\u5165\u0072\u0065\u0073\u0074\u7684\u0060\u0065\u006e\u0064\u0070\u006f\u0069\u006e\u0074\u0060\u000d\u000a\u0034\u002e\u0020\u5728\u9879\u76ee\u4e2d\u521b\u5efa\u4e00\u4e2a\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u002c\u5e76\u6307\u5b9a\u670d\u52a1\u7684\u540d\u79f0\u548c\u0065\u0075\u0072\u0065\u006b\u0061\u7684\u5730\u5740\u000d\u000a\u0035\u002e\u0020\u8c03\u7528\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u7684\u65b9\u6cd5\u0060\u0072\u0065\u0067\u0069\u0073\u0074\u0065\u0072\u0028\u0026\u0071\u0075\u006f\u0074\u003b\u0055\u0050\u0026\u0071\u0075\u006f\u0074\u003b\u0029\u0060\u4ee5\u53ca\u0060\u0073\u0074\u0061\u0072\u0074\u005f\u0068\u0065\u0061\u0072\u0074\u0062\u0065\u0061\u0074\u0060\u5411\u0065\u0075\u0072\u0065\u006b\u0061\u6ce8\u518c\u53ca\u5fc3\u8df3\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u6ce8\u610f\u4e8b\u9879\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u0041\u0070\u0069\u4e2d\u6240\u6709\u7684\u0056\u004f\u5bf9\u8c61\u0020\u90fd\u662f\u7528\u4e86\u0020\u005b\u0060\u006d\u0075\u006e\u0063\u0068\u0060\u005d\u0028\u0068\u0074\u0074\u0070\u0073\u003a\u002f\u002f\u0067\u0069\u0074\u0068\u0075\u0062\u002e\u0063\u006f\u006d\u002f\u0049\u006e\u0066\u0069\u006e\u0069\u0064\u0061\u0074\u002f\u006d\u0075\u006e\u0063\u0068\u0029\u0020\u505a\u4ea4\u4e92\u002e
 Keywords: ficus framework python
```

### Comparing `FicusFramework-3.0.9.post9/test/test_factDatasourceChangeListener.py` & `FicusFramework-3.1.0/test/test_factDatasourceChangeListener.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_abstractSimpleScripCrawlTestSuite.py` & `FicusFramework-3.1.0/test/test_abstractSimpleScripCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_utils.py` & `FicusFramework-3.1.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_customerDaoContextHolder.py` & `FicusFramework-3.1.0/test/test_customerDaoContextHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_cryptography.py` & `FicusFramework-3.1.0/test/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_distributedFactDatasourceProxy.py` & `FicusFramework-3.1.0/test/test_distributedFactDatasourceProxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 
 class TestDistributedFactDatasourceProxy(TestCase):
 
     def test_size(self):
         register_default_datasource()
         fd_context_holder = FactDatasourceContextHolder.instance()
-        fd_context1 = fd_context_holder.get_fact_datasource('test_source_1')
+        fd_context1 = fd_context_holder.get_fact_datasource('S1','test','test_source_1')
         size = fd_context1.size()
         print(f'数据源test_source_1长度{size}')
 
-        fd_context2 = fd_context_holder.get_fact_datasource('test_source_2')
+        fd_context2 = fd_context_holder.get_fact_datasource('S1','test','test_source_2')
         size = fd_context2.size()
         print(f'数据源test_source_2长度{size}')
 
         print(fd_context2.collect(5))
 
         print(fd_context1.collect(5))
```

### Comparing `FicusFramework-3.0.9.post9/test/test_abstractBatchCETestSuite.py` & `FicusFramework-3.1.0/test/test_abstractBatchCETestSuite.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         try:
             raise Exception('CE_PYTHON日志测试，这里输出错误日志')
         except Exception as e:
             self.task_logger.error(e)
 
         query_sql = """{"from": 0,"size": 200}"""
         query_result = source_fds.get_fd('test_source').query(query_sql)
+        # 与query功能相同
+        # query_result = source_fds.get_fd('test_source').query_data(query_sql)
         self.task_logger.log(f"CE_PYTHON日志测试，查询结果:{query_result}")
 
         # 缓存
         self.set_cache_value('name', 'sobey')
         cache_value = self.get_cache_value('name')
         self.task_logger.log(f"缓存值{cache_value}")
```

### Comparing `FicusFramework-3.0.9.post9/test/test_factDatasourceService.py` & `FicusFramework-3.1.0/test/test_factDatasourceService.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
 
 class TestFactDatasourceService(TestCase):
 
     def test_get_fd_by_code(self):
         register_default_datasource()
         fd_service = FactDatasourceService.instance()
-        fd = fd_service.get_fd_by_code('test_source_1')
+        fd = fd_service.get_fd_by_code('S1','test','test_source_1')
         print(fd.get_source_name())
 
-        fdx = fd_service.get_fd_by_code('test_source_x')
+        fdx = fd_service.get_fd_by_code('S1','test','test_source_x')
         print(fdx)
 
     def test_exists_fds(self):
         register_default_datasource()
         fd_service = FactDatasourceService.instance()
         fd_codes = ['test_source_1', 'test_source_2']
         # fd_codes = ['test_source_1', 'test_source_2', 'test_source_x']
         # fd_codes = ['test_source_x']
-        is_exists = fd_service.exists_fds(fd_codes)
+        is_exists = fd_service.exists_fds('S1','test',fd_codes)
         print(is_exists)
```

### Comparing `FicusFramework-3.0.9.post9/test/test_abstractSimpleScriptCETestSuite.py` & `FicusFramework-3.1.0/test/test_abstractSimpleScriptCETestSuite.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         try:
             raise Exception('CE_PYTHON日志测试，这里输出错误日志')
         except Exception as e:
             self.task_logger.error(e)
 
         query_sql = """{"from": 0,"size": 200}"""
         query_result = source_fds.get_fd('test_source').query(query_sql)
+        # 与query功能相同
+        # query_result = source_fds.get_fd('test_source').query_data(query_sql)
         self.task_logger.log(f"CE_PYTHON日志测试，查询结果:{query_result}")
 
         # 缓存
         self.set_cache_value('name', 'sobey')
         cache_value = self.get_cache_value('name')
         self.task_logger.log(f"缓存值{cache_value}")
```

### Comparing `FicusFramework-3.0.9.post9/test/test_abstractSimpleCrawlTestSuite.py` & `FicusFramework-3.1.0/test/test_abstractSimpleCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/test/test_abstractBatchCrawlTestSuite.py` & `FicusFramework-3.1.0/test/test_abstractBatchCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/setup.py` & `FicusFramework-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="FicusFramework",
-    version="3.0.9.post9",
+    version="3.1.0",
 
     packages=find_packages('src'),
     package_dir={'': 'src'},
     test_suite="test",
 
     install_requires=["flask>=1.1.2", "flask-cors>=3.0.8", "requests>=2.23.0", "apscheduler>=3.6.3", "jsonpath-rw>=1.4.0",
                       "munch>=2.5.0", "PyYaml>=5.3.1", "readerwriterlock>=1.0.7", "confluent-kafka>=1.3.0",
-                      "sqlalchemy>=1.3.3", "mysqlclient","gevent","Celery==4.4.7","redis>=3.5.3","python-consul2"],
+                      "sqlalchemy>=1.3.3", "mysqlclient","pymongo","gevent","Celery==4.4.7","redis>=3.5.3","python-consul2"],
 
     author='sunxiang0918',
     author_email="sunxiang0918@gmail.com",
     description="A framework for Ficus by Python3.",
     long_description=read("README.rst"),
     license="MIT",
     keywords="ficus framework python",
```

### Comparing `FicusFramework-3.0.9.post9/README.rst` & `FicusFramework-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/init/app.py` & `FicusFramework-3.1.0/src/init/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,16 +130,16 @@
     """
     单独启动flask
     :return:
     """
     if not celery_able:
         # 在非celery环境中,需要在主进程上启动监控
         # 这里要提前获取一次,便于提前加载和开启数据库连接以及FD的变化监听
-        from factdatasource import FactDatasourceProxyService
-        FactDatasourceProxyService.fd_client_proxy()
+        from factdatasource import FactDatasourceProxyServiceV2
+        FactDatasourceProxyServiceV2.fd_client_proxy()
         log.info("服务启动,完成FD服务加载")
 
     from config import server_port
     from gevent import pywsgi
     # import gevent.monkey
     # gevent.monkey.patch_all()
     server = pywsgi.WSGIServer(('0.0.0.0', server_port), app)
```

### Comparing `FicusFramework-3.0.9.post9/src/schedule/TaskThreadHolder.py` & `FicusFramework-3.1.0/src/schedule/TaskThreadHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/schedule/test/suite/crawl.py` & `FicusFramework-3.1.0/src/schedule/test/suite/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         :return:
         """
         if result_list is None or len(result_list) == 0:
             # 搞完了,没的结果,不处理
             return SUCCESS
         # 有结果,就需要从crawl的配置中找到目标的fd,然后调用fd的接口进行保存
         try:
-            self.send_output_result(params["code_"], result_list, output_fd_codes)
+            self.send_output_result(params['site_'], params['projectCode_'], params["code_"], result_list, output_fd_codes)
         except Exception as e:
             self._simple_script_crawl.task_logger(
                 f"{params['site_']}_{params['projectCode_']}_{params['code_']} 发送结果数据失败,",e)
             return ResultVO(FAIL_CODE, f"发送结果数据失败,错误:{str(e)}")
         return SUCCESS
 
     def get_code_thread_local(self):
```

### Comparing `FicusFramework-3.0.9.post9/src/schedule/test/suite/__init__.py` & `FicusFramework-3.1.0/src/schedule/test/suite/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,24 +55,25 @@
         from config.BootstrapPropertyLoader import init_from_yaml_property,init_from_environ_property
         config_path = self.centralized_mode_config_path()
         init_from_yaml_property(config_path)
         # 尝试从环境变量中获取 bootstrap里面的信息
         init_from_environ_property()
 
         if self.distributed_mode():
+            # 这里的测试套件还是使用V1版本
             from factdatasource.FactDatasourceProxyService import DistributedFactDatasourceProxy
             self.client = DistributedFactDatasourceProxy.instance()
             # 注册所有的数据源
             self.__register_fact_datasource()
         else:
             # from config.BootstrapPropertyLoader import init_from_yaml_property
             # init_from_yaml_property(self.centralized_mode_config_path())
             from init import app
             app.log.info('初始化加载配置')
-
+            # 这里的测试套件还是使用V1版本
             from factdatasource.FactDatasourceProxyService import CentralizedFactDatasourceProxy
             self.client = CentralizedFactDatasourceProxy.instance()
         return self.client
 
     def __register_fact_datasource(self):
         fds = self.mock_fact_datasource()
         from factdatasource.FactDatasourceContextHolder import FactDatasourceContextHolder
@@ -127,14 +128,15 @@
         :param type:  固定值 CUSTOM
         :param kwargs:  其他参数
         """
         self.site = site
         self.projectCode = projectCode
         self.code = code
         self.params = params
+        # 2023-03-31 10:59:56 要求输出的fdCode是同一个project中的
         self.outputFdCodes = outputFdCodes
         self.type = 'CUSTOM'
         self.__fields = {
             'site': site,
             'projectCode': projectCode,
             'code': code,
             'outputFdCodes': outputFdCodes,
@@ -159,15 +161,17 @@
         :param type:  固定值 CUSTOM
         :param kwargs:  其他参数
         """
         self.site = site
         self.projectCode = projectCode
         self.code = code
         self.params = params
+        # 2023-03-31 10:59:56 要求输出的fdCode是同一个project中的或者是 __NO_PROJECT__ 的
         self.sourceFdCodes = sourceFdCodes
+        # 2023-03-31 10:59:56 要求输出的fdCode是同一个project中的
         self.outputFdCodes = outputFdCodes
         self.type = 'CUSTOM'
         self.__fields = {
             'site': site,
             'projectCode': projectCode,
             'code': code,
             'sourceFdCodes': sourceFdCodes,
```

### Comparing `FicusFramework-3.0.9.post9/src/schedule/test/suite/ce.py` & `FicusFramework-3.1.0/src/schedule/test/suite/ce.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,24 +51,26 @@
         # self._simple_script_ce.task_logger = TaskLogger(log_path)
         # 这里日志输出到控制台，不向日志文件中中记录
         self._simple_script_ce.task_logger = TaskLoggerMock()
 
         try:
             self.set_local_code(data_ce.site + "_" + data_ce.projectCode + "_" + data_ce.code)
             self.set_process_id(PROCESS_LOG_ID)
+            self.set_site_and_project(data_ce.site , data_ce.projectCode)
             ScriptHandlerHolder.holder.key = self
             self.__execution_message_local.content = []
 
-            result_list = self._simple_script_ce.do_compute(FdInputPipe(data_ce.sourceFdCodes), params)
+            result_list = self._simple_script_ce.do_compute(FdInputPipe(data_ce.site , data_ce.projectCode, data_ce.sourceFdCodes), params)
         except Exception as e:
             return ResultVO(FAIL_CODE, f"执行失败,Code:{params['site_']}的CE,发生错误:{str(e)}")
         finally:
             # 清理 MessageLocal 和 LocalCode
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__execution_message_local.content = None
             ScriptHandlerHolder.holder.key = None
             self._simple_script_ce.task_logger = None
         return self._send_results(params, result_list, data_ce.outputFdCodes)
 
     def _send_results(self, params, result_list, output_fd_codes):
         """
@@ -79,15 +81,15 @@
         :return:
         """
         if result_list is None or len(result_list) == 0:
             # 搞完了,没的结果,不处理
             return SUCCESS
         # 有结果,就需要从ce的配置中找到目标的fd,然后调用fd的接口进行保存
         try:
-            self.send_output_result(params["code_"], result_list, output_fd_codes)
+            self.send_output_result(params['site_'], params['projectCode_'], params["code_"], result_list, output_fd_codes)
         except Exception as e:
             self._simple_script_ce.task_logger(
                 f"{params['site_']}_{params['projectCode_']}_{params['code_']} 发送结果数据失败,", e)
             return ResultVO(FAIL_CODE, f"发送结果数据失败,错误:{str(e)}")
         return SUCCESS
 
     def get_code_thread_local(self):
```

### Comparing `FicusFramework-3.0.9.post9/src/schedule/TaskThread.py` & `FicusFramework-3.1.0/src/schedule/TaskThread.py`

 * *Files 3% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
     def __inner_run(self, task_param):
         log_id = None
         execute_result = None
         try:
             if task_param is None:
                 # 没有任务
-                return
+                return FAIL
 
             log_id = task_param.logId
 
             FrameworkHandlerLogger.log_info(f"开始处理logId:{log_id}的任务")
 
             if task_param.actorParams is None:
                 task_param.actorParams = {}
@@ -283,14 +283,25 @@
 
             # 更新任务状态到正在执行
             import config
             self.__update_task_status_to_execute(log_id,
                                                  f"{config.server_ip or config.find_host_ip()}:{config.server_port or 5000}",
                                                  1)
 
+            # 这里再判断一下ProcessLogId所对应的状态,有可能已经是失败了,那么这个任务也就不要做了
+            if task_param.processLogId is not None:
+                # 说明是有ProcessLogId的
+                process_log = client.ScheduleJobTaskLogClient.get_task_log_by_id(task_param.processLogId)
+                if process_log is not None and process_log.executeStatus == -1:
+                    # 说明主的流程任务已经失败了,这个任务不用执行了
+                    err = f"logId:{log_id}的任务,因为主任务:{task_param.processLogId}状态为-1,不继续执行"
+                    FrameworkHandlerLogger.log_info(err)
+                    self.__update_task_status_to_finished(log_id, ResultVO(FAIL_CODE, err), False, 1)
+                    return ResultVO(FAIL_CODE, err)
+
             from schedule import ShardContext
             try:
                 from schedule.ShardContext import Sharding
                 ShardContext.set_sharding(Sharding(task_param.shardIndex, task_param.shardTotal))
                 TaskLogFileAppender.prepare_to_log(datetime.strptime(task_param.triggerTime, "%Y-%m-%d %H:%M:%S"),
                                                    task_param.logId)
                 from schedule.utils.log.TaskLogger import TaskLogger
```

### Comparing `FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogFileAppender.py` & `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogFileAppender.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogCleanScheduler.py` & `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogCleanScheduler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/schedule/utils/log/TaskLogger.py` & `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogger.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/schedule/utils/log/FrameworkHandlerLogger.py` & `FicusFramework-3.1.0/src/schedule/utils/log/FrameworkHandlerLogger.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/schedule/TriggerActor.py` & `FicusFramework-3.1.0/src/schedule/TriggerActor.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,17 @@
             remove_old_reason = "更新JobHandler或更换任务模式,终止旧任务线程"
             # 这里不需要显示的终止,在调用 registryTaskThread的时候会自己终止
             task_thread = None
             task_handler = None
 
         if task_handler is None:
             task_handler = TaskHandlerContext.load_task_handler(task_param.actorHandler)
+            if task_handler is None:
+                from api.exceptions import IllegalArgumentException
+                raise IllegalArgumentException(f"加载TaskHandler:{task_param.actorHandler} 失败,请确认handler名称正确,以及与执行器中的@TaskHandler注解一致")
 
     elif "JAVA" == task_param.jobType or "SHELL" == task_param.jobType:
         return ResultVO(FAIL_CODE, f"jobType [{task_param.jobType} 此执行器不支持")
     elif "PYTHON" == task_param.jobType:
         # 这里要创建一个 新的 ScriptPython的执行器
         from api.handler.script.ScriptPythonTaskHandler import ScriptPythonTaskHandler
         if task_thread is not None and not (isinstance(task_thread.get_handler(),
```

### Comparing `FicusFramework-3.0.9.post9/src/cloudcelery/CeleryOnRequest.py` & `FicusFramework-3.1.0/src/cloudcelery/CeleryOnRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 import logging
 
 from celery.signals import task_revoked
 
 from api.model.ResultVO import ResultVO, FAIL_CODE
 from cloudcelery import celery
+from cloudcelery import celery_redis_client
 from schedule import TriggerActor
 from munch import Munch
 import json
 
 log = logging.getLogger('Ficus')
 
+def checkTaskRepetition(task_id) -> bool:
+    """
+    判断从celery里面获取到的任务是否重复.
+    celery使用redis作为后端的时候,会有一个visibility_timeout来控制任务时候超时未完成.
+    但是他自己本身的原因, 就算把visibility_timeout设置成了12小时,他还是有可能会把任务重新触发.这是不满足我们要求的.
+    所以,就只能自己想办法了,也就是使用 redis中的 SETNX来加锁. 执行过的就不再执行了(12小时过期)
+    :return: 如果已经重复了,返回True,  否则返回False
+    """
+    redis = celery_redis_client()
+    key = f"sobeyficus.celery.repetition.{task_id}"
+    if redis.setnx(key, "1"):
+        # 没有执行过
+        redis.expire(key, 43200)
+        return False
+    return True
 
 @celery.task(name='tasks.on_request', bind=True, max_retries=2, default_retry_delay=1 * 6)
 def on_request(self, protocol):
     """
     从celery接收协议
     :param self:
     :param protocol:
     :return:
     """
     log.info(f"从celery中获取到任务:{protocol}")
+    body = Munch(json.loads(protocol))
+
+    if checkTaskRepetition(body.logId):
+        # 说明已经重复了,不能再执行了,直接返回
+        log.info(f"从celery中获取的任务:logId:{body.logId} 已经被执行过,12小时内不再重复执行.")
+        return {'status': True, 'data': {'code': 2, 'msg': 'success', 'content': None}}
+
     try:
         # 子进程中也开启eureka_client的刷新,因为celery也会起子进程,所以只能在这里初始化了
         from discovery import discovery_service_proxy
         import config
         discovery_service_proxy().registry_discovery(config.eureka_default_zone, renewal_interval_in_secs=4)
     except:
         pass
 
     try:
         # 在celery环境中,需要在celery的子进程中也初始化这个监听
         # 这里要提前获取一次,便于提前加载和开启数据库连接以及FD的变化监听
-        from factdatasource import FactDatasourceProxyService
-        FactDatasourceProxyService.fd_client_proxy()
+        from factdatasource import FactDatasourceProxyServiceV2
+        FactDatasourceProxyServiceV2.fd_client_proxy()
         log.info("完成FD服务监听加载")
     except:
         pass
 
-    body = Munch(json.loads(protocol))
-
     result: ResultVO = TriggerActor.handle_trigger(body, True)  # ResultVO
     log.info(f"任务执行完成，jobId:{body.jobId} logId:{body.logId}")
 
     if result.code == FAIL_CODE:
         # 让celery的任务也置失败
         raise RuntimeError(result.msg)
 
@@ -79,13 +100,17 @@
 
     # 这说明有这个方法了
     try:
         actorParam = Munch(json.loads(task_log.actorParam))
         #设置缓存需要的key
         CacheAbleHandlerHolder.get_handler().set_local_code(actorParam["site_"] + "_" + actorParam["projectCode_"] + "_" + actorParam["code_"])
         CacheAbleHandlerHolder.get_handler().set_process_id(actorParam.get("__processLogId__"))
-
+        CacheAbleHandlerHolder.get_handler().set_site_and_project(actorParam["site_"] , actorParam["projectCode_"])
         revoke_handler(task_log.actorCode, task_log.actorHandler, actorParam["code_"],
                        actorParam["projectCode_"], actorParam["site_"], task_log.id, task_log.jobId,
                        task_log.messageId, expired)
     except Exception as e:
         log.warning(f"任务:{task_log},取消回调失败:{str(e)}")
+    finally:
+        CacheAbleHandlerHolder.get_handler().clear_local_code()
+        CacheAbleHandlerHolder.get_handler().clear_process_id()
+        CacheAbleHandlerHolder.get_handler().clear_site_and_project()
```

### Comparing `FicusFramework-3.0.9.post9/src/cloudcelery/celery_config.py` & `FicusFramework-3.1.0/src/cloudcelery/celery_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 # 任务队列的名字
 #CELERY_DEFAULT_QUEUE = '20013'
 
 # 不提前缓存4个任务,收一个任务,做一个任务
 CELERYD_PREFETCH_MULTIPLIER = 1
 
+# 延迟进行ACK的确认,只有当任务结束(成功/失败)后,再进行ACK的确认.这样做的目的是避免执行器进行 PREFETCH.在我们的场景里面预取问题很大
+CELERY_ACKS_LATE = True
+
 # CELERYD_CONCURRENCY = 1     # 并发任务数
 
 # 记录任务的开始状态 否则就只有PENDING状态.   并且这个状态只任务结束24小时内有效.
 CELERY_TRACK_STARTED = True
 
 CELERY_TASK_SEND_SENT_EVENT = True
```

### Comparing `FicusFramework-3.0.9.post9/src/config/BootstrapPropertyLoader.py` & `FicusFramework-3.1.0/src/config/BootstrapPropertyLoader.py`

 * *Files 17% similar despite different names*

```diff
@@ -139,14 +139,34 @@
     if "spring.profiles.active" in environs:
         config.spring_profiles_active = environs["spring.profiles.active"]
         log.info(f"从系统环境变量中获取到spring.profiles.active:{config.spring_profiles_active}")
     elif "SPRING_PROFILES_ACTIVE" in environs:
         config.spring_profiles_active = environs["SPRING_PROFILES_ACTIVE"]
         log.info(f"从系统环境变量中获取到SPRING_PROFILES_ACTIVE:{config.spring_profiles_active}")
 
+    if "WORK_ON_K8S" in environs:
+        config.work_on_k8s = bool(environs["WORK_ON_K8S"])
+        log.info(f"从系统环境变量中获取到WORK_ON_K8S:{config.work_on_k8s}")
+
+    if "K8S_AUTH_SERVER_SERVICE" in environs:
+        config.k8s_auth_server_service = environs["K8S_AUTH_SERVER_SERVICE"]
+        log.info(f"从系统环境变量中获取到K8S_AUTH_SERVER_SERVICE:{config.k8s_auth_server_service}")
+
+    if "K8S_CONFIG_SERVER_SERVICE" in environs:
+        config.k8s_config_server_service = environs["K8S_CONFIG_SERVER_SERVICE"]
+        log.info(f"从系统环境变量中获取到K8S_CONFIG_SERVER_SERVICE:{config.k8s_config_server_service}")
+
+    if "K8S_FICUS_SERVER_SERVICE" in environs:
+        config.k8s_ficus_server_service = environs["K8S_FICUS_SERVER_SERVICE"]
+        log.info(f"从系统环境变量中获取到K8S_FICUS_SERVER_SERVICE:{config.k8s_ficus_server_service}")
+
+    if "K8S_SCHEDULE_SERVER_SERVICE" in environs:
+        config.k8s_schedule_server_service = environs["K8S_SCHEDULE_SERVER_SERVICE"]
+        log.info(f"从系统环境变量中获取到K8S_SCHEDULE_SERVER_SERVICE:{config.k8s_schedule_server_service}")
+
 
 def init_from_environ_property():
     import os
 
     environs = os.environ
     # 第一个: server.port
     if "server.port" in environs:
```

### Comparing `FicusFramework-3.0.9.post9/src/config/annotation.py` & `FicusFramework-3.1.0/src/config/annotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,78 @@
 REMOTE_YML_CONFIG = {}
 
+from functools import wraps
 
 def Value(value):
     """
     spring-cloud的配置获取注解
     :param value: ${zookeeper.timeout:10000}   冒号后面是默认值 可以没有
     :return:
     """
+    @wraps(value)
+    def wrapper(self, *args, **kwargs):  # 包装的具体过程
+        # 这里访问eureka去读取配置文件
+        return lambda tmp_=None: get_value(value,tmp_)
 
-    def decorate(func):
-        def wrapper(*arg, **kvargs):  # 包装的具体过程
-            # 这里访问eureka去读取配置文件
-            return get_value(value)
+    return wrapper
 
-        return wrapper
-
-    return decorate
-
-
-def __get_value(property: str):
+def __get_value(property: str,instance):
     """
         从配置中获取key对应的value
         需要注意有递归的情况
         :param value:
         :return:
         """
     tup = _do_parse_expression(property)
 
     if tup[0] == "":
         # 说明不满足 ${xxxx:xx} 这种格式.  直接返回值
         return _convertStr2Other(tup[1])
 
+    key = tup[0]
+    upper_key = tup[0].replace(".","_").replace("-","_").upper()
+
+    # 校验环境变量里面是否有这个东西
+    if instance is not None:
+        try:
+            environments = instance.__environments__
+            if environments is not None:
+                if key in environments:
+                    return _convertStr2Other(environments[key])
+                elif upper_key in environments:
+                    return _convertStr2Other(environments[upper_key])
+        except:
+            pass
+
+    # 这里增加从环境变量里面去替换的方式
+    import os
+    environs = os.environ
+    if key in environs:
+        return _convertStr2Other(environs[key])
+    elif upper_key in environs:
+        return _convertStr2Other(environs[upper_key])
+
     # 说明满足占位符的格式,开始解析占位符
     # arr[0]有值,说明需要到REMOTE_YML_CONFIG里面去找
     keys = tup[0].split(".")
     tmp = REMOTE_YML_CONFIG
     try:
         for key in keys:
             tmp = tmp[key]
         # 这个地方的tmp 有可能还需要递归做处理
-        return get_value(tmp)
+        return get_value(tmp,instance)
     except Exception as e:
         # 默认值
         if tup[1] is None or tup[1] == ":" or tup[1] == "":
             return None
         else:
             return _convertStr2Other(tup[1][1:])
 
 
-def get_value(property: str):
+def get_value(property: str, instance=None):
     """
     从配置中获取key对应的value
     需要注意有递归的情况
     :param value:
     :return:
     """
     # 这里其实还需要根据${}正则的方式,把字符串拆开. 比如: ${sobeycs.redis.host}:${sobeycs.redis.port} 其实应该拆成3个,分别的递归处理.最后再合并
@@ -62,17 +82,17 @@
 
     import re
     l = re.compile("(\${[\w\.-]+[:[\w]+]*})").split(property)
 
     l = list(filter(lambda x: x if x is not None and x!="" else "",l))
 
     if len(l) >1 :
-        return "".join(map(lambda x:str(x),map(__get_value, l)))
+        return "".join(map(lambda x:str(x),map(lambda v:__get_value(v,instance), l)))
     elif len(l) == 1:
-        return __get_value(l[0])
+        return __get_value(l[0],instance)
     else:
         return property
 
 
 def _do_parse_expression(value):
     """
     解析表达式
```

### Comparing `FicusFramework-3.0.9.post9/src/discovery/__init__.py` & `FicusFramework-3.1.0/src/discovery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,20 +122,25 @@
         eureka_client.init_discovery_client(eureka_server=server, renewal_interval_in_secs=renewal_interval_in_secs)
 
     def deregistry(self):
         # 这个不需要
         pass
 
     def check_instance_available(self, app_name):
-        cli = eureka_client.get_discovery_client()
-        if cli is None:
-            raise Exception("Discovery Client has not initialized. ")
-        app = cli.applications.get_application(app_name.upper())
-        if app.instances is None or len(app.instances) == 0:
-            raise ServiceNoInstanceException(f"{app_name}服务没有找到可用的实例")
+
+        from config import work_on_k8s
+        if not work_on_k8s:
+            # 如果没有在k8s上,就去从注册中心上找
+            cli = eureka_client.get_discovery_client()
+            if cli is None:
+                raise Exception("Discovery Client has not initialized. ")
+            app = cli.applications.get_application(app_name.upper())
+            if app.instances is None or len(app.instances) == 0:
+                raise ServiceNoInstanceException(f"{app_name}服务没有找到可用的实例")
+        # 如果在k8s上,就不需要去判断
 
     def heartbeat(self):
         # 这个不需要
         pass
 
     def do_service(self, service="", return_type="json", app_name="sobeyficus", prefer_ip=False, prefer_https=False,
                    method="GET", headers=None, params=None, data=None, timeout=None, auth=True):
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceProxyService.py` & `FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyService.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # Author: lvbiao
 # Created on 2019/1/21
+# 2023-04-14 15:54:02 被废弃,请使用V2版本
+import logging
 from abc import abstractmethod
 
-import logging
 import requests
 from munch import Munch
 
 from api.exceptions import ServiceInnerException, IllegalArgumentException, AuthException
+from api.model.FactDatasourceQueryParameter import FactDatasourceQueryParameter
 from client import check_instance_avaliable, do_service
 from config.annotation import Value
 from factdatasource.FactDatasourceContext import FactDatasourceContext
 from factdatasource.FactDatasourceContextHolder import FactDatasourceContextHolder
-from factdatasource.dao.jdbc.MultipleJdbcDatasource import register_jdbc_default_datasource
-from factdatasource.dao.kafka.MultipleKafkaDatasource import register_kafka_default_datasource
-from factdatasource.message.FactDatasourceMessageHanlder import FactDatasourceChangeListener
+from libs import HeaderHolder
 from libs.utils import Singleton
 from service.FactDatasourceService import FactDatasourceService
 
 log = logging.getLogger('Ficus')
 
+
 class FactDatasourceProxy(object):
 
     @abstractmethod
     def fd(self, fd_code: str):
         """
         返回fd对象
         :param fd_code:
@@ -77,14 +78,24 @@
         :param fd_code:
         :param query: 查询语句
         :param parameters: 查询参数
         :return: Page
         """
 
     @abstractmethod
+    def query_data(self, fd_code: str, query: str, parameters: dict):
+        """
+        使用查询语句查询数据
+        :param fd_code:
+        :param query: 查询语句
+        :param parameters: 查询参数
+        :return: Page
+        """
+
+    @abstractmethod
     def inserts(self, fd_code: str, result_list: list) -> list:
         """
         批量保存数据,要求list里面的字段和数据库里面的字段一一对应
         :param fd_code:
         :param result_list: 要保存的数据
         :return:
         """
@@ -160,46 +171,46 @@
 
     def fd(self, fd_code: str):
         """
         返回fd对象
         :param fd_code:
         :return: FactDatasource
         """
-        return self._get_fd_context(fd_code).fd()
+        return self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE), fd_code).fd()
 
     def size(self, fd_code: str):
         """
         返回数据总长度
         :param fd_code:
         :return: 数据条数:long
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'read')
         return fd_context.size()
 
     def is_empty(self, fd_code: str):
         """
         返回是否存在数据
         :param fd_code:
         :return: boolean
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'read')
         return fd_context.is_empty()
 
     def collect(self, fd_code: str, offset: int, size: int, only_model_field: bool = False):
         """
         返回指定条数的数据
         :param offset:
         :param only_model_field:
         :param fd_code:
         :param size: 返回的条数
         :return: list
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'read')
         result = fd_context.collect(size)
         # 这里需要对查询结果做字段过滤
         self._inner_field_permission(fd_context, result, only_model_field)
         return result
 
     def collect_conditions(self, fd_code: str, offset: int, size: int, condition_groups: list, only_model_field: bool = False):
@@ -208,100 +219,103 @@
         :param offset:
         :param only_model_field:
         :param fd_code:
         :param size: 返回的条数
         :param condition_groups: 查询条件
         :return: list
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'read')
         result = fd_context.collect_conditions(size, condition_groups)
         # 这里需要对查询结果做字段过滤
         self._inner_field_permission(fd_context, result, only_model_field)
         return result
 
     def query(self, fd_code: str, query: str, parameters: dict):
         """
         使用查询语句查询数据
         :param fd_code:
         :param query: 查询语句
         :param parameters: 查询参数
         :return: Page
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'read')
         result = fd_context.query(query, parameters)
         # 这里需要对查询结果做字段过滤
         self._inner_field_permission(fd_context, result, False)
         return result
 
+    def query_data(self, fd_code: str, query: str, parameters: dict):
+        self.query(fd_code, query, parameters)
+
     def inserts(self, fd_code: str, result_list: list) -> list:
         """
         批量保存数据,要求list里面的字段和数据库里面的字段一一对应
         :param fd_code:
         :param result_list: 要保存的数据
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'write')
         return fd_context.inserts(result_list)
 
     def updates(self, fd_code: str, result_list: list) -> list:
         """
         批量更新数据,要求list里面的字段和数据库里面的字段一一对应
         采用ByPrimaryKeySelective的方式,也就是主键必填,其他的字段非空就是要修改的
         :param fd_code:
         :param result_list: 要修改的数据
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'write')
         return fd_context.updates(result_list)
 
     def save_or_updates(self, fd_code: str, result_list: list) -> list:
         """
         批量saveOrUpdate数据,,数据,要求list里面的字段和数据库里面的字段一一对应
         采用ByPrimaryKeySelective的方式,也就是主键必填,其他的字段非空就是要修改的
         :param fd_code:
         :param result_list: 要添加或者需要修改的数据
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'write')
         return fd_context.inserts_or_updates(result_list)
 
     def delete_all(self, fd_code: str):
         """
         清空数据
         :param fd_code:
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'delete')
         return fd_context.delete_all()
 
     def delete(self, fd_code: str, query: str):
         """
         根据删除语句删除数据,query是完整的删除语句
         :param fd_code:
         :param query:
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'delete')
         return fd_context.delete(query)
 
     def delete_conditions(self, fd_code: str, condition_groups: list):
         """
         根据删除条件,构造删除语句
         :param fd_code:
         :param condition_groups: 传入的是 ConditionGroup对象
         :return:
         """
-        fd_context = self._get_fd_context(fd_code)
+        fd_context = self._get_fd_context(HeaderHolder.get_value(HeaderHolder.SITE), HeaderHolder.get_value(HeaderHolder.PROJECT_CODE),fd_code)
         self._inner_check_permission(fd_context, 'delete')
         return fd_context.delete_conditions(condition_groups)
 
     # def get_fact_datasource_fields(self, fd_code: str):
     #     """
     #     获取fd的字段
     #     :param fd_code:
@@ -320,18 +334,19 @@
         if not fd_codes:
             return False
 
         if not isinstance(fd_codes, list):
             raise IllegalArgumentException("检测fd是否存在失败,输入参数不是一个list")
 
         fd_service = FactDatasourceService.instance()
-        return fd_service.exists_fds(fd_codes)
+        return fd_service.exists_fds(HeaderHolder.get_value(HeaderHolder.SITE),
+                                     HeaderHolder.get_value(HeaderHolder.PROJECT_CODE), fd_codes)
 
-    def _get_fd_context(self, fd_code: str):
-        fd_context: FactDatasourceContext = FactDatasourceContextHolder.instance().get_fact_datasource(fd_code)
+    def _get_fd_context(self, site: str, project_code: str, fd_code: str):
+        fd_context: FactDatasourceContext = FactDatasourceContextHolder.instance().get_fact_datasource(site,project_code,fd_code)
         return fd_context
 
     def _inner_check_permission(self, fd_context: FactDatasourceContext, operation: str):
         # TODO 暂未实现内容权限验证
         return True
 
     def _inner_field_permission(self, fd_context, result, only_model_field):
@@ -349,15 +364,15 @@
         获取某一个FD对象
         :param fd_code: fd的唯一code
         :return: FD对象
         """
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}")
+            r = do_service(f"/remote/fd-service/{fd_code}",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
 
             if r is not None:
                 return Munch(r)
             else:
                 return None
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
@@ -373,15 +388,15 @@
         获取数据的条数
         :param fd_code:  fd的唯一code
         :return: 数据的条数 没得就返回0
         """
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}/size")
+            r = do_service(f"/remote/fd-service/{fd_code}/size",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
 
             if r is not None:
                 return r
             else:
                 return 0
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
@@ -397,15 +412,15 @@
         判断数据集是否为空
         :param fd_code: fd的唯一code
         :return: 如果为空返回True,否则返回False
         """
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}/empty")
+            r = do_service(f"/remote/fd-service/{fd_code}/empty",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
 
             if r is not None:
                 return r
             else:
                 return True
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
@@ -424,15 +439,15 @@
         :param size:
         :param fd_code: fd的唯一code
         :return:
         """
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}/all", params={'offset': offset, 'size': size, 'onlyModelField': only_model_field})
+            r = do_service(f"/remote/fd-service/{fd_code}/all", params={'offset': offset, 'size': size, 'onlyModelField': only_model_field},headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return Munch(r)
             else:
                 return None
@@ -455,15 +470,15 @@
         :param condition_groups: 查询条件
         :return: list
         """
         check_instance_avaliable()
 
         try:
             r = do_service(f"/remote/fd-service/{fd_code}/conditions", method="post", data=condition_groups,
-                           params={'offset': offset, 'size': size, 'onlyModelField': only_model_field})
+                           params={'offset': offset, 'size': size, 'onlyModelField': only_model_field},headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return Munch(r)
             else:
                 return None
@@ -484,15 +499,44 @@
         :param parameters: 查询可能涉及的参数 K/V形式
         :return:
         """
         check_instance_avaliable()
 
         try:
             r = do_service(f"/remote/fd-service/{fd_code}/query", method="post", data=parameters,
-                           params={'query': query})
+                           params={'query': query},headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
+
+            if r is not None:
+                if isinstance(r, list):
+                    return [Munch(x) for x in r]
+                else:
+                    return Munch(r)
+            else:
+                return None
+        except requests.exceptions.HTTPError as e:
+            if e.response.status_code == 500:
+                # 说明服务器端报错了
+                raise ServiceInnerException(e.response._content.decode('utf-8'))
+            elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
+                # 说明是认证相关的错误
+                raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
+            raise e
+
+    def query_data(self, fd_code: str, query: str, parameters: dict):
+        """
+        对数据集进行查询
+        :param fd_code: fd的唯一code
+        :param query: 查询语句
+        :param parameters: 查询可能涉及的参数 K/V形式
+        :return:
+        """
+        check_instance_avaliable()
+        query_parameter = FactDatasourceQueryParameter(query, parameters)
+        try:
+            r = do_service(f"/remote/fd-service/{fd_code}/queryData", method="post", data=dict(query_parameter),headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
 
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return Munch(r)
             else:
@@ -527,15 +571,15 @@
                 # 这里所有类型都要添加进去
                 request.append(result)
             else:
                 # 说明是munch的,那么就转成Dict的
                 request.append(result.toDict())
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}", method="post", data=request, return_type="json")
+            r = do_service(f"/remote/fd-service/{fd_code}", method="post", data=request, return_type="json",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return None
             else:
                 return None
@@ -569,15 +613,15 @@
                 # 这里所有类型都要添加进去
                 request.append(result)
             else:
                 # 说明是munch的,那么就转成Dict的
                 request.append(result.toDict())
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}", method="put", data=request, return_type="json")
+            r = do_service(f"/remote/fd-service/{fd_code}", method="put", data=request, return_type="json",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return None
             else:
                 return None
@@ -611,15 +655,15 @@
                 # 这里所有类型都要添加进去
                 request.append(result)
             else:
                 # 说明是munch的,那么就转成Dict的
                 request.append(result.toDict())
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}/upsert", method="post", data=request, return_type="json")
+            r = do_service(f"/remote/fd-service/{fd_code}/upsert", method="post", data=request, return_type="json",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 if isinstance(r, list):
                     return [Munch(x) for x in r]
                 else:
                     return None
             else:
                 return None
@@ -637,15 +681,15 @@
         删除数据集中所有数据
         :param fd_code: fd的唯一code
         :return:
         """
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/{fd_code}", method="delete", return_type="None")
+            r = do_service(f"/remote/fd-service/{fd_code}", method="delete", return_type="None",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
                 # 说明服务器端报错了
                 raise ServiceInnerException(e.response._content.decode('utf-8'))
             elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
                 # 说明是认证相关的错误
                 raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
@@ -658,15 +702,15 @@
         :param query_str: 查询语句
         :return:
         """
         check_instance_avaliable()
 
         try:
             r = do_service(f"/remote/fd-service/{fd_code}/query", method="delete", params={'query': query},
-                           return_type="None")
+                           return_type="None",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
                 # 说明服务器端报错了
                 raise ServiceInnerException(e.response._content.decode('utf-8'))
             elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
                 # 说明是认证相关的错误
                 raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
@@ -679,15 +723,15 @@
         :param condition_groups:
         :return:
         """
         check_instance_avaliable()
 
         try:
             r = do_service(f"/remote/fd-service/{fd_code}/conditions", method="delete", data=condition_groups,
-                           return_type="None")
+                           return_type="None",headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
                 # 说明服务器端报错了
                 raise ServiceInnerException(e.response._content.decode('utf-8'))
             elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
                 # 说明是认证相关的错误
                 raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
@@ -695,17 +739,36 @@
 
     def get_fact_datasource_fields(self, fd_code: str):
         """
         获取fd的字段
         :param fd_code:
         :return: List<FactDatasourceField>
         """
-        fd_context = self._get_fd_context(fd_code)
-        self._inner_check_permission(fd_context, 'execute')
-        return fd_context.get_fact_datasource_fields()
+        check_instance_avaliable()
+
+        try:
+            r = do_service(f"/remote/fd-service/{fd_code}/fields", method="get",
+                           return_type="json", headers={HeaderHolder.SITE: HeaderHolder.get_value(HeaderHolder.SITE),
+                                                        HeaderHolder.PROJECT_CODE: HeaderHolder.get_value(
+                                                            HeaderHolder.PROJECT_CODE)})
+            if r is not None:
+                if isinstance(r, list):
+                    return [Munch(x) for x in r]
+                else:
+                    return None
+            else:
+                return None
+        except requests.exceptions.HTTPError as e:
+            if e.response.status_code == 500:
+                # 说明服务器端报错了
+                raise ServiceInnerException(e.response._content.decode('utf-8'))
+            elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
+                # 说明是认证相关的错误
+                raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
+            raise e
 
     def exists_fds(self, fds):
         """
         判断fd是否存在
         :param fds:
         :return:
         """
@@ -714,15 +777,15 @@
 
         if not isinstance(fds, list):
             raise IllegalArgumentException("检测fd是否存在失败,输入参数不是一个list")
 
         check_instance_avaliable()
 
         try:
-            r = do_service(f"/remote/fd-service/exists", method="post", data=fds)
+            r = do_service(f"/remote/fd-service/exists", method="post", data=fds,headers={HeaderHolder.SITE:HeaderHolder.get_value(HeaderHolder.SITE),HeaderHolder.PROJECT_CODE:HeaderHolder.get_value(HeaderHolder.PROJECT_CODE)})
             if r is not None:
                 return r
             else:
                 return False
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 500:
                 # 说明服务器端报错了
@@ -746,20 +809,14 @@
             return self.__instance
 
         if mode is None:
             mode = distributed_mode()
 
         if mode:
             log.info("服务启动,使用本地模式FD服务")
-            # 注册本地数据源
-            register_jdbc_default_datasource()
-            # 注册kafka默认的数据源
-            register_kafka_default_datasource()
-            # 启动FD改变事件消息监听
-            FactDatasourceChangeListener.instance().start()
             # 获取本地操作实例
             self.__instance = DistributedFactDatasourceProxy.instance()
         else:
             log.info("服务启动,使用中心模式FD服务")
             self.__instance = CentralizedFactDatasourceProxy.instance()
         return self.__instance
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceContextHolder.py` & `FicusFramework-3.1.0/src/factdatasource/FactDatasourceContextHolder.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,49 +20,65 @@
     # fd_code ---> FactDatasource
     __fact_datasource_cache = dict()
 
     @property
     def _fd_service(self):
         return FactDatasourceService.instance()
 
-    def get_fact_datasource(self, fd_code: str) -> FactDatasourceContext:
+    def get_fact_datasource(self, site: str, project_code: str, fd_code: str) -> FactDatasourceContext:
         """
         获取一个fd_context的实现
         这里逻辑应该是这样，先通过rest接口取到fd的定义信息，然后根据这个定义信息构造fd_context
+        :param project_code:
+        :param site:
         :param fd_code:
         :return:
         """
-        if fd_code in self.__fact_datasource_context_cache.keys():
-            return self.__fact_datasource_context_cache.get(fd_code)
 
-        if fd_code not in self.__fact_datasource_cache.keys():
-            fact_datasource: FactDatasource = self._fd_service.get_fd_by_code(fd_code)
+        if site is None or project_code is None:
+            # 这里完全是为了兼容原来的程序,万一原来的CE这些并没有升级,从而导致并没有传入site/projectCode过来
+            for code in self.__fact_datasource_context_cache.keys():
+                if code.endswith(fd_code):
+                    return self.__fact_datasource_context_cache.get(code)
+            raise FDNotExistsException(f'数据源{fd_code}不存在')
+
+        source_name = self.__generate_source_name(site,project_code,fd_code)
+
+        if source_name in self.__fact_datasource_context_cache.keys():
+            return self.__fact_datasource_context_cache.get(source_name)
+
+        if source_name not in self.__fact_datasource_cache.keys():
+            fact_datasource: FactDatasource = self._fd_service.get_fd_by_code(site, project_code, fd_code)
             if not fact_datasource:
-                raise FDNotExistsException(f'数据源{fd_code}不存在')
+                raise FDNotExistsException(f'数据源{source_name}不存在')
         else:
-            fact_datasource = self.__fact_datasource_cache.get(fd_code)
+            fact_datasource = self.__fact_datasource_cache.get(source_name)
 
         if self.add_fact_datasource(fact_datasource):
-            return self.__fact_datasource_context_cache.get(fd_code)
+            return self.__fact_datasource_context_cache.get(source_name)
 
     def remove_fact_datasource(self, fact_datasource: FactDatasource):
         """
         删除一个fd实现
         这里只有消息监听处会调用，其他地方暂时没有调用这里的
         :param fact_datasource:
         :return:
         """
+        site = fact_datasource.site
+        project_code = fact_datasource.projectCode
         fd_code = fact_datasource.code
-        if self.is_using_fact_datasource(fd_code):
-            raise FDOperationException(f'数据源{fd_code}正在使用，无法删除。')
+        source_name = self.__generate_source_name(site,project_code,fd_code)
 
-        if fd_code in self.__fact_datasource_context_cache.keys():
-            del self.__fact_datasource_context_cache[fd_code]
-        if fd_code in self.__fact_datasource_cache.keys():
-            del self.__fact_datasource_cache[fd_code]
+        if self.is_using_fact_datasource(site,project_code,fd_code):
+            raise FDOperationException(f'数据源{source_name}正在使用，无法删除。')
+
+        if source_name in self.__fact_datasource_context_cache.keys():
+            del self.__fact_datasource_context_cache[source_name]
+        if source_name in self.__fact_datasource_cache.keys():
+            del self.__fact_datasource_cache[source_name]
 
         # 删除数据源中的配置
         if self._need_datasource(fact_datasource.type):
             get_multiple_datesource(fact_datasource.type).delete_datasource_type(fact_datasource.get_source_name())
         return True
 
     def add_fact_datasource(self, fact_datasource: FactDatasource):
@@ -70,61 +86,71 @@
         增加一个fd实现
         :param fact_datasource:
         :return:
         """
         if fact_datasource is None or fact_datasource.code is None:
             return False
 
+        site = fact_datasource.site
+        project_code = fact_datasource.projectCode
         fd_code = fact_datasource.code
+        source_name = self.__generate_source_name(site,project_code,fd_code)
+
         # 放到缓存中
-        if fd_code not in self.__fact_datasource_cache.keys():
-            self.__fact_datasource_cache[fd_code] = fact_datasource
+        if source_name not in self.__fact_datasource_cache.keys():
+            self.__fact_datasource_cache[source_name] = fact_datasource
 
         fact_datasource_context = self.__get_fact_datasource_context(fact_datasource)
         if fact_datasource_context:
-            self.__fact_datasource_context_cache[fd_code] = fact_datasource_context
+            self.__fact_datasource_context_cache[source_name] = fact_datasource_context
             # 添加到数据源中
             if self._need_datasource(fact_datasource.type):
                 get_multiple_datesource(fact_datasource.type).add_datasource_type(fact_datasource.get_source_name(),
                                                                                   fact_datasource.connection,
                                                                                   fact_datasource.credentials)
             return True
         return False
 
     def update_fact_datasource(self, fact_datasource: FactDatasource):
         """
         FD修改
         :param fact_datasource:
         :return:
         """
+        site = fact_datasource.site
+        project_code = fact_datasource.projectCode
         fd_code = fact_datasource.code
-        if self.is_using_fact_datasource(fd_code):
+        if self.is_using_fact_datasource(site, project_code, fd_code):
             raise FDOperationException(f'数据源{fd_code}正在使用，无法修改。')
         self.remove_fact_datasource(fact_datasource)
         self.add_fact_datasource(fact_datasource)
 
-    def is_loaded_fact_datasource(self, fd_code: str) -> bool:
+    def is_loaded_fact_datasource(self, site: str, project_code: str, fd_code: str) -> bool:
         """
         判断fd_code是否已经加载
+        :param project_code:
+        :param site:
         :param fd_code:
         :return:
         """
-        return fd_code in self.__fact_datasource_cache.keys()
+        return self.__generate_source_name(site, project_code, fd_code) in self.__fact_datasource_cache.keys()
 
-    def is_using_fact_datasource(self, fd_code: str) -> bool:
+    def is_using_fact_datasource(self, site: str, project_code: str, fd_code: str) -> bool:
         """
         判断fd_code是否正在使用，正在使用表示正在读写数据或者查询数据
+        :param project_code:
+        :param site:
         :param fd_code:
         :return:
         """
         # 没在内存中肯定就没有被使用
-        if not self.is_loaded_fact_datasource(fd_code):
+        if not self.is_loaded_fact_datasource(site,project_code,fd_code):
             return False
 
-        fd: FactDatasource = self.__fact_datasource_cache.get(fd_code)
+        fd: FactDatasource = self.__fact_datasource_cache.get(self.__generate_source_name(site, project_code, fd_code))
         return customer_dao_context_holder.is_using(fd.get_source_name())
 
     def _need_datasource(self, fd_type: FactDatasourceTypeEnum):
         """
         判断某一个fd是否需要使用数据源，比如sobeyhvie这种直接调用rest接口的，就不需要使用数据源
         默认都应该使用的
         :param fd_type:
@@ -206,12 +232,18 @@
             fd_context = RedisFactDatasourceContext(fact_datasource)
         elif fd_type == FactDatasourceTypeEnum.SOBEY_HIVE:
             from factdatasource.persistence.sobeyhive.SobeyHiveFactDatasourceContext import SobeyHiveFactDatasourceContext
             fd_context = SobeyHiveFactDatasourceContext(fact_datasource)
         elif fd_type == FactDatasourceTypeEnum.ALGORITHM:
             from factdatasource.persistence.algorithm.AlgorithmFactDatasourceContext import AlgorithmDatasourceContext
             fd_context = AlgorithmDatasourceContext(fact_datasource)
+        elif fd_type == FactDatasourceTypeEnum.TABLESTORE:
+            from factdatasource.persistence.tablestore.TableStoreDatasourceContext import TableStoreDatasourceContext
+            fd_context = TableStoreDatasourceContext(fact_datasource)
         else:
             raise NotSupportedFDException(f'暂不支持该FD类型{fd_type}')
 
         return fd_context
 
+
+    def __generate_source_name(self,site:str,project_code:str,code:str)->str:
+        return f"{site}_{project_code}_{code}"
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/ChineseToNumberTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/ChineseToNumberTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/TransformerContext.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/TransformerContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/ITransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/ITransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/CompleteGB32100Transformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/CompleteGB32100Transformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/FixItemTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/FixItemTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/ParseDateTimeTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/ParseDateTimeTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/DefaultValueTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/DefaultValueTransformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,30 @@
         # 默认值,String的
         default_string = params[DEFAULT_VALUE_KEY]
 
         # 需要根据字段类型进行变更
         # 找到目标字段类型
         data_type = target_model_field.dataType
 
-        if data_type == DataTypeEnum.STRING:
+        if data_type == DataTypeEnum.STRING or data_type == DataTypeEnum.JSON:
             return {target_model_field.fieldName: default_string if old_value is None else old_value}
         elif data_type in [DataTypeEnum.FLOAT, DataTypeEnum.LONG, DataTypeEnum.INTEGER, DataTypeEnum.DOUBLE]:
             return {target_model_field.fieldName: self.__inner_number_convert(old_value, data_type, default_string)}
         elif data_type == DataTypeEnum.DATE:
             return {target_model_field.fieldName: self.__inner_date_convert(old_value,
                                              DEFAULT_DATE_FORMAT if DATE_FORMAT_KEY not in params else params[
                                                  DATE_FORMAT_KEY], default_string)}
         elif data_type == DataTypeEnum.BOOLEAN:
             return {target_model_field.fieldName: self.__inner_boolean_convert(old_value, default_string)}
         elif data_type == DataTypeEnum.CHAR:
             return {target_model_field.fieldName: self.__inner_char_convert(old_value, default_string)}
         elif data_type == DataTypeEnum.BYTE:
             return {target_model_field.fieldName: self.__inner_byte_convert(old_value, default_string)}
+        else:
+            return None
 
     def __inner_number_convert(self, old_value, data_type, default_string):
         if old_value is not None:
             return old_value
 
         if data_type == DataTypeEnum.Long or data_type == DataTypeEnum.INTEGER:
             return int(default_string)
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/CompleteStringTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/CompleteStringTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/transformer/NumberToChineseTransformer.py` & `FicusFramework-3.1.0/src/factdatasource/transformer/NumberToChineseTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/MultipleDatasourceHolder.py` & `FicusFramework-3.1.0/src/factdatasource/dao/MultipleDatasourceHolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,12 @@
         return MultipleJdbcDatasource.instance()
     elif fd_type == FactDatasourceTypeEnum.AMQP:
         from factdatasource.dao.amqp.MultipleAmqpDatasource import MultipleAmqpDatasource
         return MultipleAmqpDatasource.instance()
     elif fd_type == FactDatasourceTypeEnum.JMS:
         from factdatasource.dao.stomp.MultipleStompDatasource import MultipleStompDatasource
         return MultipleStompDatasource.instance()
+    elif fd_type == FactDatasourceTypeEnum.TABLESTORE:
+        from factdatasource.dao.tablestore.MultipleTableStoreDatasource import MultipleTableStoreDatasource
+        return MultipleTableStoreDatasource.instance()
     else:
         raise NotSupportedFDException(f'暂未支持{fd_type}类型的数据源')
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/RedisDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/redis/RedisDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/redis/MultipleRedisDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/redis/MultipleRedisDatasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # Author: lvbiao
 # Created on 2019/1/22
 from enum import Enum
+from urllib.parse import unquote
 
 from redis import StrictRedis
 
 from api.exceptions import IllegalArgumentException
 from api.model.FactDatasource import FactDatasourceTypeEnum
 from factdatasource.execptions import DatasourceNotFoundException, FDExecuteException
 from factdatasource.dao.FactDatasource import DatasourceListener, MultipleBaseDatasource, BaseDatasource
@@ -180,15 +181,15 @@
                 url_tmp = {}
                 if ':' in url_split:
                     url_tmp['host'] = url_split.split(':', 1)[0]
                     url_tmp['port'] = int(url_split.split(':', 1)[1])
                 else:
                     url_tmp['host'] = url_split
                 if password:
-                    url_tmp['password'] = password
+                    url_tmp['password'] = unquote(password)
 
                 result.append(url_tmp)
             return (type, result,)
         elif ';' in self.url:
             # 哨兵配置  [('localhost', 26379)]
             type = RedisTypeEnum.SENTINEL
             url_split = str(self.url).split(';')
@@ -203,10 +204,10 @@
                 else:
                     result.append((host_port,))
             return (type, master_service, result,)
         else:
             # 普通单节点
             type = RedisTypeEnum.SINGLE
             # 构造url:  redis://[:password]@localhost:6379/0
-            password = ':' + str(password) + '@' if password else ''
+            password = ':' + unquote(str(password)) + '@' if password else ''
             url = f'redis://{password}{self.url}'
             return (type, url)
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/graph/GraphDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/graph/GraphDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/graph/__init__.py` & `FicusFramework-3.1.0/src/factdatasource/dao/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # Author: lvbiao
 # Created on 2019/1/22
+from urllib.parse import unquote
+
 import pika
 from pika import BlockingConnection
 
 from api.exceptions import IllegalArgumentException
 from api.model.FactDatasource import FactDatasourceTypeEnum
 from factdatasource.dao.FactDatasource import DatasourceListener, MultipleBaseDatasource, BaseDatasource
 from factdatasource.execptions import DatasourceNotFoundException, FDExecuteException
@@ -123,15 +125,15 @@
         """
         # rabbitmq暂时不支持多个url连接，如果是集群，最好配合HA做高可用配置后在连接
         con_param = self._parse_url()
         if self.credentials:
             credentials_list = self.credentials.split(':')
             username = credentials_list[0]
             password = credentials_list[1] if len(credentials_list) > 1 else ''
-            con_param['credentials'] = pika.PlainCredentials(username, password)
+            con_param['credentials'] = pika.PlainCredentials(unquote(username), unquote(password))
 
         block_con_param = pika.ConnectionParameters(**con_param)
         self.client = pika.BlockingConnection(block_con_param)
 
     def get_client(self):
         return self.client
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/amqp/AmqpDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/amqp/AmqpDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # Author: lvbiao
 # Created on 2019/1/22
 import threading
+from urllib.parse import unquote
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session, sessionmaker
 from urllib3.util import url, Url
 
 from api.exceptions import IllegalArgumentException
 from api.model.FactDatasource import JdbcTypeEnum, JdbcDriverEnum, FactDatasourceTypeEnum
@@ -228,15 +229,15 @@
                 for key, value in url_param.items():
                     query = query + str(key) + '=' + str(value) + '&'
                 # 删除最后一个&
                 query = query.rstrip('&')
 
             path = '/' + str(database)
 
-            result_url = Url(scheme=sqlalchemy_scheme.value, auth=self._credentials, host=r.host, port=r.port,
+            result_url = Url(scheme=sqlalchemy_scheme.value, auth=unquote(self._credentials), host=r.host, port=r.port,
                              path=path, query=query, fragment=r.fragment)
         elif jdbc_type == JdbcTypeEnum.ORACLE:
             # JDBC的常用形式是
             # 1.普通SID方式
             # jdbc:oracle:thin:username/password@x.x.x.1:1521:SID
             # 2.普通ServiceName 方式
             # jdbc:oracle:thin:username/password@//x.x.x.1:1522/ABCD
@@ -283,30 +284,30 @@
 
             import cx_Oracle
             if service_name:
                 dsn = cx_Oracle.makedsn(host, port, service_name=service_name)
             else:
                 dsn = cx_Oracle.makedsn(host, port, sid=sid)
 
-            credentials = str(self._credentials) + '@' if self._credentials else ''
+            credentials = unquote(str(self._credentials)) + '@' if self._credentials else ''
             return f'{sqlalchemy_scheme.value}://{credentials}{dsn}'
         else:
             # 默认可以使用的比较通用的构造方式
             r = url.parse_url(jdbc_url.split(":", 1)[1])
             # sqlalchemy mysql 这里中文一直是乱码，暂时先手动设置下编码
             query = r.query
             if jdbc_type == JdbcTypeEnum.MYSQL or jdbc_type == JdbcTypeEnum.VERNOX or jdbc_type == JdbcTypeEnum.VERNOX_NTS:
                 if not query:
                     query = 'charset=utf8mb4'
                 elif str(query).lower().find('charset=') == -1:
                     query = query + '&charset=utf8mb4'
                 # 需要去掉 useSSL=true/false
                 query = "&".join(list(filter(lambda x: x.split("=")[0] not in ["useSSL", "_type_"], query.split("&"))))
 
-            result_url = Url(scheme=sqlalchemy_scheme.value, auth=self._credentials, host=r.host, port=r.port,
+            result_url = Url(scheme=sqlalchemy_scheme.value, auth=unquote(self._credentials), host=r.host, port=r.port,
                              path=r.path, query=query, fragment=r.fragment)
         return result_url.url
 
 
 @Value("${jdbc.ip}")
 def jdbc_ip():
     pass
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/kafka/KafkaDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/kafka/KafkaDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/MultipleStompDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/stomp/MultipleStompDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/stomp/StompDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/stomp/StompDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/MongoDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/mongo/MongoDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/mongo/MultipleMongoDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/mongo/MultipleMongoDatasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 # Author: lvbiao
 # Created on 2019/1/22
-from urllib.parse import quote_plus
+from urllib.parse import quote_plus, unquote
 
 from pymongo import MongoClient
 from pymongo.database import Database
 
 from api.exceptions import IllegalArgumentException
 from api.model.FactDatasource import FactDatasourceTypeEnum
 from factdatasource.dao.FactDatasource import DatasourceListener, MultipleBaseDatasource, BaseDatasource
@@ -150,16 +150,16 @@
                 con_credential = self.credentials
                 user_db = "admin"
         else:
             con_credential = ''
             user_db = "admin"
 
         if con_credential and ':' in con_credential:
-            uri_credential = quote_plus(con_credential[0:con_credential.find(':')]) + ':' \
-                             + quote_plus(con_credential[con_credential.find(':') + 1:]) + '@'
+            uri_credential = quote_plus(unquote(con_credential[0:con_credential.find(':')])) + ':' \
+                             + quote_plus(unquote(con_credential[con_credential.find(':') + 1:])) + '@'
         else:
             uri_credential = ''
 
         if not self.url or '@' not in self.url:
             raise IllegalArgumentException(f'mongo连接信息配置错误，无法进行连接：{self.url}')
 
         con_url = self.url[0:self.url.find('@')]
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/es/EsDatasourceDao.py` & `FicusFramework-3.1.0/src/factdatasource/dao/es/EsDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/es/MultipleEsDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/es/MultipleEsDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/dao/FactDatasource.py` & `FicusFramework-3.1.0/src/factdatasource/dao/FactDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/__init__.py` & `FicusFramework-3.1.0/src/factdatasource/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/message/FactDatasourceMessageHanlder.py` & `FicusFramework-3.1.0/src/factdatasource/message/FactDatasourceMessageHanlder.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 
 log = logging.getLogger('Ficus')
 
 
 def wait_using_fd(fd_context_holder: FactDatasourceContextHolder, action: int, fact_datasource: FactDatasource):
     def listen_using_fd():
         fd_code = fact_datasource.code
-        if fd_context_holder.is_using_fact_datasource(fd_code):
-            while fd_context_holder.is_using_fact_datasource(fd_code):
-                log.debug(f'监听到数据源{fd_code}的{action}事件，等待数据源使用完毕')
+        site = fact_datasource.site
+        project_code = fact_datasource.projectCode
+        if fd_context_holder.is_using_fact_datasource(site, project_code, fd_code):
+            while fd_context_holder.is_using_fact_datasource(site, project_code, fd_code):
+                log.debug(f'监听到数据源{site}_{project_code}_{fd_code}的{action}事件，等待数据源使用完毕')
                 time.sleep(0.5)
 
         if action == FactDatasourceChangeListener.ACTION_UPDATE:
             fd_context_holder.update_fact_datasource(fact_datasource)
         elif action == FactDatasourceChangeListener.ACTION_DELETE:
             fd_context_holder.remove_fact_datasource(fact_datasource)
 
@@ -156,25 +158,25 @@
             # 第二次做遍历
             if datasource.type == "REF" and datasource.ref is not None:
                 tmp = fold_ref_fds(datasource)
                 rrr = list(filter(lambda
                                       actor_fd: actor_fd.site == fact_datasource.site and actor_fd.projectCode == fact_datasource.projectCode and actor_fd.code == fact_datasource.code,
                                   tmp))
                 if rrr is not None and len(rrr) > 0:
-                    changed_fds.add(FactDatasource(**FactDatasourceClient.fd(datasource.code)))       # TODO 这里是有问题的,应该使用 FactDatasourceClient.fd(fd_code)
+                    changed_fds.add(FactDatasource(**FactDatasourceClient.fd(datasource.site, datasource.projectCode, datasource.code)))       # TODO 这里是有问题的,应该使用 FactDatasourceClient.fd(fd_code)
             else:
                 if datasource.site == fact_datasource.site and datasource.projectCode == fact_datasource.projectCode and datasource.code == fact_datasource.code:
-                    changed_fds.add(FactDatasource(**FactDatasourceClient.fd(datasource.code)))   # TODO 这里是有问题的,应该使用 FactDatasourceClient.fd(fd_code)
+                    changed_fds.add(FactDatasource(**FactDatasourceClient.fd(datasource.site, datasource.projectCode, datasource.code)))   # TODO 这里是有问题的,应该使用 FactDatasourceClient.fd(fd_code)
 
         for fd in changed_fds:
-            if not self.fd_context_holder.is_loaded_fact_datasource(fd.code):
+            if not self.fd_context_holder.is_loaded_fact_datasource(fd.site, fd.projectCode, fd.code):
                 # 本地数据源还没有使用不进行处理
                 continue
 
-            if self.fd_context_holder.is_using_fact_datasource(fd.code):
+            if self.fd_context_holder.is_using_fact_datasource(fd.site, fd.projectCode,fd.code):
                 wait_num = 0
                 while self.fd_context_holder.is_using_fact_datasource(fd.code):
                     log.debug(f'监听到数据源{fd.code}的{action}事件，等待数据源使用完毕')
                     wait_num += 1
                     time.sleep(0.5)
                     # 5秒都还在使用的话就只能使用新线程来处理了,否则无法处理后续的事件
                     if wait_num > 10:
```

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/file/FileFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/file/FileFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/AbstractFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/AbstractFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/__init__.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/es/EsFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/es/EsFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/SqlableDeleteCondition.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/SqlableDeleteCondition.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/FactDatasourceContext.py` & `FicusFramework-3.1.0/src/factdatasource/FactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/factdatasource/execptions.py` & `FicusFramework-3.1.0/src/factdatasource/execptions.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/libs/utils.py` & `FicusFramework-3.1.0/src/libs/utils.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/py_eureka_client/__urlopen_proxy__.py` & `FicusFramework-3.1.0/src/py_eureka_client/__urlopen_proxy__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/py_eureka_client/http_client.py` & `FicusFramework-3.1.0/src/py_eureka_client/http_client.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/py_eureka_client/eureka_client.py` & `FicusFramework-3.1.0/src/py_eureka_client/eureka_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -949,33 +949,55 @@
         async_thread = Thread(target=async_thread_target)
         async_thread.daemon = True
         async_thread.start()
 
     def walk_nodes(self, app_name="", service="", prefer_ip=False, prefer_https=False, walker=None):
         assert app_name is not None and app_name != "", "application_name should not be null"
         assert inspect.isfunction(walker) or inspect.ismethod(walker), "walker must be a method or function"
-        error_nodes = []
-        app_name = app_name.upper()
-        node = self.__get_available_service(app_name)
 
-        while node is not None:
-            try:
-                url = self.__generate_service_url(node, prefer_ip, prefer_https)
-                if service.startswith("/"):
-                    url = url + service[1:]
-                else:
-                    url = url + service
-                _logger.debug("service url::" + url)
-                return walker(url)
-            except (http_client.HTTPError, http_client.URLError):
-                _logger.warn("do service %s in node [%s] error, use next node." % (service, node.instanceId))
-                error_nodes.append(node.instanceId)
-                node = self.__get_available_service(app_name, error_nodes)
+        from config import work_on_k8s, k8s_ficus_server_service, k8s_config_server_service, k8s_schedule_server_service
+        if work_on_k8s:
+            # 如果运行在k8s服务上,那么就可以不走注册中心
+            # 这里简单的实现
+            url = k8s_ficus_server_service
+            if app_name.lower() == "sobeycloud-schedule-service":
+                url = k8s_schedule_server_service
+            elif app_name.lower() == "sobeyficus-config-server":
+                url = k8s_config_server_service
+            else:
+                url = k8s_ficus_server_service
+            if not url.endswith("/"):
+                url = url + "/"
+            if service.startswith("/"):
+                url = url + service[1:]
+            else:
+                url = url + service
+            _logger.debug("service url::" + url)
+            return walker(url)
+        else:
+            # 如果没运行在k8s服务上
+            error_nodes = []
+            app_name = app_name.upper()
+            node = self.__get_available_service(app_name)
 
-        raise http_client.URLError("Try all up instances in registry, but all fail")
+            while node is not None:
+                try:
+                    url = self.__generate_service_url(node, prefer_ip, prefer_https)
+                    if service.startswith("/"):
+                        url = url + service[1:]
+                    else:
+                        url = url + service
+                    _logger.debug("service url::" + url)
+                    return walker(url)
+                except (http_client.HTTPError, http_client.URLError):
+                    _logger.warn("do service %s in node [%s] error, use next node." % (service, node.instanceId))
+                    error_nodes.append(node.instanceId)
+                    node = self.__get_available_service(app_name, error_nodes)
+
+            raise http_client.URLError("Try all up instances in registry, but all fail")
 
     def do_service_async(self, app_name="", service="", return_type="string",
                          prefer_ip=False, prefer_https=False,
                          on_success=None, on_error=None,
                          method="GET", headers=None,
                          data=None, timeout=_DEFAULT_TIME_OUT,
                          cafile=None, capath=None, cadefault=False, context=None):
```

### Comparing `FicusFramework-3.0.9.post9/src/py_eureka_client/__logger__.py` & `FicusFramework-3.1.0/src/py_eureka_client/__logger__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/registry/LoadOnRegistryLoader.py` & `FicusFramework-3.1.0/src/registry/LoadOnRegistryLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from api.exceptions import IllegalArgumentException
 from client import ComputeExecutionClient, DataCrawlClient
 from config.annotation import Value
-from factdatasource import FactDatasourceProxyService
+from factdatasource import FactDatasourceProxyServiceV2
 
 log = logging.getLogger('Ficus')
 
 
 @Value("${actor.name:unknown}")
 def actor_name():
     pass
@@ -44,15 +44,15 @@
     for computeexecution in registry["computeexecutions"]:
 
         # region 补默认值
         if "code" not in computeexecution or computeexecution["code"] == "" or computeexecution["code"] is None:
             computeexecution["code"] = f"{actor_name()}-{index}"
 
         if "execution" not in computeexecution or computeexecution["execution"] is None:
-            computeexecution["execution"] = {"schedule": "0 0 0 1 1 ? 2099", "limits": -1, "params": []}
+            computeexecution["execution"] = {"schedule": "0 0 0 1 1 ? 2099", "limits": -1, "params": [], "retryTimes": 0}
         else:
             if "schedule" not in computeexecution["execution"] or computeexecution["execution"]["schedule"] is None or \
                     computeexecution["execution"]["schedule"] == "":
                 computeexecution["execution"]["schedule"] = "0 0 0 1 1 ? 2099"
             if "limits" not in computeexecution["execution"] or computeexecution["execution"]["limits"] is None:
                 computeexecution["execution"]["limits"] = -1
             if "params" not in computeexecution["execution"] or computeexecution["execution"]["params"] is None:
@@ -102,15 +102,15 @@
         # endregion
 
         # region 第三轮的校验是对应的fd,是否存在,因为自注册的handler应该不会太多, 它对应的input和output也不会太多,因此,这里就不再先做一次多handler的聚合了
         fds = list()
         fds = fds + computeexecution["inputs"]
         fds += computeexecution["outputs"]
 
-        if not FactDatasourceProxyService.fd_client_proxy().exists_fds(fds):
+        if not FactDatasourceProxyServiceV2.fd_client_proxy().exists_fds(site, projectcode, fds):
             # 只要有一个fd不存在,就返回false
             # 表示校验异常了.
             raise IllegalArgumentException(f"自注册{computeexecution['code']}失败,{fds}不存在")
         # endregion
 
         # 到这的都是要的的
         needRegistryList.append(computeexecution)
@@ -208,15 +208,15 @@
             continue
         # endregion
 
         # region 第三轮的校验是对应的fd,是否存在,因为自注册的handler应该不会太多, 它对应的input和output也不会太多,因此,这里就不再先做一次多handler的聚合了
         fds = list()
         fds += crawl["outputs"]
 
-        if not FactDatasourceProxyService.fd_client_proxy().exists_fds(fds):
+        if not FactDatasourceProxyServiceV2.fd_client_proxy().exists_fds(site, projectcode, fds):
             # 只要有一个fd不存在,就返回false
             # 表示校验异常了.
             raise IllegalArgumentException(f"自注册{crawl['code']}失败,{fds}不存在")
         # endregion
 
         # 到这的都是要的的
         needRegistryList.append(crawl)
```

### Comparing `FicusFramework-3.0.9.post9/src/registry/LoadOnAlgorithmLoader.py` & `FicusFramework-3.1.0/src/registry/LoadOnAlgorithmLoader.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/registry/__init__.py` & `FicusFramework-3.1.0/src/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ICacheAbleHandler.py` & `FicusFramework-3.1.0/src/api/handler/ICacheAbleHandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,25 @@
         :param value:
         :return:
         """
         if key is None or value is None:
             raise IllegalArgumentException("设置任务缓存失败,传入的参数不合法")
         return ScheduleCacheClient.set_if_absent(self.__generate_key(key), value)
 
+    def set_site_and_project(self, site: str, project: str):
+        """
+        把站点和项目东西放入上下文中
+        :param site:
+        :param project:
+        :return:
+        """
+        from libs import HeaderHolder
+        HeaderHolder.set_value(HeaderHolder.SITE,site)
+        HeaderHolder.set_value(HeaderHolder.PROJECT_CODE, project)
+
     def get_cache_value(self, key):
         """
         获取缓存
         :param key:
         :return:
         """
         if key is None:
@@ -188,14 +199,24 @@
 
     def clear_process_id(self):
         """
         清空key
         :return:
         """
         self.get_process_thread_local().key = None
+
+    def clear_site_and_project(self):
+        """
+        清空站点和项目
+        :return:
+        """
+        from libs import HeaderHolder
+        HeaderHolder.remove_value(HeaderHolder.SITE)
+        HeaderHolder.remove_value(HeaderHolder.PROJECT_CODE)
+
     # endregion
 
 
 class CacheAbleHandlerHolder:
 
     class __InnerCacheAbleHandler(ICacheAbleHandler):
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/IProgressAble.py` & `FicusFramework-3.1.0/src/api/handler/IProgressAble.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/message/IMessageHandler.py` & `FicusFramework-3.1.0/src/api/handler/message/IMessageHandler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ITaskHandler.py` & `FicusFramework-3.1.0/src/api/handler/ITaskHandler.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from abc import abstractmethod
 
 from api.handler import HandlerEnum
 from api.handler.IHandler import IHandler
 from api.handler.IKillable import IKillable
 from api.handler.ILogAbleHandler import ILogAbleHandler
 from api.handler.IProgressAble import IProgressAble
+from api.handler.IRevoke import IRevoke
 
 
-class ITaskHandler(ILogAbleHandler, IHandler, IKillable, IProgressAble):
+class ITaskHandler(ILogAbleHandler, IHandler, IKillable, IProgressAble, IRevoke):
 
     @abstractmethod
     def execute(self, params):
         """
         执行任务
         :return:
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/script/ScriptPythonFactory.py` & `FicusFramework-3.1.0/src/api/handler/script/ScriptPythonFactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 def _find_class(context:dict,clazz):
     script_class = None
     for k, v in context.items():
         if k != clazz and isinstance(v, type) and _is_subclass(v,clazz):
             script_class = v
     return script_class
 
-def load_instance(name:str, code_source:str,clazz):
+
+def load_instance(name: str, code_source: str, clazz, environments: dict = None):
     if  name in PYTHON_INSTANCE_CACHE:
         # 说明在缓存中,直接返回
         return PYTHON_INSTANCE_CACHE[name]
 
     # 说明还没有实例化,
     if code_source is None or len(code_source)==0:
         raise IllegalArgumentException(f"加载{name} 失败,源码为空")
@@ -78,14 +79,18 @@
         if  script_class is None:
             # 说明没有找到,报错
             raise IllegalArgumentException(f"加载{name}的源码失败,没有继承自ISimpleScriptCE/ISimpleScriptCrawl")
 
         # 放入缓存
         PYTHON_INSTANCE_CACHE[name] = script_class()
 
+        # 如果存在环境变量,就给这个实例里面添加一个隐藏的变量,用于保存环境变量
+        if environments is not None:
+            PYTHON_INSTANCE_CACHE[name].__environments__ = environments
+
         # 返回结果
         return PYTHON_INSTANCE_CACHE[name]
 
 def destroy_instance(name:str):
     """
     清理实例
     :param name:
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/script/ICacheAbleScript.py` & `FicusFramework-3.1.0/src/api/handler/script/ICacheAbleScript.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/script/ScriptPythonTaskHandler.py` & `FicusFramework-3.1.0/src/api/handler/script/ScriptPythonTaskHandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,23 +88,48 @@
     def get_process_thread_local(self):
         """
         上下文的Id
         :return:
         """
         return self.__process_id_local
 
+    def do_revoke(self, actor_code, actor_handler, code, project, site, log_id, job_id, message_id, is_expire):
+        """
+        回调取消的时候使用
+        :param actor_code:
+        :param actor_handler:
+        :param code:
+        :param project:
+        :param site:
+        :param log_id:
+        :param job_id:
+        :param message_id:
+        :param is_expire:
+        :return:
+        """
+        # 这里动态的加载script源文件
+        instance = ScriptPythonFactory.load_instance(f"ScriptPython{self.job_id}", self.script_source, "IHandler")
+        try:
+            instance.revoke_handler(actor_code, actor_handler, code, project, site, log_id, job_id, message_id, is_expire)
+        except Exception as e:
+            # 有可能根本没有实现,就不管了
+            pass
+
     def do_crawl(self, dataCrawl, params):
         """
         执行动态的crawl
         :param dataCrawl:
         :param params:
         :return:
         """
         # 这里动态的加载script源文件
-        instance = ScriptPythonFactory.load_instance(f"ScriptPython{self.job_id}", self.script_source,"IHandler")
+        instance = ScriptPythonFactory.load_instance(f"ScriptPython{self.job_id}", self.script_source, "IHandler",
+                                                     dataCrawl.environments if 'environments' in dataCrawl else None)
+        if "environments" in dataCrawl:
+            instance.__environments__ = dataCrawl.environments
 
         if instance.handler_enum() == HandlerEnum.NORMAL:
             return self.__inner_do_normal_crawl(instance,params)
         else:
             return self.__inner_do_script_crawl(instance, dataCrawl, params)
 
     def do_script_compute_execution(self, dataComputeExecution, params):
@@ -112,15 +137,16 @@
         执行ce的脚本
         :param dataComputeExecution:
         :param params:
         :return:
         """
 
         # 这里动态的加载script源文件
-        instance = ScriptPythonFactory.load_instance(f"ScriptPython{self.job_id}", self.script_source,"IHandler")
+        instance = ScriptPythonFactory.load_instance(f"ScriptPython{self.job_id}", self.script_source, "IHandler",
+                                                     dataComputeExecution.environments if 'environments' in dataComputeExecution else None)
 
         if instance.handler_enum() == HandlerEnum.NORMAL:
             return self.__inner_do_normal_compute_execution(instance, params)
         else:
             return self.__inner_do_script_compute_execution(instance, dataComputeExecution, params)
 
 
@@ -134,15 +160,15 @@
         """
         if resultList is None or len(resultList) == 0:
             # 搞完了,没的结果,不处理
             return SUCCESS
         # 有结果,就需要从crawl的配置中找到目标的fd,然后调用fd的接口进行保存
 
         try:
-            self.send_output_result(params["code_"], resultList, outputFdCodes)
+            self.send_output_result(params['site_'], params['projectCode_'], params["code_"], resultList, outputFdCodes)
         except Exception as e:
             FrameworkHandlerLogger.log_error(
                 f"{params['site_']}_{params['projectCode_']}_{params['code_']} 发送结果数据失败,",e)
         return SUCCESS
 
     def __inner_do_script_crawl(self, instance, dataCrawl, params):
         simpleScriptCrawl = instance
@@ -155,25 +181,27 @@
             TaskLogFileAppender.get_log_file_path(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                   params["__logId__"]))
 
         try:
             self.set_local_code(
                 f"{dataCrawl.site}_{dataCrawl.projectCode}_{dataCrawl.code}")
             self.set_process_id(params.get("__processLogId__"))
+            self.set_site_and_project(dataCrawl.site, dataCrawl.projectCode)
             ScriptHandlerHolder.holder.key = self
             resultList = simpleScriptCrawl.do_crawl(params)
         except Exception as e:
             FrameworkHandlerLogger.log_error(
                 f"{dataCrawl.site}_{dataCrawl.projectCode}_{dataCrawl.code} 执行失败,", e)
             import traceback
             return ResultVO(FAIL_CODE,
                             f"{dataCrawl.site}_{dataCrawl.projectCode}_{dataCrawl.code} 执行失败,\n{traceback.format_exc()}")
         finally:
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             ScriptHandlerHolder.holder.key = None
             self.current_task = None
             simpleScriptCrawl.task_logger = None
 
         return self._send_results(params, resultList, dataCrawl.outputFdCodes)
 
     def __inner_do_normal_crawl(self, instance, params):
@@ -210,25 +238,27 @@
             TaskLogFileAppender.get_log_file_path(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                   params["__logId__"]))
 
         try:
             self.set_local_code(
                 f"{dataComputeExecution.site}_{dataComputeExecution.projectCode}_{dataComputeExecution.code}")
             self.set_process_id(params.get("__processLogId__"))
+            self.set_site_and_project(dataComputeExecution.site, dataComputeExecution.projectCode)
             ScriptHandlerHolder.holder.key = self
-            resultList = simpleScriptCE.do_compute(FdInputPipe(dataComputeExecution.sourceFdCodes), params)
+            resultList = simpleScriptCE.do_compute(FdInputPipe(dataComputeExecution.site, dataComputeExecution.projectCode, dataComputeExecution.sourceFdCodes), params)
         except Exception as e:
             FrameworkHandlerLogger.log_error(
                 f"{dataComputeExecution.site}_{dataComputeExecution.projectCode}_{dataComputeExecution.code} 执行失败,", e)
             import traceback
             return ResultVO(FAIL_CODE,
                             f"{dataComputeExecution.site}_{dataComputeExecution.projectCode}_{dataComputeExecution.code} 执行失败,\n{traceback.format_exc()}")
         finally:
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             ScriptHandlerHolder.holder.key = None
             self.current_task = None
             simpleScriptCE.task_logger = None
 
         return self._send_results(params, resultList, dataComputeExecution.outputFdCodes)
 
     def __inner_do_normal_compute_execution(self, instance, params):
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/crawl/ISampleScriptCrawl.py` & `FicusFramework-3.1.0/src/api/handler/crawl/ISampleScriptCrawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/crawl/AbstractBatchCrawl.py` & `FicusFramework-3.1.0/src/api/handler/crawl/AbstractBatchCrawl.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,30 @@
     def __action(self, data_crawl, output_stream, params, is_finished, messages):
         # 异步线程来对数据进行输入
         from schedule import ShardContext
         try:
             self.set_local_code(data_crawl.site + "_" + data_crawl.projectCode + "_" + data_crawl.code)
             self.set_process_id(params.get("__processLogId__"))
             self.__task_log_id_local.key = params.get("__logId__")
+            self.set_site_and_project(data_crawl.site , data_crawl.projectCode)
             TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                params["__logId__"])
             if "__sharding_index__" in params and "__sharding_total__" in params:
                 from schedule.ShardContext import Sharding
                 ShardContext.set_sharding(Sharding(params["__sharding_index__"], params["__sharding_total__"]))
             self.__execution_message_local.content = []
             self.do_crawl(BatchOutputPipe(output_stream, len(data_crawl.outputFdCodes)), params)
         finally:
             is_finished[0] = True
             messages[0] = "success" if self.__execution_message_local.content is None or len(
                 self.__execution_message_local.content) == 0 else str(self.__execution_message_local.content)
             # 清理 MessageLocal 和 LocalCode
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__task_log_id_local.key = None
             self.__execution_message_local.content = None
             ShardContext.reset()
             TaskLogFileAppender.end_log()
 
     def execute(self, params: dict):
 
@@ -80,15 +82,15 @@
                 messages = [None]
 
                 self.__tasks_local_host.tasks.append(
                     executor.submit(self.__action, data_crawl, output_stream, params, is_finished, messages))
 
                 # 增加发送结果的线程
                 self.__tasks_local_host.tasks.append(
-                    executor.submit(self.batch_output, params["code_"], data_crawl.outputFdCodes,
+                    executor.submit(self.batch_output, params["site_"], params["projectCode_"], params["code_"], data_crawl.outputFdCodes,
                                     is_finished, output_stream,params))
 
                 # 阻塞主线程
                 for future in as_completed(self.__tasks_local_host.tasks):
                     try:
                         data = future.result()
                     except Exception as e:
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/crawl/AbstractSimpleCrawl.py` & `FicusFramework-3.1.0/src/api/handler/crawl/AbstractSimpleCrawl.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,28 @@
 
         # 每一次新的任务都重置这个标识
         self.killed = False
 
         try:
             self.set_local_code(data_crawl.site + "_" + data_crawl.projectCode + "_" + data_crawl.code)
             self.set_process_id(params.get("__processLogId__"))
+            self.set_site_and_project(params["site_"], params["projectCode_"])
             self.__task_log_id_local.key = params.get("__logId__")
             self.__execution_message_local.content = []
-            TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),params["__logId__"])
+            TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
+                                               params["__logId__"])
             result_list = self.do_crawl(params)
         except Exception as e:
             import traceback
             return ResultVO(FAIL_CODE, f"执行失败,Code:{params['site_']}的Crawl,发生错误:\n{traceback.format_exc()}")
         finally:
             # 清理 MessageLocal 和 LocalCode
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__task_log_id_local.key = None
             self.__execution_message_local.content = None
             TaskLogFileAppender.end_log()
 
         message = "success" if self.__execution_message_local.content is None or len(
             self.__execution_message_local.content) == 0 else str(self.__execution_message_local.content)
 
@@ -75,21 +78,22 @@
 
         insert_cache = defaultdict(list)
         update_cache = defaultdict(list)
         upsert_cache = defaultdict(list)
 
         for serializableOutputWrapper in result_list:
             output_fd = self.find_output_fd(output_fd_codes, serializableOutputWrapper.index())
-            self.put_in_cache(data_crawl.code, insert_cache, update_cache, upsert_cache, output_fd,
+            self.put_in_cache(data_crawl.site, data_crawl.projectCode, data_crawl.code, insert_cache, update_cache,
+                              upsert_cache, output_fd,
                               serializableOutputWrapper)
 
         try:
             TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                params["__logId__"])
-            self.flush_cache(data_crawl.code, insert_cache, update_cache, upsert_cache)
+            self.flush_cache(data_crawl.site, data_crawl.projectCode,data_crawl.code, insert_cache, update_cache, upsert_cache)
         finally:
             TaskLogFileAppender.end_log()
 
         return ResultVO(SUCCESS_CODE, message)
 
     def kill(self):
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/crawl/ISimpleScriptCrawl.py` & `FicusFramework-3.1.0/src/api/handler/crawl/ISimpleScriptCrawl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from abc import abstractmethod
 
 from api.handler import HandlerEnum
 from api.handler.IHandler import IHandler
+from api.handler.IRevoke import IRevoke
 from api.handler.script.ICacheAbleScript import ICacheAbleScript
 from api.handler.IKillable import IKillable
 from api.handler.ILogAbleHandler import ILogAbleHandler
 from api.handler.script.IProgressAbleScript import IProgressAbleScript
 
 
-class ISimpleScriptCrawl(IKillable, ILogAbleHandler, ICacheAbleScript, IHandler, IProgressAbleScript):
+class ISimpleScriptCrawl(IKillable, ILogAbleHandler, ICacheAbleScript, IHandler, IProgressAbleScript, IRevoke):
     """
     Python脚本式的Crawl的基类
     """
 
     @abstractmethod
     def do_crawl(self, params: dict):
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/outputer/ISimpleOutputer.py` & `FicusFramework-3.1.0/src/api/handler/outputer/ISimpleOutputer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from api.handler.outputer.IBaseOutputer import IBaseOutputer
 
 
 class ISimpleOutputer(IBaseOutputer):
 
-    def send_output_result(self, code, result_list, output_fd_codes):
+    def send_output_result(self, site, project_code, code, result_list, output_fd_codes):
         """
         发送任务到FD
+        :param project_code:
+        :param site:
         :param code:
         :param result_list:
         :param output_fd_codes:
         :return:
         """
 
         insert_cache = {}
         update_cache = {}
         upsert_cache = {}
 
         # 把任务放入缓存
         for serializable_output_wrapper in result_list:
             output_fd = self.find_output_fd(output_fd_codes, serializable_output_wrapper.index())
-            self.put_in_cache(code, insert_cache, update_cache, upsert_cache, output_fd, serializable_output_wrapper)
+            self.put_in_cache(site, project_code, code, insert_cache, update_cache, upsert_cache, output_fd, serializable_output_wrapper)
 
         # 清理缓存中的任务
-        self.flush_cache(code, insert_cache, update_cache, upsert_cache)
+        self.flush_cache(site, project_code, code, insert_cache, update_cache, upsert_cache)
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/outputer/IBatchOutputer.py` & `FicusFramework-3.1.0/src/api/handler/outputer/IBatchOutputer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 from datetime import datetime
 from queue import Queue, Empty
 
 from api.handler.outputer.IBaseOutputer import IBaseOutputer
 from client import ServiceInnerException
-from factdatasource import FactDatasourceProxyService
+from factdatasource import FactDatasourceProxyServiceV2
 from schedule.utils.log import FrameworkHandlerLogger
 
 
 class IBatchOutputer(IBaseOutputer):
 
     @abstractmethod
     def get_batch_size(self) -> int:
@@ -19,17 +19,19 @@
 
     def __logResult(self,task_logger,results):
         if results is not None and len(results) > 0:
             results = filter(lambda x: not x.success, results)
             for res in results:
                 task_logger.log(f"{res.error} data:{res.content}")
 
-    def batch_output(self, code, output_fd_codes, is_finished, output_stream: Queue, params):
+    def batch_output(self,site: str, project_code: str, code, output_fd_codes, is_finished, output_stream: Queue, params):
         """
         批量发送任务出去
+        :param site:
+        :param project_code:
         :param params:
         :param code:
         :param output_fd_codes:
         :param is_finished:
         :param output_stream:
         :return:
         """
@@ -52,39 +54,39 @@
                     poll = output_stream.get(timeout=1)
                 except Empty:
                     # 表示这个任务为null,不处理
                     continue
 
                 output_fd = self.find_output_fd(output_fd_codes, poll.index())
                 # 把输出放入缓存中
-                self.put_in_cache(code, insert_cache, update_cache, upsert_cache, output_fd, poll)
+                self.put_in_cache(site, project_code, code, insert_cache, update_cache, upsert_cache, output_fd, poll)
 
                 # 清空批量任务
                 try:
                     serializables = insert_cache.get(output_fd)
                     if serializables is not None and len(serializables) >= self.get_batch_size():
-                        results = FactDatasourceProxyService.fd_client_proxy().inserts(output_fd, serializables)
+                        results = FactDatasourceProxyServiceV2.fd_client_proxy().inserts(site,project_code,output_fd, serializables)
                         self.__logResult(task_logger,results)
                         serializables.clear()
 
                     serializables = update_cache.get(output_fd)
                     if serializables is not None and len(serializables) >= self.get_batch_size():
-                        results = FactDatasourceProxyService.fd_client_proxy().updates(output_fd, serializables)
+                        results = FactDatasourceProxyServiceV2.fd_client_proxy().updates(site,project_code,output_fd, serializables)
                         self.__logResult(task_logger, results)
                         serializables.clear()
 
                     serializables = upsert_cache.get(output_fd)
                     if serializables is not None and len(serializables) >= self.get_batch_size():
-                        results = FactDatasourceProxyService.fd_client_proxy().save_or_updates(output_fd, serializables)
+                        results = FactDatasourceProxyServiceV2.fd_client_proxy().save_or_updates(site,project_code,output_fd, serializables)
                         self.__logResult(task_logger, results)
                         serializables.clear()
                 except Exception as e:
                     import traceback
                     raise ServiceInnerException(f"执行失败,Code: {code}的执行器,保存数据发生错误:\n{traceback.format_exc()}")
 
             # 把剩余的任务清空了
-            self.flush_cache(code, insert_cache, update_cache, upsert_cache)
+            self.flush_cache(site, project_code, code, insert_cache, update_cache, upsert_cache)
         finally:
             TaskLogFileAppender.end_log()
 
         # 到这来了 就表示是完成了
         return
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/outputer/IBaseOutputer.py` & `FicusFramework-3.1.0/src/api/handler/outputer/IBaseOutputer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from api.exceptions import IllegalArgumentException, ServiceInnerException
 from api.model import OutputWrapper
-from factdatasource import FactDatasourceProxyService
+from factdatasource import FactDatasourceProxyServiceV2
 from schedule.utils.log import FrameworkHandlerLogger
 
 
 class IBaseOutputer:
 
     def __logResult(self,task_logger,results):
         if task_logger is not None and results is not None and len(results) > 0:
             results = filter(lambda x: not x.success, results)
             for res in results:
                 task_logger.log(f"{res.error} data:{res.content}")
 
-    def put_in_cache(self, code, insert_cache: dict, update_cache, upsert_cache, output_fd, poll: OutputWrapper):
+    def put_in_cache(self,site: str, project_code: str, code, insert_cache: dict, update_cache, upsert_cache, output_fd, poll: OutputWrapper):
         """
         把数据放入缓存中
+        :param site:
+        :param project_code:
         :param code:
         :param insert_cache:
         :param update_cache:
         :param upsert_cache:
         :param output_fd:
         :param poll:
         :return:
@@ -34,28 +36,30 @@
 
         elif poll.operation() == OperationEnum.UPSERT:
             upsert_cache[output_fd] = upsert_cache.get(output_fd, [])
             upsert_cache[output_fd].append(poll.content())
 
         elif poll.operation() == OperationEnum.CLEAN:
             try:
-                FactDatasourceProxyService.fd_client_proxy().delete_all(output_fd)
+                FactDatasourceProxyServiceV2.fd_client_proxy().delete_all(site,project_code,output_fd)
             except Exception as e:
                 raise ServiceInnerException(f"执行失败,Code: {code}的执行器,清空数据发生错误:{str(e)}")
         elif poll.operation() == OperationEnum.DELETE:
             try:
-                FactDatasourceProxyService.fd_client_proxy().delete(output_fd, poll.content())
+                FactDatasourceProxyServiceV2.fd_client_proxy().delete(site,project_code,output_fd, poll.content())
             except Exception as e:
                 raise ServiceInnerException(f"执行失败,Code: {code}的执行器,删除数据发生错误:{str(e)}")
         elif poll.operation() == OperationEnum.FLUSH:
-            self.flush_cache(code, insert_cache, update_cache, upsert_cache)
+            self.flush_cache(site,project_code,code, insert_cache, update_cache, upsert_cache)
 
-    def flush_cache(self, code, insert_cache, update_cache, upsert_cache):
+    def flush_cache(self,site: str, project_code: str, code, insert_cache, update_cache, upsert_cache):
         """
         把缓存中的数据 发送到FD中
+        :param site:
+        :param project_code:
         :param code:
         :param insert_cache:
         :param update_cache:
         :param upsert_cache:
         :return:
         """
 
@@ -69,37 +73,37 @@
             for key, value in insert_cache.items():
                 if self.is_killed():
                     FrameworkHandlerLogger.log_warn("任务被强制停止,停止变更数据")
                     task_logger.log("任务被强制停止,停止变更数据")
                     return
 
                 if len(value) > 0:
-                    results = FactDatasourceProxyService.fd_client_proxy().inserts(key, value)
+                    results = FactDatasourceProxyServiceV2.fd_client_proxy().inserts(site,project_code,key, value)
                     self.__logResult(task_logger, results)
                     value.clear()
 
             for key, value in update_cache.items():
                 if self.is_killed():
                     FrameworkHandlerLogger.log_warn("任务被强制停止,停止变更数据")
                     task_logger.log("任务被强制停止,停止变更数据")
                     return
 
                 if len(value) > 0:
-                    results = FactDatasourceProxyService.fd_client_proxy().updates(key, value)
+                    results = FactDatasourceProxyServiceV2.fd_client_proxy().updates(site,project_code,key, value)
                     self.__logResult(task_logger, results)
                     value.clear()
 
             for key, value in upsert_cache.items():
                 if self.is_killed():
                     FrameworkHandlerLogger.log_warn("任务被强制停止,停止变更数据")
                     task_logger.log("任务被强制停止,停止变更数据")
                     return
 
                 if len(value) > 0:
-                    results = FactDatasourceProxyService.fd_client_proxy().save_or_updates(key, value)
+                    results = FactDatasourceProxyServiceV2.fd_client_proxy().save_or_updates(site,project_code,key, value)
                     self.__logResult(task_logger, results)
                     value.clear()
         except Exception as e:
             import traceback
             raise ServiceInnerException(f"执行失败,Code: {code}的执行器,保存数据发生错误:\n{traceback.format_exc()}")
 
     def find_output_fd(self, output_fds: list, index: int):
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ICacheAble.py` & `FicusFramework-3.1.0/src/api/handler/ICacheAble.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/IMessageCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/IMessageCE.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from confluent_kafka.cimpl import Consumer, KafkaError, KafkaException
 
 from api.exceptions import IllegalArgumentException
 from api.handler.message.IMessageHandler import IMessageHandler
 from api.model.ResultVO import ResultVO, FAIL_CODE, SUCCESS
 from api.model.FactDatasource import FactDatasourceTypeEnum
 from config.annotation import Value
-from factdatasource import FactDatasourceProxyService
+from factdatasource import FactDatasourceProxyServiceV2
 from schedule.utils.log import FrameworkHandlerLogger
 
 
 class IMessageCE(IMessageHandler):
     """
 
     """
@@ -41,17 +41,17 @@
         if sourceFdCodes is None or len(sourceFdCodes) == 0:
             return ResultVO(FAIL_CODE, f"执行失败,没有找到Code:{code}的Ce 没有配置sourceFactData")
 
         sourceFd = None
 
         for sourceFdCode in sourceFdCodes:
             # 找到FD的定义
-            fd = FactDatasourceProxyService.fd_client_proxy().fd(sourceFdCode)
+            fd = FactDatasourceProxyServiceV2.fd_client_proxy().fd(site, projectCode, sourceFdCode)
             if fd is None:
-                return ResultVO(FAIL_CODE, f"执行失败,没有找到Code:{code}的Ce 配置的sourceFactData {sourceFdCode} 不存在")
+                return ResultVO(FAIL_CODE, f"执行失败,没有找到Code:{code}的Ce 配置的sourceFactData {site}-{projectCode}-{sourceFdCode} 不存在")
             if fd.type in ["KAFKA", "AMQP", "JMS", FactDatasourceTypeEnum.KAFKA, FactDatasourceTypeEnum.AMQP, FactDatasourceTypeEnum.JMS]:
                 # 说明找到了kafka或amqp或jms的来源fd,只找头一个
                 sourceFd = fd
                 break
 
         if sourceFd is None:
             return ResultVO(FAIL_CODE, f"执行失败,没有找到Code:{code}的Ce 没有配置消息的来源")
@@ -167,15 +167,15 @@
     def __init__(self, messageCe: IMessageCE, group_id, topic, brokers):
         threading.Thread.__init__(self)
         # 初始化
         self.messageCe = messageCe
 
         # 开启kafka的消息监听
         config = {'bootstrap.servers': brokers, 'group.id': group_id, 'session.timeout.ms': 6000,
-                  'default.topic.config': {'auto.offset.reset': 'earliest'}}
+                  'default.topic.config': {'auto.offset.reset': 'latest'}} # 跟java一样，改成从最新的地方读
         import logging
         self.consumer = Consumer(config, logger=logging.getLogger("Ficus"))  # TODO 这里的入参好像有问题
         self.consumer.subscribe([topic])
 
         self.go_on = True
 
     def stop(self):
@@ -201,10 +201,16 @@
                         raise KafkaException(msg.error())
                 else:
                     # 进行消息的处理
                     self.messageCe.message(msg.value())
             except Exception as e:
                 FrameworkHandlerLogger.log_error(f"接收消息出现问题,", e)
             finally:
-                if self.go_on == False:
+                if not self.go_on:
                     # 把消息队列关闭掉
                     self.consumer.close()
+
+        if not self.go_on:
+            try:
+                self.consumer.close()
+            except Exception as e:
+                FrameworkHandlerLogger.log_error(f"关闭consumer失败,出现问题", e)
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractAsyncServiceBatchCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/AbstractAsyncServiceBatchCE.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,20 @@
         try:
             # 这里构造的其实就是 与执行器交互的 协议
             self.set_local_code(
                 data_compute_execution.site + "_" + data_compute_execution.projectCode + "_" + data_compute_execution.code)
             self.set_process_id(params.get("__processLogId__"))
             TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                params["__logId__"])
-            request = self.generate_request(FdInputPipe(data_compute_execution.sourceFdCodes), params)
+            self.set_site_and_project(data_compute_execution.site, data_compute_execution.projectCode)
+            request = self.generate_request(FdInputPipe(data_compute_execution.site, data_compute_execution.projectCode, data_compute_execution.sourceFdCodes), params)
         finally:
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             TaskLogFileAppender.end_log()
 
         if request is None:
             # 返回为空,直接就返回了
             return SUCCESS
 
         jobId = params.get("__jobId__")
@@ -115,18 +117,28 @@
                 elif "DELETE" == request.method:
                     r = requests.delete(request.url, headers=headers)
                 elif "HEAD" == request.method:
                     r = requests.head(request.url, headers=headers)
             except Exception as e:
                 return ResultVO(FAIL_CODE, f"任务:{taskLogId} 请求{request.url} 失败,请求出错: {str(e)}")
 
-            succeeded, message = self.analysis_sync_response(r.status_code, r.content, r.headers)
-
-            if not succeeded:
-                return ResultVO(FAIL_CODE, f"任务:{taskLogId} 请求{request.url} 失败,请求出错: {message}")
+            try:
+                # 这里因为 analysis_sync_response 也需要他们自己实现, 里面可能会需要使用到 chache的东西,所以这里也需要包一下
+                self.set_local_code(
+                    data_compute_execution.site + "_" + data_compute_execution.projectCode + "_" + data_compute_execution.code)
+                self.set_process_id(params.get("__processLogId__"))
+                TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
+                                                   params["__logId__"])
+                succeeded, message = self.analysis_sync_response(r.status_code, r.content, r.headers)
+                if not succeeded:
+                    return ResultVO(FAIL_CODE, f"任务:{taskLogId} 请求{request.url} 失败,请求出错: {message}")
+            finally:
+                self.clear_local_code()
+                self.clear_process_id()
+                TaskLogFileAppender.end_log()
 
         return DOING
 
     def __action(self, response, header: dict, task_status: int, data_compute_execution, output_stream, params,
                  is_finished, messages):
         """
         异步线程来对数据进行输入
@@ -137,26 +149,29 @@
         :param messages:
         :return:
         """
         try:
             self.set_local_code(
                 data_compute_execution.site + "_" + data_compute_execution.projectCode + "_" + data_compute_execution.code)
             self.set_process_id(params.get("__processLogId__"))
+            self.set_site_and_project(data_compute_execution.site , data_compute_execution.projectCode)
             self.__execution_message_local.content = []
             TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                params["__logId__"])
             messages[0] = self.do_compute(response, header, task_status,
                                           BatchOutputPipe(output_stream, len(data_compute_execution.outputFdCodes)),
-                                          FdInputPipe(data_compute_execution.sourceFdCodes), params)
+                                          FdInputPipe(data_compute_execution.site, data_compute_execution.projectCode,
+                                                      data_compute_execution.sourceFdCodes), params)
         finally:
             # 清理 MessageLocal 和 LocalCode
             is_finished[0] = True
 
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__execution_message_local.content = None
             TaskLogFileAppender.end_log()
 
     def do_finish(self, task_log_id: int, response, header: dict, ficus_param: dict, task_status: int) -> ResultVO:
         """
         完成的回调处理
         :param task_log_id:
@@ -188,17 +203,18 @@
 
                 self.__tasks_local_host.tasks.append(
                     executor.submit(self.__action, response, header, task_status, data_compute_execution, output_stream,
                                     ficus_param, is_finished, messages))
 
                 # 增加发送结果的线程
                 self.__tasks_local_host.tasks.append(
-                    executor.submit(self.batch_output, ficus_param["code_"], data_compute_execution.outputFdCodes,
+                    executor.submit(self.batch_output, ficus_param["site_"], ficus_param["projectCode_"],
+                                    ficus_param["code_"], data_compute_execution.outputFdCodes,
                                     is_finished,
-                                    output_stream,ficus_param))
+                                    output_stream, ficus_param))
                 # 阻塞主线程
                 for future in as_completed(self.__tasks_local_host.tasks):
                     try:
                         data = future.result()
                     except Exception as e:
                         return ResultVO(FAIL_CODE, f"执行失败,Code:{ficus_param['code_']}的CE,原因:{str(e)}")
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractBatchCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/AbstractBatchCE.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,29 +35,31 @@
         from schedule import ShardContext
         try:
             self.set_local_code(
                 data_compute_execution.site + "_" + data_compute_execution.projectCode + "_" + data_compute_execution.code)
             self.set_process_id(params.get("__processLogId__"))
             self.__task_log_id_local.key = params.get("__logId__")
             self.__execution_message_local.content = []
+            self.set_site_and_project(data_compute_execution.site, data_compute_execution.projectCode)
             TaskLogFileAppender.prepare_to_log(datetime.strptime(params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),params["__logId__"])
 
             if "__sharding_index__" in params and "__sharding_total__" in params:
                 from schedule.ShardContext import Sharding
                 ShardContext.set_sharding(Sharding(params["__sharding_index__"], params["__sharding_total__"]))
 
             self.do_compute(BatchOutputPipe(output_stream, len(data_compute_execution.outputFdCodes)),
-                            FdInputPipe(data_compute_execution.sourceFdCodes), params)
+                            FdInputPipe(data_compute_execution.site, data_compute_execution.projectCode, data_compute_execution.sourceFdCodes), params)
         finally:
             # 清理 MessageLocal 和 LocalCode
             is_finished[0] = True
             messages[0] = "success" if self.__execution_message_local.content is None or len(
                 self.__execution_message_local.content) == 0 else str(self.__execution_message_local.content)
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__task_log_id_local.key = None
             self.__execution_message_local.content = None
             ShardContext.reset()
             TaskLogFileAppender.end_log()
 
 
     def execute(self, params):
@@ -87,15 +89,15 @@
                 messages = [None]
 
                 self.__tasks_local_host.tasks.append(executor.submit(self.__action,data_compute_execution,output_stream,params,is_finished,messages))
 
 
                 # 增加发送结果的线程
                 self.__tasks_local_host.tasks.append(
-                    executor.submit(self.batch_output, params["code_"], data_compute_execution.outputFdCodes, is_finished, output_stream,params))
+                    executor.submit(self.batch_output, params["site_"], params["projectCode_"], params["code_"], data_compute_execution.outputFdCodes, is_finished, output_stream,params))
 
 
                 # 阻塞主线程
                 for future in as_completed(self.__tasks_local_host.tasks):
                     try:
                         data = future.result()
                     except Exception as e:
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/ISampleScriptCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/ISampleScriptCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/ISimpleScriptCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/ISimpleScriptCE.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import abstractmethod
 
 from api.handler import HandlerEnum
 from api.handler.IHandler import IHandler
+from api.handler.IRevoke import IRevoke
 from api.handler.script.ICacheAbleScript import ICacheAbleScript
 from api.handler.IKillable import IKillable
 from api.handler.ILogAbleHandler import ILogAbleHandler
 from api.handler.script.IProgressAbleScript import IProgressAbleScript
 from api.model.FdInputPipe import FdInputPipe
 
 
-class ISimpleScriptCE(IKillable, ILogAbleHandler, ICacheAbleScript, IHandler, IProgressAbleScript):
+class ISimpleScriptCE(IKillable, ILogAbleHandler, ICacheAbleScript, IHandler, IProgressAbleScript, IRevoke):
     """
     Python脚本式的CE的基类
     """
 
     @abstractmethod
     def do_compute(self, source_fds: FdInputPipe, params: dict):
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/handler/ce/AbstractMessageCE.py` & `FicusFramework-3.1.0/src/api/handler/ce/AbstractMessageCE.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,38 +40,40 @@
 
         resultList = None
         try:
             self.set_local_code(
                 f"{self.dataComputeExecution.site}_{self.dataComputeExecution.projectCode}_{self.dataComputeExecution.code}")
             self.set_process_id(self.params.get("__processLogId__"))
             self.__task_log_id_local.key = self.params.get("__logId__")
+            self.set_site_and_project(self.dataComputeExecution.site, self.dataComputeExecution.projectCode)
             TaskLogFileAppender.prepare_to_log(datetime.strptime(self.params["__triggerTime__"], "%Y-%m-%d %H:%M:%S"),
                                                self.params["code_"])
-            resultList = self.do_compute(FdInputPipe(self.dataComputeExecution.sourceFdCodes), data.decode('utf-8'),
+            resultList = self.do_compute(FdInputPipe(self.dataComputeExecution.site, self.dataComputeExecution.projectCode, self.dataComputeExecution.sourceFdCodes), data.decode('utf-8'),
                                          self.params)
         except Exception as e:
             FrameworkHandlerLogger.log_error(
                 f"{self.dataComputeExecution.site}_{self.dataComputeExecution.projectCode}_{self.dataComputeExecution.code} 接收到消息执行失败,",
                 e)
             return
         finally:
             self.clear_local_code()
             self.clear_process_id()
+            self.clear_site_and_project()
             self.__task_log_id_local.key = None
             TaskLogFileAppender.end_log()
 
         if resultList is None or len(resultList) == 0:
             # 搞完了,没的结果,不处理
             return
 
         # 有结果,就需要从crawl的配置中找到目标的fd,然后调用fd的接口进行保存
         outputFdCodes = self.dataComputeExecution.outputFdCodes
 
         try:
-            self.send_output_result(self.dataComputeExecution.code, resultList, outputFdCodes)
+            self.send_output_result(self.dataComputeExecution.site, self.dataComputeExecution.projectCode, self.dataComputeExecution.code, resultList, outputFdCodes)
         except Exception as e:
             FrameworkHandlerLogger.log_error(
                 f"{self.dataComputeExecution.site}_{self.dataComputeExecution.projectCode}_{self.dataComputeExecution.code} 发送结果数据失败,",
                 e)
 
     def execute(self, params):
         """
```

### Comparing `FicusFramework-3.0.9.post9/src/api/model/OutputWrapper.py` & `FicusFramework-3.1.0/src/api/model/OutputWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/AsyncServiceRequest.py` & `FicusFramework-3.1.0/src/api/model/AsyncServiceRequest.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/AlgorithmFdInputWrapper.py` & `FicusFramework-3.1.0/src/api/model/AlgorithmFdInputWrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 class AlgorithmFdInputWrapper(FdInputWrapper):
     """
     算法fd输入的一个包装
     """
     sub_path: str = None
     input_stream = None
 
-
-    def __init__(self, fd_code: str, sub_path):
-        super().__init__(fd_code)
+    def __init__(self, site: str, project_code: str, fd_code: str, sub_path):
+        super().__init__(site, project_code, fd_code)
         self.sub_path = sub_path
 
     def path(self):
         fd = self.info()
         if fd is None or not isinstance(fd, FactDatasource):
             return None
         if fd.target:
@@ -44,17 +43,19 @@
             return None
         self.input_stream = open(path, 'rb')
         return self.input_stream
 
     def close(self):
         if self.input_stream is not None:
             self.input_stream.close()
+
     """
     获取子文件
     """
+
     def child(self, sub_path: str):
         fd = self.info()
         if not isinstance(fd, FactDatasource) or fd.target:
             # 说明本身就是文件类型的，没有子文件
             return None
         if self.sub_path:
             absolute_path = get_algo_abs_path(fd.site, fd.connection, self.sub_path)
@@ -66,24 +67,26 @@
                 if not directory.startswith(os.sep):
                     directory = os.sep + directory
                 if not directory.endswith(os.sep):
                     directory = directory + os.sep
                 if sub_path.startswith(os.sep):
                     sub_path = sub_path[1:]
                 # self.sub_path = directory + sub_path
-                #return self
-                return AlgorithmFdInputWrapper(self._fact_datasource_code, directory + sub_path)
+                # return self
+                return AlgorithmFdInputWrapper(self._site, self._project_code, self._fact_datasource_code,
+                                               directory + sub_path)
         else:
-            #self.sub_path = sub_path
-            #return self
-            return AlgorithmFdInputWrapper(self._fact_datasource_code, sub_path)
+            # self.sub_path = sub_path
+            # return self
+            return AlgorithmFdInputWrapper(self._site, self._project_code, self._fact_datasource_code, sub_path)
 
     """
     返回子文件/文件夹，只返回一层
     """
+
     def list(self):
         results = []
         abs_path = self.path()
         if abs_path is None:
             return results
         if not os.path.isdir(abs_path):
             # 不是文件夹就没有子文件了
@@ -96,11 +99,11 @@
                 directory = ''
                 if self.sub_path:
                     directory = self.sub_path
                     if not directory.startswith(os.sep):
                         directory = os.sep + directory
                     if not directory.endswith(os.sep):
                         directory = directory + os.sep
-                #self.sub_path = directory + file
-                #results.append(self)
-                results.append(AlgorithmFdInputWrapper(self._fact_datasource_code, directory + file))
+                # self.sub_path = directory + file
+                # results.append(self)
+                results.append(AlgorithmFdInputWrapper(self._site, self._project_code, self._fact_datasource_code, directory + file))
             return results
```

### Comparing `FicusFramework-3.0.9.post9/src/api/model/GraphNode.py` & `FicusFramework-3.1.0/src/api/model/GraphNode.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/ReadWriteLock.py` & `FicusFramework-3.1.0/src/api/model/ReadWriteLock.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/MetaModel.py` & `FicusFramework-3.1.0/src/api/model/MetaModel.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/ResultVO.py` & `FicusFramework-3.1.0/src/api/model/ResultVO.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/GraphRelation.py` & `FicusFramework-3.1.0/src/api/model/GraphRelation.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/AsyncServiceResponse.py` & `FicusFramework-3.1.0/src/api/model/AsyncServiceResponse.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/__init__.py` & `FicusFramework-3.1.0/src/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/BatchOutputPipe.py` & `FicusFramework-3.1.0/src/api/model/BatchOutputPipe.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/Page.py` & `FicusFramework-3.1.0/src/api/model/Page.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/MetaModelField.py` & `FicusFramework-3.1.0/src/api/model/MetaModelField.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from enum import Enum
 
 _defaultValues = {'STRING': "''", 'INTEGER': '0', 'LONG': '0', 'FLOAT': '0', 'DOUBLE': '0', 'BOOLEAN': "''",
-                  'DATE': 'CURRENT_TIMESTAMP()', 'CHAR': "''", 'BYTE': "''", 'MODEL': "''"}
+                  'DATE': 'CURRENT_TIMESTAMP()', 'CHAR': "''", 'BYTE': "''", 'MODEL': "''", 'JSON': "''", 'BLOB': "''"}
 
 
 class DataTypeEnum(Enum):
     STRING = "STRING"
     INTEGER = "INTEGER"
     LONG = "LONG"
     FLOAT = "FLOAT"
     DOUBLE = "DOUBLE"
     BOOLEAN = "BOOLEAN"
     DATE = "DATE"
     CHAR = "CHAR"
     BYTE = "BYTE"
     MODEL = "MODEL"
+    JSON = "JSON"
+    BLOB = "BLOB"
 
     def __new__(cls, name):
         obj = object.__new__(cls)
         obj._value_ = name
         obj._default_ = _defaultValues.get(name)
         return obj
```

### Comparing `FicusFramework-3.0.9.post9/src/api/model/MetaModelTransform.py` & `FicusFramework-3.1.0/src/api/model/MetaModelTransform.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/Condition.py` & `FicusFramework-3.1.0/src/api/model/Condition.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/AlgoOutWrapper.py` & `FicusFramework-3.1.0/src/api/model/AlgoOutWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/FdInputPipe.py` & `FicusFramework-3.1.0/src/api/model/FdInputPipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from api.model.FdInputWrapper import FdInputWrapper
 from api.model.AlgorithmFdInputWrapper import AlgorithmFdInputWrapper
-from factdatasource import FactDatasourceProxyService
+from factdatasource import FactDatasourceProxyServiceV2
 from api.exceptions import IllegalArgumentException
 from api.model.FactDatasource import FactDatasourceTypeEnum
 
 
 class FdInputPipe:
     """
     输入包装
     """
     __source_fd_codes = None
 
-    def __init__(self, source_fd_codes):
+    def __init__(self, site: str, project_code: str, source_fd_codes):
+        self.__site = site
+        self.__project_code = project_code
         self.__source_fd_codes = source_fd_codes
 
     def list_source_fd_codes(self):
         """
         列出所有与之关联的来源FD的code
         :return:
         """
         return self.__source_fd_codes
 
-    def get_fd(self, fd_code):
+    def get_fd(self, fd_code, site: str = None, project_code: str = None):
         """
         返回一个Fd的输入代理对象
+        :param site:
+        :param project_code:
         :param fd_code:
         :return: FdInputWrapper对象
         """
-        fd = FactDatasourceProxyService.fd_client_proxy().fd(fd_code)
+        inner_site = site if site is not None else self.__site
+        inner_project = project_code if project_code is not None else self.__project_code
+
+        fd = FactDatasourceProxyServiceV2.fd_client_proxy().fd(inner_site, inner_project, fd_code)
         if fd is None:
             raise IllegalArgumentException(f"无法查询到FD:{fd_code}的数据")
         if fd.type == FactDatasourceTypeEnum.ALGORITHM:
-            return AlgorithmFdInputWrapper(fd_code, None)
+            return AlgorithmFdInputWrapper(inner_site, inner_project, fd_code, None)
         else:
-            return FdInputWrapper(fd_code)
+            return FdInputWrapper(inner_site, inner_project, fd_code)
```

### Comparing `FicusFramework-3.0.9.post9/src/api/model/OtherTargetOutputPipe.py` & `FicusFramework-3.1.0/src/api/model/OtherTargetOutputPipe.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/api/model/FactDatasource.py` & `FicusFramework-3.1.0/src/api/model/FactDatasource.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  **kwargs):
         """
         描述数据源的对象
         :param site: 事实库所属的站点,必填
         :param projectCode: 事实库所属的工程,必填
         :param code: 事实库的唯一标示,必填,要求全局code唯一,允许大小写字母加数字下划线,最大128个字符
         :param name: 事实库显示名字,必填,允许中文/英文大小写字母加数字,最大256个字符
-        :param type: 事实库的类型,必填 allowableValues = "FILE,JDBC,REDIS,KAFKA,MONGO,ES,SOBEY_HIVE,GRAPH,CUSTOM,AMQP,ALGORITHM"
+        :param type: 事实库的类型,必填 allowableValues = "FILE,JDBC,REDIS,KAFKA,MONGO,ES,SOBEY_HIVE,GRAPH,CUSTOM,AMQP,ALGORITHM,FORMTRAVEL"
         :param connection: 事实库的连接字符串,必填  FILE就是文件路径 JDBC/GRAPH就是jdbcUrl等等,KAFKA/AMQP/REDIS/MONGO/ES就是服务器的IP加端口 ,
             sobeyHive 就是hivecore的地址 带端口号  CUSTOM 是 微服务的名字也就是actor.name
             REIDS:单机：ip:port  集群（英文逗号分割）： ip:port,ip:port,ip:port  哨兵（第一个表示主节点名字，英文分号分割）：MASTERNAME;哨兵IP1:PORT1;哨兵IP2:PORT2;哨兵IP3:PORT3
             algorithm是一个相对路径
         :param target: 事实库的数据目标,必填,FILE文件名/MYSQL,ORACLE表名/redis(key的前缀)?/kafka队列名/es索引名/mongo Collection名/
             sobeyHive 就是目标索引名 entity/ CUSTOM是 handler的名字/AMQP exchange:routingKey/ JMS 发送消息的目标位置 https://stomp.github.io/stomp-specification-1.2.html#SEND
             algorithm如果是空，表示文件夹，如果不空，表示文件
@@ -92,15 +92,16 @@
     JMS = 'JMS'
     ALGORITHM = 'ALGORITHM'
     REF = 'REF'  # 表示这个FD是关联的其他的FD
     FTP = 'FTP'
     S3 = 'S3'
     NAS = 'NAS'
     HOTFOLDER = 'HOTFOLDER'
-
+    FORMTRAVEL = 'FORMTRAVEL'       # 表达
+    TABLESTORE = 'TABLESTORE'
 
 class JdbcTypeEnum(Enum):
     MYSQL = 'MYSQL'
     ORACLE = 'ORACLE'
     VERNOX = 'VERNOX'
     VERNOX_NTS = 'VERNOX_NTS'
     SQL_SERVER = 'SQL_SERVER'
```

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/operation/__init__.py` & `FicusFramework-3.1.0/src/rule_engine/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/RuleEngineInitialize.py` & `FicusFramework-3.1.0/src/rule_engine/RuleEngineInitialize.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/core/SimpleValueProvider.py` & `FicusFramework-3.1.0/src/rule_engine/core/SimpleValueProvider.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/core/__init__.py` & `FicusFramework-3.1.0/src/rule_engine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/core/SimpleRuleGroupSession.py` & `FicusFramework-3.1.0/src/rule_engine/core/SimpleRuleGroupSession.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/core/DefaultAgenda.py` & `FicusFramework-3.1.0/src/rule_engine/core/DefaultAgenda.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/core/PattenMatcher.py` & `FicusFramework-3.1.0/src/rule_engine/core/PattenMatcher.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/RuleEngine.py` & `FicusFramework-3.1.0/src/rule_engine/RuleEngine.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/__init__.py` & `FicusFramework-3.1.0/src/rule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/action/__init__.py` & `FicusFramework-3.1.0/src/rule_engine/action/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/rule_engine/RuleEngineCustomScriptFactory.py` & `FicusFramework-3.1.0/src/rule_engine/RuleEngineCustomScriptFactory.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/service/FactDatasourceService.py` & `FicusFramework-3.1.0/src/service/FactDatasourceService.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,40 +10,44 @@
 
 class FactDatasourceService(Singleton):
 
     @property
     def dao(self):
         return JdbcDatasourceDao.instance()
 
-    def get_fd_by_code(self, fd_code: str) -> FactDatasource:
+    def get_fd_by_code(self, site: str, project_code: str, fd_code: str) -> FactDatasource:
         """
         根据code查询FD的信息
+        :param site
+        :param project_code
         :param fd_code: 数据源code,code具有全局唯一性，所以这里可以直接根据code查询出数据
         :return: FactDatasource
         """
         if not fd_code:
             return None
 
         # 2020-09-16 16:46:18 sun 这里还是不能直接去查询数据库
-        fd = FactDatasourceClient.fd(fd_code)
+        fd = FactDatasourceClient.fd(site, project_code, fd_code)
         if fd is None:
             return None
         else:
             return FactDatasource(**fd)
 
-    def exists_fds(self, fd_codes: list) -> bool:
+    def exists_fds(self, site: str, project_code: str, fd_codes: list) -> bool:
         """
         判断fd_codes是否全部存在
+        :param site
+        :param project_code
         :param fd_codes:
         :return: bool
         """
         if not fd_codes:
             return False
 
-        return FactDatasourceClient.exists_fds(fd_codes)
+        return FactDatasourceClient.exists_fds(site, project_code, fd_codes)
         #
         # sql = f'SELECT code FROM `sc_factdatasource` WHERE code IN :fd_codes'
         # codes_dict = {'fd_codes': fd_codes}
         # codes_result = self.dao.select_all(sql, codes_dict)
         # if codes_result:
         #     codes_list = [re['code'] for re in codes_result]
         #     if len(fd_codes) == len(codes_list):
```

### Comparing `FicusFramework-3.0.9.post9/src/service/TaskQueueService.py` & `FicusFramework-3.1.0/src/service/TaskQueueService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/PKG-INFO` & `FicusFramework-3.1.0/src/FicusFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: FicusFramework
-Version: 3.0.9.post9
+Version: 3.1.0
 Summary: A framework for Ficus by Python3.
 Home-page: https://git.sobey.com/SobeyHive/FicusFramework4Py
 Author: sunxiang0918
 Author-email: sunxiang0918@gmail.com
 License: MIT
 Description: \u0023\u0020\u0046\u0069\u0063\u0075\u0073\u0020\u0050\u0079\u0074\u0068\u006f\u006e\u0020\u5f00\u53d1\u5957\u4ef6\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u5f00\u53d1\u6b65\u9aa4\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u5fc5\u987b\u8981\u6709\u4e00\u4e2a\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u6587\u4ef6\u002c\u7528\u4e8e\u53d1\u5e03\u0060\u0066\u006c\u0061\u0073\u006b\u0060\u7684\u0072\u0065\u0073\u0074\u0066\u0075\u006c\u0020\u0041\u0070\u0069\u000d\u000a\u0032\u002e\u0020\u5728\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u4e2d\u6267\u884c\u0060\u0061\u0070\u0070\u0020\u003d\u0020\u0046\u006c\u0061\u0073\u006b\u0028\u005f\u005f\u006e\u0061\u006d\u0065\u005f\u005f\u0029\u0060\u7528\u4e8e\u542f\u52a8\u0046\u006c\u0061\u0073\u006b\u670d\u52a1\u000d\u000a\u0033\u002e\u0020\u4f7f\u7528\u0060\u0066\u0072\u006f\u006d\u0020\u0072\u0065\u006d\u006f\u0074\u0065\u0020\u0069\u006d\u0070\u006f\u0072\u0074\u0020\u002a\u0060\u0020\u5bfc\u5165\u0072\u0065\u0073\u0074\u7684\u0060\u0065\u006e\u0064\u0070\u006f\u0069\u006e\u0074\u0060\u000d\u000a\u0034\u002e\u0020\u5728\u9879\u76ee\u4e2d\u521b\u5efa\u4e00\u4e2a\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u002c\u5e76\u6307\u5b9a\u670d\u52a1\u7684\u540d\u79f0\u548c\u0065\u0075\u0072\u0065\u006b\u0061\u7684\u5730\u5740\u000d\u000a\u0035\u002e\u0020\u8c03\u7528\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u7684\u65b9\u6cd5\u0060\u0072\u0065\u0067\u0069\u0073\u0074\u0065\u0072\u0028\u0026\u0071\u0075\u006f\u0074\u003b\u0055\u0050\u0026\u0071\u0075\u006f\u0074\u003b\u0029\u0060\u4ee5\u53ca\u0060\u0073\u0074\u0061\u0072\u0074\u005f\u0068\u0065\u0061\u0072\u0074\u0062\u0065\u0061\u0074\u0060\u5411\u0065\u0075\u0072\u0065\u006b\u0061\u6ce8\u518c\u53ca\u5fc3\u8df3\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u6ce8\u610f\u4e8b\u9879\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u0041\u0070\u0069\u4e2d\u6240\u6709\u7684\u0056\u004f\u5bf9\u8c61\u0020\u90fd\u662f\u7528\u4e86\u0020\u005b\u0060\u006d\u0075\u006e\u0063\u0068\u0060\u005d\u0028\u0068\u0074\u0074\u0070\u0073\u003a\u002f\u002f\u0067\u0069\u0074\u0068\u0075\u0062\u002e\u0063\u006f\u006d\u002f\u0049\u006e\u0066\u0069\u006e\u0069\u0064\u0061\u0074\u002f\u006d\u0075\u006e\u0063\u0068\u0029\u0020\u505a\u4ea4\u4e92\u002e
 Keywords: ficus framework python
```

### Comparing `FicusFramework-3.0.9.post9/src/FicusFramework.egg-info/SOURCES.txt` & `FicusFramework-3.1.0/src/FicusFramework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/api/handler/IAsyncAble.py
 src/api/handler/ICacheAble.py
 src/api/handler/ICacheAbleHandler.py
 src/api/handler/IHandler.py
 src/api/handler/IKillable.py
 src/api/handler/ILogAbleHandler.py
 src/api/handler/IProgressAble.py
+src/api/handler/IRevoke.py
 src/api/handler/ITaskHandler.py
 src/api/handler/__init__.py
 src/api/handler/ce/AbstractAsyncServiceBatchCE.py
 src/api/handler/ce/AbstractBatchCE.py
 src/api/handler/ce/AbstractMessageCE.py
 src/api/handler/ce/IMessageCE.py
 src/api/handler/ce/ISampleScriptCE.py
@@ -47,14 +48,15 @@
 src/api/model/AlgoOutWrapper.py
 src/api/model/AlgorithmFdInputWrapper.py
 src/api/model/AsyncServiceRequest.py
 src/api/model/AsyncServiceResponse.py
 src/api/model/BatchOutputPipe.py
 src/api/model/Condition.py
 src/api/model/FactDatasource.py
+src/api/model/FactDatasourceQueryParameter.py
 src/api/model/FdInputPipe.py
 src/api/model/FdInputWrapper.py
 src/api/model/GraphNode.py
 src/api/model/GraphRelation.py
 src/api/model/MetaModel.py
 src/api/model/MetaModelField.py
 src/api/model/MetaModelTransform.py
@@ -83,14 +85,15 @@
 src/config/BootstrapPropertyLoader.py
 src/config/__init__.py
 src/config/annotation.py
 src/discovery/__init__.py
 src/factdatasource/FactDatasourceContext.py
 src/factdatasource/FactDatasourceContextHolder.py
 src/factdatasource/FactDatasourceProxyService.py
+src/factdatasource/FactDatasourceProxyServiceV2.py
 src/factdatasource/__init__.py
 src/factdatasource/execptions.py
 src/factdatasource/dao/FactDatasource.py
 src/factdatasource/dao/MultipleDatasourceHolder.py
 src/factdatasource/dao/__init__.py
 src/factdatasource/dao/amqp/AmqpDatasourceDao.py
 src/factdatasource/dao/amqp/MultipleAmqpDatasource.py
@@ -111,14 +114,17 @@
 src/factdatasource/dao/mongo/__init__.py
 src/factdatasource/dao/redis/MultipleRedisDatasource.py
 src/factdatasource/dao/redis/RedisDatasourceDao.py
 src/factdatasource/dao/redis/__init__.py
 src/factdatasource/dao/stomp/MultipleStompDatasource.py
 src/factdatasource/dao/stomp/StompDatasourceDao.py
 src/factdatasource/dao/stomp/__init__.py
+src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py
+src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py
+src/factdatasource/dao/tablestore/__init__.py
 src/factdatasource/message/FactDatasourceMessageHanlder.py
 src/factdatasource/message/__init__.py
 src/factdatasource/persistence/AbstractFactDatasourceContext.py
 src/factdatasource/persistence/SqlableDeleteCondition.py
 src/factdatasource/persistence/__init__.py
 src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py
 src/factdatasource/persistence/algorithm/__init__.py
@@ -148,26 +154,29 @@
 src/factdatasource/persistence/mongo/__init__.py
 src/factdatasource/persistence/redis/RedisFactDatasourceContext.py
 src/factdatasource/persistence/redis/__init__.py
 src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py
 src/factdatasource/persistence/sobeyhive/__init__.py
 src/factdatasource/persistence/stomp/StompFactDatasourceContext.py
 src/factdatasource/persistence/stomp/__init__.py
+src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py
+src/factdatasource/persistence/tablestore/__init__.py
 src/factdatasource/transformer/ChineseToNumberTransformer.py
 src/factdatasource/transformer/CompleteGB32100Transformer.py
 src/factdatasource/transformer/CompleteStringTransformer.py
 src/factdatasource/transformer/DefaultValueTransformer.py
 src/factdatasource/transformer/FixItemTransformer.py
 src/factdatasource/transformer/ITransformer.py
 src/factdatasource/transformer/NumberToChineseTransformer.py
 src/factdatasource/transformer/ParseDateTimeTransformer.py
 src/factdatasource/transformer/TransformerContext.py
 src/factdatasource/transformer/__init__.py
 src/init/__init__.py
 src/init/app.py
+src/libs/HeaderHolder.py
 src/libs/__init__.py
 src/libs/utils.py
 src/py_eureka_client/__init__.py
 src/py_eureka_client/__logger__.py
 src/py_eureka_client/__urlopen_proxy__.py
 src/py_eureka_client/eureka_client.py
 src/py_eureka_client/http_client.py
```

### Comparing `FicusFramework-3.0.9.post9/src/client/ComputeExecutionClient.py` & `FicusFramework-3.1.0/src/client/ComputeExecutionClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/FactDatasourceManageClient.py` & `FicusFramework-3.1.0/src/client/FactDatasourceManageClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/ScheduleJobTaskLogClient.py` & `FicusFramework-3.1.0/src/client/ScheduleJobTaskLogClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     :param log_id:
     :param progress:
     :return:
     """
     check_instance_avaliable()
 
     try:
-        r = do_service(f"remote/sjtl-service/{log_id}/progress", params={"progress": progress})
+        r = do_service(f"remote/sjtl-service/{log_id}/progress", method="put", params={"progress": progress})
     except requests.exceptions.HTTPError as e:
         if e.response.status_code == 500:
             # 说明服务器端报错了
             raise ServiceInnerException(e.response._content.decode('utf-8'))
         elif e.response.status_code >= 400 and e.response.status_code < 500 and e.response.status_code != 404:
             # 说明是认证相关的错误
             raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
```

### Comparing `FicusFramework-3.0.9.post9/src/client/ScheduleCloudClient.py` & `FicusFramework-3.1.0/src/client/ScheduleCloudClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/HandlerLogClient.py` & `FicusFramework-3.1.0/src/client/HandlerLogClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/JobScheduleClient.py` & `FicusFramework-3.1.0/src/client/JobScheduleClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/DataCrawlClient.py` & `FicusFramework-3.1.0/src/client/DataCrawlClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/ClientAuth.py` & `FicusFramework-3.1.0/src/client/ClientAuth.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     pass
 
 
 @Value("${sobeycube.oauth.client_secret:}")
 def secret_key():
     pass
 
+
 @Value("${sobeycube.oauth.oauth_uri}")
 def user_center_uri():
     pass
 
+
 @Value("${sobeycube.oauth.username:}")
 def user_name():
     pass
 
 
 @Value("${sobeycube.oauth.password:}")
 def user_password():
@@ -43,37 +45,51 @@
 
 def acquire_access_token():
     """
     重新申请accessToken
     :return:
     """
     from client import AuthClient
+    from config import work_on_k8s, k8s_auth_server_service
+    auth_uri = k8s_auth_server_service if work_on_k8s else user_center_uri()
 
-    server, grant_type = ("sobeyficus", "client_credentials") if oauth2_type() == "server" else (
-        user_center_uri(), "password")
+    server, grant_type = (auth_uri, "client_credentials") if oauth2_type() == "client" else (
+        auth_uri, "password")
 
     token, expiration = AuthClient.oauth_access_token(server, grant_type, application_key(), secret_key(), user_name(),
                                                       user_password())
 
     global access_token
     access_token = token
 
     global oauth_expiration
     oauth_expiration = expiration
 
     return access_token
 
 
+def cancel_oauth_token():
+    """
+    废除当前的token
+    :return:
+    """
+    global access_token
+    global oauth_expiration
+    access_token = None
+    oauth_expiration = None
+
+
 def get_oauth_token():
     """
     生成oauth2的token
     :return:
     """
 
     global access_token
+    global oauth_expiration
     if access_token is None or (oauth_expiration is not None and oauth_expiration <= datetime.now()):
         #  说明没有token, 或者token过期了
         access_token = acquire_access_token()
 
     return access_token
```

### Comparing `FicusFramework-3.0.9.post9/src/client/DataAlgorithmClient.py` & `FicusFramework-3.1.0/src/client/DataAlgorithmClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/client/AuthClient.py` & `FicusFramework-3.1.0/src/client/AuthClient.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,19 @@
     :return:
     """
     check_instance_avaliable()
 
     try:
         from urllib.parse import quote
         # url 中需要编码处理下，避免其中有特殊字符
-        url = f"{server}/oauth/token?grant_type={quote(grant_type)}&scope=all&username={quote(str(username))}&password={quote(str(password))}"
+        url = f"{server}/oauth/token?grant_type={quote(grant_type)}&scope=all"
+        if "password" == grant_type:
+            # password方式再加上username和password
+            url = f"{url}&username={quote(str(username))}&password={quote(str(password))}"
+
         authorization = get_authorization_header(client_id, client_secret)
 
         r = requests.post(url, headers={"Authorization": authorization})
 
         if r is not None and r.status_code == 200:
             entity = Munch(r.json())
```

### Comparing `FicusFramework-3.0.9.post9/src/client/FactDatasourceClient.py` & `FicusFramework-3.1.0/src/client/FactDatasourceClient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
-针对FD的一些操作, 现已重构到 FactDatasourceProxyService.py 中
+针对FD的一些操作, 现已重构到 FactDatasourceProxyServiceV2.py 中
 2020-09-16 16:21:26 sun 不得行, 还是需要
 """
 import requests
 from munch import Munch
 
 from api.exceptions import ServiceInnerException, IllegalArgumentException, AuthException
 from client import check_instance_avaliable, do_service
 
 
-def fd(fd_code):
+def fd(site, project_code, fd_code):
     """
     获取某一个FD对象
+    :param site:
+    :param project_code:
     :param fd_code: fd的唯一code
     :return: FD对象
     """
     check_instance_avaliable()
 
     try:
-        r = do_service(f"/remote/fd-service/{fd_code}")
+        r = do_service(f"/remote/fd-service-v2/{site}/{project_code}/{fd_code}")
 
         if r is not None:
             return Munch(r)
         else:
             return None
     except requests.exceptions.HTTPError as e:
         if e.response.status_code == 500:
@@ -30,30 +32,32 @@
             raise ServiceInnerException(e.response._content.decode('utf-8'))
         elif e.response.status_code >= 400 and e.response.status_code<500 and e.response.status_code!=404:
             # 说明是认证相关的错误
             raise AuthException(f"服务端异常 {str(e)} {e.response._content.decode('utf-8')}")
         raise e
 
 
-def exists_fds(fds):
+def exists_fds(site, project_code,fds):
     """
     判断fd是否存在
+    :param project_code:
+    :param site:
     :param fds:
     :return:
     """
     if fds is None:
         return False
 
     if not isinstance(fds, list):
         raise IllegalArgumentException("检测fd是否存在失败,输入参数不是一个list")
 
     check_instance_avaliable()
 
     try:
-        r = do_service(f"/remote/fd-service/exists", method="post", data=fds,return_type = "bool")
+        r = do_service(f"/remote/fd-service-v2/{site}/{project_code}/exists", method="post", data=fds,return_type = "bool")
         if r is not None:
             return bool(r)
         else:
             return False
     except requests.exceptions.HTTPError as e:
         if e.response.status_code == 500:
             # 说明服务器端报错了
```

### Comparing `FicusFramework-3.0.9.post9/src/client/ScheduleCacheClient.py` & `FicusFramework-3.1.0/src/client/ScheduleCacheClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/remote/TriggerRemoteActor.py` & `FicusFramework-3.1.0/src/remote/TriggerRemoteActor.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/remote/__init__.py` & `FicusFramework-3.1.0/src/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/remote/PrometheusMetricsRemoteService.py` & `FicusFramework-3.1.0/src/remote/PrometheusMetricsRemoteService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/remote/LogReadRemoteService.py` & `FicusFramework-3.1.0/src/remote/LogReadRemoteService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.0.9.post9/src/remote/AsyncResponseRestService.py` & `FicusFramework-3.1.0/src/remote/AsyncResponseRestService.py`

 * *Files identical despite different names*

