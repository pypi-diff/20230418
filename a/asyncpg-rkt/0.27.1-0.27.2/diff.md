# Comparing `tmp/asyncpg-rkt-0.27.1.tar.gz` & `tmp/asyncpg-rkt-0.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg-rkt-0.27.1.tar", last modified: Thu Apr 13 17:40:02 2023, max compression
+gzip compressed data, was "asyncpg-rkt-0.27.2.tar", last modified: Tue Apr 18 16:34:51 2023, max compression
```

## Comparing `asyncpg-rkt-0.27.1.tar` & `asyncpg-rkt-0.27.2.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/_testbase/
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/_testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/_testbase/fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/asyncpg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86027 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/connresource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.172517 asyncpg-rkt-0.27.1/asyncpg/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/exceptions/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/introspection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.176518 asyncpg-rkt-0.27.1/asyncpg/pgproto/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.180518 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bits.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bytea.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/context.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/datetime.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/float.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/geometry.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/hstore.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/int.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/json.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/jsonpath.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/misc.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/network.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/pg_snapshot.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/text.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/tid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/uuid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonunsafe.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/debug.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/frb.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.h
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/memalign.h
--rw-r--r--   0 runner    (1001) docker     (123)  2206477 2023-04-13 17:40:00.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.c
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.h
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/utf8_to_ucs4.h
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-13 17:39:52.000000 asyncpg-rkt-0.27.1/asyncpg/pgproto/uuid.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    39219 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/prepared_stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/array.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    33079 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/pgproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/range.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/record.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/textutils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/cpythonx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/encodings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/pgtypes.pxi
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  4537051 2023-04-13 17:40:02.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.c
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    34375 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg/protocol/record/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    27538 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.c
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.h
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/rkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/serverversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/asyncpg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-13 17:40:02.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:39:57.000000 asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.188518 asyncpg-rkt-0.27.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23944 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/performance.png
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.192519 asyncpg-rkt-0.27.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:40:02.196519 asyncpg-rkt-0.27.1/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.crl.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/ca.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.csr.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client.key.protected.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client_ca.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/client_ca.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/server.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/certs/server.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test__environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test__sourcecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_adversity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cache_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    67068 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_numpy_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    36764 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_rkt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 17:39:51.000000 asyncpg-rkt-0.27.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.161664 asyncpg-rkt-0.27.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-18 16:34:51.161664 asyncpg-rkt-0.27.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.129664 asyncpg-rkt-0.27.2/asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.129664 asyncpg-rkt-0.27.2/asyncpg/_testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/_testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/_testbase/fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 16:34:51.161664 asyncpg-rkt-0.27.2/asyncpg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/connect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86027 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/connresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.129664 asyncpg-rkt-0.27.2/asyncpg/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/introspection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.137664 asyncpg-rkt-0.27.2/asyncpg/pgproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/array_writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/array_writer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/buffer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.141664 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/bits.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/bytea.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/datetime.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/float.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/geometry.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/hstore.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/int.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/json.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/jsonpath.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/misc.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/network.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/pg_snapshot.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/text.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/tid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/uuid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/cpythonunsafe.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/cpythonx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/debug.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/frb.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/hton.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/hton.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/memalign.h
+-rw-r--r--   0 runner    (1001) docker     (123)  2206477 2023-04-18 16:34:48.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/pgproto.c
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/pgproto.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/pgproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/tohex.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/tohex.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/utf8_to_ucs4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pgproto/uuid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    39219 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/prepared_stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.149664 asyncpg-rkt-0.27.2/asyncpg/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.149664 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/array.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    33079 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/pgproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/range.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/record.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/textutils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/coreproto.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/coreproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/cpythonx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/encodings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/pgtypes.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/prepared_stmt.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/prepared_stmt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  4538181 2023-04-18 16:34:51.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34375 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.149664 asyncpg-rkt-0.27.2/asyncpg/protocol/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/record/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    27538 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/record/recordobj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/record/recordobj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/scram.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/scram.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/settings.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/protocol/settings.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/rkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/serverversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/asyncpg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.153664 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-18 16:34:45.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 16:34:51.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:34:45.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:34:45.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-18 16:34:45.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 16:34:45.000000 asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.153664 asyncpg-rkt-0.27.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.153664 asyncpg-rkt-0.27.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.153664 asyncpg-rkt-0.27.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23944 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/performance.png
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:34:51.161664 asyncpg-rkt-0.27.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.157664 asyncpg-rkt-0.27.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:34:51.161664 asyncpg-rkt-0.27.2/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/ca.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/ca.crl.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/ca.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client.csr.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client.key.protected.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client_ca.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/client_ca.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/server.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/certs/server.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test__environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test__sourcecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_adversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_cache_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67068 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_numpy_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36764 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_rkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 16:34:36.000000 asyncpg-rkt-0.27.2/tests/test_utils.py
```

### Comparing `asyncpg-rkt-0.27.1/LICENSE` & `asyncpg-rkt-0.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/Makefile` & `asyncpg-rkt-0.27.2/Makefile`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/PKG-INFO` & `asyncpg-rkt-0.27.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-rkt
-Version: 0.27.1
+Version: 0.27.2
 Summary: An asyncio PostgreSQL driver that returns numpy arrays
 Home-page: https://github.com/MagicStack/asyncpg
 Author: MagicStack Inc
 Author-email: hello@magic.io
 License: Apache License, Version 2.0
 Platform: macOS
 Platform: POSIX
```

