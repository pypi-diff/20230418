# Comparing `tmp/splitio_client-9.4.0.tar.gz` & `tmp/splitio_client-9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splitio_client-9.4.0.tar", last modified: Wed Mar  1 20:24:53 2023, max compression
+gzip compressed data, was "dist/splitio_client-9.4.1.tar", last modified: Tue Apr 18 21:32:21 2023, max compression
```

## Comparing `splitio_client-9.4.0.tar` & `splitio_client-9.4.1.tar`

### file list

```diff
@@ -1,166 +1,168 @@
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-03-01 20:24:53.000000 splitio_client-9.4.0/PKG-INFO
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4097 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/SOURCES.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      296 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/requires.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/top_level.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio_client.egg-info/dependency_links.txt
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/integration/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    53057 2023-02-27 20:31:04.000000 splitio_client-9.4.0/tests/integration/test_client_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/integration/test_redis_integration.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-02-21 16:39:16.000000 splitio_client-9.4.0/tests/integration/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    60236 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/integration/test_streaming_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3469 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_segment_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1535 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_split_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11528 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2437 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/push/test_processor.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/recorder/test_recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-02-21 16:39:16.000000 splitio_client-9.4.0/tests/sync/test_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/test_impressions_count_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/test_unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-03-01 19:53:45.000000 splitio_client-9.4.0/tests/sync/test_segments_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/test_impressions_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21492 2023-02-28 02:57:11.000000 splitio_client-9.4.0/tests/sync/test_splits_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-02-28 02:47:29.000000 splitio_client-9.4.0/tests/sync/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7105 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/test_telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/sync/test_events_synchronizer.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/tests/helpers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/helpers/mockserver.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-02-21 16:39:06.000000 splitio_client-9.4.0/tests/helpers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4546 2023-02-21 16:39:06.000000 splitio_client-9.4.0/README.md
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1651 2023-02-21 16:39:06.000000 splitio_client-9.4.0/setup.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/tasks/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/split_sync.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/tasks/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/util/workerpool.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/util/asynctask.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/telemetry_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/events_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/segment_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/impressions_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/tasks/unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       22 2023-02-21 16:40:00.000000 splitio_client-9.4.0/splitio/version.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/util/time.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/util/backoff.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/util/threadutil.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/util/decorators.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/factories.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/models/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/models/grammar/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/partitions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4085 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/condition.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/misc.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/numeric.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/string.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/sets.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/grammar/matchers/base.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/token.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/notification.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    32493 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/datatypes.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/models/splits.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/storage/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/storage/adapters/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/adapters/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/adapters/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/adapters/cache_trait.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/adapters/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24562 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20617 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/storage/inmemmory.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/segmentworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2950 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/processor.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14206 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2048 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/splitworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9064 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/push/manager.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/recorder/recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/api/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2429 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/auth.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2921 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2866 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5162 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4136 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5182 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/commons.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2607 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/api/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/exceptions.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/impression.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/event.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-02-21 16:39:16.000000 splitio_client-9.4.0/splitio/sync/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3175 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20083 2023-02-27 20:34:37.000000 splitio_client-9.4.0/splitio/sync/split.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20973 2023-02-21 16:39:16.000000 splitio_client-9.4.0/splitio/sync/synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12478 2023-03-01 19:20:46.000000 splitio_client-9.4.0/splitio/sync/segment.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2916 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/sync/unique_keys.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/engine/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/engine/cache/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/cache/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/cache/lru.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12184 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/splitters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/engine/hashfns/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/hashfns/legacy.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/hashfns/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/hashfns/murmur3py.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/engine/impressions/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/strategies.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2688 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2970 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/unique_keys_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4572 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/impressions/adapters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6742 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/evaluator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/engine/filters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-03-01 20:24:53.000000 splitio_client-9.4.0/splitio/client/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4077 2023-02-21 16:39:16.000000 splitio_client-9.4.0/splitio/client/config.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    17747 2023-02-21 16:39:16.000000 splitio_client-9.4.0/splitio/client/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    25671 2023-02-21 16:39:16.000000 splitio_client-9.4.0/splitio/client/factory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/localhost.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16582 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/input_validator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3492 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-02-21 16:39:06.000000 splitio_client-9.4.0/splitio/client/listener.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-03-01 20:24:53.000000 splitio_client-9.4.0/setup.cfg
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-04-18 21:32:21.000000 splitio_client-9.4.1/PKG-INFO
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4174 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/requires.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/top_level.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/dependency_links.txt
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/integration/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    89669 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_client_e2e.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_redis_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11819 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_pluggable_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    60236 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_streaming_e2e.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/tests/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3469 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_segment_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1535 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_split_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_status_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11528 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2437 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_processor.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/recorder/test_recorder.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/recorder/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_impressions_count_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_unique_keys_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_segments_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_impressions_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21492 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_splits_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7167 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_events_synchronizer.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/helpers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/helpers/mockserver.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/helpers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4517 2023-04-18 21:32:05.000000 splitio_client-9.4.1/README.md
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1672 2023-04-18 21:32:05.000000 splitio_client-9.4.1/setup.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/tasks/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/split_sync.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/tasks/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/workerpool.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/asynctask.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/telemetry_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/events_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/segment_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/impressions_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/unique_keys_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       21 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/version.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/time.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/backoff.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/threadutil.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/decorators.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/factories.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/grammar/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/partitions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4085 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/condition.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/misc.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/numeric.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/string.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/sets.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/base.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/token.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/notification.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    32610 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/datatypes.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/splits.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/storage/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    30128 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/pluggable.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/storage/adapters/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/cache_trait.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24198 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20617 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/inmemmory.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/segmentworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2950 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/processor.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14206 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/status_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2048 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/splitworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9064 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/manager.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/recorder/recorder.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/recorder/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/api/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2429 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/auth.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2921 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2866 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5162 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4136 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5182 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/commons.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2607 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/exceptions.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/impression.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/event.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3175 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20083 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/split.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    22571 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12478 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/segment.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2916 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/unique_keys.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/cache/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/cache/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/cache/lru.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12184 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/splitters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/hashfns/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/legacy.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/murmur3py.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/impressions/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/strategies.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2970 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/unique_keys_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7035 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/adapters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6742 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/evaluator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/filters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/client/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4825 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/config.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    17773 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    28999 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/factory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/localhost.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18655 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/input_validator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3492 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/listener.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-04-18 21:32:21.000000 splitio_client-9.4.1/setup.cfg
```

### Comparing `splitio_client-9.4.0/PKG-INFO` & `splitio_client-9.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio_client
-Version: 9.4.0
+Version: 9.4.1
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.0
+Download-URL: https://github.com/splitio/python-client/tarball/9.4.1
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: cpphash
 Provides-Extra: uwsgi
 Provides-Extra: redis
 Provides-Extra: test
+Provides-Extra: cpphash
```

### Comparing `splitio_client-9.4.0/splitio_client.egg-info/PKG-INFO` & `splitio_client-9.4.1/splitio_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio-client
-Version: 9.4.0
+Version: 9.4.1
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.0
+Download-URL: https://github.com/splitio/python-client/tarball/9.4.1
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: cpphash
 Provides-Extra: uwsgi
 Provides-Extra: redis
 Provides-Extra: test
+Provides-Extra: cpphash
```

### Comparing `splitio_client-9.4.0/splitio_client.egg-info/SOURCES.txt` & `splitio_client-9.4.1/splitio_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 splitio/push/splitworker.py
 splitio/push/sse.py
 splitio/push/status_tracker.py
 splitio/recorder/__init__.py
 splitio/recorder/recorder.py
 splitio/storage/__init__.py
 splitio/storage/inmemmory.py
+splitio/storage/pluggable.py
 splitio/storage/redis.py
 splitio/storage/adapters/__init__.py
 splitio/storage/adapters/cache_trait.py
 splitio/storage/adapters/redis.py
 splitio/storage/adapters/util.py
 splitio/sync/__init__.py
 splitio/sync/event.py
@@ -110,14 +111,15 @@
 splitio_client.egg-info/requires.txt
 splitio_client.egg-info/top_level.txt
 tests/__init__.py
 tests/helpers/__init__.py
 tests/helpers/mockserver.py
 tests/integration/__init__.py
 tests/integration/test_client_e2e.py
+tests/integration/test_pluggable_integration.py
 tests/integration/test_redis_integration.py
 tests/integration/test_streaming_e2e.py
 tests/push/__init__.py
 tests/push/test_manager.py
 tests/push/test_parser.py
 tests/push/test_processor.py
 tests/push/test_segment_worker.py
```

### Comparing `splitio_client-9.4.0/tests/integration/test_client_e2e.py` & `splitio_client-9.4.1/tests/integration/test_client_e2e.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,26 +11,34 @@
 from splitio.exceptions import TimeoutException
 from splitio.client.factory import get_factory, SplitFactory
 from splitio.client.util import SdkMetadata
 from splitio.storage.inmemmory import InMemoryEventStorage, InMemoryImpressionStorage, \
     InMemorySegmentStorage, InMemorySplitStorage, InMemoryTelemetryStorage
 from splitio.storage.redis import RedisEventsStorage, RedisImpressionsStorage, \
     RedisSplitStorage, RedisSegmentStorage, RedisTelemetryStorage
