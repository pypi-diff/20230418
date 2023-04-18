# Comparing `tmp/pins-0.8.0.tar.gz` & `tmp/pins-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pins-0.8.0.tar", last modified: Tue Mar 21 21:16:34 2023, max compression
+gzip compressed data, was "pins-0.8.1.tar", last modified: Tue Apr 18 19:03:33 2023, max compression
```

## Comparing `pins-0.8.0.tar` & `pins-0.8.1.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-21 21:16:23.000000 pins-0.8.0/.env.dev
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-21 21:16:23.000000 pins-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-21 21:16:23.000000 pins-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-21 21:16:23.000000 pins-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-21 21:16:23.000000 pins-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-21 21:16:23.000000 pins-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-21 21:16:23.000000 pins-0.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-21 21:16:34.316774 pins-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-21 21:16:23.000000 pins-0.8.0/README.Rmd
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-21 21:16:23.000000 pins-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/binder/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 21:16:23.000000 pins-0.8.0/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-03-21 21:16:23.000000 pins-0.8.0/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 21:16:23.000000 pins-0.8.0/binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 21:16:23.000000 pins-0.8.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-21 21:16:23.000000 pins-0.8.0/pins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-21 21:16:23.000000 pins-0.8.0/pins/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-03-21 21:16:23.000000 pins-0.8.0/pins/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-03-21 21:16:23.000000 pins-0.8.0/pins/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-21 21:16:23.000000 pins-0.8.0/pins/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-03-21 21:16:23.000000 pins-0.8.0/pins/constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/data/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-21 21:16:23.000000 pins-0.8.0/pins/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-21 21:16:23.000000 pins-0.8.0/pins/data/mtcars.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-03-21 21:16:23.000000 pins-0.8.0/pins/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-21 21:16:23.000000 pins-0.8.0/pins/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-03-21 21:16:23.000000 pins-0.8.0/pins/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/rsconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/rsconnect/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/rsconnect/html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins/rsconnect/html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-03-21 21:16:23.000000 pins-0.8.0/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/_snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/example-bundle/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/example-bundle/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/example-bundle/data_frame.csv
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/example-bundle/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/example-bundle/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/pin-board/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/_pins.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pin-board/x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/pin-board/x/20221215T180351Z-c3943/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pin-board/y/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.312775 pins-0.8.0/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pin-board/y/20221215T180400Z-b81d5/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-compat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-compat/df_arrow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-compat/df_csv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-compat/df_rds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-compat/df_unversioned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-old-types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.304774 pins-0.8.0/pins/tests/pins-old-types/a-table/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/pins/tests/pins-old-types/a-table/v/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-old-types/a-table/v/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-old-types/a-table/v/data.rds
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/pins-old-types/a-table/v/data.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_boards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_compat_old_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_rsconnect_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-21 21:16:23.000000 pins-0.8.0/pins/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-21 21:16:23.000000 pins-0.8.0/pins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-21 21:16:23.000000 pins-0.8.0/pins/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.308775 pins-0.8.0/pins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-21 21:16:34.000000 pins-0.8.0/pins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-21 21:16:34.000000 pins-0.8.0/pins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 21:16:34.000000 pins-0.8.0/pins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-21 21:16:34.000000 pins-0.8.0/pins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-21 21:16:34.000000 pins-0.8.0/pins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-21 21:16:23.000000 pins-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-03-21 21:16:23.000000 pins-0.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-21 21:16:23.000000 pins-0.8.0/requirements/minimum.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/script/ci-compat-check/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/dump_py_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/dump_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/validate_py_to_r.R
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-21 21:16:23.000000 pins-0.8.0/script/ci-compat-check/validate_r_to_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 21:16:34.316774 pins-0.8.0/script/setup-rsconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-21 21:16:23.000000 pins-0.8.0/script/setup-rsconnect/add-users.sh
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-21 21:16:23.000000 pins-0.8.0/script/setup-rsconnect/dump_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-21 21:16:23.000000 pins-0.8.0/script/setup-rsconnect/rstudio-connect.gcfg
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-21 21:16:23.000000 pins-0.8.0/script/setup-rsconnect/users.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-21 21:16:23.000000 pins-0.8.0/script/stage_example_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-21 21:16:23.000000 pins-0.8.0/script/stage_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-21 21:16:23.000000 pins-0.8.0/script/stage_r_pins_old_types.R
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-21 21:16:34.320775 pins-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.276189 pins-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-18 19:03:21.000000 pins-0.8.1/.env.dev
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 19:03:21.000000 pins-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 19:03:21.000000 pins-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-18 19:03:21.000000 pins-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 19:03:21.000000 pins-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 19:03:21.000000 pins-0.8.1/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 19:03:21.000000 pins-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-18 19:03:21.000000 pins-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-18 19:03:33.276189 pins-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-18 19:03:21.000000 pins-0.8.1/README.Rmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-18 19:03:21.000000 pins-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 19:03:21.000000 pins-0.8.1/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-18 19:03:21.000000 pins-0.8.1/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 19:03:21.000000 pins-0.8.1/binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 19:03:21.000000 pins-0.8.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.260188 pins-0.8.1/pins/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 19:03:21.000000 pins-0.8.1/pins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 19:03:21.000000 pins-0.8.1/pins/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-04-18 19:03:21.000000 pins-0.8.1/pins/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-18 19:03:21.000000 pins-0.8.1/pins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-18 19:03:21.000000 pins-0.8.1/pins/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-18 19:03:21.000000 pins-0.8.1/pins/constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.260188 pins-0.8.1/pins/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-18 19:03:21.000000 pins-0.8.1/pins/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-18 19:03:21.000000 pins-0.8.1/pins/data/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-18 19:03:21.000000 pins-0.8.1/pins/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 19:03:21.000000 pins-0.8.1/pins/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-18 19:03:21.000000 pins-0.8.1/pins/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.264189 pins-0.8.1/pins/rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.264189 pins-0.8.1/pins/rsconnect/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.264189 pins-0.8.1/pins/rsconnect/html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.264189 pins-0.8.1/pins/rsconnect/html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-04-18 19:03:21.000000 pins-0.8.1/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.252188 pins-0.8.1/pins/tests/_snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (123)    34769 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/example-bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/example-bundle/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/example-bundle/data_frame.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/example-bundle/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/example-bundle/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/pin-board/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/_pins.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.252188 pins-0.8.1/pins/tests/pin-board/x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.268189 pins-0.8.1/pins/tests/pin-board/x/20221215T180351Z-c3943/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.252188 pins-0.8.1/pins/tests/pin-board/y/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pin-board/y/20221215T180400Z-b81d5/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/pins/tests/pins-compat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.252188 pins-0.8.1/pins/tests/pins-compat/df_arrow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.252188 pins-0.8.1/pins/tests/pins-compat/df_csv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/pins/tests/pins-compat/df_rds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/pins/tests/pins-compat/df_unversioned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/pins/tests/pins-old-types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.256188 pins-0.8.1/pins/tests/pins-old-types/a-table/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.272189 pins-0.8.1/pins/tests/pins-old-types/a-table/v/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-old-types/a-table/v/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-old-types/a-table/v/data.rds
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/pins-old-types/a-table/v/data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_compat_old_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_rsconnect_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-18 19:03:21.000000 pins-0.8.1/pins/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-18 19:03:21.000000 pins-0.8.1/pins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-18 19:03:21.000000 pins-0.8.1/pins/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.260188 pins-0.8.1/pins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-18 19:03:33.000000 pins-0.8.1/pins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-18 19:03:33.000000 pins-0.8.1/pins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:03:33.000000 pins-0.8.1/pins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 19:03:33.000000 pins-0.8.1/pins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 19:03:33.000000 pins-0.8.1/pins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 19:03:21.000000 pins-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.276189 pins-0.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-18 19:03:21.000000 pins-0.8.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 19:03:21.000000 pins-0.8.1/requirements/minimum.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.276189 pins-0.8.1/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.276189 pins-0.8.1/script/ci-compat-check/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/dump_py_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/dump_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/validate_py_to_r.R
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 19:03:21.000000 pins-0.8.1/script/ci-compat-check/validate_r_to_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:03:33.276189 pins-0.8.1/script/setup-rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 19:03:21.000000 pins-0.8.1/script/setup-rsconnect/add-users.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 19:03:21.000000 pins-0.8.1/script/setup-rsconnect/dump_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 19:03:21.000000 pins-0.8.1/script/setup-rsconnect/rstudio-connect.gcfg
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 19:03:21.000000 pins-0.8.1/script/setup-rsconnect/users.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-18 19:03:21.000000 pins-0.8.1/script/stage_example_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 19:03:21.000000 pins-0.8.1/script/stage_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 19:03:21.000000 pins-0.8.1/script/stage_r_pins_old_types.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-18 19:03:33.276189 pins-0.8.1/setup.cfg
```

### Comparing `pins-0.8.0/.env.dev` & `pins-0.8.1/.env.dev`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/.gitignore` & `pins-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/CONTRIBUTING.md` & `pins-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/LICENSE` & `pins-0.8.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RStudio
+Copyright (c) 2023 pins-python authors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pins-0.8.0/Makefile` & `pins-0.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/PKG-INFO` & `pins-0.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.0
+Version: 0.8.1
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/machow/pins-python
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: data,tidyverse
 Classifier: Programming Language :: Python :: 3.7
@@ -18,16 +18,14 @@
 Provides-Extra: gcs
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # pins-python
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/machow/pins-python/HEAD)
-
 The pins package publishes data, models, and other Python objects, making it
 easy to share them across projects and with your colleagues. You can pin
 objects to a variety of pin *boards*, including folders (to share on a
 networked drive or with services like DropBox), Posit Connect, Amazon
 S3, and Google Cloud Storage.
 Pins can be automatically versioned, making it straightforward to track changes,
 re-run analyses on historical data, and undo mistakes.
@@ -65,21 +63,21 @@
 
 ```python
 board.pin_write(mtcars.head(), "mtcars", type="csv")
 ```
 
     Writing pin:
     Name: 'mtcars'
-    Version: 20230321T151326Z-120a5
+    Version: 20230410T151442Z-120a5
 
 
 
 
 
-    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230321T151326Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 3, 21, 15, 13, 26, 362951), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
+    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230410T151442Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 4, 10, 15, 14, 42, 55001), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
 
 
 
 Above, we saved the data as a CSV, but depending on
 what you’re saving and who else you want to read it, you might use the
 `type` argument to instead save it as a `joblib`, `parquet`, or `json` file.
 
@@ -102,30 +100,30 @@
 
 
 
 A board on your computer is good place to start, but the real power of
 pins comes when you use a board that’s shared with multiple people. To
 get started, you can use `board_folder()` with a directory on a shared
 drive or in DropBox, or if you use [Posit
-Connect](https://www.rstudio.com/products/connect/) you can use
-`board_rsconnect()`:
+Connect](https://posit.co/products/enterprise/connect/) you can use
+`board_connect()`:
 
 ```python
 # Note that this uses one approach to connecting,
 # the environment variables CONNECT_SERVER and CONNECT_API_KEY
 