### Comparing `asyncpg-rkt-0.27.1/README.rst` & `asyncpg-rkt-0.27.2/README.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/__init__.py` & `asyncpg-rkt-0.27.2/asyncpg/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/_testbase/__init__.py` & `asyncpg-rkt-0.27.2/asyncpg/_testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/_testbase/fuzzer.py` & `asyncpg-rkt-0.27.2/asyncpg/_testbase/fuzzer.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/_version.py` & `asyncpg-rkt-0.27.2/asyncpg/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # The commit message MUST contain a properly formatted release
 # log, and the commit must be signed.
 #
 # The release automation will: build and test the packages for the
 # supported platforms, publish the packages on PyPI, merge the PR
 # to the target branch, create a Git tag pointing to the commit.
 
-__version__ = '0.27.1'
+__version__ = '0.27.2'
```

### Comparing `asyncpg-rkt-0.27.1/asyncpg/cluster.py` & `asyncpg-rkt-0.27.2/asyncpg/cluster.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/compat.py` & `asyncpg-rkt-0.27.2/asyncpg/compat.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/connect_utils.py` & `asyncpg-rkt-0.27.2/asyncpg/connect_utils.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/connection.py` & `asyncpg-rkt-0.27.2/asyncpg/connection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/connresource.py` & `asyncpg-rkt-0.27.2/asyncpg/connresource.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/cursor.py` & `asyncpg-rkt-0.27.2/asyncpg/cursor.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/exceptions/__init__.py` & `asyncpg-rkt-0.27.2/asyncpg/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/exceptions/_base.py` & `asyncpg-rkt-0.27.2/asyncpg/exceptions/_base.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/introspection.py` & `asyncpg-rkt-0.27.2/asyncpg/introspection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/array_writer.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/array_writer.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/array_writer.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/buffer.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/buffer.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/buffer.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/__init__.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/__init__.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bits.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/bits.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/bytea.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/bytea.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/datetime.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/datetime.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/float.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/float.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/geometry.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/geometry.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/hstore.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/hstore.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/int.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/int.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/json.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/json.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/jsonpath.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/jsonpath.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/misc.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/misc.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/network.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/network.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/numeric.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/numeric.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/pg_snapshot.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/pg_snapshot.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/text.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/text.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/tid.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/tid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/codecs/uuid.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/codecs/uuid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonunsafe.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/cpythonunsafe.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/cpythonx.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/cpythonx.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/frb.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/frb.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.h` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/hton.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/hton.pxd` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/hton.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.c` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/pgproto.c`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/pgproto.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/pgproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/tohex.h` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/tohex.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/types.py` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/utf8_to_ucs4.h` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/utf8_to_ucs4.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pgproto/uuid.pyx` & `asyncpg-rkt-0.27.2/asyncpg/pgproto/uuid.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/pool.py` & `asyncpg-rkt-0.27.2/asyncpg/pool.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/prepared_stmt.py` & `asyncpg-rkt-0.27.2/asyncpg/prepared_stmt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/array.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/array.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/base.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/base.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/base.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/pgproto.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/pgproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/range.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/range.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/record.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/record.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/codecs/textutils.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/codecs/textutils.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/coreproto.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/coreproto.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/coreproto.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/cpythonx.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/cpythonx.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/encodings.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/encodings.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/pgtypes.pxi` & `asyncpg-rkt-0.27.2/asyncpg/protocol/pgtypes.pxi`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/prepared_stmt.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/prepared_stmt.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/prepared_stmt.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -406,15 +406,15 @@
             return
         end = query.find("🚀\n", pos)
         if end < 0:
             self.dtype = None
             return
         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
         assert isinstance(self.dtype, np_dtype)
-        self.query = query[end + 2:]
+        self.query = query[:pos - 3] + query[end + 2:]
 
 cdef _decode_parameters_desc(object desc):
     cdef:
         ReadBuffer reader
         int16_t nparams
         uint32_t p_oid
         list result = []