+from splitio.storage.pluggable import PluggableEventsStorage, PluggableImpressionsStorage, PluggableSegmentStorage, \
+    PluggableTelemetryStorage, PluggableSplitStorage
 from splitio.storage.adapters.redis import build, RedisAdapter
 from splitio.models import splits, segments
 from splitio.engine.impressions.impressions import Manager as ImpressionsManager, ImpressionsMode
-from splitio.engine.impressions.strategies import StrategyDebugMode, StrategyOptimizedMode
+from splitio.engine.impressions import set_classes
+from splitio.engine.impressions.strategies import StrategyDebugMode, StrategyOptimizedMode, StrategyNoneMode
 from splitio.engine.impressions.manager import Counter
 from splitio.engine.telemetry import TelemetryStorageConsumer, TelemetryStorageProducer
 from splitio.engine.impressions.manager import Counter as ImpressionsCounter
 from splitio.recorder.recorder import StandardRecorder, PipelinedRecorder
 from splitio.client.config import DEFAULT_CONFIG
-from splitio.sync.synchronizer import SplitTasks, SplitSynchronizers, Synchronizer
-from splitio.sync.manager import Manager
+from splitio.sync.synchronizer import SplitTasks, SplitSynchronizers, Synchronizer, RedisSynchronizer
+from splitio.sync.manager import Manager, RedisManager
+from splitio.sync.synchronizer import PluggableSynchronizer
+
 from tests.integration import splits_json
+from tests.storage.test_pluggable import StorageMockAdapter
+
+
 class InMemoryIntegrationTests(object):
     """Inmemory storage-based integration tests."""
 
     def setup_method(self):
         """Prepare storages with test data."""
         split_storage = InMemorySplitStorage()
         segment_storage = InMemorySegmentStorage()
@@ -1120,7 +1128,751 @@
         }
         assert manager.split('other_feature').configs == {}
         assert manager.split('other_feature_2').configs == {}
         assert manager.split('other_feature_3').configs == {}
         event = threading.Event()
         factory.destroy(event)
         event.wait()