-board = pins.board_rsconnect()
+board = pins.board_connect()
 board.pin_write(tidy_sales_data, "hadley/sales-summary", type="csv")
 ```
 
 Then, someone else (or an automated report) can read and use your
 pin:
 
 ```python
-board = board_rsconnect()
+board = board_connect()
 board.pin_read("hadley/sales-summary")
 ```
 
 You can easily control who gets to access the data using the Posit
 Connect permissions pane.
 
 The pins package also includes boards that allow you to share data on
```

### Comparing `pins-0.8.0/README.Rmd` & `pins-0.8.1/README.Rmd`

 * *Files 4% similar despite different names*

```diff
@@ -8,188 +8,181 @@
 00000070: 6368 2064 6f6e 2774 2072 656e 6465 7220  ch don't render 
 00000080: 6f6e 2067 6974 6875 620a 696d 706f 7274  on github.import
 00000090: 2070 616e 6461 7320 6173 2070 640a 7064   pandas as pd.pd
 000000a0: 2e73 6574 5f6f 7074 696f 6e28 2264 6973  .set_option("dis
 000000b0: 706c 6179 2e6e 6f74 6562 6f6f 6b5f 7265  play.notebook_re
 000000c0: 7072 5f68 746d 6c22 2c20 4661 6c73 6529  pr_html", False)
 000000d0: 0a60 6060 0a0a 2320 7069 6e73 2d70 7974  .```..# pins-pyt