```

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.c` & `asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.c`

 * *Files 0% similar despite different names*

```diff
@@ -56928,15 +56928,15 @@
   }
 
   /* "asyncpg/protocol/prepared_stmt.pyx":411
  *             self.dtype = None
  *             return
  *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))             # <<<<<<<<<<<<<<
  *         assert isinstance(self.dtype, np_dtype)
- *         self.query = query[end + 2:]
+ *         self.query = query[:pos - 3] + query[end + 2:]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pickle); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_loads); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyBytes_Type)), __pyx_n_s_fromhex); if (unlikely(!__pyx_t_7)) __PYX_ERR(7, 411, __pyx_L1_error)
@@ -57005,15 +57005,15 @@
   __pyx_v_self->dtype = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "asyncpg/protocol/prepared_stmt.pyx":412
  *             return
  *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  *         assert isinstance(self.dtype, np_dtype)             # <<<<<<<<<<<<<<
- *         self.query = query[end + 2:]
+ *         self.query = query[:pos - 3] + query[end + 2:]
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     __pyx_t_1 = __pyx_v_self->dtype;
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_5numpy_dtype); 
@@ -57024,39 +57024,59 @@
     }
   }
   #endif
 
   /* "asyncpg/protocol/prepared_stmt.pyx":413
  *         self.dtype = pickle.loads(bytes.fromhex(query[pos:end]))
  *         assert isinstance(self.dtype, np_dtype)
- *         self.query = query[end + 2:]             # <<<<<<<<<<<<<<
+ *         self.query = query[:pos - 3] + query[end + 2:]             # <<<<<<<<<<<<<<
  * 
  * cdef _decode_parameters_desc(object desc):
  */
   if (unlikely(__pyx_v_query == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(7, 413, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_end, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_pos, __pyx_int_3, 3, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_t_1 == Py_None);
   if (__pyx_t_3) {
-    __pyx_t_4 = 0;
+    __pyx_t_4 = PY_SSIZE_T_MAX;
   } else {
     __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 413, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_2;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_query, __pyx_t_4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_query, 0, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_1);
+  if (unlikely(__pyx_v_query == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(7, 413, __pyx_L1_error)
+  }
+  __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_v_end, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 413, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_3 = (__pyx_t_6 == Py_None);
+  if (__pyx_t_3) {
+    __pyx_t_4 = 0;
+  } else {
+    __pyx_t_2 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_2 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(7, 413, __pyx_L1_error)
+    __pyx_t_4 = __pyx_t_2;
+  }
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyUnicode_Substring(__pyx_v_query, __pyx_t_4, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_6)) __PYX_ERR(7, 413, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(7, 413, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->query);
   __Pyx_DECREF(__pyx_v_self->query);
-  __pyx_v_self->query = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_v_self->query = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
 
   /* "asyncpg/protocol/prepared_stmt.pyx":391
  *             raise BufferError(f'unexpected trailing {frb_get_len(&rbuf)} bytes in buffer')
  * 
  *     cdef _parse_dtype(self):             # <<<<<<<<<<<<<<
  *         cdef str query = self.query
  *         pos = 0
@@ -57482,15 +57502,15 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "asyncpg/protocol/prepared_stmt.pyx":415
- *         self.query = query[end + 2:]
+ *         self.query = query[:pos - 3] + query[end + 2:]
  * 
  * cdef _decode_parameters_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
 static PyObject *__pyx_f_7asyncpg_8protocol_8protocol__decode_parameters_desc(PyObject *__pyx_v_desc) {
@@ -57586,15 +57606,15 @@
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
   /* "asyncpg/protocol/prepared_stmt.pyx":415
- *         self.query = query[end + 2:]
+ *         self.query = query[:pos - 3] + query[end + 2:]
  * 
  * cdef _decode_parameters_desc(object desc):             # <<<<<<<<<<<<<<
  *     cdef:
  *         ReadBuffer reader
  */
 
   /* function exit code */
```

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/protocol.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/protocol.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.c` & `asyncpg-rkt-0.27.2/asyncpg/protocol/record/recordobj.c`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/record/recordobj.h` & `asyncpg-rkt-0.27.2/asyncpg/protocol/record/recordobj.h`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/scram.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/scram.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/scram.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pxd` & `asyncpg-rkt-0.27.2/asyncpg/protocol/settings.pxd`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/protocol/settings.pyx` & `asyncpg-rkt-0.27.2/asyncpg/protocol/settings.pyx`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/rkt.py` & `asyncpg-rkt-0.27.2/asyncpg/rkt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/serverversion.py` & `asyncpg-rkt-0.27.2/asyncpg/serverversion.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/transaction.py` & `asyncpg-rkt-0.27.2/asyncpg/transaction.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/types.py` & `asyncpg-rkt-0.27.2/asyncpg/types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg/utils.py` & `asyncpg-rkt-0.27.2/asyncpg/utils.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/PKG-INFO` & `asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-rkt
-Version: 0.27.1
+Version: 0.27.2
 Summary: An asyncio PostgreSQL driver that returns numpy arrays
 Home-page: https://github.com/MagicStack/asyncpg
 Author: MagicStack Inc
 Author-email: hello@magic.io
 License: Apache License, Version 2.0
 Platform: macOS
 Platform: POSIX