+
+
+class PluggableIntegrationTests(object):
+    """Pluggable storage-based integration tests."""
+
+    def setup_method(self):
+        """Prepare storages with test data."""
+        metadata = SdkMetadata('python-1.2.3', 'some_ip', 'some_name')
+        self.pluggable_storage_adapter = StorageMockAdapter()
+        split_storage = PluggableSplitStorage(self.pluggable_storage_adapter, 'myprefix')
+        segment_storage = PluggableSegmentStorage(self.pluggable_storage_adapter, 'myprefix')
+
+        telemetry_pluggable_storage = PluggableTelemetryStorage(self.pluggable_storage_adapter, metadata, 'myprefix')
+        telemetry_producer = TelemetryStorageProducer(telemetry_pluggable_storage)
+        telemetry_consumer = TelemetryStorageConsumer(telemetry_pluggable_storage)
+        telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
+
+        storages = {
+            'splits': split_storage,
+            'segments': segment_storage,
+            'impressions': PluggableImpressionsStorage(self.pluggable_storage_adapter, metadata),
+            'events': PluggableEventsStorage(self.pluggable_storage_adapter, metadata),
+            'telemetry': telemetry_pluggable_storage
+        }
+
+        impmanager = ImpressionsManager(StrategyDebugMode(), telemetry_runtime_producer) # no listener
+        recorder = StandardRecorder(impmanager, storages['events'],
+                                    storages['impressions'], storages['telemetry'])
+
+        self.factory = SplitFactory('some_api_key',
+                                    storages,
+                                    True,
+                                    recorder,
+                                    RedisManager(PluggableSynchronizer()),
+                                    sdk_ready_flag=None,
+                                    telemetry_producer=telemetry_producer,
+                                    telemetry_init_producer=telemetry_producer.get_telemetry_init_producer(),
+                                    )  # pylint:disable=attribute-defined-outside-init
+
+        # Adding data to storage
+        split_fn = os.path.join(os.path.dirname(__file__), 'files', 'splitChanges.json')
+        with open(split_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        for split in data['splits']:
+            self.pluggable_storage_adapter.set(split_storage._prefix.format(split_name=split['name']), split)
+        self.pluggable_storage_adapter.set(split_storage._split_till_prefix, data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentEmployeesChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentHumanBeignsChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+
+    def _validate_last_events(self, client, *to_validate):
+        """Validate the last N impressions are present disregarding the order."""
+        event_storage = client._factory._get_storage('events')
+        events_raw = []
+        stored_events = self.pluggable_storage_adapter.pop_items(event_storage._events_queue_key)
+        if stored_events is not None:
+            events_raw = [json.loads(im) for im in stored_events]
+
+        as_tup_set = set(
+            (i['e']['key'], i['e']['trafficTypeName'], i['e']['eventTypeId'], i['e']['value'], str(i['e']['properties']))
+            for i in events_raw
+        )
+        assert as_tup_set == set(to_validate)
+
+    def _validate_last_impressions(self, client, *to_validate):
+        """Validate the last N impressions are present disregarding the order."""
+        imp_storage = client._factory._get_storage('impressions')
+        impressions_raw = []
+        stored_impressions = self.pluggable_storage_adapter.pop_items(imp_storage._impressions_queue_key)
+        if stored_impressions is not None:
+            impressions_raw = [json.loads(im) for im in stored_impressions]
+        as_tup_set = set(
+            (i['i']['f'], i['i']['k'], i['i']['t'])
+            for i in impressions_raw
+        )
+
+        assert as_tup_set == set(to_validate)
+
+    def test_get_treatment(self):
+        """Test client.get_treatment()."""
+        client = self.factory.client()
+
+        assert client.get_treatment('user1', 'sample_feature') == 'on'
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        assert client.get_treatment('invalidKey', 'sample_feature') == 'off'
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        assert client.get_treatment('invalidKey', 'invalid_feature') == 'control'
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        assert client.get_treatment('invalidKey', 'killed_feature') == 'defTreatment'
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        assert client.get_treatment('invalidKey', 'all_feature') == 'on'
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing WHITELIST matcher
+        assert client.get_treatment('whitelisted_user', 'whitelist_feature') == 'on'
+        self._validate_last_impressions(client, ('whitelist_feature', 'whitelisted_user', 'on'))
+        assert client.get_treatment('unwhitelisted_user', 'whitelist_feature') == 'off'
+        self._validate_last_impressions(client, ('whitelist_feature', 'unwhitelisted_user', 'off'))
+
+        #  testing INVALID matcher
+        assert client.get_treatment('some_user_key', 'invalid_matcher_feature') == 'control'
+        self._validate_last_impressions(client)
+
+        #  testing Dependency matcher
+        assert client.get_treatment('somekey', 'dependency_test') == 'off'
+        self._validate_last_impressions(client, ('dependency_test', 'somekey', 'off'))
+
+        #  testing boolean matcher
+        assert client.get_treatment('True', 'boolean_test') == 'on'
+        self._validate_last_impressions(client, ('boolean_test', 'True', 'on'))
+
+        #  testing regex matcher
+        assert client.get_treatment('abc4', 'regex_test') == 'on'
+        self._validate_last_impressions(client, ('regex_test', 'abc4', 'on'))
+
+    def test_get_treatment_with_config(self):
+        """Test client.get_treatment_with_config()."""
+        client = self.factory.client()
+
+        result = client.get_treatment_with_config('user1', 'sample_feature')
+        assert result == ('on', '{"size":15,"test":20}')
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        result = client.get_treatment_with_config('invalidKey', 'sample_feature')
+        assert result == ('off', None)
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        result = client.get_treatment_with_config('invalidKey', 'invalid_feature')
+        assert result == ('control', None)
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        result = client.get_treatment_with_config('invalidKey', 'killed_feature')
+        assert ('defTreatment', '{"size":15,"defTreatment":true}') == result
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        result = client.get_treatment_with_config('invalidKey', 'all_feature')
+        assert result == ('on', None)
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+    def test_get_treatments(self):
+        """Test client.get_treatments()."""
+        client = self.factory.client()
+
+        result = client.get_treatments('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'on'
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        result = client.get_treatments('invalidKey', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'off'
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        result = client.get_treatments('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == 'control'
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        result = client.get_treatments('invalidKey', ['killed_feature'])
+        assert len(result) == 1
+        assert result['killed_feature'] == 'defTreatment'
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        result = client.get_treatments('invalidKey', ['all_feature'])
+        assert len(result) == 1
+        assert result['all_feature'] == 'on'
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing multiple splitNames
+        result = client.get_treatments('invalidKey', [
+            'all_feature',
+            'killed_feature',
+            'invalid_feature',
+            'sample_feature'
+        ])
+        assert len(result) == 4
+        assert result['all_feature'] == 'on'
+        assert result['killed_feature'] == 'defTreatment'
+        assert result['invalid_feature'] == 'control'
+        assert result['sample_feature'] == 'off'
+        self._validate_last_impressions(
+            client,
+            ('all_feature', 'invalidKey', 'on'),
+            ('killed_feature', 'invalidKey', 'defTreatment'),
+            ('sample_feature', 'invalidKey', 'off')
+        )
+
+    def test_get_treatments_with_config(self):
+        """Test client.get_treatments_with_config()."""
+        client = self.factory.client()
+
+        result = client.get_treatments_with_config('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('on', '{"size":15,"test":20}')
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        result = client.get_treatments_with_config('invalidKey', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('off', None)
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        result = client.get_treatments_with_config('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == ('control', None)
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        result = client.get_treatments_with_config('invalidKey', ['killed_feature'])
+        assert len(result) == 1
+        assert result['killed_feature'] == ('defTreatment', '{"size":15,"defTreatment":true}')
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        result = client.get_treatments_with_config('invalidKey', ['all_feature'])
+        assert len(result) == 1
+        assert result['all_feature'] == ('on', None)
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing multiple splitNames
+        result = client.get_treatments_with_config('invalidKey', [
+            'all_feature',
+            'killed_feature',
+            'invalid_feature',
+            'sample_feature'
+        ])
+        assert len(result) == 4
+        assert result['all_feature'] == ('on', None)
+        assert result['killed_feature'] == ('defTreatment', '{"size":15,"defTreatment":true}')
+        assert result['invalid_feature'] == ('control', None)
+        assert result['sample_feature'] == ('off', None)
+        self._validate_last_impressions(
+            client,
+            ('all_feature', 'invalidKey', 'on'),
+            ('killed_feature', 'invalidKey', 'defTreatment'),
+            ('sample_feature', 'invalidKey', 'off'),
+        )
+
+    def test_track(self):
+        """Test client.track()."""
+        client = self.factory.client()
+        assert(client.track('user1', 'user', 'conversion', 1, {"prop1": "value1"}))
+        assert(not client.track(None, 'user', 'conversion'))
+        assert(not client.track('user1', None, 'conversion'))
+        assert(not client.track('user1', 'user', None))
+        self._validate_last_events(
+            client,
+            ('user1', 'user', 'conversion', 1, "{'prop1': 'value1'}")
+        )
+
+    def test_manager_methods(self):
+        """Test manager.split/splits."""
+        try:
+            manager = self.factory.manager()
+        except:
+            pass
+        result = manager.split('all_feature')
+        assert result.name == 'all_feature'
+        assert result.traffic_type is None
+        assert result.killed is False
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs == {}
+
+        result = manager.split('killed_feature')
+        assert result.name == 'killed_feature'
+        assert result.traffic_type is None
+        assert result.killed is True
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs['defTreatment'] == '{"size":15,"defTreatment":true}'
+        assert result.configs['off'] == '{"size":15,"test":20}'
+
+        result = manager.split('sample_feature')
+        assert result.name == 'sample_feature'
+        assert result.traffic_type is None
+        assert result.killed is False
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs['on'] == '{"size":15,"test":20}'
+
+        assert len(manager.split_names()) == 7
+        assert len(manager.splits()) == 7
+
+    def teardown_method(self):
+        """Clear pluggable cache."""
+        keys_to_delete = [
+            "SPLITIO.segment.human_beigns",
+            "SPLITIO.segment.employees.till",
+            "SPLITIO.split.sample_feature",
+            "SPLITIO.splits.till",
+            "SPLITIO.split.killed_feature",
+            "SPLITIO.split.all_feature",
+            "SPLITIO.split.whitelist_feature",
+            "SPLITIO.segment.employees",
+            "SPLITIO.split.regex_test",
+            "SPLITIO.segment.human_beigns.till",
+            "SPLITIO.split.boolean_test",
+            "SPLITIO.split.dependency_test"
+        ]
+
+        for key in keys_to_delete:
+            self.pluggable_storage_adapter.delete(key)
+
+class PluggableOptimizedIntegrationTests(object):
+    """Pluggable storage-based integration tests."""
+
+    def setup_method(self):
+        """Prepare storages with test data."""
+        metadata = SdkMetadata('python-1.2.3', 'some_ip', 'some_name')
+        self.pluggable_storage_adapter = StorageMockAdapter()
+        split_storage = PluggableSplitStorage(self.pluggable_storage_adapter, 'myprefix')
+        segment_storage = PluggableSegmentStorage(self.pluggable_storage_adapter, 'myprefix')
+
+        telemetry_pluggable_storage = PluggableTelemetryStorage(self.pluggable_storage_adapter, metadata, 'myprefix')
+        telemetry_producer = TelemetryStorageProducer(telemetry_pluggable_storage)
+        telemetry_consumer = TelemetryStorageConsumer(telemetry_pluggable_storage)
+        telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
+
+        storages = {
+            'splits': split_storage,
+            'segments': segment_storage,
+            'impressions': PluggableImpressionsStorage(self.pluggable_storage_adapter, metadata, 'myprefix'),
+            'events': PluggableEventsStorage(self.pluggable_storage_adapter, metadata, 'myprefix'),
+            'telemetry': telemetry_pluggable_storage
+        }
+
+        impmanager = ImpressionsManager(StrategyOptimizedMode(ImpressionsCounter()), telemetry_runtime_producer) # no listener
+        recorder = StandardRecorder(impmanager, storages['events'],
+                                    storages['impressions'], storages['telemetry'])
+
+        self.factory = SplitFactory('some_api_key',
+                                    storages,
+                                    True,
+                                    recorder,
+                                    RedisManager(PluggableSynchronizer()),
+                                    sdk_ready_flag=None,
+                                    telemetry_producer=telemetry_producer,
+                                    telemetry_init_producer=telemetry_producer.get_telemetry_init_producer(),
+                                    )  # pylint:disable=attribute-defined-outside-init
+
+        # Adding data to storage
+        split_fn = os.path.join(os.path.dirname(__file__), 'files', 'splitChanges.json')
+        with open(split_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        for split in data['splits']:
+            self.pluggable_storage_adapter.set(split_storage._prefix.format(split_name=split['name']), split)
+        self.pluggable_storage_adapter.set(split_storage._split_till_prefix, data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentEmployeesChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentHumanBeignsChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+
+    def _validate_last_events(self, client, *to_validate):
+        """Validate the last N impressions are present disregarding the order."""
+        event_storage = client._factory._get_storage('events')
+        events_raw = []
+        stored_events = self.pluggable_storage_adapter.pop_items(event_storage._events_queue_key)
+        if stored_events is not None:
+            events_raw = [json.loads(im) for im in stored_events]
+
+        as_tup_set = set(
+            (i['e']['key'], i['e']['trafficTypeName'], i['e']['eventTypeId'], i['e']['value'], str(i['e']['properties']))
+            for i in events_raw
+        )
+        assert as_tup_set == set(to_validate)
+
+    def _validate_last_impressions(self, client, *to_validate):
+        """Validate the last N impressions are present disregarding the order."""
+        imp_storage = client._factory._get_storage('impressions')
+        impressions_raw = []
+        stored_impressions = self.pluggable_storage_adapter.pop_items(imp_storage._impressions_queue_key)
+        if stored_impressions is not None:
+            impressions_raw = [json.loads(im) for im in stored_impressions]
+        as_tup_set = set(
+            (i['i']['f'], i['i']['k'], i['i']['t'])
+            for i in impressions_raw
+        )
+
+        assert as_tup_set == set(to_validate)
+
+    def test_get_treatment(self):
+        """Test client.get_treatment()."""
+        client = self.factory.client()
+
+        assert client.get_treatment('user1', 'sample_feature') == 'on'
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+        client.get_treatment('user1', 'sample_feature')
+        client.get_treatment('user1', 'sample_feature')
+        client.get_treatment('user1', 'sample_feature')
+
+        # Only one impression was added, and popped when validating, the rest were ignored
+#        pytest.set_trace()
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+        assert client.get_treatment('invalidKey', 'sample_feature') == 'off'
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        assert client.get_treatment('invalidKey', 'invalid_feature') == 'control'
+        self._validate_last_impressions(client)  # No impressions should be present
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        assert client.get_treatment('invalidKey', 'killed_feature') == 'defTreatment'
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        assert client.get_treatment('invalidKey', 'all_feature') == 'on'
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing WHITELIST matcher
+        assert client.get_treatment('whitelisted_user', 'whitelist_feature') == 'on'
+        self._validate_last_impressions(client, ('whitelist_feature', 'whitelisted_user', 'on'))
+        assert client.get_treatment('unwhitelisted_user', 'whitelist_feature') == 'off'
+        self._validate_last_impressions(client, ('whitelist_feature', 'unwhitelisted_user', 'off'))
+
+        #  testing INVALID matcher
+        assert client.get_treatment('some_user_key', 'invalid_matcher_feature') == 'control'
+        self._validate_last_impressions(client)  # No impressions should be present
+
+        #  testing Dependency matcher
+        assert client.get_treatment('somekey', 'dependency_test') == 'off'
+        self._validate_last_impressions(client, ('dependency_test', 'somekey', 'off'))
+
+        #  testing boolean matcher
+        assert client.get_treatment('True', 'boolean_test') == 'on'
+        self._validate_last_impressions(client, ('boolean_test', 'True', 'on'))
+
+        #  testing regex matcher
+        assert client.get_treatment('abc4', 'regex_test') == 'on'
+        self._validate_last_impressions(client, ('regex_test', 'abc4', 'on'))
+
+    def test_get_treatments(self):
+        """Test client.get_treatments()."""
+        client = self.factory.client()
+
+        result = client.get_treatments('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'on'
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        result = client.get_treatments('invalidKey', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'off'
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        result = client.get_treatments('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == 'control'
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        result = client.get_treatments('invalidKey', ['killed_feature'])
+        assert len(result) == 1
+        assert result['killed_feature'] == 'defTreatment'
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        result = client.get_treatments('invalidKey', ['all_feature'])
+        assert len(result) == 1
+        assert result['all_feature'] == 'on'
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing multiple splitNames
+        result = client.get_treatments('invalidKey', [
+            'all_feature',
+            'killed_feature',
+            'invalid_feature',
+            'sample_feature'
+        ])
+        assert len(result) == 4
+        assert result['all_feature'] == 'on'
+        assert result['killed_feature'] == 'defTreatment'
+        assert result['invalid_feature'] == 'control'
+        assert result['sample_feature'] == 'off'
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+    def test_get_treatments_with_config(self):
+        """Test client.get_treatments_with_config()."""
+        client = self.factory.client()
+
+        result = client.get_treatments_with_config('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('on', '{"size":15,"test":20}')
+        self._validate_last_impressions(client, ('sample_feature', 'user1', 'on'))
+
+        result = client.get_treatments_with_config('invalidKey', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('off', None)
+        self._validate_last_impressions(client, ('sample_feature', 'invalidKey', 'off'))
+
+        result = client.get_treatments_with_config('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == ('control', None)
+        self._validate_last_impressions(client)
+
+        # testing a killed feature. No matter what the key, must return default treatment
+        result = client.get_treatments_with_config('invalidKey', ['killed_feature'])
+        assert len(result) == 1
+        assert result['killed_feature'] == ('defTreatment', '{"size":15,"defTreatment":true}')
+        self._validate_last_impressions(client, ('killed_feature', 'invalidKey', 'defTreatment'))
+
+        # testing ALL matcher
+        result = client.get_treatments_with_config('invalidKey', ['all_feature'])
+        assert len(result) == 1
+        assert result['all_feature'] == ('on', None)
+        self._validate_last_impressions(client, ('all_feature', 'invalidKey', 'on'))
+
+        # testing multiple splitNames
+        result = client.get_treatments_with_config('invalidKey', [
+            'all_feature',
+            'killed_feature',
+            'invalid_feature',
+            'sample_feature'
+        ])
+        assert len(result) == 4
+
+        assert result['all_feature'] == ('on', None)
+        assert result['killed_feature'] == ('defTreatment', '{"size":15,"defTreatment":true}')
+        assert result['invalid_feature'] == ('control', None)
+        assert result['sample_feature'] == ('off', None)
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+    def test_manager_methods(self):
+        """Test manager.split/splits."""
+        manager = self.factory.manager()
+        result = manager.split('all_feature')
+        assert result.name == 'all_feature'
+        assert result.traffic_type is None
+        assert result.killed is False
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs == {}
+
+        result = manager.split('killed_feature')
+        assert result.name == 'killed_feature'
+        assert result.traffic_type is None
+        assert result.killed is True
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs['defTreatment'] == '{"size":15,"defTreatment":true}'
+        assert result.configs['off'] == '{"size":15,"test":20}'
+
+        result = manager.split('sample_feature')
+        assert result.name == 'sample_feature'
+        assert result.traffic_type is None
+        assert result.killed is False
+        assert len(result.treatments) == 2
+        assert result.change_number == 123
+        assert result.configs['on'] == '{"size":15,"test":20}'
+
+        assert len(manager.split_names()) == 7
+        assert len(manager.splits()) == 7
+
+    def test_track(self):
+        """Test client.track()."""
+        client = self.factory.client()
+        assert(client.track('user1', 'user', 'conversion', 1, {"prop1": "value1"}))
+        assert(not client.track(None, 'user', 'conversion'))
+        assert(not client.track('user1', None, 'conversion'))
+        assert(not client.track('user1', 'user', None))
+        self._validate_last_events(
+            client,
+            ('user1', 'user', 'conversion', 1, "{'prop1': 'value1'}")
+        )
+
+class PluggableNoneIntegrationTests(object):
+    """Pluggable storage-based integration tests."""
+
+    def setup_method(self):
+        """Prepare storages with test data."""
+        metadata = SdkMetadata('python-1.2.3', 'some_ip', 'some_name')
+        self.pluggable_storage_adapter = StorageMockAdapter()
+        split_storage = PluggableSplitStorage(self.pluggable_storage_adapter, 'myprefix')
+        segment_storage = PluggableSegmentStorage(self.pluggable_storage_adapter, 'myprefix')
+
+        telemetry_pluggable_storage = PluggableTelemetryStorage(self.pluggable_storage_adapter, metadata, 'myprefix')
+        telemetry_producer = TelemetryStorageProducer(telemetry_pluggable_storage)
+        telemetry_consumer = TelemetryStorageConsumer(telemetry_pluggable_storage)
+        telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
+
+        storages = {
+            'splits': split_storage,
+            'segments': segment_storage,
+            'impressions': PluggableImpressionsStorage(self.pluggable_storage_adapter, metadata, 'myprefix'),
+            'events': PluggableEventsStorage(self.pluggable_storage_adapter, metadata, 'myprefix'),
+            'telemetry': telemetry_pluggable_storage
+        }
+
+        unique_keys_synchronizer, clear_filter_sync, unique_keys_task, \
+        clear_filter_task, impressions_count_sync, impressions_count_task, \
+        imp_strategy = set_classes('PLUGGABLE', ImpressionsMode.NONE, self.pluggable_storage_adapter, 'myprefix')
+        impmanager = ImpressionsManager(imp_strategy, telemetry_runtime_producer) # no listener
+
+        recorder = StandardRecorder(impmanager, storages['events'],
+                                    storages['impressions'], storages['telemetry'])
+
+        synchronizers = SplitSynchronizers(None, None, None, None,
+            impressions_count_sync,
+            None,
+            unique_keys_synchronizer,
+            clear_filter_sync
+        )
+
+        tasks = SplitTasks(None, None, None, None,
+            impressions_count_task,
+            None,
+            unique_keys_task,
+            clear_filter_task
+        )
+
+        synchronizer = RedisSynchronizer(synchronizers, tasks)
+
+        manager = RedisManager(synchronizer)
+        manager.start()
+        self.factory = SplitFactory('some_api_key',
+                                    storages,
+                                    True,
+                                    recorder,
+                                    manager,
+                                    sdk_ready_flag=None,
+                                    telemetry_producer=telemetry_producer,
+                                    telemetry_init_producer=telemetry_producer.get_telemetry_init_producer(),
+                                    )  # pylint:disable=attribute-defined-outside-init
+
+        # Adding data to storage
+        split_fn = os.path.join(os.path.dirname(__file__), 'files', 'splitChanges.json')
+        with open(split_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        for split in data['splits']:
+            self.pluggable_storage_adapter.set(split_storage._prefix.format(split_name=split['name']), split)
+        self.pluggable_storage_adapter.set(split_storage._split_till_prefix, data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentEmployeesChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+
+        segment_fn = os.path.join(os.path.dirname(__file__), 'files', 'segmentHumanBeignsChanges.json')
+        with open(segment_fn, 'r') as flo:
+            data = json.loads(flo.read())
+        self.pluggable_storage_adapter.set(segment_storage._prefix.format(segment_name=data['name']), set(data['added']))
+        self.pluggable_storage_adapter.set(segment_storage._segment_till_prefix.format(segment_name=data['name']), data['till'])
+        self.client = self.factory.client()
+
+
+    def _validate_last_events(self, client, *to_validate):
+        """Validate the last N impressions are present disregarding the order."""
+        event_storage = client._factory._get_storage('events')
+        events_raw = []
+        stored_events = self.pluggable_storage_adapter.pop_items(event_storage._events_queue_key)
+        if stored_events is not None:
+            events_raw = [json.loads(im) for im in stored_events]
+
+        as_tup_set = set(
+            (i['e']['key'], i['e']['trafficTypeName'], i['e']['eventTypeId'], i['e']['value'], str(i['e']['properties']))
+            for i in events_raw
+        )
+        assert as_tup_set == set(to_validate)
+
+    def test_get_treatment(self):
+        """Test client.get_treatment()."""
+        assert self.client.get_treatment('user1', 'sample_feature') == 'on'
+        assert self.client.get_treatment('invalidKey', 'sample_feature') == 'off'
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+    def test_get_treatments(self):
+        """Test client.get_treatments()."""
+        result = self.client.get_treatments('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'on'
+
+        result = self.client.get_treatments('invalidKey', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == 'off'
+
+        result = self.client.get_treatments('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == 'control'
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+    def test_get_treatments_with_config(self):
+        """Test client.get_treatments_with_config()."""
+        result = self.client.get_treatments_with_config('user1', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('on', '{"size":15,"test":20}')
+
+        result = self.client.get_treatments_with_config('invalidKey2', ['sample_feature'])
+        assert len(result) == 1
+        assert result['sample_feature'] == ('off', None)
+
+        result = self.client.get_treatments_with_config('invalidKey', ['invalid_feature'])
+        assert len(result) == 1
+        assert result['invalid_feature'] == ('control', None)
+        assert self.pluggable_storage_adapter._keys['myprefix.SPLITIO.impressions'] == []
+
+    def test_track(self):
+        """Test client.track()."""
+        assert(self.client.track('user1', 'user', 'conversion', 1, {"prop1": "value1"}))
+        assert(not self.client.track(None, 'user', 'conversion'))
+        assert(not self.client.track('user1', None, 'conversion'))
+        assert(not self.client.track('user1', 'user', None))
+        self._validate_last_events(
+            self.client,
+            ('user1', 'user', 'conversion', 1, "{'prop1': 'value1'}")
+        )
+
+    def test_mtk(self):
+        self.client.get_treatment('user1', 'sample_feature')
+        self.client.get_treatment('invalidKey', 'sample_feature')
+        self.client.get_treatment('invalidKey2', 'sample_feature')
+        self.client.get_treatment('user22', 'invalidFeature')
+        event = threading.Event()
+        self.factory.destroy(event)
+        event.wait()
+        assert(json.loads(self.pluggable_storage_adapter._keys['myprefix.SPLITIO.uniquekeys'][0])["f"] =="sample_feature")
+        assert(json.loads(self.pluggable_storage_adapter._keys['myprefix.SPLITIO.uniquekeys'][0])["ks"].sort() ==
+               ["invalidKey2", "invalidKey", "user1"].sort())
```

### Comparing `splitio_client-9.4.0/tests/integration/test_redis_integration.py` & `splitio_client-9.4.1/tests/integration/test_redis_integration.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/integration/__init__.py` & `splitio_client-9.4.1/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/integration/test_streaming_e2e.py` & `splitio_client-9.4.1/tests/integration/test_streaming_e2e.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_parser.py` & `splitio_client-9.4.1/tests/push/test_parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_splitsse.py` & `splitio_client-9.4.1/tests/push/test_splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_sse.py` & `splitio_client-9.4.1/tests/push/test_sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_segment_worker.py` & `splitio_client-9.4.1/tests/push/test_segment_worker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_split_worker.py` & `splitio_client-9.4.1/tests/push/test_split_worker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_status_tracker.py` & `splitio_client-9.4.1/tests/push/test_status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_manager.py` & `splitio_client-9.4.1/tests/push/test_manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/push/test_processor.py` & `splitio_client-9.4.1/tests/push/test_processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/recorder/test_recorder.py` & `splitio_client-9.4.1/tests/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_impressions_count_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_impressions_count_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_unique_keys_sync.py` & `splitio_client-9.4.1/tests/sync/test_unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_segments_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_segments_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_impressions_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_impressions_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_splits_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_splits_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_manager.py` & `splitio_client-9.4.1/tests/sync/test_manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/sync/test_telemetry.py` & `splitio_client-9.4.1/tests/sync/test_telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         telemetry_storage._http_latencies._impression = [0] * 23
         telemetry_storage._http_latencies._impression_count = [0] * 23
         telemetry_storage._http_latencies._event = [0] * 23
         telemetry_storage._http_latencies._telemetry = [0] * 23
         telemetry_storage._http_latencies._token =  [0] * 23
 
         telemetry_storage.record_config({'operationMode': 'inmemory',
+                                         'storageType': None,
                                         'streamingEnabled': True,
                                         'impressionsQueueSize': 100,
                                         'eventsQueueSize': 200,
                                         'impressionsMode': 'DEBUG',
                                         'impressionListener': None,
                                         'featuresRefreshRate': 30,
                                         'segmentsRefreshRate': 30,
```

### Comparing `splitio_client-9.4.0/tests/sync/test_events_synchronizer.py` & `splitio_client-9.4.1/tests/sync/test_events_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/tests/helpers/mockserver.py` & `splitio_client-9.4.1/tests/helpers/mockserver.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/README.md` & `splitio_client-9.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Split Python SDK 
-[![Build Status](https://api.travis-ci.com/splitio/python-client.svg?branch=master)](https://api.travis-ci.com/splitio/python-client)
+# Split Python SDK
+![Build Status](https://github.com/splitio/python-client/actions/workflows/ci.yml/badge.svg?branch=master)
 
 ## Overview
 This SDK is designed to work with Split, the platform for controlled rollouts, which serves features to your users via a Split feature flag to manage your complete customer experience.
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/splitsoftware.svg?style=social&label=Follow&maxAge=1529000)](https://twitter.com/intent/follow?screen_name=splitsoftware)
 
 ## Compatibility
@@ -19,15 +19,15 @@
 from splitio import get_factory
 from splitio.exceptions import TimeoutException
 factory = get_factory('YOUR_SDK_TYPE_API_KEY', config=config)
 try:
     factory.block_until_ready(5) # wait up to 5 seconds
     split = factory.client()
     treatment = split.get_treatment('CUSTOMER_ID', 'SPLIT_NAME')
-    if treatment == "on": 
+    if treatment == "on":
         # insert code here to show on treatment
     elif treatment == "off":
         # insert code here to show off treatment
     else:
         # insert your control treatment code here
 except TimeoutException:
     # Now the user can choose whether to abort the whole execution, or just keep going
```

### Comparing `splitio_client-9.4.0/setup.py` & `splitio_client-9.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     'flake8',
     'pytest==7.0.1',
     'pytest-mock>=3.5.1',
     'coverage==6.2',
     'pytest-cov',
     'importlib-metadata==4.2',
     'tomli==1.2.3',
-    'iniconfig==1.1.1'
+    'iniconfig==1.1.1',
+    'attrs==22.1.0'
 ]
 
 INSTALL_REQUIRES = [
     'requests>=2.9.1',
     'pyyaml>=5.4',
     'docopt>=0.6.2',
     'enum34;python_version<"3.4"',
```

### Comparing `splitio_client-9.4.0/splitio/tasks/split_sync.py` & `splitio_client-9.4.1/splitio/tasks/split_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/util/workerpool.py` & `splitio_client-9.4.1/splitio/tasks/util/workerpool.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/util/asynctask.py` & `splitio_client-9.4.1/splitio/tasks/util/asynctask.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/telemetry_sync.py` & `splitio_client-9.4.1/splitio/tasks/telemetry_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/__init__.py` & `splitio_client-9.4.1/splitio/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/events_sync.py` & `splitio_client-9.4.1/splitio/tasks/events_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/segment_sync.py` & `splitio_client-9.4.1/splitio/tasks/segment_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/impressions_sync.py` & `splitio_client-9.4.1/splitio/tasks/impressions_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/tasks/unique_keys_sync.py` & `splitio_client-9.4.1/splitio/tasks/unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/util/time.py` & `splitio_client-9.4.1/splitio/util/time.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/util/backoff.py` & `splitio_client-9.4.1/splitio/util/backoff.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/util/threadutil.py` & `splitio_client-9.4.1/splitio/util/threadutil.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/partitions.py` & `splitio_client-9.4.1/splitio/models/grammar/partitions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/condition.py` & `splitio_client-9.4.1/splitio/models/grammar/condition.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/misc.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/misc.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/__init__.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/keys.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/numeric.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/numeric.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/string.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/string.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/sets.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/sets.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/grammar/matchers/base.py` & `splitio_client-9.4.1/splitio/models/grammar/matchers/base.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/token.py` & `splitio_client-9.4.1/splitio/models/token.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/segments.py` & `splitio_client-9.4.1/splitio/models/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/notification.py` & `splitio_client-9.4.1/splitio/models/notification.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/telemetry.py` & `splitio_client-9.4.1/splitio/models/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     437894, 656841, 985261, 1477892, 2216838,
     3325257, 4987885, 7481828
 )
 
 MAX_LATENCY = 7481828
 MAX_LATENCY_BUCKET_COUNT = 23
 MAX_STREAMING_EVENTS = 20
+MAX_TAGS = 10
 
 class CounterConstants(Enum):
     """Impressions and events counters constants"""
     IMPRESSIONS_QUEUED = 'impressionsQueued'
     IMPRESSIONS_DEDUPED = 'impressionsDeduped'
     IMPRESSIONS_DROPPED = 'impressionsDropped'
     EVENTS_QUEUED = 'eventsQueued'
@@ -118,20 +119,21 @@
     ABLY_ERROR = 60
     SYNC_MODE_UPDATE = 70
 
 class StorageType(Enum):
     """Storage types constants"""
     MEMORY = 'memory'
     REDIS = 'redis'
-    LOCALHOST = 'localhost'
+    PLUGGABLE = 'pluggable'
 
 class OperationMode(Enum):
     """Storage modes constants"""
-    MEMORY = 'inmemory'
-    REDIS = 'redis-consumer'
+    STANDALONE = 'standalone'
+    CONSUMER = 'consumer'
+    PARTIAL_CONSUMER = 'partial_consumer'
 
 def get_latency_bucket_index(micros):
     """
     Find the bucket index for a measured latency.
 
     :param micros: Measured latency in microseconds
     :type micros: int
@@ -720,15 +722,15 @@
             self._redundant_factory_count = 0
 
     def record_config(self, config, extra_config):
         """
         Record configurations.
 
         :param config: config dict: {
-            'operationMode': string, 'storageType': string, 'streamingEnabled': boolean,
+            'operationMode': int, 'storageType': string, 'streamingEnabled': boolean,
             'refreshRate' : {
                 'featuresRefreshRate': int,
                 'segmentsRefreshRate': int,
                 'impressionsRefreshRate': int,
                 'eventsPushRate': int,
                 'metricsRefreshRate': int
             }
@@ -739,15 +741,15 @@
             'impressionsQueueSize': int, 'eventsQueueSize': int, 'impressionsMode': string,
             'impressionsListener': boolean, 'activeFactoryCount': int, 'redundantFactoryCount': int
         }
         :type config: dict
         """
         with self._lock:
             self._operation_mode = self._get_operation_mode(config[ConfigParams.OPERATION_MODE.value])
-            self._storage_type = self._get_storage_type(config[ConfigParams.OPERATION_MODE.value])
+            self._storage_type = self._get_storage_type(config[ConfigParams.OPERATION_MODE.value], config[ConfigParams.STORAGE_TYPE.value])
             self._streaming_enabled = config[ConfigParams.STREAMING_ENABLED.value]
             self._refresh_rate = self._get_refresh_rates(config)
             self._url_override = self._get_url_overrides(extra_config)
             self._impressions_queue_size = config[ConfigParams.IMPRESSIONS_QUEUE_SIZE.value]
             self._events_queue_size = config[ConfigParams.EVENTS_QUEUE_SIZE.value]
             self._impressions_mode = self._get_impressions_mode(config[ConfigParams.IMPRESSIONS_MODE.value])
             self._impression_listener = True if config[ConfigParams.IMPRESSIONS_LISTENER.value] is not None else False
@@ -846,38 +848,38 @@
         :param op_mode: config operation mode
         :type config: str
 
         :return: operation mode
         :rtype: int
         """
         with self._lock:
-            if OperationMode.MEMORY.value in op_mode:
+            if op_mode == OperationMode.STANDALONE.value:
                 return 0
-            elif op_mode == OperationMode.REDIS.value:
+            elif op_mode == OperationMode.CONSUMER.value:
                 return 1
             else:
                 return 2
 
-    def _get_storage_type(self, op_mode):
+    def _get_storage_type(self, op_mode, st_type):
         """
         Get storage type from operation mode
 
         :param op_mode: config operation mode
         :type config: str
 
         :return: storage type
         :rtype: str
         """
         with self._lock:
-            if OperationMode.MEMORY.value in op_mode:
+            if op_mode == OperationMode.STANDALONE.value:
                 return StorageType.MEMORY.value
-            elif StorageType.REDIS.value in op_mode:
+            elif st_type == StorageType.REDIS.value:
                 return StorageType.REDIS.value
             else:
-                return StorageType.LOCALHOST.value
+                return StorageType.PLUGGABLE.value
 
     def _get_refresh_rates(self, config):
         """
         Get refresh rates within config dict
 
         :param config: config dict
         :type config: dict
```

### Comparing `splitio_client-9.4.0/splitio/models/impressions.py` & `splitio_client-9.4.1/splitio/models/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/datatypes.py` & `splitio_client-9.4.1/splitio/models/datatypes.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/models/splits.py` & `splitio_client-9.4.1/splitio/models/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/storage/__init__.py` & `splitio_client-9.4.1/splitio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/storage/adapters/util.py` & `splitio_client-9.4.1/splitio/storage/adapters/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/storage/adapters/cache_trait.py` & `splitio_client-9.4.1/splitio/storage/adapters/cache_trait.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/storage/adapters/redis.py` & `splitio_client-9.4.1/splitio/storage/adapters/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/storage/redis.py` & `splitio_client-9.4.1/splitio/storage/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Redis storage module."""
 import json
 import logging
 import threading
 
 from splitio.models.impressions import Impression
 from splitio.models import splits, segments
-from splitio.models.telemetry import MethodExceptions, MethodLatencies, TelemetryConfig
+from splitio.models.telemetry import MethodExceptions, MethodLatencies, TelemetryConfig, get_latency_bucket_index
 from splitio.storage import SplitStorage, SegmentStorage, ImpressionStorage, EventStorage, \
     ImpressionPipelinedStorage, TelemetryStorage
 from splitio.storage.adapters.redis import RedisAdapterException
 from splitio.storage.adapters.cache_trait import decorate as add_cache, DEFAULT_MAX_AGE
 
 
 _LOGGER = logging.getLogger(__name__)
@@ -645,36 +645,27 @@
             't': self.pop_config_tags()
         })
 
     def record_active_and_redundant_factories(self, active_factory_count, redundant_factory_count):
         """Record active and redundant factories."""
         self._tel_config.record_active_and_redundant_factories(active_factory_count, redundant_factory_count)
 
-    def add_latency_to_pipe(self, method, latency, pipe):
+    def add_latency_to_pipe(self, method, bucket, pipe):
         """
         record latency data
 
         :param method: method name
         :type method: string
         :param latency: latency
         :type latency: int64
         :param pipe: Redis pipe.
         :type pipe: redis.pipe
         """
-        self._method_latencies.add_latency(method, latency)
-        latencies = self._method_latencies.pop_all()['methodLatencies']
-        values = latencies[method.value]
-        total_keys = 0
-        bucket_number = 0
-        for bucket in values:
-            if bucket > 0:
-                pipe.hincrby(self._TELEMETRY_LATENCIES_KEY, self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
-                        method.value + '/' + str(bucket_number), bucket)
-                total_keys += 1
-            bucket_number = bucket_number + 0
+        pipe.hincrby(self._TELEMETRY_LATENCIES_KEY, self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
+            method.value + '/' + str(bucket), 1)
 
     def record_latency(self, method, latency):
         """
         Not implemented
         """
         raise NotImplementedError('Only redis pipe is used.')
```

### Comparing `splitio_client-9.4.0/splitio/storage/inmemmory.py` & `splitio_client-9.4.1/splitio/storage/inmemmory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/splitsse.py` & `splitio_client-9.4.1/splitio/push/splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/segmentworker.py` & `splitio_client-9.4.1/splitio/push/segmentworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/processor.py` & `splitio_client-9.4.1/splitio/push/processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/sse.py` & `splitio_client-9.4.1/splitio/push/sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/parser.py` & `splitio_client-9.4.1/splitio/push/parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/status_tracker.py` & `splitio_client-9.4.1/splitio/push/status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/splitworker.py` & `splitio_client-9.4.1/splitio/push/splitworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/push/manager.py` & `splitio_client-9.4.1/splitio/push/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/recorder/recorder.py` & `splitio_client-9.4.1/splitio/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/auth.py` & `splitio_client-9.4.1/splitio/api/auth.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/events.py` & `splitio_client-9.4.1/splitio/api/events.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/segments.py` & `splitio_client-9.4.1/splitio/api/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/client.py` & `splitio_client-9.4.1/splitio/api/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/telemetry.py` & `splitio_client-9.4.1/splitio/api/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/impressions.py` & `splitio_client-9.4.1/splitio/api/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/commons.py` & `splitio_client-9.4.1/splitio/api/commons.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/api/splits.py` & `splitio_client-9.4.1/splitio/api/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/impression.py` & `splitio_client-9.4.1/splitio/sync/impression.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/event.py` & `splitio_client-9.4.1/splitio/sync/event.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/util.py` & `splitio_client-9.4.1/splitio/sync/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/telemetry.py` & `splitio_client-9.4.1/splitio/sync/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/split.py` & `splitio_client-9.4.1/splitio/sync/split.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/synchronizer.py` & `splitio_client-9.4.1/splitio/sync/synchronizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -585,7 +585,73 @@
         """
         Stop tasks.
 
         :param blocking:flag to wait until tasks are stopped
         :type blocking: bool
         """
         self.stop_periodic_fetching()
+
+
+class PluggableSynchronizer(BaseSynchronizer):
+    """Plugable Synchronizer."""
+
+    def synchronize_segment(self, segment_name, till):
+        """
+        Synchronize particular segment.
+
+        :param segment_name: segment associated
+        :type segment_name: str
+        :param till: to fetch
+        :type till: int
+        """
+        pass
+
+    def synchronize_splits(self, till):
+        """
+        Synchronize all splits.
+
+        :param till: to fetch
+        :type till: int
+        """
+        pass
+
+    def sync_all(self):
+        """Synchronize all split data."""
+        pass
+
+    def start_periodic_fetching(self):
+        """Start fetchers for splits and segments."""
+        pass
+
+    def stop_periodic_fetching(self):
+        """Stop fetchers for splits and segments."""
+        pass
+
+    def start_periodic_data_recording(self):
+        """Start recorders."""
+        pass
+
+    def stop_periodic_data_recording(self, blocking):
+        """Stop recorders."""
+        pass
+
+    def kill_split(self, split_name, default_treatment, change_number):
+        """
+        Kill a split locally.
+
+        :param split_name: name of the split to perform kill
+        :type split_name: str
+        :param default_treatment: name of the default treatment to return
+        :type default_treatment: str
+        :param change_number: change_number
+        :type change_number: int
+        """
+        pass
+
+    def shutdown(self, blocking):
+        """
+        Stop tasks.
+
+        :param blocking:flag to wait until tasks are stopped
+        :type blocking: bool
+        """
+        pass
```

### Comparing `splitio_client-9.4.0/splitio/sync/segment.py` & `splitio_client-9.4.1/splitio/sync/segment.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/manager.py` & `splitio_client-9.4.1/splitio/sync/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/sync/unique_keys.py` & `splitio_client-9.4.1/splitio/sync/unique_keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/cache/lru.py` & `splitio_client-9.4.1/splitio/engine/cache/lru.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/telemetry.py` & `splitio_client-9.4.1/splitio/engine/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/splitters.py` & `splitio_client-9.4.1/splitio/engine/splitters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/hashfns/legacy.py` & `splitio_client-9.4.1/splitio/engine/hashfns/legacy.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/hashfns/__init__.py` & `splitio_client-9.4.1/splitio/engine/hashfns/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/hashfns/murmur3py.py` & `splitio_client-9.4.1/splitio/engine/hashfns/murmur3py.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/impressions/strategies.py` & `splitio_client-9.4.1/splitio/engine/impressions/strategies.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/impressions/__init__.py` & `splitio_client-9.4.1/splitio/engine/impressions/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from splitio.engine.impressions.impressions import ImpressionsMode
 from splitio.engine.impressions.manager import Counter as ImpressionsCounter
 from splitio.engine.impressions.strategies import StrategyNoneMode, StrategyDebugMode, StrategyOptimizedMode
-from splitio.engine.impressions.adapters import InMemorySenderAdapter, RedisSenderAdapter
+from splitio.engine.impressions.adapters import InMemorySenderAdapter, RedisSenderAdapter, PluggableSenderAdapter
 from splitio.tasks.unique_keys_sync import UniqueKeysSyncTask, ClearFilterSyncTask
 from splitio.sync.unique_keys import UniqueKeysSynchronizer, ClearFilterSynchronizer
 from splitio.sync.impression import ImpressionsCountSynchronizer
 from splitio.tasks.impressions_sync import ImpressionsCountSyncTask
 
-def set_classes(storage_mode, impressions_mode, api_adapter):
+def set_classes(storage_mode, impressions_mode, api_adapter, prefix=None):
     unique_keys_synchronizer = None
     clear_filter_sync = None
     unique_keys_task = None
     clear_filter_task = None
     impressions_count_sync = None
     impressions_count_task = None
     sender_adapter = None
-    if storage_mode == 'REDIS':
+    if storage_mode == 'PLUGGABLE':
+        sender_adapter = PluggableSenderAdapter(api_adapter, prefix)
+        api_telemetry_adapter = sender_adapter
+        api_impressions_adapter = sender_adapter
+    elif storage_mode == 'REDIS':
         sender_adapter = RedisSenderAdapter(api_adapter)
         api_telemetry_adapter = sender_adapter
         api_impressions_adapter = sender_adapter
     else:
         api_telemetry_adapter = api_adapter['telemetry']
         api_impressions_adapter = api_adapter['impressions']
         sender_adapter = InMemorySenderAdapter(api_telemetry_adapter)
```

### Comparing `splitio_client-9.4.0/splitio/engine/impressions/impressions.py` & `splitio_client-9.4.1/splitio/engine/impressions/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/impressions/unique_keys_tracker.py` & `splitio_client-9.4.1/splitio/engine/impressions/unique_keys_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/impressions/manager.py` & `splitio_client-9.4.1/splitio/engine/impressions/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/evaluator.py` & `splitio_client-9.4.1/splitio/engine/evaluator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/engine/filters.py` & `splitio_client-9.4.1/splitio/engine/filters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/client/config.py` & `splitio_client-9.4.1/splitio/client/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 _LOGGER = logging.getLogger(__name__)
 DEFAULT_DATA_SAMPLING = 1
 
 
 DEFAULT_CONFIG = {
-    'operationMode': 'in-memory',
+    'operationMode': 'standalone',
     'connectionTimeout': 1500,
     'streamingEnabled': True,
     'featuresRefreshRate': 30,
     'segmentsRefreshRate': 30,
     'metricsRefreshRate': 3600,
     'impressionsRefreshRate': 5 * 60,
     'impressionsBulkSize': 5000,
@@ -52,54 +52,68 @@
     'machineName': None,
     'machineIp': None,
     'splitFile': os.path.join(os.path.expanduser('~'), '.split'),
     'segmentDirectory': os.path.expanduser('~'),
     'localhostRefreshEnabled': False,
     'preforkedInitialization': False,
     'dataSampling': DEFAULT_DATA_SAMPLING,
+    'storageWrapper': None,
+    'storagePrefix': None,
+    'storageType': None
 }
 
 
 def _parse_operation_mode(apikey, config):
     """
-    Process incoming config to determine operation mode.
+    Process incoming config to determine operation mode and storage type
 
     :param config: user supplied config
     :type config: dict
 
-    :returns: operation mode
-    :rtype: str
+    :returns: operation mode and storage type
+    :rtype: Tuple (str, str)
     """
     if apikey == 'localhost':
-        return 'localhost-standalone'
+        _LOGGER.debug('Using Localhost operation mode')
+        return 'localhost', 'localhost'
 
     if 'redisHost' in config or 'redisSentinels' in config:
-        return 'redis-consumer'
+        _LOGGER.debug('Using Redis storage operation mode')
+        return 'consumer', 'redis'
 
-    return 'inmemory-standalone'
+    if  config.get('storageType') is not None:
+        if config.get('storageType').lower() == 'pluggable':
+            _LOGGER.debug('Using Pluggable storage operation mode')
+            return 'consumer', 'pluggable'
 
+        _LOGGER.warning('You passed an invalid storageType, acceptable value is '
+                            '`pluggable`. Defaulting storage to In-Memory mode.')
 
-def _sanitize_impressions_mode(mode, refresh_rate=None):
+    _LOGGER.debug('Using In-Memory operation mode')
+    return 'standalone', 'memory'
+
+
+def _sanitize_impressions_mode(storage_type, mode, refresh_rate=None):
     """
     Check supplied impressions mode and adjust refresh rate.
 
     :param config: default + supplied config
     :type config: dict
 
     :returns: config with sanitized impressions mode & refresh rate
     :rtype: config
     """
     if not isinstance(mode, ImpressionsMode):
         try:
             mode = ImpressionsMode(mode.upper())
         except (ValueError, AttributeError):
-            _LOGGER.warning('You passed an invalid impressionsMode, impressionsMode should be '
-                            'one of the following values: `debug`, `none` or `optimized`. '
-                            'Defaulting to `optimized` mode.')
             mode = ImpressionsMode.OPTIMIZED
+            _LOGGER.warning('You passed an invalid impressionsMode, impressionsMode should be ' \
+                            'one of the following values: `debug`, `none` or `optimized`. '
+                            ' Defaulting to `optimized` mode.')
 
     if mode == ImpressionsMode.DEBUG:
         refresh_rate = max(1, refresh_rate) if refresh_rate is not None else 60
     else:
         refresh_rate = max(60, refresh_rate) if refresh_rate is not None else 5 * 60
 
     return mode, refresh_rate
@@ -114,18 +128,18 @@
 
     :param config: DEFAULT + user supplied config
     :type config: dict
 
     :returns: sanitized config
     :rtype: dict
     """
-    config['operationMode'] = _parse_operation_mode(apikey, config)
+    config['operationMode'], config['storageType'] = _parse_operation_mode(apikey, config)
     processed = DEFAULT_CONFIG.copy()
     processed.update(config)
-    imp_mode, imp_rate = _sanitize_impressions_mode(config.get('impressionsMode'),
+    imp_mode, imp_rate = _sanitize_impressions_mode(config['storageType'], config.get('impressionsMode'),
                                                     config.get('impressionsRefreshRate'))
     processed['impressionsMode'] = imp_mode
     processed['impressionsRefreshRate'] = imp_rate
     if processed['metricsRefreshRate'] < 60:
         _LOGGER.warning('metricRefreshRate parameter minimum value is 60 seconds, defaulting to 3600 seconds.')
         processed['metricsRefreshRate'] = 3600
```

### Comparing `splitio_client-9.4.0/splitio/client/util.py` & `splitio_client-9.4.1/splitio/client/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/client/key.py` & `splitio_client-9.4.1/splitio/client/key.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/client/client.py` & `splitio_client-9.4.1/splitio/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,14 +400,14 @@
             properties=properties,
         )
 
         try:
             return_flag = self._recorder.record_track_stats([EventWrapper(
                 event=event,
                 size=size,
-            )], get_current_epoch_time_ms() - start)
+            )], get_latency_bucket_index(get_current_epoch_time_ms() - start))
             return return_flag
         except Exception:  # pylint: disable=broad-except
             self._telemetry_evaluation_producer.record_exception(MethodExceptionsAndLatencies.TRACK)
             _LOGGER.error('Error processing track event')
             _LOGGER.debug('Error: ', exc_info=True)
             return False
```

### Comparing `splitio_client-9.4.0/splitio/client/factory.py` & `splitio_client-9.4.1/splitio/client/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 # Storage
 from splitio.storage.inmemmory import InMemorySplitStorage, InMemorySegmentStorage, \
     InMemoryImpressionStorage, InMemoryEventStorage, InMemoryTelemetryStorage, LocalhostTelemetryStorage
 from splitio.storage.adapters import redis
 from splitio.storage.redis import RedisSplitStorage, RedisSegmentStorage, RedisImpressionsStorage, \
     RedisEventsStorage, RedisTelemetryStorage
+from splitio.storage.pluggable import PluggableEventsStorage, PluggableImpressionsStorage, PluggableSegmentStorage, \
+    PluggableSplitStorage, PluggableTelemetryStorage
 
 # APIs
 from splitio.api.client import HttpClient
 from splitio.api.splits import SplitsAPI
 from splitio.api.segments import SegmentsAPI
 from splitio.api.impressions import ImpressionsAPI
 from splitio.api.events import EventsAPI
@@ -41,15 +43,15 @@
 from splitio.tasks.impressions_sync import ImpressionsSyncTask, ImpressionsCountSyncTask
 from splitio.tasks.events_sync import EventsSyncTask
 from splitio.tasks.unique_keys_sync import UniqueKeysSyncTask, ClearFilterSyncTask
 from splitio.tasks.telemetry_sync import TelemetrySyncTask
 
 # Synchronizer
 from splitio.sync.synchronizer import SplitTasks, SplitSynchronizers, Synchronizer, \
-    LocalhostSynchronizer, RedisSynchronizer
+    LocalhostSynchronizer, RedisSynchronizer, PluggableSynchronizer
 from splitio.sync.manager import Manager, RedisManager
 from splitio.sync.split import SplitSynchronizer, LocalSplitSynchronizer, LocalhostMode
 from splitio.sync.segment import SegmentSynchronizer, LocalSegmentSynchronizer
 from splitio.sync.impression import ImpressionSynchronizer, ImpressionsCountSynchronizer
 from splitio.sync.event import EventSynchronizer
 from splitio.sync.unique_keys import UniqueKeysSynchronizer, ClearFilterSynchronizer
 from splitio.sync.telemetry import TelemetrySynchronizer, InMemoryTelemetrySubmitter, LocalhostTelemetrySubmitter, RedisTelemetrySubmitter
@@ -508,14 +510,92 @@
     redundant_factory_count, active_factory_count = _get_active_and_redundant_count()
     storages['telemetry'].record_active_and_redundant_factories(active_factory_count, redundant_factory_count)
     telemetry_submitter.synchronize_config()
 
     return split_factory
 
 
+def _build_pluggable_factory(api_key, cfg):
+    """Build and return a split factory with pluggable storage."""
+    sdk_metadata = util.get_metadata(cfg)
+    if not input_validator.validate_pluggable_adapter(cfg):
+        raise Exception("Pluggable Adapter validation failed, exiting")
+
+    pluggable_adapter = cfg.get('storageWrapper')
+    storage_prefix = cfg.get('storagePrefix')
+    storages = {
+        'splits': PluggableSplitStorage(pluggable_adapter, storage_prefix),
+        'segments': PluggableSegmentStorage(pluggable_adapter, storage_prefix),
+        'impressions': PluggableImpressionsStorage(pluggable_adapter, sdk_metadata, storage_prefix),
+        'events': PluggableEventsStorage(pluggable_adapter, sdk_metadata, storage_prefix),
+        'telemetry': PluggableTelemetryStorage(pluggable_adapter, sdk_metadata, storage_prefix)
+    }
+    telemetry_producer = TelemetryStorageProducer(storages['telemetry'])
+    telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
+    telemetry_init_producer = telemetry_producer.get_telemetry_init_producer()
+    # Using same class as redis
+    telemetry_submitter = RedisTelemetrySubmitter(storages['telemetry'])
+
+    unique_keys_synchronizer, clear_filter_sync, unique_keys_task, \
+    clear_filter_task, impressions_count_sync, impressions_count_task, \
+    imp_strategy = set_classes('PLUGGABLE', cfg['impressionsMode'], pluggable_adapter, storage_prefix)
+
+    imp_manager = ImpressionsManager(
+        imp_strategy,
+        telemetry_runtime_producer,
+        _wrap_impression_listener(cfg['impressionListener'], sdk_metadata),
+        )
+
+    synchronizers = SplitSynchronizers(None, None, None, None,
+        impressions_count_sync,
+        None,
+        unique_keys_synchronizer,
+        clear_filter_sync
+    )
+
+    tasks = SplitTasks(None, None, None, None,
+        impressions_count_task,
+        None,
+        unique_keys_task,
+        clear_filter_task
+    )
+
+    # Using same class as redis for consumer mode only
+    synchronizer = RedisSynchronizer(synchronizers, tasks)
+    recorder = StandardRecorder(
+        imp_manager,
+        storages['events'],
+        storages['impressions'],
+        storages['telemetry']
+    )
+
+    # Using same class as redis for consumer mode only
+    manager = RedisManager(synchronizer)
+    initialization_thread = threading.Thread(target=manager.start, name="SDKInitializer", daemon=True)
+    initialization_thread.start()
+
+    telemetry_init_producer.record_config(cfg, {})
+
+    split_factory = SplitFactory(
+        api_key,
+        storages,
+        cfg['labelsEnabled'],
+        recorder,
+        manager,
+        sdk_ready_flag=None,
+        telemetry_producer=telemetry_producer,
+        telemetry_init_producer=telemetry_init_producer
+    )
+    redundant_factory_count, active_factory_count = _get_active_and_redundant_count()
+    storages['telemetry'].record_active_and_redundant_factories(active_factory_count, redundant_factory_count)
+    telemetry_submitter.synchronize_config()
+
+    return split_factory
+
+
 def _build_localhost_factory(cfg):
     """Build and return a localhost factory for testing/development purposes."""
     telemetry_storage = LocalhostTelemetryStorage()
     telemetry_producer = TelemetryStorageProducer(telemetry_storage)
     telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
     telemetry_evaluation_producer = telemetry_producer.get_telemetry_evaluation_producer()
 
@@ -602,18 +682,20 @@
             )
 
     _INSTANTIATED_FACTORIES.update([api_key])
     _INSTANTIATED_FACTORIES_LOCK.release()
 
     config = sanitize_config(api_key, kwargs.get('config', {}))
 
-    if config['operationMode'] == 'localhost-standalone':
+    if config['operationMode'] == 'localhost':
         split_factory =  _build_localhost_factory(config)
-    elif config['operationMode'] == 'redis-consumer':
+    elif config['storageType'] == 'redis':
         split_factory = _build_redis_factory(api_key, config)
+    elif config['storageType'] == 'pluggable':
+        split_factory = _build_pluggable_factory(api_key, config)
     else:
         split_factory = _build_in_memory_factory(
         api_key,
         config,
         kwargs.get('sdk_api_base_url'),
         kwargs.get('events_api_base_url'),
         kwargs.get('auth_api_base_url'),
```

### Comparing `splitio_client-9.4.0/splitio/client/localhost.py` & `splitio_client-9.4.1/splitio/client/localhost.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/client/input_validator.py` & `splitio_client-9.4.1/splitio/client/input_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Input validation module."""
 from numbers import Number
 import logging
 import re
 import math
+import inspect
 
 from splitio.api import APIException
 from splitio.api.commons import FetchOptions
 from splitio.client.key import Key
 from splitio.engine.evaluator import CONTROL
 
 
@@ -513,7 +514,55 @@
             )
             return False, None, size
 
     if len(valid_properties.keys()) > 300:
         _LOGGER.warning('Event has more than 300 properties. Some of them will be trimmed' +
                         ' when processed')
     return True, valid_properties if len(valid_properties) else None, size
+
+def validate_pluggable_adapter(config):
+    """
+    Check if pluggable adapter contains the expected method signature
+
+    :param config: config parameters
+    :type config: Dict
+
+    :return: True if no issue found otherwise False
+    :rtype: bool
+    """
+    if config.get('storageType') != 'pluggable':
+        return True
+
+    if config.get('storageWrapper') is None:
+        _LOGGER.error("Expecting pluggable storage `wrapper` in options, but no valid wrapper instance was provided.")
+        return False
+
+    if config.get('storagePrefix') is not None:
+        if not isinstance(config.get('storagePrefix'), str):
+            _LOGGER.error("Pluggable storage prefix should be string type only")
+            return False
+
+    pluggable_adapter = config.get('storageWrapper')
+    if not isinstance(pluggable_adapter, object):
+        _LOGGER.error("Pluggable storage instance is not inherted from object class")
+        return False
+
+    expected_methods = {'get': 1, 'get_items': 1, 'get_many': 1, 'set': 2, 'push_items': 2,
+                        'delete': 1, 'increment': 2, 'decrement': 2, 'get_keys_by_prefix': 1,
+                        'get_many': 1, 'add_items' : 2, 'remove_items': 2, 'item_contains': 2,
+                        'get_items_count': 1, 'expire': 2}
+    methods = inspect.getmembers(pluggable_adapter, predicate=inspect.ismethod)
+    for exp_method in expected_methods:
+        method_found = False
+        get_method_args = set()
+        for method in methods:
+            if exp_method == method[0]:
+                method_found = True
+                get_method_args = inspect.signature(method[1]).parameters
+                break
+        if not method_found:
+            _LOGGER.error("Pluggable adapter does not have required method: %s" % exp_method)
+            return False
+        if len(get_method_args) < expected_methods[exp_method]:
+            _LOGGER.error("Pluggable adapter method %s has less than required arguments count: %s : " % (exp_method, len(get_method_args)))
+            return False
+    return True
```

### Comparing `splitio_client-9.4.0/splitio/client/manager.py` & `splitio_client-9.4.1/splitio/client/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.0/splitio/client/listener.py` & `splitio_client-9.4.1/splitio/client/listener.py`

 * *Files identical despite different names*