-000000e0: 686f 6e0a 0a5b 215b 4269 6e64 6572 5d28  hon..[![Binder](
-000000f0: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-00000100: 2e6f 7267 2f62 6164 6765 5f6c 6f67 6f2e  .org/badge_logo.
-00000110: 7376 6729 5d28 6874 7470 733a 2f2f 6d79  svg)](https://my
-00000120: 6269 6e64 6572 2e6f 7267 2f76 322f 6768  binder.org/v2/gh
-00000130: 2f6d 6163 686f 772f 7069 6e73 2d70 7974  /machow/pins-pyt
-00000140: 686f 6e2f 4845 4144 290a 0a54 6865 2070  hon/HEAD)..The p
-00000150: 696e 7320 7061 636b 6167 6520 7075 626c  ins package publ
-00000160: 6973 6865 7320 6461 7461 2c20 6d6f 6465  ishes data, mode
-00000170: 6c73 2c20 616e 6420 6f74 6865 7220 5079  ls, and other Py
-00000180: 7468 6f6e 206f 626a 6563 7473 2c20 6d61  thon objects, ma
-00000190: 6b69 6e67 2069 740a 6561 7379 2074 6f20  king it.easy to 
-000001a0: 7368 6172 6520 7468 656d 2061 6372 6f73  share them acros
-000001b0: 7320 7072 6f6a 6563 7473 2061 6e64 2077  s projects and w
-000001c0: 6974 6820 796f 7572 2063 6f6c 6c65 6167  ith your colleag
-000001d0: 7565 732e 2059 6f75 2063 616e 2070 696e  ues. You can pin
-000001e0: 0a6f 626a 6563 7473 2074 6f20 6120 7661  .objects to a va
-000001f0: 7269 6574 7920 6f66 2070 696e 202a 626f  riety of pin *bo
-00000200: 6172 6473 2a2c 2069 6e63 6c75 6469 6e67  ards*, including
-00000210: 2066 6f6c 6465 7273 2028 746f 2073 6861   folders (to sha
-00000220: 7265 206f 6e20 610a 6e65 7477 6f72 6b65  re on a.networke
-00000230: 6420 6472 6976 6520 6f72 2077 6974 6820  d drive or with 
-00000240: 7365 7276 6963 6573 206c 696b 6520 4472  services like Dr
-00000250: 6f70 426f 7829 2c20 506f 7369 7420 436f  opBox), Posit Co
-00000260: 6e6e 6563 742c 2041 6d61 7a6f 6e0a 5333  nnect, Amazon.S3
-00000270: 2c20 616e 6420 476f 6f67 6c65 2043 6c6f  , and Google Clo
-00000280: 7564 2053 746f 7261 6765 2e0a 5069 6e73  ud Storage..Pins
-00000290: 2063 616e 2062 6520 6175 746f 6d61 7469   can be automati
-000002a0: 6361 6c6c 7920 7665 7273 696f 6e65 642c  cally versioned,
-000002b0: 206d 616b 696e 6720 6974 2073 7472 6169   making it strai
-000002c0: 6768 7466 6f72 7761 7264 2074 6f20 7472  ghtforward to tr
-000002d0: 6163 6b20 6368 616e 6765 732c 0a72 652d  ack changes,.re-
-000002e0: 7275 6e20 616e 616c 7973 6573 206f 6e20  run analyses on 
-000002f0: 6869 7374 6f72 6963 616c 2064 6174 612c  historical data,
-00000300: 2061 6e64 2075 6e64 6f20 6d69 7374 616b   and undo mistak
-00000310: 6573 2e0a 0a53 6565 2074 6865 205b 646f  es...See the [do
-00000320: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00000330: 7073 3a2f 2f72 7374 7564 696f 2e67 6974  ps://rstudio.git
-00000340: 6875 622e 696f 2f70 696e 732d 7079 7468  hub.io/pins-pyth
-00000350: 6f6e 2920 666f 7220 6765 7474 696e 6720  on) for getting 
-00000360: 7374 6172 7465 642e 0a0a 2323 2049 6e73  started...## Ins
-00000370: 7461 6c6c 6174 696f 6e0a 0a60 6060 7368  tallation..```sh
-00000380: 656c 6c0a 7079 7468 6f6e 202d 6d20 7069  ell.python -m pi
-00000390: 7020 696e 7374 616c 6c20 7069 6e73 0a60  p install pins.`
-000003a0: 6060 0a0a 2323 2055 7361 6765 0a0a 5365  ``..## Usage..Se
-000003b0: 6520 7468 6520 5b64 6f63 756d 656e 7461  e the [documenta
-000003c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 7273  tion](https://rs
-000003d0: 7475 6469 6f2e 6769 7468 7562 2e69 6f2f  tudio.github.io/
-000003e0: 7069 6e73 2d70 7974 686f 6e29 2066 6f72  pins-python) for
-000003f0: 2067 6574 7469 6e67 2073 7461 7274 6564   getting started
-00000400: 2e0a 0a54 6f20 7573 6520 7468 6520 7069  ...To use the pi
-00000410: 6e73 2070 6163 6b61 6765 2c20 796f 7520  ns package, you 
-00000420: 6d75 7374 2066 6972 7374 2063 7265 6174  must first creat
-00000430: 6520 6120 7069 6e20 626f 6172 642e 2041  e a pin board. A
-00000440: 2067 6f6f 6420 706c 6163 650a 746f 2073   good place.to s
-00000450: 7461 7274 2069 7320 6062 6f61 7264 5f66  tart is `board_f
-00000460: 6f6c 6465 7228 2960 2c20 7768 6963 6820  older()`, which 
-00000470: 7374 6f72 6573 2070 696e 7320 696e 2061  stores pins in a
-00000480: 2064 6972 6563 746f 7279 2079 6f75 0a73   directory you.s
-00000490: 7065 6369 6679 2e20 4865 7265 2049 e280  pecify. Here I..
-000004a0: 996c 6c20 7573 6520 6120 7370 6563 6961  .ll use a specia
-000004b0: 6c20 7665 7273 696f 6e20 6f66 2060 626f  l version of `bo
-000004c0: 6172 645f 666f 6c64 6572 2829 6020 6361  ard_folder()` ca
-000004d0: 6c6c 6564 0a60 626f 6172 645f 7465 6d70  lled.`board_temp
-000004e0: 2829 6020 7768 6963 6820 6372 6561 7465  ()` which create
-000004f0: 7320 6120 7465 6d70 6f72 6172 7920 626f  s a temporary bo
-00000500: 6172 6420 7468 6174 e280 9973 2061 7574  ard that...s aut
-00000510: 6f6d 6174 6963 616c 6c79 0a64 656c 6574  omatically.delet
-00000520: 6564 2077 6865 6e20 796f 7572 2050 7974  ed when your Pyt
-00000530: 686f 6e20 7363 7269 7074 206f 7220 6e6f  hon script or no
-00000540: 7465 626f 6f6b 2073 6573 7369 6f6e 2065  tebook session e
-00000550: 6e64 732e 2054 6869 7320 6973 2067 7265  nds. This is gre
-00000560: 6174 2066 6f72 2065 7861 6d70 6c65 732c  at for examples,
-00000570: 2062 7574 0a6f 6276 696f 7573 6c79 2079   but.obviously y
-00000580: 6f75 2073 686f 756c 646e 2774 2075 7365  ou shouldn't use
-00000590: 2069 7420 666f 7220 7265 616c 2077 6f72   it for real wor
-000005a0: 6b21 0a0a 6060 607b 7079 7468 6f6e 7d0a  k!..```{python}.
-000005b0: 696d 706f 7274 2070 696e 730a 6672 6f6d  import pins.from
-000005c0: 2070 696e 732e 6461 7461 2069 6d70 6f72   pins.data impor
-000005d0: 7420 6d74 6361 7273 0a0a 626f 6172 6420  t mtcars..board 
-000005e0: 3d20 7069 6e73 2e62 6f61 7264 5f74 656d  = pins.board_tem
-000005f0: 7028 290a 6060 600a 0a59 6f75 2063 616e  p().```..You can
-00000600: 2022 7069 6e22 2028 7361 7665 2920 6461   "pin" (save) da
-00000610: 7461 2074 6f20 6120 626f 6172 6420 7769  ta to a board wi
-00000620: 7468 2074 6865 2060 2e70 696e 5f77 7269  th the `.pin_wri
-00000630: 7465 2829 6020 6d65 7468 6f64 2e20 4974  te()` method. It
-00000640: 2072 6571 7569 7265 7320 7468 7265 650a   requires three.
-00000650: 6172 6775 6d65 6e74 733a 2061 6e20 6f62  arguments: an ob
-00000660: 6a65 6374 2c20 6120 6e61 6d65 2c20 616e  ject, a name, an
-00000670: 6420 6120 7069 6e20 7479 7065 3a0a 0a60  d a pin type:..`
-00000680: 6060 7b70 7974 686f 6e7d 0a62 6f61 7264  ``{python}.board
-00000690: 2e70 696e 5f77 7269 7465 286d 7463 6172  .pin_write(mtcar
-000006a0: 732e 6865 6164 2829 2c20 226d 7463 6172  s.head(), "mtcar
-000006b0: 7322 2c20 7479 7065 3d22 6373 7622 290a  s", type="csv").
-000006c0: 6060 600a 0a41 626f 7665 2c20 7765 2073  ```..Above, we s
-000006d0: 6176 6564 2074 6865 2064 6174 6120 6173  aved the data as
-000006e0: 2061 2043 5356 2c20 6275 7420 6465 7065   a CSV, but depe
-000006f0: 6e64 696e 6720 6f6e 0a77 6861 7420 796f  nding on.what yo
-00000700: 75e2 8099 7265 2073 6176 696e 6720 616e  u...re saving an
-00000710: 6420 7768 6f20 656c 7365 2079 6f75 2077  d who else you w
-00000720: 616e 7420 746f 2072 6561 6420 6974 2c20  ant to read it, 
-00000730: 796f 7520 6d69 6768 7420 7573 6520 7468  you might use th
-00000740: 650a 6074 7970 6560 2061 7267 756d 656e  e.`type` argumen
-00000750: 7420 746f 2069 6e73 7465 6164 2073 6176  t to instead sav
-00000760: 6520 6974 2061 7320 6120 606a 6f62 6c69  e it as a `jobli
-00000770: 6260 2c20 6070 6172 7175 6574 602c 206f  b`, `parquet`, o
-00000780: 7220 606a 736f 6e60 2066 696c 652e 0a0a  r `json` file...
-00000790: 596f 7520 6361 6e20 6c61 7465 7220 7265  You can later re
-000007a0: 7472 6965 7665 2074 6865 2070 696e 6e65  trieve the pinne
-000007b0: 6420 6461 7461 2077 6974 6820 602e 7069  d data with `.pi
-000007c0: 6e5f 7265 6164 2829 603a 0a0a 6060 607b  n_read()`:..```{
-000007d0: 7079 7468 6f6e 7d0a 626f 6172 642e 7069  python}.board.pi
-000007e0: 6e5f 7265 6164 2822 6d74 6361 7273 2229  n_read("mtcars")
-000007f0: 0a60 6060 0a0a 4120 626f 6172 6420 6f6e  .```..A board on
-00000800: 2079 6f75 7220 636f 6d70 7574 6572 2069   your computer i
-00000810: 7320 676f 6f64 2070 6c61 6365 2074 6f20  s good place to 
-00000820: 7374 6172 742c 2062 7574 2074 6865 2072  start, but the r
-00000830: 6561 6c20 706f 7765 7220 6f66 0a70 696e  eal power of.pin
-00000840: 7320 636f 6d65 7320 7768 656e 2079 6f75  s comes when you
-00000850: 2075 7365 2061 2062 6f61 7264 2074 6861   use a board tha
-00000860: 74e2 8099 7320 7368 6172 6564 2077 6974  t...s shared wit
-00000870: 6820 6d75 6c74 6970 6c65 2070 656f 706c  h multiple peopl
-00000880: 652e 2054 6f0a 6765 7420 7374 6172 7465  e. To.get starte
-00000890: 642c 2079 6f75 2063 616e 2075 7365 2060  d, you can use `
-000008a0: 626f 6172 645f 666f 6c64 6572 2829 6020  board_folder()` 
-000008b0: 7769 7468 2061 2064 6972 6563 746f 7279  with a directory
-000008c0: 206f 6e20 6120 7368 6172 6564 0a64 7269   on a shared.dri
-000008d0: 7665 206f 7220 696e 2044 726f 7042 6f78  ve or in DropBox
-000008e0: 2c20 6f72 2069 6620 796f 7520 7573 6520  , or if you use 
-000008f0: 5b50 6f73 6974 0a43 6f6e 6e65 6374 5d28  [Posit.Connect](
-00000900: 6874 7470 733a 2f2f 7777 772e 7273 7475  https://www.rstu
-00000910: 6469 6f2e 636f 6d2f 7072 6f64 7563 7473  dio.com/products
-00000920: 2f63 6f6e 6e65 6374 2f29 2079 6f75 2063  /connect/) you c
-00000930: 616e 2075 7365 0a60 626f 6172 645f 7273  an use.`board_rs
-00000940: 636f 6e6e 6563 7428 2960 3a0a 0a60 6060  connect()`:..```
-00000950: 7079 7468 6f6e 0a23 204e 6f74 6520 7468  python.# Note th
-00000960: 6174 2074 6869 7320 7573 6573 206f 6e65  at this uses one
-00000970: 2061 7070 726f 6163 6820 746f 2063 6f6e   approach to con
-00000980: 6e65 6374 696e 672c 0a23 2074 6865 2065  necting,.# the e
-00000990: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000009a0: 626c 6573 2043 4f4e 4e45 4354 5f53 4552  bles CONNECT_SER
-000009b0: 5645 5220 616e 6420 434f 4e4e 4543 545f  VER and CONNECT_
-000009c0: 4150 495f 4b45 590a 0a62 6f61 7264 203d  API_KEY..board =
-000009d0: 2070 696e 732e 626f 6172 645f 7273 636f   pins.board_rsco
-000009e0: 6e6e 6563 7428 290a 626f 6172 642e 7069  nnect().board.pi
-000009f0: 6e5f 7772 6974 6528 7469 6479 5f73 616c  n_write(tidy_sal
-00000a00: 6573 5f64 6174 612c 2022 6861 646c 6579  es_data, "hadley
-00000a10: 2f73 616c 6573 2d73 756d 6d61 7279 222c  /sales-summary",
-00000a20: 2074 7970 653d 2263 7376 2229 0a60 6060   type="csv").```
-00000a30: 0a0a 5468 656e 2c20 736f 6d65 6f6e 6520  ..Then, someone 
-00000a40: 656c 7365 2028 6f72 2061 6e20 6175 746f  else (or an auto
-00000a50: 6d61 7465 6420 7265 706f 7274 2920 6361  mated report) ca
-00000a60: 6e20 7265 6164 2061 6e64 2075 7365 2079  n read and use y
-00000a70: 6f75 720a 7069 6e3a 0a0a 6060 6070 7974  our.pin:..```pyt
-00000a80: 686f 6e0a 626f 6172 6420 3d20 626f 6172  hon.board = boar
-00000a90: 645f 7273 636f 6e6e 6563 7428 290a 626f  d_rsconnect().bo
-00000aa0: 6172 642e 7069 6e5f 7265 6164 2822 6861  ard.pin_read("ha
-00000ab0: 646c 6579 2f73 616c 6573 2d73 756d 6d61  dley/sales-summa
-00000ac0: 7279 2229 0a60 6060 0a0a 596f 7520 6361  ry").```..You ca
-00000ad0: 6e20 6561 7369 6c79 2063 6f6e 7472 6f6c  n easily control
-00000ae0: 2077 686f 2067 6574 7320 746f 2061 6363   who gets to acc
-00000af0: 6573 7320 7468 6520 6461 7461 2075 7369  ess the data usi
-00000b00: 6e67 2074 6865 2050 6f73 6974 0a43 6f6e  ng the Posit.Con
-00000b10: 6e65 6374 2070 6572 6d69 7373 696f 6e73  nect permissions
-00000b20: 2070 616e 652e 0a0a 5468 6520 7069 6e73   pane...The pins
-00000b30: 2070 6163 6b61 6765 2061 6c73 6f20 696e   package also in
-00000b40: 636c 7564 6573 2062 6f61 7264 7320 7468  cludes boards th
-00000b50: 6174 2061 6c6c 6f77 2079 6f75 2074 6f20  at allow you to 
-00000b60: 7368 6172 6520 6461 7461 206f 6e0a 7365  share data on.se
-00000b70: 7276 6963 6573 206c 696b 6520 416d 617a  rvices like Amaz
-00000b80: 6f6e e280 9973 2053 3320 2860 626f 6172  on...s S3 (`boar
-00000b90: 645f 7333 2829 6029 2c20 476f 6f67 6c65  d_s3()`), Google
-00000ba0: 2043 6c6f 7564 2053 746f 7261 6765 2028   Cloud Storage (
-00000bb0: 6062 6f61 7264 5f67 6373 2829 6029 2c0a  `board_gcs()`),.
-00000bc0: 616e 6420 417a 7572 6520 626c 6f62 2073  and Azure blob s
-00000bd0: 746f 7261 6765 2028 6062 6f61 7264 5f61  torage (`board_a
-00000be0: 7a75 7265 2829 6029 2e0a 0a23 2320 4465  zure()`)...## De
-00000bf0: 7665 6c6f 706d 656e 740a 0a53 6565 205b  velopment..See [
-00000c00: 434f 4e54 5249 4255 5449 4e47 2e6d 645d  CONTRIBUTING.md]
-00000c10: 2843 4f4e 5452 4942 5554 494e 472e 6d64  (CONTRIBUTING.md
-00000c20: 290a                                     ).
+000000e0: 686f 6e0a 0a54 6865 2070 696e 7320 7061  hon..The pins pa
+000000f0: 636b 6167 6520 7075 626c 6973 6865 7320  ckage publishes 
+00000100: 6461 7461 2c20 6d6f 6465 6c73 2c20 616e  data, models, an
+00000110: 6420 6f74 6865 7220 5079 7468 6f6e 206f  d other Python o
+00000120: 626a 6563 7473 2c20 6d61 6b69 6e67 2069  bjects, making i
+00000130: 740a 6561 7379 2074 6f20 7368 6172 6520  t.easy to share 
+00000140: 7468 656d 2061 6372 6f73 7320 7072 6f6a  them across proj
+00000150: 6563 7473 2061 6e64 2077 6974 6820 796f  ects and with yo
+00000160: 7572 2063 6f6c 6c65 6167 7565 732e 2059  ur colleagues. Y
+00000170: 6f75 2063 616e 2070 696e 0a6f 626a 6563  ou can pin.objec
+00000180: 7473 2074 6f20 6120 7661 7269 6574 7920  ts to a variety 
+00000190: 6f66 2070 696e 202a 626f 6172 6473 2a2c  of pin *boards*,
+000001a0: 2069 6e63 6c75 6469 6e67 2066 6f6c 6465   including folde
+000001b0: 7273 2028 746f 2073 6861 7265 206f 6e20  rs (to share on 
+000001c0: 610a 6e65 7477 6f72 6b65 6420 6472 6976  a.networked driv
+000001d0: 6520 6f72 2077 6974 6820 7365 7276 6963  e or with servic
+000001e0: 6573 206c 696b 6520 4472 6f70 426f 7829  es like DropBox)
+000001f0: 2c20 506f 7369 7420 436f 6e6e 6563 742c  , Posit Connect,
+00000200: 2041 6d61 7a6f 6e0a 5333 2c20 616e 6420   Amazon.S3, and 
+00000210: 476f 6f67 6c65 2043 6c6f 7564 2053 746f  Google Cloud Sto
+00000220: 7261 6765 2e0a 5069 6e73 2063 616e 2062  rage..Pins can b
+00000230: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+00000240: 7665 7273 696f 6e65 642c 206d 616b 696e  versioned, makin
+00000250: 6720 6974 2073 7472 6169 6768 7466 6f72  g it straightfor
+00000260: 7761 7264 2074 6f20 7472 6163 6b20 6368  ward to track ch
+00000270: 616e 6765 732c 0a72 652d 7275 6e20 616e  anges,.re-run an
+00000280: 616c 7973 6573 206f 6e20 6869 7374 6f72  alyses on histor
+00000290: 6963 616c 2064 6174 612c 2061 6e64 2075  ical data, and u
+000002a0: 6e64 6f20 6d69 7374 616b 6573 2e0a 0a53  ndo mistakes...S
+000002b0: 6565 2074 6865 205b 646f 6375 6d65 6e74  ee the [document
+000002c0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f72  ation](https://r
+000002d0: 7374 7564 696f 2e67 6974 6875 622e 696f  studio.github.io
+000002e0: 2f70 696e 732d 7079 7468 6f6e 2920 666f  /pins-python) fo
+000002f0: 7220 6765 7474 696e 6720 7374 6172 7465  r getting starte
+00000300: 642e 0a0a 2323 2049 6e73 7461 6c6c 6174  d...## Installat
+00000310: 696f 6e0a 0a60 6060 7368 656c 6c0a 7079  ion..```shell.py
+00000320: 7468 6f6e 202d 6d20 7069 7020 696e 7374  thon -m pip inst
+00000330: 616c 6c20 7069 6e73 0a60 6060 0a0a 2323  all pins.```..##
+00000340: 2055 7361 6765 0a0a 5365 6520 7468 6520   Usage..See the 
+00000350: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+00000360: 6874 7470 733a 2f2f 7273 7475 6469 6f2e  https://rstudio.
+00000370: 6769 7468 7562 2e69 6f2f 7069 6e73 2d70  github.io/pins-p
+00000380: 7974 686f 6e29 2066 6f72 2067 6574 7469  ython) for getti
+00000390: 6e67 2073 7461 7274 6564 2e0a 0a54 6f20  ng started...To 
+000003a0: 7573 6520 7468 6520 7069 6e73 2070 6163  use the pins pac
+000003b0: 6b61 6765 2c20 796f 7520 6d75 7374 2066  kage, you must f
+000003c0: 6972 7374 2063 7265 6174 6520 6120 7069  irst create a pi
+000003d0: 6e20 626f 6172 642e 2041 2067 6f6f 6420  n board. A good 
+000003e0: 706c 6163 650a 746f 2073 7461 7274 2069  place.to start i
+000003f0: 7320 6062 6f61 7264 5f66 6f6c 6465 7228  s `board_folder(
+00000400: 2960 2c20 7768 6963 6820 7374 6f72 6573  )`, which stores
+00000410: 2070 696e 7320 696e 2061 2064 6972 6563   pins in a direc
+00000420: 746f 7279 2079 6f75 0a73 7065 6369 6679  tory you.specify
+00000430: 2e20 4865 7265 2049 e280 996c 6c20 7573  . Here I...ll us
+00000440: 6520 6120 7370 6563 6961 6c20 7665 7273  e a special vers
+00000450: 696f 6e20 6f66 2060 626f 6172 645f 666f  ion of `board_fo
+00000460: 6c64 6572 2829 6020 6361 6c6c 6564 0a60  lder()` called.`
+00000470: 626f 6172 645f 7465 6d70 2829 6020 7768  board_temp()` wh
+00000480: 6963 6820 6372 6561 7465 7320 6120 7465  ich creates a te
+00000490: 6d70 6f72 6172 7920 626f 6172 6420 7468  mporary board th
+000004a0: 6174 e280 9973 2061 7574 6f6d 6174 6963  at...s automatic
+000004b0: 616c 6c79 0a64 656c 6574 6564 2077 6865  ally.deleted whe
+000004c0: 6e20 796f 7572 2050 7974 686f 6e20 7363  n your Python sc
+000004d0: 7269 7074 206f 7220 6e6f 7465 626f 6f6b  ript or notebook
+000004e0: 2073 6573 7369 6f6e 2065 6e64 732e 2054   session ends. T
+000004f0: 6869 7320 6973 2067 7265 6174 2066 6f72  his is great for
+00000500: 2065 7861 6d70 6c65 732c 2062 7574 0a6f   examples, but.o
+00000510: 6276 696f 7573 6c79 2079 6f75 2073 686f  bviously you sho
+00000520: 756c 646e 2774 2075 7365 2069 7420 666f  uldn't use it fo
+00000530: 7220 7265 616c 2077 6f72 6b21 0a0a 6060  r real work!..``
+00000540: 607b 7079 7468 6f6e 7d0a 696d 706f 7274  `{python}.import
+00000550: 2070 696e 730a 6672 6f6d 2070 696e 732e   pins.from pins.
+00000560: 6461 7461 2069 6d70 6f72 7420 6d74 6361  data import mtca
+00000570: 7273 0a0a 626f 6172 6420 3d20 7069 6e73  rs..board = pins
+00000580: 2e62 6f61 7264 5f74 656d 7028 290a 6060  .board_temp().``
+00000590: 600a 0a59 6f75 2063 616e 2022 7069 6e22  `..You can "pin"
+000005a0: 2028 7361 7665 2920 6461 7461 2074 6f20   (save) data to 
+000005b0: 6120 626f 6172 6420 7769 7468 2074 6865  a board with the
+000005c0: 2060 2e70 696e 5f77 7269 7465 2829 6020   `.pin_write()` 
+000005d0: 6d65 7468 6f64 2e20 4974 2072 6571 7569  method. It requi
+000005e0: 7265 7320 7468 7265 650a 6172 6775 6d65  res three.argume
+000005f0: 6e74 733a 2061 6e20 6f62 6a65 6374 2c20  nts: an object, 
+00000600: 6120 6e61 6d65 2c20 616e 6420 6120 7069  a name, and a pi
+00000610: 6e20 7479 7065 3a0a 0a60 6060 7b70 7974  n type:..```{pyt
+00000620: 686f 6e7d 0a62 6f61 7264 2e70 696e 5f77  hon}.board.pin_w
+00000630: 7269 7465 286d 7463 6172 732e 6865 6164  rite(mtcars.head
+00000640: 2829 2c20 226d 7463 6172 7322 2c20 7479  (), "mtcars", ty
+00000650: 7065 3d22 6373 7622 290a 6060 600a 0a41  pe="csv").```..A
+00000660: 626f 7665 2c20 7765 2073 6176 6564 2074  bove, we saved t
+00000670: 6865 2064 6174 6120 6173 2061 2043 5356  he data as a CSV
+00000680: 2c20 6275 7420 6465 7065 6e64 696e 6720  , but depending 
+00000690: 6f6e 0a77 6861 7420 796f 75e2 8099 7265  on.what you...re
+000006a0: 2073 6176 696e 6720 616e 6420 7768 6f20   saving and who 
+000006b0: 656c 7365 2079 6f75 2077 616e 7420 746f  else you want to
+000006c0: 2072 6561 6420 6974 2c20 796f 7520 6d69   read it, you mi
+000006d0: 6768 7420 7573 6520 7468 650a 6074 7970  ght use the.`typ
+000006e0: 6560 2061 7267 756d 656e 7420 746f 2069  e` argument to i
+000006f0: 6e73 7465 6164 2073 6176 6520 6974 2061  nstead save it a
+00000700: 7320 6120 606a 6f62 6c69 6260 2c20 6070  s a `joblib`, `p
+00000710: 6172 7175 6574 602c 206f 7220 606a 736f  arquet`, or `jso
+00000720: 6e60 2066 696c 652e 0a0a 596f 7520 6361  n` file...You ca
+00000730: 6e20 6c61 7465 7220 7265 7472 6965 7665  n later retrieve
+00000740: 2074 6865 2070 696e 6e65 6420 6461 7461   the pinned data
+00000750: 2077 6974 6820 602e 7069 6e5f 7265 6164   with `.pin_read
+00000760: 2829 603a 0a0a 6060 607b 7079 7468 6f6e  ()`:..```{python
+00000770: 7d0a 626f 6172 642e 7069 6e5f 7265 6164  }.board.pin_read
+00000780: 2822 6d74 6361 7273 2229 0a60 6060 0a0a  ("mtcars").```..
+00000790: 4120 626f 6172 6420 6f6e 2079 6f75 7220  A board on your 
+000007a0: 636f 6d70 7574 6572 2069 7320 676f 6f64  computer is good
+000007b0: 2070 6c61 6365 2074 6f20 7374 6172 742c   place to start,
+000007c0: 2062 7574 2074 6865 2072 6561 6c20 706f   but the real po
+000007d0: 7765 7220 6f66 0a70 696e 7320 636f 6d65  wer of.pins come
+000007e0: 7320 7768 656e 2079 6f75 2075 7365 2061  s when you use a
+000007f0: 2062 6f61 7264 2074 6861 74e2 8099 7320   board that...s 
+00000800: 7368 6172 6564 2077 6974 6820 6d75 6c74  shared with mult
+00000810: 6970 6c65 2070 656f 706c 652e 2054 6f0a  iple people. To.
+00000820: 6765 7420 7374 6172 7465 642c 2079 6f75  get started, you
+00000830: 2063 616e 2075 7365 2060 626f 6172 645f   can use `board_
+00000840: 666f 6c64 6572 2829 6020 7769 7468 2061  folder()` with a
+00000850: 2064 6972 6563 746f 7279 206f 6e20 6120   directory on a 
+00000860: 7368 6172 6564 0a64 7269 7665 206f 7220  shared.drive or 
+00000870: 696e 2044 726f 7042 6f78 2c20 6f72 2069  in DropBox, or i
+00000880: 6620 796f 7520 7573 6520 5b50 6f73 6974  f you use [Posit
+00000890: 0a43 6f6e 6e65 6374 5d28 6874 7470 733a  .Connect](https:
+000008a0: 2f2f 706f 7369 742e 636f 2f70 726f 6475  //posit.co/produ
+000008b0: 6374 732f 656e 7465 7270 7269 7365 2f63  cts/enterprise/c
+000008c0: 6f6e 6e65 6374 2f29 2079 6f75 2063 616e  onnect/) you can
+000008d0: 2075 7365 0a60 626f 6172 645f 636f 6e6e   use.`board_conn
+000008e0: 6563 7428 2960 3a0a 0a60 6060 7079 7468  ect()`:..```pyth
+000008f0: 6f6e 0a23 204e 6f74 6520 7468 6174 2074  on.# Note that t
+00000900: 6869 7320 7573 6573 206f 6e65 2061 7070  his uses one app
+00000910: 726f 6163 6820 746f 2063 6f6e 6e65 6374  roach to connect
+00000920: 696e 672c 0a23 2074 6865 2065 6e76 6972  ing,.# the envir
+00000930: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00000940: 2043 4f4e 4e45 4354 5f53 4552 5645 5220   CONNECT_SERVER 
+00000950: 616e 6420 434f 4e4e 4543 545f 4150 495f  and CONNECT_API_
+00000960: 4b45 590a 0a62 6f61 7264 203d 2070 696e  KEY..board = pin
+00000970: 732e 626f 6172 645f 636f 6e6e 6563 7428  s.board_connect(
+00000980: 290a 626f 6172 642e 7069 6e5f 7772 6974  ).board.pin_writ
+00000990: 6528 7469 6479 5f73 616c 6573 5f64 6174  e(tidy_sales_dat
+000009a0: 612c 2022 6861 646c 6579 2f73 616c 6573  a, "hadley/sales
+000009b0: 2d73 756d 6d61 7279 222c 2074 7970 653d  -summary", type=
+000009c0: 2263 7376 2229 0a60 6060 0a0a 5468 656e  "csv").```..Then
+000009d0: 2c20 736f 6d65 6f6e 6520 656c 7365 2028  , someone else (
+000009e0: 6f72 2061 6e20 6175 746f 6d61 7465 6420  or an automated 
+000009f0: 7265 706f 7274 2920 6361 6e20 7265 6164  report) can read
+00000a00: 2061 6e64 2075 7365 2079 6f75 720a 7069   and use your.pi
+00000a10: 6e3a 0a0a 6060 6070 7974 686f 6e0a 626f  n:..```python.bo
+00000a20: 6172 6420 3d20 626f 6172 645f 636f 6e6e  ard = board_conn
+00000a30: 6563 7428 290a 626f 6172 642e 7069 6e5f  ect().board.pin_
+00000a40: 7265 6164 2822 6861 646c 6579 2f73 616c  read("hadley/sal
+00000a50: 6573 2d73 756d 6d61 7279 2229 0a60 6060  es-summary").```
+00000a60: 0a0a 596f 7520 6361 6e20 6561 7369 6c79  ..You can easily
+00000a70: 2063 6f6e 7472 6f6c 2077 686f 2067 6574   control who get
+00000a80: 7320 746f 2061 6363 6573 7320 7468 6520  s to access the 
+00000a90: 6461 7461 2075 7369 6e67 2074 6865 2050  data using the P
+00000aa0: 6f73 6974 0a43 6f6e 6e65 6374 2070 6572  osit.Connect per
+00000ab0: 6d69 7373 696f 6e73 2070 616e 652e 0a0a  missions pane...
+00000ac0: 5468 6520 7069 6e73 2070 6163 6b61 6765  The pins package
+00000ad0: 2061 6c73 6f20 696e 636c 7564 6573 2062   also includes b
+00000ae0: 6f61 7264 7320 7468 6174 2061 6c6c 6f77  oards that allow
+00000af0: 2079 6f75 2074 6f20 7368 6172 6520 6461   you to share da
+00000b00: 7461 206f 6e0a 7365 7276 6963 6573 206c  ta on.services l
+00000b10: 696b 6520 416d 617a 6f6e e280 9973 2053  ike Amazon...s S
+00000b20: 3320 2860 626f 6172 645f 7333 2829 6029  3 (`board_s3()`)
+00000b30: 2c20 476f 6f67 6c65 2043 6c6f 7564 2053  , Google Cloud S
+00000b40: 746f 7261 6765 2028 6062 6f61 7264 5f67  torage (`board_g
+00000b50: 6373 2829 6029 2c0a 616e 6420 417a 7572  cs()`),.and Azur
+00000b60: 6520 626c 6f62 2073 746f 7261 6765 2028  e blob storage (
+00000b70: 6062 6f61 7264 5f61 7a75 7265 2829 6029  `board_azure()`)
+00000b80: 2e0a 0a23 2320 4465 7665 6c6f 706d 656e  ...## Developmen
+00000b90: 740a 0a53 6565 205b 434f 4e54 5249 4255  t..See [CONTRIBU
+00000ba0: 5449 4e47 2e6d 645d 2843 4f4e 5452 4942  TING.md](CONTRIB
+00000bb0: 5554 494e 472e 6d64 290a                 UTING.md).
```

### Comparing `pins-0.8.0/README.md` & `pins-0.8.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # pins-python
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/machow/pins-python/HEAD)
-
 The pins package publishes data, models, and other Python objects, making it
 easy to share them across projects and with your colleagues. You can pin
 objects to a variety of pin *boards*, including folders (to share on a
 networked drive or with services like DropBox), Posit Connect, Amazon
 S3, and Google Cloud Storage.
 Pins can be automatically versioned, making it straightforward to track changes,
 re-run analyses on historical data, and undo mistakes.