```

### Comparing `asyncpg-rkt-0.27.1/asyncpg_rkt.egg-info/SOURCES.txt` & `asyncpg-rkt-0.27.2/asyncpg_rkt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/Makefile` & `asyncpg-rkt-0.27.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/api/index.rst` & `asyncpg-rkt-0.27.2/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/conf.py` & `asyncpg-rkt-0.27.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/faq.rst` & `asyncpg-rkt-0.27.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/index.rst` & `asyncpg-rkt-0.27.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/installation.rst` & `asyncpg-rkt-0.27.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/docs/usage.rst` & `asyncpg-rkt-0.27.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/performance.png` & `asyncpg-rkt-0.27.2/performance.png`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/pyproject.toml` & `asyncpg-rkt-0.27.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/setup.py` & `asyncpg-rkt-0.27.2/setup.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/__init__.py` & `asyncpg-rkt-0.27.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/ca.cert.pem` & `asyncpg-rkt-0.27.2/tests/certs/ca.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/ca.crl.pem` & `asyncpg-rkt-0.27.2/tests/certs/ca.crl.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/ca.key.pem` & `asyncpg-rkt-0.27.2/tests/certs/ca.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client.cert.pem` & `asyncpg-rkt-0.27.2/tests/certs/client.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client.csr.pem` & `asyncpg-rkt-0.27.2/tests/certs/client.csr.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client.key.pem` & `asyncpg-rkt-0.27.2/tests/certs/client.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client.key.protected.pem` & `asyncpg-rkt-0.27.2/tests/certs/client.key.protected.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client_ca.cert.pem` & `asyncpg-rkt-0.27.2/tests/certs/client_ca.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/client_ca.key.pem` & `asyncpg-rkt-0.27.2/tests/certs/client_ca.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/gen.py` & `asyncpg-rkt-0.27.2/tests/certs/gen.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/server.cert.pem` & `asyncpg-rkt-0.27.2/tests/certs/server.cert.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/certs/server.key.pem` & `asyncpg-rkt-0.27.2/tests/certs/server.key.pem`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/histogram.py` & `asyncpg-rkt-0.27.2/tests/histogram.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test__environment.py` & `asyncpg-rkt-0.27.2/tests/test__environment.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test__sourcecode.py` & `asyncpg-rkt-0.27.2/tests/test__sourcecode.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_adversity.py` & `asyncpg-rkt-0.27.2/tests/test_adversity.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_cache_invalidation.py` & `asyncpg-rkt-0.27.2/tests/test_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_cancellation.py` & `asyncpg-rkt-0.27.2/tests/test_cancellation.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_codecs.py` & `asyncpg-rkt-0.27.2/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_connect.py` & `asyncpg-rkt-0.27.2/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_copy.py` & `asyncpg-rkt-0.27.2/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_cursor.py` & `asyncpg-rkt-0.27.2/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_exceptions.py` & `asyncpg-rkt-0.27.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_execute.py` & `asyncpg-rkt-0.27.2/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_introspection.py` & `asyncpg-rkt-0.27.2/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_listeners.py` & `asyncpg-rkt-0.27.2/tests/test_listeners.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_numpy.py` & `asyncpg-rkt-0.27.2/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_numpy_benchmark.py` & `asyncpg-rkt-0.27.2/tests/test_numpy_benchmark.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_pool.py` & `asyncpg-rkt-0.27.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_prepare.py` & `asyncpg-rkt-0.27.2/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_record.py` & `asyncpg-rkt-0.27.2/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_rkt.py` & `asyncpg-rkt-0.27.2/tests/test_rkt.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_test.py` & `asyncpg-rkt-0.27.2/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_timeout.py` & `asyncpg-rkt-0.27.2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_transaction.py` & `asyncpg-rkt-0.27.2/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_types.py` & `asyncpg-rkt-0.27.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `asyncpg-rkt-0.27.1/tests/test_utils.py` & `asyncpg-rkt-0.27.2/tests/test_utils.py`

 * *Files identical despite different names*