@@ -43,21 +41,21 @@
 
 ```python
 board.pin_write(mtcars.head(), "mtcars", type="csv")
 ```
 
     Writing pin:
     Name: 'mtcars'
-    Version: 20230321T151326Z-120a5
+    Version: 20230410T151442Z-120a5
 
 
 
 
 
-    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230321T151326Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 3, 21, 15, 13, 26, 362951), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
+    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230410T151442Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 4, 10, 15, 14, 42, 55001), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
 
 
 
 Above, we saved the data as a CSV, but depending on
 what you’re saving and who else you want to read it, you might use the
 `type` argument to instead save it as a `joblib`, `parquet`, or `json` file.
 
@@ -80,30 +78,30 @@
 
 
 
 A board on your computer is good place to start, but the real power of
 pins comes when you use a board that’s shared with multiple people. To
 get started, you can use `board_folder()` with a directory on a shared
 drive or in DropBox, or if you use [Posit
-Connect](https://www.rstudio.com/products/connect/) you can use
-`board_rsconnect()`:
+Connect](https://posit.co/products/enterprise/connect/) you can use
+`board_connect()`:
 
 ```python
 # Note that this uses one approach to connecting,
 # the environment variables CONNECT_SERVER and CONNECT_API_KEY
 
-board = pins.board_rsconnect()
+board = pins.board_connect()
 board.pin_write(tidy_sales_data, "hadley/sales-summary", type="csv")
 ```
 
 Then, someone else (or an automated report) can read and use your
 pin:
 
 ```python
-board = board_rsconnect()
+board = board_connect()
 board.pin_read("hadley/sales-summary")
 ```
 
 You can easily control who gets to access the data using the Posit
 Connect permissions pane.
 
 The pins package also includes boards that allow you to share data on
```

### Comparing `pins-0.8.0/binder/requirements.txt` & `pins-0.8.1/binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/boards.py` & `pins-0.8.1/pins/boards.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/cache.py` & `pins-0.8.1/pins/cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/config.py` & `pins-0.8.1/pins/config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/constructors.py` & `pins-0.8.1/pins/constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/data/mtcars.csv` & `pins-0.8.1/pins/data/mtcars.csv`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/drivers.py` & `pins-0.8.1/pins/drivers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/meta.py` & `pins-0.8.1/pins/meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/api.py` & `pins-0.8.1/pins/rsconnect/api.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/fs.py` & `pins-0.8.1/pins/rsconnect/fs.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/html/highlight.js-9.15.9/highlight.js` & `pins-0.8.1/pins/rsconnect/html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.1/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/html/index.html` & `pins-0.8.1/pins/rsconnect/html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/html/pagedtable-1.1/pagedtable.css` & `pins-0.8.1/pins/rsconnect/html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/rsconnect/html/pagedtable-1.1/pagedtable.js` & `pins-0.8.1/pins/rsconnect/html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js` & `pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html` & `pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css` & `pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js` & `pins-0.8.1/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/conftest.py` & `pins-0.8.1/pins/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/helpers.py` & `pins-0.8.1/pins/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow` & `pins-0.8.1/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_boards.py` & `pins-0.8.1/pins/tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_cache.py` & `pins-0.8.1/pins/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_compat.py` & `pins-0.8.1/pins/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_config.py` & `pins-0.8.1/pins/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_constructors.py` & `pins-0.8.1/pins/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_drivers.py` & `pins-0.8.1/pins/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_meta.py` & `pins-0.8.1/pins/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_rsconnect_api.py` & `pins-0.8.1/pins/tests/test_rsconnect_api.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/tests/test_versions.py` & `pins-0.8.1/pins/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/utils.py` & `pins-0.8.1/pins/utils.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins/versions.py` & `pins-0.8.1/pins/versions.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/pins.egg-info/PKG-INFO` & `pins-0.8.1/pins.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.0
+Version: 0.8.1
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/machow/pins-python
 Author: Michael Chow
 Author-email: mc_al_github@fastmail.com
 License: MIT
 Keywords: data,tidyverse
 Classifier: Programming Language :: Python :: 3.7
@@ -18,16 +18,14 @@
 Provides-Extra: gcs
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
 # pins-python
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/machow/pins-python/HEAD)
-
 The pins package publishes data, models, and other Python objects, making it
 easy to share them across projects and with your colleagues. You can pin
 objects to a variety of pin *boards*, including folders (to share on a
 networked drive or with services like DropBox), Posit Connect, Amazon
 S3, and Google Cloud Storage.
 Pins can be automatically versioned, making it straightforward to track changes,
 re-run analyses on historical data, and undo mistakes.
@@ -65,21 +63,21 @@
 
 ```python
 board.pin_write(mtcars.head(), "mtcars", type="csv")
 ```
 
     Writing pin:
     Name: 'mtcars'
-    Version: 20230321T151326Z-120a5
+    Version: 20230410T151442Z-120a5
 
 
 
 
 
-    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230321T151326Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 3, 21, 15, 13, 26, 362951), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
+    Meta(title='mtcars: a pinned 5 x 11 DataFrame', description=None, created='20230410T151442Z', pin_hash='120a54f7e0818041', file='mtcars.csv', file_size=249, type='csv', api_version=1, version=Version(created=datetime.datetime(2023, 4, 10, 15, 14, 42, 55001), hash='120a54f7e0818041'), tags=None, name='mtcars', user={}, local={})
 
 
 
 Above, we saved the data as a CSV, but depending on
 what you’re saving and who else you want to read it, you might use the
 `type` argument to instead save it as a `joblib`, `parquet`, or `json` file.
 
@@ -102,30 +100,30 @@
 
 
 
 A board on your computer is good place to start, but the real power of
 pins comes when you use a board that’s shared with multiple people. To
 get started, you can use `board_folder()` with a directory on a shared
 drive or in DropBox, or if you use [Posit
-Connect](https://www.rstudio.com/products/connect/) you can use
-`board_rsconnect()`:
+Connect](https://posit.co/products/enterprise/connect/) you can use
+`board_connect()`:
 
 ```python
 # Note that this uses one approach to connecting,
 # the environment variables CONNECT_SERVER and CONNECT_API_KEY
 
-board = pins.board_rsconnect()
+board = pins.board_connect()
 board.pin_write(tidy_sales_data, "hadley/sales-summary", type="csv")
 ```
 
 Then, someone else (or an automated report) can read and use your
 pin:
 
 ```python
-board = board_rsconnect()
+board = board_connect()
 board.pin_read("hadley/sales-summary")
 ```
 
 You can easily control who gets to access the data using the Posit
 Connect permissions pane.
 
 The pins package also includes boards that allow you to share data on
```

### Comparing `pins-0.8.0/pins.egg-info/SOURCES.txt` & `pins-0.8.1/pins.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .env.dev
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
+MAINTAINERS.md
 MANIFEST.in
 Makefile
 README.Rmd
 README.md
 docker-compose.yml
 pyproject.toml
 setup.cfg
```

### Comparing `pins-0.8.0/requirements/dev.txt` & `pins-0.8.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/script/stage_example_bundle.py` & `pins-0.8.1/script/stage_example_bundle.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/script/stage_r_pins.R` & `pins-0.8.1/script/stage_r_pins.R`

 * *Files identical despite different names*

### Comparing `pins-0.8.0/setup.cfg` & `pins-0.8.1/setup.cfg`

 * *Files identical despite different names*

