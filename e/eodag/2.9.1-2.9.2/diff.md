# Comparing `tmp/eodag-2.9.1.tar.gz` & `tmp/eodag-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/eodag/eodag/dist/.tmp-ih_n9z1l/eodag-2.9.1.tar", last modified: Mon Feb 27 17:22:08 2023, max compression
+gzip compressed data, was "/home/runner/work/eodag/eodag/dist/.tmp-sn865xtb/eodag-2.9.2.tar", last modified: Fri Mar 31 13:59:31 2023, max compression
```

## Comparing `eodag-2.9.1.tar` & `eodag-2.9.2.tar`

### file list

```diff
@@ -1,231 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-27 17:21:18.000000 eodag-2.9.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-27 17:21:18.000000 eodag-2.9.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-27 17:21:18.000000 eodag-2.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/workflows/fetch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-02-27 17:21:18.000000 eodag-2.9.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-27 17:21:18.000000 eodag-2.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-27 17:21:18.000000 eodag-2.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27538 2023-02-27 17:21:18.000000 eodag-2.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-02-27 17:21:18.000000 eodag-2.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-02-27 17:21:18.000000 eodag-2.9.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-02-27 17:21:18.000000 eodag-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-27 17:21:18.000000 eodag-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-02-27 17:21:18.000000 eodag-2.9.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-02-27 17:22:08.000000 eodag-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-02-27 17:21:18.000000 eodag-2.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-27 17:21:18.000000 eodag-2.9.1/docker/run-stac-server.sh
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-27 17:21:18.000000 eodag-2.9.1/docker/stac-browser.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-27 17:21:18.000000 eodag-2.9.1/docker/stac-server.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-27 17:21:18.000000 eodag-2.9.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    34908 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/download_methods.png
--rw-r--r--   0 runner    (1001) docker     (123)   251705 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_advanced_calls_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36060 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_bycs.png
--rw-r--r--   0 runner    (1001) docker     (123)    51185 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_fetch_product_types.png
--rw-r--r--   0 runner    (1001) docker     (123)    41102 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   106300 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_main_calls_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)   197652 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)   144489 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_stac_client.png
--rw-r--r--   0 runner    (1001) docker     (123)   143909 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/eodag_stac_server.png
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/params_mapping_extra.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/params_mapping_offline_infos.json
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/params_mapping_opensearch.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/product_types.js
--rw-r--r--   0 runner    (1001) docker     (123)    59594 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/product_types_information.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/progress_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/progress_1_none.png
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/progress_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/progress_2_none.png
--rw-r--r--   0 runner    (1001) docker     (123)   193081 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/stac_browser_example.png
--rw-r--r--   0 runner    (1001) docker     (123)   173920 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/_static/stac_browser_example_600.png
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/add_provider.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/call_graphs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/eoproduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/searchresult.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/api_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/cli_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/contribute.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/getting_started_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/configure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/product_storage_status.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/product_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/providers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/register.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/getting_started_guide/side_projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/notebooks/api_user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)   614025 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/1_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/2_providers_products_available.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/3_configuration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3517127 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/4_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/5_serialize_deserialize.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/6_crunch.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   622491 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/7_download.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   146309 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/8_post_process.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/notebooks/api_user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (123)   386277 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/data/crunch_search_results.geojson
--rw-r--r--   0 runner    (1001) docker     (123)    50866 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/api_user_guide/data/download_search_results.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/intro_notebooks.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/notebooks/tutos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.cpg
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.prj
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qix
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qpj
--rw-r--r--   0 runner    (1001) docker     (123)  1622304 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shp
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shx
--rw-r--r--   0 runner    (1001) docker     (123)   729711 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/auxdata/sentinel2_tiling_grid_centroids.zip
--rw-r--r--   0 runner    (1001) docker     (123)  3396880 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_burnt_areas_snappy.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   102790 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_cds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   334188 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_cop_dem.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    92318 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_ecmwf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    66086 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_meteoblue.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   515530 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_search_location_tile.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1220197 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_ship_detection.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/notebooks/tutos/tuto_stac_client.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/docs/plugins_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins_reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins_reference/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins_reference/crunch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins_reference/download.rst
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/plugins_reference/search.rst
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/stac.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/stac_rest.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-27 17:21:18.000000 eodag-2.9.1/docs/tutos.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/api/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82403 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/api/product/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/product/_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/api/product/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/product/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/product/drivers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42031 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/product/metadata_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/api/search_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28155 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/crunch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/apis/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/apis/ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/apis/usgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/aws_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/openid_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/qsauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/authentication/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/filter_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/filter_latest_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/filter_latest_tpl_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/filter_overlap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/crunch/filter_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/download/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41378 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/download/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    27442 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/download/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/download/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/download/s3rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/plugins/search/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/build_search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/csw.py
--rw-r--r--   0 runner    (1001) docker     (123)    57955 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/qssearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/plugins/search/static_stac_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    20922 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/ext_product_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/locations_conf_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    82127 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/product_types.yml
--rw-r--r--   0 runner    (1001) docker     (123)   119414 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/providers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/resources/shp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.cpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   393747 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.dbf
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.prj
--rwxr-xr-x   0 runner    (1001) docker     (123)   181628 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.shp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1564 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.shx
--rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/stac.yml
--rw-r--r--   0 runner    (1001) docker     (123)    55420 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/stac_api.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/stac_provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/resources/user_conf_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15081 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/server.wsgi
--rw-r--r--   0 runner    (1001) docker     (123)    44867 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/rest/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/templates/README
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/rest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    41015 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/import_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-02-27 17:21:18.000000 eodag-2.9.1/eodag/utils/stac_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 17:22:08.000000 eodag-2.9.1/eodag.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-02-27 17:21:18.000000 eodag-2.9.1/get_pypi_latest_version.sh
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-27 17:21:18.000000 eodag-2.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-27 17:21:18.000000 eodag-2.9.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-27 17:21:18.000000 eodag-2.9.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 17:21:18.000000 eodag-2.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-27 17:21:18.000000 eodag-2.9.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 17:21:18.000000 eodag-2.9.1/requirements-tutorials.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-27 17:21:18.000000 eodag-2.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-02-27 17:22:08.000000 eodag-2.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-02-27 17:21:18.000000 eodag-2.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-02-27 17:21:18.000000 eodag-2.9.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 17:22:08.000000 eodag-2.9.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-02-27 17:21:18.000000 eodag-2.9.1/utils/params_mapping_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-02-27 17:21:18.000000 eodag-2.9.1/utils/product_types_information_to_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-31 13:58:26.000000 eodag-2.9.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-31 13:58:26.000000 eodag-2.9.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-31 13:58:26.000000 eodag-2.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/workflows/fetch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-31 13:58:26.000000 eodag-2.9.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-31 13:58:26.000000 eodag-2.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-31 13:58:26.000000 eodag-2.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-03-31 13:58:26.000000 eodag-2.9.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-31 13:58:26.000000 eodag-2.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-03-31 13:58:26.000000 eodag-2.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-31 13:58:26.000000 eodag-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-31 13:58:26.000000 eodag-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-31 13:58:26.000000 eodag-2.9.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-03-31 13:59:31.000000 eodag-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-03-31 13:58:26.000000 eodag-2.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-31 13:58:26.000000 eodag-2.9.2/docker/run-stac-server.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-31 13:58:26.000000 eodag-2.9.2/docker/stac-browser.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-31 13:58:26.000000 eodag-2.9.2/docker/stac-server.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-31 13:58:26.000000 eodag-2.9.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    34908 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/download_methods.png
+-rw-r--r--   0 runner    (1001) docker     (123)   251705 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_advanced_calls_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36060 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_bycs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51185 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_fetch_product_types.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41102 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106300 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_main_calls_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   197652 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   144489 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_stac_client.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143909 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/eodag_stac_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/params_mapping_extra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/params_mapping_offline_infos.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/params_mapping_opensearch.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/product_types.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60144 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/product_types_information.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/progress_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/progress_1_none.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/progress_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/progress_2_none.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193081 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/stac_browser_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   173920 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/_static/stac_browser_example_600.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/add_provider.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/call_graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/eoproduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/searchresult.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/api_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/cli_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/contribute.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/getting_started_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/product_storage_status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/product_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/providers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/register.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/getting_started_guide/side_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/notebooks/api_user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)   614025 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/1_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/2_providers_products_available.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/3_configuration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3517127 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/4_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/5_serialize_deserialize.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/6_crunch.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   622491 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/7_download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   146309 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/8_post_process.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/notebooks/api_user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   386277 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/data/crunch_search_results.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)    50866 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/api_user_guide/data/download_search_results.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/intro_notebooks.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/notebooks/tutos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.prj
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qix
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qpj
+-rw-r--r--   0 runner    (1001) docker     (123)  1622304 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shx
+-rw-r--r--   0 runner    (1001) docker     (123)   729711 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/auxdata/sentinel2_tiling_grid_centroids.zip
+-rw-r--r--   0 runner    (1001) docker     (123)  3396880 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_burnt_areas_snappy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   102790 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_cds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   334188 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_cop_dem.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    92318 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_ecmwf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    66086 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_meteoblue.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   515530 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_search_location_tile.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1220197 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_ship_detection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/notebooks/tutos/tuto_stac_client.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/docs/plugins_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins_reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins_reference/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins_reference/crunch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins_reference/download.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/plugins_reference/search.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/stac.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/stac_rest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-31 13:58:26.000000 eodag-2.9.2/docs/tutos.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84587 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/api/product/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/product/_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/api/product/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/product/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/product/drivers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40258 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/product/metadata_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/api/search_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28155 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/crunch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/apis/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/apis/ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/apis/usgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/aws_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/openid_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/qsauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/sas_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/authentication/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/filter_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/filter_latest_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/filter_latest_tpl_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/filter_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/crunch/filter_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41410 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/download/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27442 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/download/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/download/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/download/s3rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/plugins/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/build_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/csw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60425 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/qssearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/plugins/search/static_stac_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   325589 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/ext_product_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/locations_conf_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    82127 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/product_types.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   120053 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/providers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/resources/shp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.cpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   393747 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.dbf
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.prj
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181628 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.shp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1564 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.shx
+-rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/stac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    55420 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/stac_api.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/stac_provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/resources/user_conf_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15081 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/server.wsgi
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/rest/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/templates/README
+-rw-r--r--   0 runner    (1001) docker     (123)    24007 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/rest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    46635 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/import_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-03-31 13:58:26.000000 eodag-2.9.2/eodag/utils/stac_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 13:59:31.000000 eodag-2.9.2/eodag.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-03-31 13:58:26.000000 eodag-2.9.2/get_pypi_latest_version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-31 13:58:26.000000 eodag-2.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-31 13:58:26.000000 eodag-2.9.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-31 13:58:26.000000 eodag-2.9.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-31 13:58:26.000000 eodag-2.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-31 13:58:26.000000 eodag-2.9.2/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-31 13:58:26.000000 eodag-2.9.2/requirements-tutorials.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-31 13:58:26.000000 eodag-2.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-31 13:59:31.000000 eodag-2.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1396 2023-03-31 13:58:26.000000 eodag-2.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-31 13:58:26.000000 eodag-2.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 13:59:31.000000 eodag-2.9.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-03-31 13:58:26.000000 eodag-2.9.2/utils/params_mapping_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-03-31 13:58:26.000000 eodag-2.9.2/utils/product_types_information_to_csv.py
```

### Comparing `eodag-2.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `eodag-2.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `eodag-2.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/.github/pull_request_template.md` & `eodag-2.9.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/.github/workflows/deploy.yml` & `eodag-2.9.2/.github/workflows/deploy.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 jobs:
   build-n-publish:
     name: Build and publish to PyPI
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout source
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
       - name: Set up Python 3.7
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.7"
 
       - name: Check that the current version isn't already on PyPi
         run: |
           if [ "$(./get_pypi_latest_version.sh)" != "$(python setup.py --version)" ]
           then
```

### Comparing `eodag-2.9.1/.github/workflows/fetch.yml` & `eodag-2.9.2/.github/workflows/fetch.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 jobs:
   fetch-product-types:
     name: Fetch providers for new product types
     runs-on: ubuntu-latest
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.7"
     - name: Update pip
       run: python -m pip install --upgrade pip
     - name: Get pip cache dir
       id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
+      shell: bash
+      run: echo "DIR=$(pip cache dir)" >> $GITHUB_OUTPUT
     - name: Get current week number
       id: get-week
       shell: bash
-      run: echo "::set-output name=week::$(date +'%V')"
+      run: echo "WEEK=$(date +'%V')" >> $GITHUB_OUTPUT
     - name: Pip cache
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.week }}-${{ hashFiles('setup.py') }}
+        path: ${{ steps.pip-cache.outputs.DIR }}
+        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.WEEK }}-${{ hashFiles('setup.cfg') }}
     - name: Install eodag
       run: |
         python -m pip install .
     - name: Fetch and update external product types reference
       run: |
         export JSON_OUTPUT_FILE="eodag/resources/ext_product_types.json"
         export JSON_REF_FILE=$(python -c "import eodag; print(eodag.config.EXT_PRODUCT_TYPES_CONF_URI)")
```

### Comparing `eodag-2.9.1/.github/workflows/test.yml` & `eodag-2.9.2/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -11,86 +11,86 @@
 
 jobs:
   lint:
     name: Linting (pre-commit)
     runs-on: ubuntu-latest
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.7"
     - name: Run pre-commit action
-      uses: pre-commit/action@v2.0.0
+      uses: pre-commit/action@v3.0.0
 
   tests:
     name: Test it!
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         python-version: [3.7, "3.11"]
         os: [ubuntu-latest, windows-latest]
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python ${{ matrix.python-version }} on ${{ matrix.os }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Update pip
       run: python -m pip install --upgrade pip
     - name: Get pip cache dir
       id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
+      shell: bash
+      run: echo "DIR=$(pip cache dir)" >> $GITHUB_OUTPUT
     - name: Get current week number
       id: get-week
       shell: bash
-      run: echo "::set-output name=week::$(date +'%V')"
+      run: echo "WEEK=$(date +'%V')" >> $GITHUB_OUTPUT
     - name: Pip cache
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key: ${{ runner.os }}-pip-${{ matrix.python-version }}-${{ steps.get-week.outputs.week }}-${{ hashFiles('setup.py') }}
+        path: ${{ steps.pip-cache.outputs.DIR }}
+        key: ${{ runner.os }}-pip-${{ matrix.python-version }}-${{ steps.get-week.outputs.WEEK }}-${{ hashFiles('setup.cfg') }}
     - name: Install tox and tox-gh-actions
       run: python -m pip install tox tox-gh-actions
     - name: Test with tox
       run: tox
     - name: Upload Unit Test Results
       if: always()
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: unit-test-results-python${{ matrix.python-version }}
         path: |
           test-reports/junit-report.xml
           test-reports/coverage.xml
 
   publish-test-results:
     name: "Publish Unit Tests Results"
     needs: tests
     runs-on: ubuntu-latest
     if: always()
 
     steps:
     - name: Download Artifacts
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         path: artifacts
 
     - name: Publish Unit Test Results
-      uses: EnricoMi/publish-unit-test-result-action@v1
+      uses: EnricoMi/publish-unit-test-result-action@v2
       continue-on-error: true
       with:
         files: artifacts/**/*junit-report.xml
     - name: Publish Coverage Report
       uses: 5monkeys/cobertura-action@master
       if: ${{ github.event_name == 'pull_request' }}
       with:
@@ -101,38 +101,38 @@
         only_changed_files: true
 
   build-docs:
     name: Build the docs
     runs-on: ubuntu-latest
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.7"
     - name: Update pip
       run: python -m pip install --upgrade pip
     - name: Get pip cache dir
       id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
+      shell: bash
+      run: echo "DIR=$(pip cache dir)" >> $GITHUB_OUTPUT
     - name: Get current week number
       id: get-week
       shell: bash
-      run: echo "::set-output name=week::$(date +'%V')"
+      run: echo "WEEK=$(date +'%V')" >> $GITHUB_OUTPUT
     - name: Pip cache
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.week }}-${{ hashFiles('setup.py') }}
+        path: ${{ steps.pip-cache.outputs.DIR }}
+        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.WEEK }}-${{ hashFiles('setup.cfg') }}
     - name: Install pandoc
       run: |
         sudo apt update
         sudo apt install -y make pandoc
     - name: Install tox
       run: |
         python -m pip install tox
@@ -140,36 +140,36 @@
       run: python -m tox -e docs
 
   check-pypi:
     name: Long description check for PyPI
     runs-on: ubuntu-latest
     steps:
     - name: Checkout the repo
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Get history and tags for SCM versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.7"
     - name: Update pip
       run: python -m pip install --upgrade pip
     - name: Get pip cache dir
       id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
+      shell: bash
+      run: echo "DIR=$(pip cache dir)" >> $GITHUB_OUTPUT
     - name: Get current week number
       id: get-week
       shell: bash
-      run: echo "::set-output name=week::$(date +'%V')"
+      run: echo "WEEK=$(date +'%V')" >> $GITHUB_OUTPUT
     - name: Pip cache
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.week }}-${{ hashFiles('setup.py') }}
+        path: ${{ steps.pip-cache.outputs.DIR }}
+        key: ${{ runner.os }}-pip-${{ steps.get-week.outputs.WEEK }}-${{ hashFiles('setup.cfg') }}
     - name: Install tox and sphinx (to have rst2html.py utility available)
       run: |
         python -m pip install tox sphinx
     - name: Testing with tox
       run: python -m tox -e pypi
```

### Comparing `eodag-2.9.1/.gitignore` & `eodag-2.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/.pre-commit-config.yaml` & `eodag-2.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/CHANGES.rst` & `eodag-2.9.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Release history
 ---------------
 
+2.9.2 (2023-03-31)
+++++++++++++++++++
+
+* `planetary_computer`, `Microsoft Planetary Computer <https://planetarycomputer.microsoft.com/>`_  as new provider
+  (:pull:`659`)
+* Fetch product types optimization (:pull:`683`)
+* Fixes external product types update for unknown provider (:pull:`682`)
+* Default dates and refactor for `CdsApi` and `EcmwfApi` (:pull:`672`)(:pull:`678`)(:pull:`679`)
+* `peps` `storageStatus` update (:pull:`677`)
+* Customized and faster `deepcopy` (:pull:`664`)
+* Various minor fixes and improvements (:pull:`665`)(:pull:`666`)(:pull:`667`)(:pull:`668`)(:pull:`669`)(:pull:`670`)
+  (:pull:`675`)(:pull:`688`)(:pull:`690`)(:pull:`691`)
+
 2.9.1 (2023-02-27)
 ++++++++++++++++++
 
 * ``cop_dataspace``, `Copernicus Data Space <https://dataspace.copernicus.eu>`_  as new provider (:pull:`658`)
 * EODAG specific `User-Agent` appended to requests headers (:pull:`656`)
 * ``Sentinel-5P`` and other product types updates for ``creodias``, ``mundi`` and ``onda`` (:pull:`657`)
 * Handle missing geometries through new ``defaultGeometry`` :class:`~eodag.api.product._product.EOProduct` property
@@ -38,14 +51,16 @@
 * `SARA <https://copernicus.nci.org.au/sara.client>`_ (Sentinel Australasia Regional Access) as new provider
   (:pull:`578`, thanks `@catchSheep <https://github.com/catchSheep>`_)(:pull:`602`)
 * Removes unavailable ```sobloo``` provider (:pull:`607`)
 * Landsat collection-1 data no more available on `usgs` (:pull:`601`)
 * `Product types catalog\
   <https://eodag.readthedocs.io/en/latest/getting_started_guide/product_types.html#product-types-information-csv>`_
   more visible in documentation (:pull:`603`)
+* Metadata mapping `to_geo_interface()` renammed to `to_geojson()`
+  (`d7565a4 <https://github.com/CS-SI/eodag/pull/604/commits/d7565a4984d356aca20310a87c02692cb879427e>`_)
 * Added support for `python3.11` (:pull:`552`)
 * Improved http asset size discovery in :class:`~eodag.plugins.download.http.HTTPDownload` (:pull:`566`)
 * Various minor fixes and improvements (:pull:`572`)(:pull:`574`)(:pull:`576`)(:pull:`579`)(:pull:`580`)(:pull:`582`)
   (:pull:`586`)(:pull:`588`)(:pull:`589`)(:pull:`590`)(:pull:`592`)(:pull:`593`)(:pull:`595`)(:pull:`597`)(:pull:`598`)
   (:pull:`599`)(:pull:`609`)(:pull:`610`)
 
 2.7.0 (2022-11-29)
```

### Comparing `eodag-2.9.1/CODE_OF_CONDUCT.md` & `eodag-2.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/CONTRIBUTING.rst` & `eodag-2.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/LICENSE` & `eodag-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/NOTICE` & `eodag-2.9.2/NOTICE`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/PKG-INFO` & `eodag-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodag
-Version: 2.9.1
+Version: 2.9.2
 Summary: Earth Observation Data Access Gateway
 Home-page: https://github.com/CS-SI/eodag
 Author: CS GROUP - France (CSSI)
 Author-email: admin@geostorm.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/CS-SI/eodag/issues/
 Project-URL: Documentation, https://eodag.readthedocs.io
```

### Comparing `eodag-2.9.1/README.rst` & `eodag-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docker/stac-browser.dockerfile` & `eodag-2.9.2/docker/stac-browser.dockerfile`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docker/stac-server.dockerfile` & `eodag-2.9.2/docker/stac-server.dockerfile`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docker-compose.yml` & `eodag-2.9.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/Makefile` & `eodag-2.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/custom.css` & `eodag-2.9.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/download_methods.png` & `eodag-2.9.2/docs/_static/download_methods.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_advanced_calls_graph.svg` & `eodag-2.9.2/docs/_static/eodag_advanced_calls_graph.svg`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_bycs.png` & `eodag-2.9.2/docs/_static/eodag_bycs.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_fetch_product_types.png` & `eodag-2.9.2/docs/_static/eodag_fetch_product_types.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_logo.png` & `eodag-2.9.2/docs/_static/eodag_logo.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_main_calls_graph.svg` & `eodag-2.9.2/docs/_static/eodag_main_calls_graph.svg`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_overview.png` & `eodag-2.9.2/docs/_static/eodag_overview.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_stac_client.png` & `eodag-2.9.2/docs/_static/eodag_stac_client.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/eodag_stac_server.png` & `eodag-2.9.2/docs/_static/eodag_stac_server.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/favicon-32x32.png` & `eodag-2.9.2/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/params_mapping_extra.csv` & `eodag-2.9.2/docs/_static/params_mapping_extra.csv`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-parameter,astraea_eod,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,mundi,onda,peps,sara,theia,usgs_satapi_aws
-assets,metadata only,,,,,metadata only,metadata only,metadata only,,,,,,,metadata only
-awsProductId,,,,,,,,,,,,,,,metadata only
-collection,,,,:green:`queryable metadata`,:green:`queryable metadata`,,,,,,,,,,
-defaultGeometry,,,,,,,,,,metadata only,,,,,
-downloadLink,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
-geometry,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-id,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
-orderLink,,,,,,,,,,metadata only,metadata only,,,,
-polarizationChannels,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,metadata only,,,metadata only,:green:`queryable metadata`
-polarizationMode,,,,,,,metadata only,,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,
-productIdentifier,,,,metadata only,metadata only,,,,,,,,,,
-quicklook,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
-searchLink,,,,,,,,,,metadata only,,,,,
-specification,,,,,,,,,,metadata only,,,,,
-storageStatus,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
-thumbnail,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,,metadata only,metadata only,metadata only,metadata only
-uid,,,,metadata only,metadata only,,,,,metadata only,metadata only,metadata only,metadata only,metadata only,
+parameter,astraea_eod,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,mundi,onda,peps,planetary_computer,sara,theia,usgs_satapi_aws
+assets,metadata only,,,,,metadata only,metadata only,metadata only,,,,,metadata only,,,metadata only
+awsProductId,,,,,,,,,,,,,,,,metadata only
+collection,,,,:green:`queryable metadata`,:green:`queryable metadata`,,,,,,,,,,,
+defaultGeometry,,,,,,,,,,metadata only,,,,,,
+downloadLink,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
+geometry,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+id,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
+orderLink,,,,,,,,,,metadata only,metadata only,,,,,
+polarizationChannels,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,metadata only,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+polarizationMode,,,,,,,metadata only,,,metadata only,,:green:`queryable metadata`,,:green:`queryable metadata`,metadata only,
+productIdentifier,,,,metadata only,metadata only,,,,,,,,,,,
+quicklook,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
+searchLink,,,,,,,,,,metadata only,,,,,,
+specification,,,,,,,,,,metadata only,,,,,,
+storageStatus,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
+thumbnail,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only
+uid,,,,metadata only,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,metadata only,
```

### Comparing `eodag-2.9.1/docs/_static/params_mapping_offline_infos.json` & `eodag-2.9.2/docs/_static/params_mapping_offline_infos.json`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/params_mapping_opensearch.csv` & `eodag-2.9.2/docs/_static/params_mapping_opensearch.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-parameter,astraea_eod,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,mundi,onda,peps,sara,theia,usgs_satapi_aws
-:abbr:`abstract ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Abstract. (String))`,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,,metadata only,metadata only,,metadata only
-":abbr:`accessConstraint ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource (String ))`",,,,,,,,,,metadata only,,metadata only,metadata only,metadata only,
-acquisitionStation,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-acquisitionSubType,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-acquisitionType,,,,,,,,,,metadata only,,metadata only,metadata only,,
-antennaLookDirection,,,,,,,,,,metadata only,,,,metadata only,
-archivingCenter,,,,,,,,,,metadata only,,,,metadata only,
-availabilityTime,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-:abbr:`classification ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Name of the handling restrictions on the resource or metadata (String ))`,,,,,,,,,,metadata only,,,,,
-cloudCover,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-completionTimeFromAscendingNode,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-:abbr:`compositeType ([OpenSearch Parameters for Collection Search] Type of composite product expressed as time period that the composite product covers (e.g. P10D for a 10 day composite) (String))`,,,,,,,,,,metadata only,,,,,
-creationDate,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,metadata only,metadata only,metadata only,metadata only,:green:`queryable metadata`
-":abbr:`dissemination ([OpenSearch Parameters for Collection Search] A string identifying the dissemination method (e.g. EUMETCast, EUMETCast-Europe, DataCentre) (String))`",,,,,,,,,,metadata only,,,,,
-:abbr:`doi ([OpenSearch Parameters for Collection Search] Digital Object Identifier identifying the product (see http://www.doi.org) (String))`,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,,:green:`queryable metadata`
-dopplerFrequency,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-frame,,,,,,,,,,metadata only,,,,,
-":abbr:`hasSecurityConstraints ([OpenSearch Parameters for Collection Search] A string informing if the resource has any security constraints. Possible values: TRUE, FALSE (String))`",,,,,,,,,,metadata only,,,,,
-highestLocation,,,,,,,,,,metadata only,,,,,
-illuminationAzimuthAngle,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-illuminationElevationAngle,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,,metadata only,:green:`queryable metadata`
-illuminationZenithAngle,,,,,,,,,,metadata only,,,,metadata only,
-incidenceAngleVariation,,,,,,,,,,metadata only,,,,metadata only,
-":abbr:`instrument ([OpenSearch Parameters for Collection Search] A string identifying the instrument (e.g. MERIS, AATSR, ASAR, HRVIR. SAR). (String))`",metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-:abbr:`keyword ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Commonly used word(s) or formalised word(s) or phrase(s) used to describe the subject. (String))`,,,,,,,,,,metadata only,,metadata only,metadata only,metadata only,
-:abbr:`language ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Language of the intellectual content of the metadata record (String ))`,,,,,,,,,,metadata only,,,,,
-:abbr:`lineage ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] General explanation of the data producer’s knowledge about the lineage of a dataset. (String))`,,,,,,,,,,metadata only,:green:`queryable metadata`,,,,
-lowestLocation,,,,,,,,,,metadata only,,,,,
-maximumIncidenceAngle,,,,,,,,,,metadata only,,,,metadata only,
-minimumIncidenceAngle,,,,,,,,,,metadata only,,,,metadata only,
-modificationDate,metadata only,,,metadata only,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,metadata only,metadata only,metadata only,:green:`queryable metadata`
-orbitDirection,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`
-orbitNumber,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
-":abbr:`orbitType ([OpenSearch Parameters for Collection Search] A string identifying the platform orbit type (e.g. LEO, GEO) (String))`",,,,,,,,,,metadata only,,,,,
-:abbr:`organisationName ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A string identifying the name of the organization responsible for the resource (String))`,,,,:green:`queryable metadata`,:green:`queryable metadata`,,,,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,
-:abbr:`organisationRole ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] The function performed by the responsible party (String ))`,,,,,,,,,,metadata only,,,,,
-:abbr:`otherConstraint ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Other restrictions and legal prerequisites for accessing and using the resource or metadata. (String))`,,,,,,,,,,metadata only,,,,,
-parentIdentifier,,,,,,,,,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,
-:abbr:`platform ([OpenSearch Parameters for Collection Search] A string with the platform short name (e.g. Sentinel-1) (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,metadata only,metadata only,:green:`queryable metadata`,:green:`queryable metadata`
-:abbr:`platformSerialIdentifier ([OpenSearch Parameters for Collection Search] A string with the Platform serial identifier (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-processingCenter,,,,,,,,,,metadata only,,metadata only,metadata only,,
-processingDate,,,,,,,,,,metadata only,metadata only,,,metadata only,
-:abbr:`processingLevel ([OpenSearch Parameters for Collection Search] A string identifying the processing level applied to the entry (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-processingMode,,,,,,,,,,metadata only,,,,metadata only,
-processorName,,,,,,,,,,metadata only,,metadata only,metadata only,,
-productQualityDegradationTag,,,,,,,,,,metadata only,,,,,
-productQualityStatus,,,,,,,,,,metadata only,:green:`queryable metadata`,metadata only,metadata only,,
-":abbr:`productType ([OpenSearch Parameters for Collection Search] A string identifying the entry type (e.g. ER02_SAR_IM__0P, MER_RR__1P, SM_SLC__1S, GES_DISC_AIRH3STD_V005) (String ))`",:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
-productVersion,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,metadata only,metadata only,metadata only,:green:`queryable metadata`
-:abbr:`publicationDate ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] The date when the resource was issued (Date time))`,metadata only,,,metadata only,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,metadata only,metadata only,metadata only,:green:`queryable metadata`
-resolution,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
-sensorMode,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
-":abbr:`sensorType ([OpenSearch Parameters for Collection Search] A string identifying the sensor type. Suggested values are: OPTICAL, RADAR, ALTIMETRIC, ATMOSPHERIC, LIMB (String))`",,,,,,,,,,metadata only,:green:`queryable metadata`,,,,
-snowCover,,,,,,,,,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,
-":abbr:`spectralRange ([OpenSearch Parameters for Collection Search] A string identifying the sensor spectral range (e.g. INFRARED, NEAR-INFRARED, UV, VISIBLE) (String))`",,,,,,,,,,metadata only,,,,,
-startTimeFromAscendingNode,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,metadata only,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only
-swathIdentifier,,,,,,,,,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,,
-:abbr:`title ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A name given to the resource (String ))`,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
-:abbr:`topicCategory ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Main theme(s) of the dataset (String ))`,,,,,,,,,,metadata only,:green:`queryable metadata`,metadata only,metadata only,,
-track,,,,,,,,,,metadata only,,,,,
-:abbr:`useLimitation ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A string identifying informing if the resource has usage limitations (String))`,,,,,,,,,,metadata only,,,,,
-wavelengths,,,,,,,,,,metadata only,,,,,
+parameter,astraea_eod,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,mundi,onda,peps,planetary_computer,sara,theia,usgs_satapi_aws
+:abbr:`abstract ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Abstract. (String))`,metadata only,,,,,metadata only,metadata only,metadata only,,metadata only,,metadata only,metadata only,metadata only,,metadata only
+":abbr:`accessConstraint ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Applied to assure the protection of privacy or intellectual property, and any special restrictions or limitations on obtaining the resource (String ))`",,,,,,,,,,metadata only,,metadata only,,metadata only,metadata only,
+acquisitionStation,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+acquisitionSubType,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+acquisitionType,,,,,,,,,,metadata only,,metadata only,,metadata only,,
+antennaLookDirection,,,,,,,,,,metadata only,,,,,metadata only,
+archivingCenter,,,,,,,,,,metadata only,,,,,metadata only,
+availabilityTime,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+:abbr:`classification ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Name of the handling restrictions on the resource or metadata (String ))`,,,,,,,,,,metadata only,,,,,,
+cloudCover,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+completionTimeFromAscendingNode,:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+:abbr:`compositeType ([OpenSearch Parameters for Collection Search] Type of composite product expressed as time period that the composite product covers (e.g. P10D for a 10 day composite) (String))`,,,,,,,,,,metadata only,,,,,,
+creationDate,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,metadata only,metadata only,:green:`queryable metadata`,metadata only,metadata only,:green:`queryable metadata`
+":abbr:`dissemination ([OpenSearch Parameters for Collection Search] A string identifying the dissemination method (e.g. EUMETCast, EUMETCast-Europe, DataCentre) (String))`",,,,,,,,,,metadata only,,,,,,
+:abbr:`doi ([OpenSearch Parameters for Collection Search] Digital Object Identifier identifying the product (see http://www.doi.org) (String))`,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,,:green:`queryable metadata`
+dopplerFrequency,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+frame,,,,,,,,,,metadata only,,,,,,
+":abbr:`hasSecurityConstraints ([OpenSearch Parameters for Collection Search] A string informing if the resource has any security constraints. Possible values: TRUE, FALSE (String))`",,,,,,,,,,metadata only,,,,,,
+highestLocation,,,,,,,,,,metadata only,,,,,,
+illuminationAzimuthAngle,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+illuminationElevationAngle,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`
+illuminationZenithAngle,,,,,,,,,,metadata only,,,,,metadata only,
+incidenceAngleVariation,,,,,,,,,,metadata only,,,,,metadata only,
+":abbr:`instrument ([OpenSearch Parameters for Collection Search] A string identifying the instrument (e.g. MERIS, AATSR, ASAR, HRVIR. SAR). (String))`",metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+:abbr:`keyword ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Commonly used word(s) or formalised word(s) or phrase(s) used to describe the subject. (String))`,,,,,,,,,,metadata only,,metadata only,,metadata only,metadata only,
+:abbr:`language ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Language of the intellectual content of the metadata record (String ))`,,,,,,,,,,metadata only,,,,,,
+:abbr:`lineage ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] General explanation of the data producer’s knowledge about the lineage of a dataset. (String))`,,,,,,,,,,metadata only,:green:`queryable metadata`,,,,,
+lowestLocation,,,,,,,,,,metadata only,,,,,,
+maximumIncidenceAngle,,,,,,,,,,metadata only,,,,,metadata only,
+minimumIncidenceAngle,,,,,,,,,,metadata only,,,,,metadata only,
+modificationDate,metadata only,,,metadata only,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,metadata only,:green:`queryable metadata`,metadata only,metadata only,:green:`queryable metadata`
+orbitDirection,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`
+orbitNumber,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
+":abbr:`orbitType ([OpenSearch Parameters for Collection Search] A string identifying the platform orbit type (e.g. LEO, GEO) (String))`",,,,,,,,,,metadata only,,,,,,
+:abbr:`organisationName ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A string identifying the name of the organization responsible for the resource (String))`,,,,:green:`queryable metadata`,:green:`queryable metadata`,,,,,metadata only,,:green:`queryable metadata`,,:green:`queryable metadata`,metadata only,
+:abbr:`organisationRole ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] The function performed by the responsible party (String ))`,,,,,,,,,,metadata only,,,,,,
+:abbr:`otherConstraint ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Other restrictions and legal prerequisites for accessing and using the resource or metadata. (String))`,,,,,,,,,,metadata only,,,,,,
+parentIdentifier,,,,,,,,,,metadata only,,:green:`queryable metadata`,,:green:`queryable metadata`,metadata only,
+:abbr:`platform ([OpenSearch Parameters for Collection Search] A string with the platform short name (e.g. Sentinel-1) (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,:green:`queryable metadata`
+:abbr:`platformSerialIdentifier ([OpenSearch Parameters for Collection Search] A string with the Platform serial identifier (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+processingCenter,,,,,,,,,,metadata only,,metadata only,,metadata only,,
+processingDate,,,,,,,,,,metadata only,metadata only,,,,metadata only,
+:abbr:`processingLevel ([OpenSearch Parameters for Collection Search] A string identifying the processing level applied to the entry (String))`,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+processingMode,,,,,,,,,,metadata only,,,,,metadata only,
+processorName,,,,,,,,,,metadata only,,metadata only,,metadata only,,
+productQualityDegradationTag,,,,,,,,,,metadata only,,,,,,
+productQualityStatus,,,,,,,,,,metadata only,:green:`queryable metadata`,metadata only,,metadata only,,
+":abbr:`productType ([OpenSearch Parameters for Collection Search] A string identifying the entry type (e.g. ER02_SAR_IM__0P, MER_RR__1P, SM_SLC__1S, GES_DISC_AIRH3STD_V005) (String ))`",:green:`queryable metadata`,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`
+productVersion,metadata only,,,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,metadata only,metadata only,:green:`queryable metadata`
+:abbr:`publicationDate ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] The date when the resource was issued (Date time))`,metadata only,,,metadata only,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,metadata only,:green:`queryable metadata`,metadata only,metadata only,:green:`queryable metadata`
+resolution,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
+sensorMode,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`
+":abbr:`sensorType ([OpenSearch Parameters for Collection Search] A string identifying the sensor type. Suggested values are: OPTICAL, RADAR, ALTIMETRIC, ATMOSPHERIC, LIMB (String))`",,,,,,,,,,metadata only,:green:`queryable metadata`,,,,,
+snowCover,,,,,,,,,,metadata only,,:green:`queryable metadata`,,:green:`queryable metadata`,metadata only,
+":abbr:`spectralRange ([OpenSearch Parameters for Collection Search] A string identifying the sensor spectral range (e.g. INFRARED, NEAR-INFRARED, UV, VISIBLE) (String))`",,,,,,,,,,metadata only,,,,,,
+startTimeFromAscendingNode,metadata only,,,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,metadata only,metadata only,,:green:`queryable metadata`,:green:`queryable metadata`,:green:`queryable metadata`,metadata only,:green:`queryable metadata`,:green:`queryable metadata`,metadata only
+swathIdentifier,,,,,,,,,,metadata only,,:green:`queryable metadata`,,:green:`queryable metadata`,,
+:abbr:`title ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A name given to the resource (String ))`,metadata only,,,metadata only,metadata only,metadata only,metadata only,metadata only,,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only,metadata only
+:abbr:`topicCategory ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] Main theme(s) of the dataset (String ))`,,,,,,,,,,metadata only,:green:`queryable metadata`,metadata only,,metadata only,,
+track,,,,,,,,,,metadata only,,,,,,
+:abbr:`useLimitation ([Additional INSPIRE obligated OpenSearch Parameters for Collection Search] A string identifying informing if the resource has usage limitations (String))`,,,,,,,,,,metadata only,,,,,,
+wavelengths,,,,,,,,,,metadata only,,,,,,
```

### Comparing `eodag-2.9.1/docs/_static/product_types.js` & `eodag-2.9.2/docs/_static/product_types.js`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/product_types_information.csv` & `eodag-2.9.2/docs/_static/product_types_information.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,97 +1,98 @@
-product type,abstract,instrument,platform,platformSerialIdentifier,processingLevel,keywords,sensorType,license,title,missionStartDate,astraea_eod,aws_eos,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,meteoblue,mundi,onda,peps,sara,theia,usgs,usgs_satapi_aws
-CAMS_EAC4,CAMS (Copernicus Atmosphere Monitoring Service) ECMWF Atmospheric Composition Reanalysis 4 from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Reanalysis,CAMS,EAC4,ADS,ECMWF",ATMOSPHERIC,proprietary,CAMS ECMWF Atmospheric Composition Reanalysis 4,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,
-CAMS_GACF_AOT,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Aerosol Optical Thickness from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,AOT,ADS",ATMOSPHERIC,proprietary,CAMS GACF Aerosol Optical Thickness,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,
-CAMS_GACF_MR,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Mixing Ratios from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,MR,ADS",ATMOSPHERIC,proprietary,CAMS GACF Mixing Ratios,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,
-CAMS_GACF_RH,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Relative Humidity from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,RH,ADS",ATMOSPHERIC,proprietary,CAMS GACF Relative Humidity,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,
-CBERS4_AWFI_L2,"China-Brazil Earth Resources Satellite, CBERS-4 AWFI camera Level-2 product. System corrected images, expect some translation error. ",AWFI,CBERS,CBERS-4,L2,"AWFI,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 AWFI Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_AWFI_L4,"China-Brazil Earth Resources Satellite, CBERS-4 AWFI camera Level-4 product. Orthorectified with ground control points. ",AWFI,CBERS,CBERS-4,L4,"AWFI,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 AWFI Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_MUX_L2,"China-Brazil Earth Resources Satellite, CBERS-4 MUX camera Level-2 product. System corrected images, expect some translation error. ",MUX,CBERS,CBERS-4,L2,"MUX,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 MUX Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_MUX_L4,"China-Brazil Earth Resources Satellite, CBERS-4 MUX camera Level-4 product. Orthorectified with ground control points. ",MUX,CBERS,CBERS-4,L4,"MUX,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 MUX Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_PAN10M_L2,"China-Brazil Earth Resources Satellite, CBERS-4 PAN10M camera Level-2 product. System corrected images, expect some translation error. ",PAN10M,CBERS,CBERS-4,L2,"PAN10M,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 PAN10M Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_PAN10M_L4,"China-Brazil Earth Resources Satellite, CBERS-4 PAN10M camera Level-4 product. Orthorectified with ground control points. ",PAN10M,CBERS,CBERS-4,L4,"PAN10M,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 PAN10M Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_PAN5M_L2,"China-Brazil Earth Resources Satellite, CBERS-4 PAN5M camera Level-2 product. System corrected images, expect some translation error. ",PAN5M,CBERS,CBERS-4,L2,"PAN5M,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 PAN5M Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-CBERS4_PAN5M_L4,"China-Brazil Earth Resources Satellite, CBERS-4 PAN5M camera Level-4 product. Orthorectified with ground control points. ",PAN5M,CBERS,CBERS-4,L4,"PAN5M,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 PAN5M Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,
-ERA5_SL,"ERA5 ECMWF climate reanalysis data on many atmospheric, land-surface and sea-state parameters together with estimates of uncertainty. Hourly data on Single Levels from 1959 to present. ",,ERA5,ERA5,,"ECMWF,Reanalysis,ERA5,CDS,Atmospheric,land,sea,hourly,single,levels",ATMOSPHERIC,proprietary,ERA5 Hourly data on Single Levels,1959-01-01T00:00:00Z,,,,available,,,,,,,,,,,,,,
-L57_REFLECTANCE,"Landsat 5,7,8 L2A data (old format) distributed by Theia (2014 to 2017-03-20) using MUSCATE prototype, Lamber 93 projection. ","OLI,TIRS",LANDSAT,"L5,L7,L8",L2A,"OLI,TIRS,LANDSAT,L5,L7,L8,L2,L2A,MUSCATE",OPTICAL,proprietary,"Landsat 5,7,8 Level-2A",2014-01-01T00:00:00Z,,,,,,,,,,,,,,,,available,,
-L8_OLI_TIRS_C1L1,Landsat 8 Operational Land Imager and Thermal Infrared Sensor Collection 1 Level-1 products. Details at https://landsat.usgs.gov/sites/default/files/documents/LSDS-1656_Landsat_Level-1_Product_Collection_Definition.pdf ,"OLI,TIRS",LANDSAT8,L8,L1,"OLI,TIRS,LANDSAT,LANDSAT8,L8,L1,C1,COLLECTION1",OPTICAL,proprietary,Landsat 8 Level-1,2013-02-11T00:00:00Z,,available,,,,,available,,available,,,,available,,,,,
-L8_REFLECTANCE,"Landsat 8 L2A data distributed by Theia since 2017-03-20 using operational version of MUSCATE, UTM projection, and tiled using Sentinel-2 tiles. ","OLI,TIRS",LANDSAT8,L8,L2A,"OLI,TIRS,LANDSAT,LANDSAT8,L8,L2,L2A,MUSCATE",OPTICAL,proprietary,Landsat 8 Level-2A,2013-02-11T00:00:00Z,,,,,,,,,,,,,,,,available,,
-LANDSAT_C2L1,The Landsat Level-1 product is a top of atmosphere product distributed as scaled and calibrated digital numbers. ,"OLI,TIRS",LANDSAT,"L1,L2,L3,L4,L5,L6,L7,L8",L1,"OLI,TIRS,LANDSAT,L1,L2,L3,L4,L5,L6,L7,L8,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-1 Product,1972-07-25T00:00:00Z,available,,,,,,,,,,,,,,,,available,available
-LANDSAT_C2L2ALB_BT,"The Landsat Top of Atmosphere Brightness Temperature (BT) product is a top of atmosphere product with radiance calculated 'at-sensor', not atmospherically corrected, and expressed in units of Kelvin. ","OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,BT,Brightness,Temperature,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Top of Atmosphere Brightness Temperature (BT) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-LANDSAT_C2L2ALB_SR,The Landsat Surface Reflectance (SR) product measures the fraction of incoming solar radiation that is reflected from Earth's surface to the Landsat sensor. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,SR,Surface,Reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Surface Reflectance (SR) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-LANDSAT_C2L2ALB_ST,The Landsat Surface Temperature (ST) product represents the temperature of the Earth's surface in Kelvin (K). ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,Surface,Temperature,ST,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Surface Temperature (ST) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-LANDSAT_C2L2ALB_TA,The Landsat Top of Atmosphere (TA) Reflectance product applies per pixel angle band corrections to the Level-1 radiance product. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,TA,Top,Atmosphere,Reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Top of Atmosphere (TA) Reflectance Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-LANDSAT_C2L2_SR,The Landsat Surface Reflectance (SR) product measures the fraction of incoming solar radiation that is reflected from Earth's surface to the Landsat sensor. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,SR,surface,reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 UTM Surface Reflectance (SR) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-LANDSAT_C2L2_ST,The Landsat Surface Temperature (ST) product represents the temperature of the Earth's surface in Kelvin (K). ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,ST,surface,temperature,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 UTM Surface Temperature (ST) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,available
-MODIS_MCD43A4,"The MODerate-resolution Imaging Spectroradiometer (MODIS) Reflectance product MCD43A4 provides 500 meter reflectance data adjusted using a bidirectional reflectance distribution function (BRDF) to model the values as if they were taken from nadir view. The MCD43A4 product contains 16 days of data provided in a level-3 gridded data set in Sinusoidal projection. Both Terra and Aqua data are used in the generation of this product, providing the highest probability for quality assurance input data. It is designated with a shortname beginning with MCD, which is used to refer to 'combined' products, those comprised of data using both Terra and Aqua. ",MODIS,Terra+Aqua,EOS AM-1+PM-1,L3,"MODIS,Terra,Aqua,EOS,AM-1+PM-1,L3,MCD43A4",OPTICAL,proprietary,MODIS MCD43A4,2000-03-05T00:00:00Z,available,available,,,,,,,,,,,,,,,,
-NAIP,"The National Agriculture Imagery Program (NAIP) acquires aerial imagery during the agricultural growing seasons in the continental U.S. This ""leaf-on"" imagery and typically ranges from 60 centimeters to 100 centimeters in resolution and is available from the naip-analytic Amazon S3 bucket as 4-band (RGB + NIR) imagery in MRF format. NAIP data is delivered at the state level; every year, a number of states receive updates, with an overall update cycle of two or three years. The tiling format of NAIP imagery is based on a 3.75' x 3.75' quarter quadrangle with a 300 meter buffer on all four sides. NAIP imagery is formatted to the UTM coordinate system using NAD83. NAIP imagery may contain as much as 10% cloud cover per tile. ",film and digital cameras,National Agriculture Imagery Program,NAIP,N/A,"film,digital,cameras,Agriculture,NAIP",OPTICAL,proprietary,National Agriculture Imagery Program,2003-01-01T00:00:00Z,available,available,,,,,,,,,,,,,,,,
-NEMSAUTO_TCDC,Total cloud cover from NOAAmodel Environment Monitoring System (NEMS) automatic domain switch. NEMSAUTO is the automatic delivery of the highest resolution meteoblue model available for any requested period of time and location. The NEMS model family are improved NMM successors (operational since 2013). NEMS is a multi-scale model (used from global down to local domains) and significantly improves cloud-development and precipitation forecast. Note that Automatic domain switching is only supported for multi point queries. Support for polygons may follow later. ,,NEMSAUTO,NEMSAUTO,,"meteoblue,NEMS,NEMSAUTO,CLOUD,COVER,TOTAL,TCDC,DAILY,MEAN",ATMOSPHERIC,proprietary,NEMSAUTO Total Cloud Cover daily mean,1984-01-01T00:00:00Z,,,,,,,,,,,available,,,,,,,
-NEMSGLOBAL_TCDC,Total cloud cover from NOAAmodel Environment Monitoring System (NEMS) global model. NEMSGLOBAL has 30km spatial and 1h temporal resolutions and produces seamless datasets from 1984 to 7 days ahead. ,,NEMSGLOBAL,NEMSGLOBAL,,"meteoblue,NEMS,NEMSGLOBAL,CLOUD,COVER,TOTAL,TCDC,DAILY,MEAN",ATMOSPHERIC,proprietary,NEMSGLOBAL Total Cloud Cover daily mean,1984-01-01T00:00:00Z,,,,,,,,,,,available,,,,,,,
-OSO,An overview of OSO Land Cover data is given on https://www.theia-land.fr/en/ceslist/land-cover-sec/ and the specific description of OSO products is available on https://www.theia-land.fr/product/carte-doccupation-des-sols-de-la-france-metropolitaine/ ,,,,L3B,"L3B,OSO,land,cover",,proprietary,OSO Land Cover,2016-01-01T00:00:00Z,,,,,,,,,,,,,,,,available,,
-PLD_BUNDLE,"Pleiades Bundle (Pan, XS)",PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,BUNDLE,Pan,Xs",OPTICAL,proprietary,Pleiades Bundle,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,available,,
-PLD_PAN,Pleiades Panchromatic (Pan),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,PAN,Panchromatic",OPTICAL,proprietary,Pleiades Panchromatic,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,available,,
-PLD_PANSHARPENED,Pleiades Pansharpened (Pan+XS),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,PANSHARPENED,Pan,Xs",OPTICAL,proprietary,Pleiades Pansharpened,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,available,,
-PLD_XS,Pleiades Multispectral (XS),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,XS,Multispectral",OPTICAL,proprietary,Pleiades Multispectral,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,available,,
-S1_SAR_GRD,"Level-1 Ground Range Detected (GRD) products consist of focused SAR data that has been detected, multi-looked and projected to ground range using an Earth ellipsoid model. Phase information is lost. The resulting product has approximately square spatial resolution pixels and square pixel spacing with reduced speckle at the cost of worse spatial resolution. GRD products can be in one of three resolutions:   Full Resolution (FR),   High Resolution (HR),   Medium Resolution (MR). The resolution is dependent upon the amount of multi-looking performed. Level-1 GRD products are available in MR and HR for IW and EW modes, MR for WV mode and MR, HR and FR for SM mode. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L1,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L1,GRD,SAFE",RADAR,proprietary,SENTINEL1 Level-1 Ground Range Detected,2014-04-03T00:00:00Z,available,available,,,available,available,,,,,,available,available,available,available,,,
-S1_SAR_OCN,"Level-2 OCN products include components for Ocean Swell spectra (OSW) providing continuity with ERS and ASAR WV and two new components: Ocean Wind Fields (OWI) and Surface Radial Velocities (RVL). The OSW is a two-dimensional ocean surface swell spectrum and includes an estimate of the wind speed and direction per swell spectrum. The OSW is generated from Stripmap and Wave modes only. For Stripmap mode, there are multiple spectra derived from internally generated Level-1 SLC images. For Wave mode, there is one spectrum per vignette. The OWI is a ground range gridded estimate of the surface wind speed and direction at 10 m above the surface derived from internally generated Level-1 GRD images of SM, IW or EW modes. The RVL is a ground range gridded difference between the measured Level-2 Doppler grid and the Level-1 calculated geometrical Doppler. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L2,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L2,OCN,SAFE",RADAR,proprietary,SENTINEL1 Level-2 OCN,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,available,available,,,
-S1_SAR_RAW,"The SAR Level-0 products consist of the sequence of Flexible Dynamic Block Adaptive Quantization (FDBAQ) compressed unfocused SAR raw data. For the data to be usable, it will need to be decompressed and processed using a SAR processor. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L0,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L0,RAW,SAFE",RADAR,proprietary,SENTINEL1 SAR Level-0,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S1_SAR_SLC,"Level-1 Single Look Complex (SLC) products consist of focused SAR data geo-referenced using orbit and attitude data from the satellite and provided in zero-Doppler slant-range geometry. The products include a single look in each dimension using the full transmit signal bandwidth and consist of complex samples preserving the phase information. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L1,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L1,SLC,SAFE",RADAR,proprietary,SENTINEL1 Level-1 Single Look Complex,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,available,available,,,
-S2_MSI_L1C,"The Level-1C product is composed of 100x100 km2 tiles (ortho-images in UTM/WGS84 projection). It results from using a Digital Elevation Model (DEM) to project the image in cartographic geometry. Per-pixel radiometric measurements are provided in Top Of Atmosphere (TOA) reflectances along with the parameters to transform them into radiances. Level-1C products are resampled with a constant Ground Sampling Distance (GSD) of 10, 20 and 60 meters depending on the native resolution of the different spectral bands. In Level-1C  products, pixel coordinates refer to the upper left corner of the pixel. Level-1C products will additionally include Cloud Masks and ECMWF data (total column of ozone, total column of water vapour and mean sea level pressure). SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi/data-formats ",MSI,SENTINEL2,"S2A,S2B",L1,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L1,L1C,SAFE",OPTICAL,proprietary,SENTINEL2 Level-1C,2015-06-23T00:00:00Z,available,available,,,available,available,available,,available,,,available,available,available,available,,available,
-S2_MSI_L2A,"The Level-2A product provides Bottom Of Atmosphere (BOA) reflectance images derived from the associated Level-1C products. Each Level-2A product is composed of 100x100 km2 tiles in cartographic geometry (UTM/WGS84 projection). SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi/data-formats ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,SAFE",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,available,available,,,available,available,available,,,,,available,available,available,available,,,
-S2_MSI_L2A_COG,"The Level-2A product provides Bottom Of Atmosphere (BOA) reflectance images derived from the associated Level-1C products. Each Level-2A product is composed of 100x100 km2 tiles in cartographic geometry (UTM/WGS84 projection). Product containing Cloud Optimized GeoTIFF images, without SAFE formatting. ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,COG",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,,,,,,,,available,,,,,,,,,,
-S2_MSI_L2A_MAJA,"The level 2A products correct the data for atmospheric effects and detect the clouds and their shadows using MAJA. MAJA uses MUSCATE processing center at CNES, in the framework of THEIA land data center. Sentinel-2 level 1C data are downloaded from PEPS. The full description of the product format is available at https://theia.cnes.fr/atdistrib/documents/PSC-NT-411-0362-CNES_01_00_SENTINEL-2A_L2A_Products_Description.pdf ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,MAJA",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,available,,
-S2_MSI_L2B_MAJA_SNOW,The Theia snow product is derived from Sentinel-2 L2A images generated by Theia. It  indicates the snow presence or absence on the land surface every fifth day if there is no cloud. The product is distributed by Theia as a raster file (8 bits GeoTIFF) of 20 m resolution and a vector file (Shapefile polygons). More details about the snow products description are available at http://www.cesbio.ups-tlse.fr/multitemp/?page_id=10748#en ,MSI,SENTINEL2,"S2A,S2B",L2,"MSI,MAJA,SENTINEL,sentinel2,S2,S2A,S2B,L2,L2B,SNOW",OPTICAL,proprietary,SENTINEL2 snow product,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,available,,
-S2_MSI_L2B_MAJA_WATER,A description of the Land Water Quality data distributed by Theia is available at https://theia.cnes.fr/atdistrib/documents/THEIA-ST-411-0477-CNES_01-03_Format_Specification_of_OBS2CO_WaterColor_Products.pdf ,MSI,SENTINEL2,"S2A,S2B",L2,"MSI,MAJA,SENTINEL,sentinel2,S2,S2A,S2B,L2,L2B,WATER",OPTICAL,proprietary,SENTINEL2 L2B-WATER,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,available,,
-S2_MSI_L3A_WASP,"The Level-3A product provides a monthly synthesis of surface reflectances from Theia's L2A products. The synthesis is based on a weighted arithmetic mean of clear observations. The data processing is produced by WASP (Weighted Average Synthesis Processor), by MUSCATE data center at CNES, in the framework of THEIA data center. The full description of the product format is available at https://theia.cnes.fr/atdistrib/documents/THEIA-ST-411-0419-CNES_01-04_Format_Specification_of_MUSCATE_Level-3A_Products-signed.pdf ",MSI,SENTINEL2,"S2A,S2B",L3,"MSI,SENTINEL,sentinel2,S2,S2A,S2B,L3,L3A,WASP",OPTICAL,proprietary,SENTINEL2 Level-3A,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,available,,
-S3_EFR,,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,EFR",OPTICAL,proprietary,SENTINEL3 EFR,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_ERR,,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,ERR",OPTICAL,proprietary,SENTINEL3 ERR,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_LAN,LAN or SR_2_LAN___ (peps),SRAL,SENTINEL3,"S3A,S3B",L2,"SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,LAN",RADAR,proprietary,SENTINEL3 SRAL Level-2 LAN,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_OLCI_L2LFR,"The OLCI Level-2 Water Full Resolution (OL_2_WFR) products contain water and atmospheric geophysical products at Full resolution with a spatial sampling of approximately 300 m. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WFR,WFR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Full Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_OLCI_L2LRR,"The OLCI Level-2 Land Reduced Resolution (OL_2_LRR) products contain land and atmospheric geophysical products at Reduced resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-land ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2LRR,LRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Land Reduced Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_OLCI_L2WFR,"The OLCI Level-2 Water Full Resolution (OL_2_WRR) products contain water and atmospheric geophysical products at Full resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WRR,WRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Full Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,available,,,
-S3_OLCI_L2WRR,"The OLCI Level-2 Water Reduced Resolution (OL_2_WRR) products contain water and atmospheric geophysical products at Reduced resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WRR,WRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Reduced Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,available,,,
-S3_RAC,Sentinel 3 OLCI products output during Radiometric Calibration mode ,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,L2,RAC",OPTICAL,proprietary,SENTINEL3 RAC,2016-02-16T00:00:00Z,,,,,,,,,,,,,,,available,,,
-S3_SLSTR_L1RBT,"SLSTR Level-1 observation mode products consisting of full resolution, geolocated, co-located nadir and along track view, Top of Atmosphere (TOA) brightness temperatures (in the case of thermal IR channels) or radiances (in the case of visible, NIR and SWIR channels) from all SLSTR channels, and quality flags, pixel classification information and meteorological annotations ",SLSTR,SENTINEL3,"S3A,S3B",L1,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,L1RBT,RBT",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SLSTR_L2AOD,"The Copernicus NRT S3 AOD processor quantifies the abundance of aerosol particles and monitors their global distribution and long-range transport, at the scale of 9.5 x 9.5 km2. All observations are made available in less than three hours from the SLSTR observation sensing time. It is only applicable during daytime. NOTE: The SLSTR L2 AOD product is generated by EUMETSAT in NRT only. An offline (NTC) AOD product is generated from SYN data by ESA, exploiting the synergy between the SLSTR and OLCI instruments. ",SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2AOD,AOD",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 AOD,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,,,available,,,
-S3_SLSTR_L2FRP,"The SLSTR Level-2 FRP product is providing one measurement data file, FRP_in.nc, with Fire Radiative Power (FRP) values and associated parameters generated for each fire detected over land and projected on the SLSTR 1 km grid. The fire detection is based on a mixed thermal band, combining S7 radiometric measurements and, for pixels associated with a saturated value of S7 (i.e. above 311 K), F1 radiometric measurements. ",SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2FRP,FRP",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 FRP,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SLSTR_L2LST,The SLSTR Level-2 LST product provides land surface parameters generated on the wide 1 km measurement grid. It contains measurement file with Land Surface Temperature (LST) values with associated parameters (LST parameters are computed and provided for each pixel (re-gridded or orphan) included in the 1 km measurement grid) ,SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2LST,LST",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 LST,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SLSTR_L2WST,The SLSTR Level-2 WST product provides land surface parameters generated on the wide 1 km measurement grid. It contains measurement file with Water Surface Temperature (WST) values with associated parameters (WST parameters are computed and provided for each pixel (re-gridded or orphan) included in the 1 km measurement grid) ,SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WST,WST",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 WST,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,available,,,
-S3_SRA,,SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SRA_A,"A Level 1A SRAL product contains one ""measurement data file"" containing the L1A measurements parameters: ECHO_SAR_Ku: L1A Tracking measurements (sorted and calibrated) in SAR mode - Ku-band (80-Hz) ECHO_PLRM: L1A Tracking measurements (sorted and calibrated) in pseudo-LRM mode - Ku and C bands (80-Hz) ",SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1 SRA_A,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SRA_BS,"A Level 1B-S SRAL product contains one ""measurement data file"" containing the L1b measurements parameters: ECHO_SAR_Ku : L1b Tracking measurements in SAR mode - Ku band (20-Hz) as defined in the L1b MEAS product               completed with SAR expert information ECHO_PLRM : L1b Tracking measurements in pseudo-LRM mode - Ku and C bands (20-Hz) as defined in the L1b             MEAS product ",SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1 SRA_BS,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SY_AOD,"The Level-2 SYN AOD product (SY_2_AOD) is produced by a dedicated processor including the whole SYN L1 processing module and a global synergy level 2 processing module retrieving, over land and sea, aerosol optical thickness. The resolution of this product is wider than classic S3 products, as the dataset are provided on a 4.5 km² resolution ",SYNERGY,SENTINEL3,"S3A,S3B",L2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,AOD","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 AOD,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,available,,,
-S3_SY_SYN,"The Level-2 SYN product (SY_2_SYN) is produced by the Synergy Level-1/2 SDR software and contains surface reflectance and aerosol parameters over land. All measurement datasets are provided on the OLCI image grid, similar to the one included in the OLCI L1b product. Some sub-sampled annotations and atmospheric datasets are provided on the OLCI tie-points grid. Several associated variables are also provided in annotation data files. ",SYNERGY,SENTINEL3,"S3A,S3B",L2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,SYN","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 SYN,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SY_V10,"The Level-2 VG1 and V10 SYN products (SY_2_VG1 and SY_2_V10 respectively) are produced by the SYNERGY Level-2 processor and contain 1 km VEGETATION-like product, 1 and 10 days synthesis surface reflectances and NDVI. The product grid and the four spectral bands are similar to the SYN Level-2 VGP product. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2W,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,V10","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 V10,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SY_VG1,"The Level-2 VG1 and V10 SYN products (SY_2_VG1 and SY_2_V10 respectively) are produced by the SYNERGY Level-2 processor and contain 1 km VEGETATION-like product, 1 and 10 days synthesis surface reflectances and NDVI. The product grid and the four spectral bands are similar to the SYN Level-2 VGP product. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,VG1","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 VG1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_SY_VGP,"The Level-2 VGP SYN product (SY_2_VGP) is produced by the Global Synergy Level-1/2 software and contains 1 km VEGETATION-like product TOA reflectances. The ""1 km VEGETATION-like product"" label means that measurements are provided on a regular latitude-longitude grid, with an equatorial sampling distance of approximately 1 km. This product is restricted in longitude, including only filled ones. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,VGP","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 VGP,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,available,,,
-S3_WAT,,SRAL,SENTINEL3,"S3A,S3B",L2,"SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,WAT",RADAR,proprietary,SENTINEL3 SRAL Level-2 WAT,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,available,,,
-S5P_L1B_IR_SIR,"Solar irradiance spectra for the SWIR bands (band 7 and band 8). TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,IR,SIR,SWIR,Irradiances",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Irradiances for the SWIR bands,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,
-S5P_L1B_IR_UVN,"Solar irradiance spectra for the UVN bands (band 1 through band 6). TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,IR,UVN,Irradiances",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Irradiances for the UVN bands,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,
-S5P_L1B_RA_BD1,"Sentinel-5 Precursor Level 1B Radiances for spectral band 1. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD1,BAND1,B01",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 1,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD2,"Sentinel-5 Precursor Level 1B Radiances for spectral band 2. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD2,BAND2,B02",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 2,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD3,"Sentinel-5 Precursor Level 1B Radiances for spectral band 3. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD3,BAND3,B03",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 3,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD4,"Sentinel-5 Precursor Level 1B Radiances for spectral band 4. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD4,BAND4,B04",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 4,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD5,"Sentinel-5 Precursor Level 1B Radiances for spectral band 5. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD5,BAND5,B05",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 5,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD6,"Sentinel-5 Precursor Level 1B Radiances for spectral band 6. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD6,BAND6,B06",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 6,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD7,"Sentinel-5 Precursor Level 1B Radiances for spectral band 7. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD7,BAND7,B07",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 7,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L1B_RA_BD8,"Sentinel-5 Precursor Level 1B Radiances for spectral band 8. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD8,BAND8,B08",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 8,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_AER_AI,"TROPOMI aerosol index is referred to as the Ultraviolet Aerosol Index (UVAI). The relatively simple calculation of the Aerosol Index is based on wavelength dependent changes in Rayleigh scattering in the UV spectral range where ozone absorption is very small. UVAI can also be calculated in the presence of clouds so that daily, global coverage is possible. This is ideal for tracking the evolution of episodic aerosol plumes from dust outbreaks, volcanic ash, and biomass burning. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,AER,AI,Ultraviolet,Aerosol,Index",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ultraviolet Aerosol Index,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_AER_LH,"The TROPOMI Aerosol Layer Height product focuses on retrieval of vertically localised aerosol layers in the free troposphere, such as desert dust, biomass burning aerosol, or volcanic ash plumes. The height of such layers is retrieved for cloud-free conditions. Height information for aerosols in the free troposphere is particularly important for aviation safety. Scientific applications include radiative forcing studies, long-range transport modelling and studies of cloud formation processes. Aerosol height information also helps to interpret the UV Aerosol Index (UVAI) in terms of aerosol absorption as the index is strongly height-dependent. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,AER,LH,Aerosol,Layer,Height",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Aerosol Layer Height,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_CH4,"Methane (CH4) is, after carbon dioxide (CO2), the most important contributor to the anthropogenically enhanced greenhouse effect. Roughly three-quarters of methane emissions are anthropogenic and as such it is important to continue the record of satellite-based measurements. TROPOMI aims at providing CH4 column concentrations with high sensitivity to the Earth's surface, good spatio/temporal coverage, and sufficient accuracy to facilitate inverse modelling of sources and sinks. The output product consists of the retrieved methane column and a row vector referred to as the column averaging kernel A. The column averaging kernel describes how the retrieved column relates to the true profile and should be used in validation exercises (when possible) or use of the product in source/sink inverse modelling. The output product also contains altitude levels of the layer interfaces to which the column averaging kernel corresponds. Additional output for Level-2 data products: viewing geometry, precision of retrieved methane, residuals of the fit, quality flags (cloudiness, terrain roughness etc.) and retrieved albedo and aerosol properties. The latter properties are required for a posteriori filtering and for estimation of total retrieval error. The Sentinel-5 Precursor mission flies in loose formation (about 3.5 - 5 minutes behind) with the S-NPP (SUOMI-National Polar-orbiting Partnership) mission to use VIIRS (Visible Infrared Imaging Radiometer Suite) cloud information to select cloud free TROPOMI pixels for high quality methane retrieval. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CH4,Methane",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Methane,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_CLOUD,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves operationally the most important quantities for cloud correction of satellite trace gas retrievals: cloud fraction, cloud optical thickness (albedo), and cloud-top pressure (height). Cloud parameters from TROPOMI are not only used for enhancing the accuracy of trace gas retrievals, but also to extend the satellite data record of cloud information derived from oxygen A-band measurements initiated with GOME. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CLOUD",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Cloud,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_CO,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves the CO global abundance exploiting clear-sky and cloudy-sky Earth radiance measurements in the 2.3 µm spectral range of the shortwave infrared (SWIR) part of the solar spectrum. TROPOMI clear sky observations provide CO total columns with sensitivity to the tropospheric boundary layer. For cloudy atmospheres, the column sensitivity changes according to the light path. The TROPOMI CO retrieval uses the same method employed by SCIAMACHY. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CO,Carbon,Monoxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Carbon Monoxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_HCHO,"Formaldehyde is an intermediate gas in almost all oxidation chains of Non-Methane Volatile Organic Compounds (NMVOC), leading eventually to CO2. NMVOCs are, together with NOx, CO and CH4, among the most important precursors of tropospheric O3. The major HCHO source in the remote atmosphere is CH4 oxidation. Over the continents, the oxidation of higher NMVOCs emitted from vegetation, fires, traffic and industrial sources results in important and localised enhancements of the HCHO levels. In addition to the main product results, such as HCHO slant column, vertical column and air mass factor, the level 2 data files contain several additional parameters and diagnostic information. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,HCHO,Formaldehyde",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Formaldehyde,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_NO2,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves operationally tropospheric and stratospheric NO2 column products. The TROPOMI NO2 data products pose an improvement over previous NO2 data sets, particularly in their unprecedented spatial resolution, but also in the separation of the stratospheric and tropospheric contributions of the retrieved slant columns, and in the calculation of the air-mass factors used to convert slant to total columns. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NO2,Nitrogen,Dioxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Nitrogen Dioxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_NP_BD3,"S5P-NPP Cloud for spectral band 3. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD3,B03,BAND3",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 3,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_NP_BD6,"S5P-NPP Cloud for spectral band 6. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD6,B06,BAND6",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 6,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_NP_BD7,"S5P-NPP Cloud for spectral band 7. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD7,B07,BAND7",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 7,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_O3,"Ozone (O3) is of crucial importance for the equilibrium of the Earth's atmosphere. In the stratosphere, the ozone layer shields the biosphere from dangerous solar ultraviolet radiation. In the troposphere, it acts as an efficient cleansing agent, but at high concentration it also becomes harmful to the health of humans, animals, and vegetation. Ozone is also an important greenhouse-gas contributor to ongoing climate change. These products are provided in NetCDF-CF format and contain total ozone, ozone temperature, and error information including averaging kernels. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,Ozone",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ozone,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_O3_PR,"Retrieved ozone profiles are used to monitor the evolution of stratospheric and tropospheric ozone. Such monitoring is important as the ozone layer protects life on Earth against harmful UV radiation. The ozone layer is recovering from depletion due to manmade Chlorofluorocarbons (CFCs). Tropospheric ozone is toxic and it plays an important role in tropospheric chemistry. Also, ozone is a greenhouse gas and is therefore also relevant for climate change. The main parameters in the file are the retrieved ozone profile at 33 levels and the retrieved sub-columns of ozone in 6 layers. In addition, the total ozone column and tropospheric ozone columns are provided. For the ozone profile, the precision and smoothing errors, the a-priori profile and the averaging kernel are also provided. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,PR,Ozone,Profile",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ozone Profile,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-S5P_L2_O3_TCL,"Ozone in the tropical troposphere plays various important roles. The intense UV radiation and high humidity in the tropics stimulate the formation of the hydroxyl radical (OH) by the photolysis of ozone. OH is the most important oxidant in the troposphere because it reacts with virtually all trace gases, such as CO, CH4 and other hydrocarbons. The tropics are also characterized by large emissions of nitrogen oxides (NOx), carbon monoxide (CO) and hydrocarbons, both from natural and anthropogenic sources. Ozone that is formed over regions where large amounts of these ozone precursors are emitted, can be transported over great distances and affects areas far from the source. The TROPOMI tropospheric ozone product is a level-2c product that represents three day averaged tropospheric ozone columns on a 0.5° by 1° latitude-longitude grid for the tropical region between 20°N and 20°S. The TROPOMI tropospheric ozone column product uses the TROPOMI Level-2 total OZONE and CLOUD products as input. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,TCL,Tropospheric,Ozone",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Tropospheric Ozone,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,
-S5P_L2_SO2,"Sulphur dioxide (SO2) enters the Earth's atmosphere through both natural (~30%) and anthropogenic processes (~70%). It plays a role in chemistry on a local and global scale and its impact ranges from short term pollution to effects on climate. Beside the total column of SO2, enhanced levels of SO2 are flagged within the products. The recognition of enhanced SO2 values is essential in order to detect and monitor volcanic eruptions and anthropogenic pollution sources. Volcanic SO2 emissions may also pose a threat to aviation, along with volcanic ash. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,SO2,Sulphur,Dioxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Sulphur Dioxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,
-SPOT5_SPIRIT,SPOT 5 stereoscopic survey of Polar Ice. ,,SPOT5,SPOT5,L1A,"SPOT,SPOT5,L1A",OPTICAL,proprietary,Spot 5 SPIRIT,2002-05-04T00:00:00Z,,,,,,,,,,,,,,,,available,,
-SPOT_SWH,The Spot World Heritage (SWH) programme objective is the free availability for non-commercial use of orthorectified products derived from multispectral images of more than 5 years old from the Spot 1-5 satellites family. More informations on https://www.theia-land.fr/en/product/spot-world-heritage/ ,,SPOT1-5,SPOT1-5,L1C,"SPOT,SPOT1,SPOT2,SPOT3,SPOT4,SPOT5,L1C",OPTICAL,proprietary,Spot World Heritage,1986-02-22T00:00:00Z,,,,,,,,,,,,,,,,available,,
-SPOT_SWH_OLD,Spot world heritage Old format. ,,SPOT1-5,SPOT1-5,L1C,"SPOT,SPOT1,SPOT2,SPOT3,SPOT4,SPOT5,L1C",OPTICAL,proprietary,Spot World Heritage,1986-02-22T00:00:00Z,,,,,,,,,,,,,,,,available,,
-TIGGE_CF_SFC,TIGGE (THORPEX Interactive Grand Global Ensemble) Surface Control forecast from ECMWF ,,TIGGE,TIGGE,,"THORPEX,TIGGE,CF,SFC,ECMWF",ATMOSPHERIC,proprietary,TIGGE ECMWF Surface Control forecast,2003-01-01T00:00:00Z,,,,,,,,,,available,,,,,,,,
-VENUS_L1C,A light description of Venus L1 data is available at http://www.cesbio.ups-tlse.fr/multitemp/?page_id=12984 ,,VENUS,VENUS,L1C,"VENUS,L1,L1C",OPTICAL,proprietary,Venus Level1-C,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,available,,
-VENUS_L2A_MAJA,"Level2 products provide surface reflectances after atmospheric correction, along with masks of clouds and their shadows. Data is processed by MAJA (before called MACCS) for THEIA land data center. ",,VENUS,VENUS,L2A,"VENUS,L2,L2A",OPTICAL,proprietary,Venus Level2-A,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,available,,
-VENUS_L3A_MAJA,,,VENUS,VENUS,L3A,"VENUS,L3,L3A",OPTICAL,proprietary,Venus Level3-A,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,available,,
+product type,abstract,instrument,platform,platformSerialIdentifier,processingLevel,keywords,sensorType,license,title,missionStartDate,astraea_eod,aws_eos,cop_ads,cop_cds,cop_dataspace,creodias,earth_search,earth_search_cog,earth_search_gcs,ecmwf,meteoblue,mundi,onda,peps,planetary_computer,sara,theia,usgs,usgs_satapi_aws
+CAMS_EAC4,CAMS (Copernicus Atmosphere Monitoring Service) ECMWF Atmospheric Composition Reanalysis 4 from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Reanalysis,CAMS,EAC4,ADS,ECMWF",ATMOSPHERIC,proprietary,CAMS ECMWF Atmospheric Composition Reanalysis 4,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,,
+CAMS_GACF_AOT,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Aerosol Optical Thickness from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,AOT,ADS",ATMOSPHERIC,proprietary,CAMS GACF Aerosol Optical Thickness,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,,
+CAMS_GACF_MR,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Mixing Ratios from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,MR,ADS",ATMOSPHERIC,proprietary,CAMS GACF Mixing Ratios,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,,
+CAMS_GACF_RH,CAMS (Copernicus Atmosphere Monitoring Service) Global Atmospheric Composition Forecast of Relative Humidity from Copernicus ADS ,,CAMS,CAMS,,"Copernicus,Atmosphere,Atmospheric,Forecast,CAMS,GACF,RH,ADS",ATMOSPHERIC,proprietary,CAMS GACF Relative Humidity,2003-01-01T00:00:00Z,,,available,,,,,,,,,,,,,,,,
+CBERS4_AWFI_L2,"China-Brazil Earth Resources Satellite, CBERS-4 AWFI camera Level-2 product. System corrected images, expect some translation error. ",AWFI,CBERS,CBERS-4,L2,"AWFI,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 AWFI Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_AWFI_L4,"China-Brazil Earth Resources Satellite, CBERS-4 AWFI camera Level-4 product. Orthorectified with ground control points. ",AWFI,CBERS,CBERS-4,L4,"AWFI,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 AWFI Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_MUX_L2,"China-Brazil Earth Resources Satellite, CBERS-4 MUX camera Level-2 product. System corrected images, expect some translation error. ",MUX,CBERS,CBERS-4,L2,"MUX,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 MUX Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_MUX_L4,"China-Brazil Earth Resources Satellite, CBERS-4 MUX camera Level-4 product. Orthorectified with ground control points. ",MUX,CBERS,CBERS-4,L4,"MUX,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 MUX Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_PAN10M_L2,"China-Brazil Earth Resources Satellite, CBERS-4 PAN10M camera Level-2 product. System corrected images, expect some translation error. ",PAN10M,CBERS,CBERS-4,L2,"PAN10M,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 PAN10M Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_PAN10M_L4,"China-Brazil Earth Resources Satellite, CBERS-4 PAN10M camera Level-4 product. Orthorectified with ground control points. ",PAN10M,CBERS,CBERS-4,L4,"PAN10M,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 PAN10M Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_PAN5M_L2,"China-Brazil Earth Resources Satellite, CBERS-4 PAN5M camera Level-2 product. System corrected images, expect some translation error. ",PAN5M,CBERS,CBERS-4,L2,"PAN5M,CBERS,CBERS-4,L2",OPTICAL,proprietary,CBERS-4 PAN5M Level-2,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+CBERS4_PAN5M_L4,"China-Brazil Earth Resources Satellite, CBERS-4 PAN5M camera Level-4 product. Orthorectified with ground control points. ",PAN5M,CBERS,CBERS-4,L4,"PAN5M,CBERS,CBERS-4,L4",OPTICAL,proprietary,CBERS-4 PAN5M Level-4,2014-12-07T00:00:00Z,,available,,,,,,,,,,,,,,,,,
+ERA5_SL,"ERA5 ECMWF climate reanalysis data on many atmospheric, land-surface and sea-state parameters together with estimates of uncertainty. Hourly data on Single Levels from 1959 to present. ",,ERA5,ERA5,,"ECMWF,Reanalysis,ERA5,CDS,Atmospheric,land,sea,hourly,single,levels",ATMOSPHERIC,proprietary,ERA5 Hourly data on Single Levels,1959-01-01T00:00:00Z,,,,available,,,,,,,,,,,,,,,
+L57_REFLECTANCE,"Landsat 5,7,8 L2A data (old format) distributed by Theia (2014 to 2017-03-20) using MUSCATE prototype, Lamber 93 projection. ","OLI,TIRS",LANDSAT,"L5,L7,L8",L2A,"OLI,TIRS,LANDSAT,L5,L7,L8,L2,L2A,MUSCATE",OPTICAL,proprietary,"Landsat 5,7,8 Level-2A",2014-01-01T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+L8_OLI_TIRS_C1L1,Landsat 8 Operational Land Imager and Thermal Infrared Sensor Collection 1 Level-1 products. Details at https://landsat.usgs.gov/sites/default/files/documents/LSDS-1656_Landsat_Level-1_Product_Collection_Definition.pdf ,"OLI,TIRS",LANDSAT8,L8,L1,"OLI,TIRS,LANDSAT,LANDSAT8,L8,L1,C1,COLLECTION1",OPTICAL,proprietary,Landsat 8 Level-1,2013-02-11T00:00:00Z,,available,,,,,available,,available,,,,available,,,,,,
+L8_REFLECTANCE,"Landsat 8 L2A data distributed by Theia since 2017-03-20 using operational version of MUSCATE, UTM projection, and tiled using Sentinel-2 tiles. ","OLI,TIRS",LANDSAT8,L8,L2A,"OLI,TIRS,LANDSAT,LANDSAT8,L8,L2,L2A,MUSCATE",OPTICAL,proprietary,Landsat 8 Level-2A,2013-02-11T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+LANDSAT_C2L1,The Landsat Level-1 product is a top of atmosphere product distributed as scaled and calibrated digital numbers. ,"OLI,TIRS",LANDSAT,"L1,L2,L3,L4,L5,L6,L7,L8",L1,"OLI,TIRS,LANDSAT,L1,L2,L3,L4,L5,L6,L7,L8,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-1 Product,1972-07-25T00:00:00Z,available,,,,,,,,,,,,,,available,,,available,available
+LANDSAT_C2L2,Collection 2 Landsat OLI/TIRS Level-2 Science Products (L2SP) include Surface Reflectance and Surface Temperature scene-based products. ,"OLI,TIRS",LANDSAT,"L8,L9",L1,"OLI,TIRS,LANDSAT,L8,L9,L2,C2,COLLECTION2",OPTICAL,proprietary,Landsat OLI and TIRS Collection 2 Level-2 Science Products 30-meter multispectral data.,2013-02-11T00:00:00Z,,,,,,,,,,,,,,,available,,,available,
+LANDSAT_C2L2ALB_BT,"The Landsat Top of Atmosphere Brightness Temperature (BT) product is a top of atmosphere product with radiance calculated 'at-sensor', not atmospherically corrected, and expressed in units of Kelvin. ","OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,BT,Brightness,Temperature,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Top of Atmosphere Brightness Temperature (BT) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+LANDSAT_C2L2ALB_SR,The Landsat Surface Reflectance (SR) product measures the fraction of incoming solar radiation that is reflected from Earth's surface to the Landsat sensor. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,SR,Surface,Reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Surface Reflectance (SR) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+LANDSAT_C2L2ALB_ST,The Landsat Surface Temperature (ST) product represents the temperature of the Earth's surface in Kelvin (K). ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,Surface,Temperature,ST,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Surface Temperature (ST) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+LANDSAT_C2L2ALB_TA,The Landsat Top of Atmosphere (TA) Reflectance product applies per pixel angle band corrections to the Level-1 radiance product. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,L2ALB,TA,Top,Atmosphere,Reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 Albers Top of Atmosphere (TA) Reflectance Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+LANDSAT_C2L2_SR,The Landsat Surface Reflectance (SR) product measures the fraction of incoming solar radiation that is reflected from Earth's surface to the Landsat sensor. ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,SR,surface,reflectance,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 UTM Surface Reflectance (SR) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+LANDSAT_C2L2_ST,The Landsat Surface Temperature (ST) product represents the temperature of the Earth's surface in Kelvin (K). ,"OLI,TIRS",LANDSAT,"L4,L5,L7,L8",L2,"OLI,TIRS,LANDSAT,L4,L5,L7,L8,L2,ST,surface,temperature,C2,COLLECTION2",OPTICAL,proprietary,Landsat Collection 2 Level-2 UTM Surface Temperature (ST) Product,1982-08-22T00:00:00Z,,,,,,,,,,,,,,,,,,,available
+MODIS_MCD43A4,"The MODerate-resolution Imaging Spectroradiometer (MODIS) Reflectance product MCD43A4 provides 500 meter reflectance data adjusted using a bidirectional reflectance distribution function (BRDF) to model the values as if they were taken from nadir view. The MCD43A4 product contains 16 days of data provided in a level-3 gridded data set in Sinusoidal projection. Both Terra and Aqua data are used in the generation of this product, providing the highest probability for quality assurance input data. It is designated with a shortname beginning with MCD, which is used to refer to 'combined' products, those comprised of data using both Terra and Aqua. ",MODIS,Terra+Aqua,EOS AM-1+PM-1,L3,"MODIS,Terra,Aqua,EOS,AM-1+PM-1,L3,MCD43A4",OPTICAL,proprietary,MODIS MCD43A4,2000-03-05T00:00:00Z,available,available,,,,,,,,,,,,,available,,,,
+NAIP,"The National Agriculture Imagery Program (NAIP) acquires aerial imagery during the agricultural growing seasons in the continental U.S. This ""leaf-on"" imagery and typically ranges from 60 centimeters to 100 centimeters in resolution and is available from the naip-analytic Amazon S3 bucket as 4-band (RGB + NIR) imagery in MRF format. NAIP data is delivered at the state level; every year, a number of states receive updates, with an overall update cycle of two or three years. The tiling format of NAIP imagery is based on a 3.75' x 3.75' quarter quadrangle with a 300 meter buffer on all four sides. NAIP imagery is formatted to the UTM coordinate system using NAD83. NAIP imagery may contain as much as 10% cloud cover per tile. ",film and digital cameras,National Agriculture Imagery Program,NAIP,N/A,"film,digital,cameras,Agriculture,NAIP",OPTICAL,proprietary,National Agriculture Imagery Program,2003-01-01T00:00:00Z,available,available,,,,,,,,,,,,,available,,,,
+NEMSAUTO_TCDC,Total cloud cover from NOAAmodel Environment Monitoring System (NEMS) automatic domain switch. NEMSAUTO is the automatic delivery of the highest resolution meteoblue model available for any requested period of time and location. The NEMS model family are improved NMM successors (operational since 2013). NEMS is a multi-scale model (used from global down to local domains) and significantly improves cloud-development and precipitation forecast. Note that Automatic domain switching is only supported for multi point queries. Support for polygons may follow later. ,,NEMSAUTO,NEMSAUTO,,"meteoblue,NEMS,NEMSAUTO,CLOUD,COVER,TOTAL,TCDC,DAILY,MEAN",ATMOSPHERIC,proprietary,NEMSAUTO Total Cloud Cover daily mean,1984-01-01T00:00:00Z,,,,,,,,,,,available,,,,,,,,
+NEMSGLOBAL_TCDC,Total cloud cover from NOAAmodel Environment Monitoring System (NEMS) global model. NEMSGLOBAL has 30km spatial and 1h temporal resolutions and produces seamless datasets from 1984 to 7 days ahead. ,,NEMSGLOBAL,NEMSGLOBAL,,"meteoblue,NEMS,NEMSGLOBAL,CLOUD,COVER,TOTAL,TCDC,DAILY,MEAN",ATMOSPHERIC,proprietary,NEMSGLOBAL Total Cloud Cover daily mean,1984-01-01T00:00:00Z,,,,,,,,,,,available,,,,,,,,
+OSO,An overview of OSO Land Cover data is given on https://www.theia-land.fr/en/ceslist/land-cover-sec/ and the specific description of OSO products is available on https://www.theia-land.fr/product/carte-doccupation-des-sols-de-la-france-metropolitaine/ ,,,,L3B,"L3B,OSO,land,cover",,proprietary,OSO Land Cover,2016-01-01T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+PLD_BUNDLE,"Pleiades Bundle (Pan, XS)",PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,BUNDLE,Pan,Xs",OPTICAL,proprietary,Pleiades Bundle,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+PLD_PAN,Pleiades Panchromatic (Pan),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,PAN,Panchromatic",OPTICAL,proprietary,Pleiades Panchromatic,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+PLD_PANSHARPENED,Pleiades Pansharpened (Pan+XS),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,PANSHARPENED,Pan,Xs",OPTICAL,proprietary,Pleiades Pansharpened,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+PLD_XS,Pleiades Multispectral (XS),PHR,PLEIADES,"P1A,P1B",PRIMARY,"PHR,PLEIADES,P1A,P1B,PRIMARY,PLD,XS,Multispectral",OPTICAL,proprietary,Pleiades Multispectral,2011-12-17T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+S1_SAR_GRD,"Level-1 Ground Range Detected (GRD) products consist of focused SAR data that has been detected, multi-looked and projected to ground range using an Earth ellipsoid model. Phase information is lost. The resulting product has approximately square spatial resolution pixels and square pixel spacing with reduced speckle at the cost of worse spatial resolution. GRD products can be in one of three resolutions:   Full Resolution (FR),   High Resolution (HR),   Medium Resolution (MR). The resolution is dependent upon the amount of multi-looking performed. Level-1 GRD products are available in MR and HR for IW and EW modes, MR for WV mode and MR, HR and FR for SM mode. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L1,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L1,GRD,SAFE",RADAR,proprietary,SENTINEL1 Level-1 Ground Range Detected,2014-04-03T00:00:00Z,available,available,,,available,available,,,,,,available,available,available,available,available,,,
+S1_SAR_OCN,"Level-2 OCN products include components for Ocean Swell spectra (OSW) providing continuity with ERS and ASAR WV and two new components: Ocean Wind Fields (OWI) and Surface Radial Velocities (RVL). The OSW is a two-dimensional ocean surface swell spectrum and includes an estimate of the wind speed and direction per swell spectrum. The OSW is generated from Stripmap and Wave modes only. For Stripmap mode, there are multiple spectra derived from internally generated Level-1 SLC images. For Wave mode, there is one spectrum per vignette. The OWI is a ground range gridded estimate of the surface wind speed and direction at 10 m above the surface derived from internally generated Level-1 GRD images of SM, IW or EW modes. The RVL is a ground range gridded difference between the measured Level-2 Doppler grid and the Level-1 calculated geometrical Doppler. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L2,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L2,OCN,SAFE",RADAR,proprietary,SENTINEL1 Level-2 OCN,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,available,,available,,,
+S1_SAR_RAW,"The SAR Level-0 products consist of the sequence of Flexible Dynamic Block Adaptive Quantization (FDBAQ) compressed unfocused SAR raw data. For the data to be usable, it will need to be decompressed and processed using a SAR processor. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L0,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L0,RAW,SAFE",RADAR,proprietary,SENTINEL1 SAR Level-0,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S1_SAR_SLC,"Level-1 Single Look Complex (SLC) products consist of focused SAR data geo-referenced using orbit and attitude data from the satellite and provided in zero-Doppler slant-range geometry. The products include a single look in each dimension using the full transmit signal bandwidth and consist of complex samples preserving the phase information. SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/data-formats/safe-specification ",SAR,SENTINEL1,"S1A,S1B",L1,"SAR,SENTINEL,SENTINEL1,S1,S1A,S1B,L1,SLC,SAFE",RADAR,proprietary,SENTINEL1 Level-1 Single Look Complex,2014-04-03T00:00:00Z,,,,,available,available,,,,,,available,available,available,,available,,,
+S2_MSI_L1C,"The Level-1C product is composed of 100x100 km2 tiles (ortho-images in UTM/WGS84 projection). It results from using a Digital Elevation Model (DEM) to project the image in cartographic geometry. Per-pixel radiometric measurements are provided in Top Of Atmosphere (TOA) reflectances along with the parameters to transform them into radiances. Level-1C products are resampled with a constant Ground Sampling Distance (GSD) of 10, 20 and 60 meters depending on the native resolution of the different spectral bands. In Level-1C  products, pixel coordinates refer to the upper left corner of the pixel. Level-1C products will additionally include Cloud Masks and ECMWF data (total column of ozone, total column of water vapour and mean sea level pressure). SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi/data-formats ",MSI,SENTINEL2,"S2A,S2B",L1,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L1,L1C,SAFE",OPTICAL,proprietary,SENTINEL2 Level-1C,2015-06-23T00:00:00Z,available,available,,,available,available,available,,available,,,available,available,available,,available,,available,
+S2_MSI_L2A,"The Level-2A product provides Bottom Of Atmosphere (BOA) reflectance images derived from the associated Level-1C products. Each Level-2A product is composed of 100x100 km2 tiles in cartographic geometry (UTM/WGS84 projection). SAFE formatted product, see https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi/data-formats ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,SAFE",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,available,available,,,available,available,available,,,,,available,available,available,available,available,,,
+S2_MSI_L2A_COG,"The Level-2A product provides Bottom Of Atmosphere (BOA) reflectance images derived from the associated Level-1C products. Each Level-2A product is composed of 100x100 km2 tiles in cartographic geometry (UTM/WGS84 projection). Product containing Cloud Optimized GeoTIFF images, without SAFE formatting. ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,COG",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,,,,,,,,available,,,,,,,,,,,
+S2_MSI_L2A_MAJA,"The level 2A products correct the data for atmospheric effects and detect the clouds and their shadows using MAJA. MAJA uses MUSCATE processing center at CNES, in the framework of THEIA land data center. Sentinel-2 level 1C data are downloaded from PEPS. The full description of the product format is available at https://theia.cnes.fr/atdistrib/documents/PSC-NT-411-0362-CNES_01_00_SENTINEL-2A_L2A_Products_Description.pdf ",MSI,SENTINEL2,"S2A,S2B",L2,"MSI,SENTINEL,SENTINEL2,S2,S2A,S2B,L2,L2A,MAJA",OPTICAL,proprietary,SENTINEL2 Level-2A,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+S2_MSI_L2B_MAJA_SNOW,The Theia snow product is derived from Sentinel-2 L2A images generated by Theia. It  indicates the snow presence or absence on the land surface every fifth day if there is no cloud. The product is distributed by Theia as a raster file (8 bits GeoTIFF) of 20 m resolution and a vector file (Shapefile polygons). More details about the snow products description are available at http://www.cesbio.ups-tlse.fr/multitemp/?page_id=10748#en ,MSI,SENTINEL2,"S2A,S2B",L2,"MSI,MAJA,SENTINEL,sentinel2,S2,S2A,S2B,L2,L2B,SNOW",OPTICAL,proprietary,SENTINEL2 snow product,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+S2_MSI_L2B_MAJA_WATER,A description of the Land Water Quality data distributed by Theia is available at https://theia.cnes.fr/atdistrib/documents/THEIA-ST-411-0477-CNES_01-03_Format_Specification_of_OBS2CO_WaterColor_Products.pdf ,MSI,SENTINEL2,"S2A,S2B",L2,"MSI,MAJA,SENTINEL,sentinel2,S2,S2A,S2B,L2,L2B,WATER",OPTICAL,proprietary,SENTINEL2 L2B-WATER,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+S2_MSI_L3A_WASP,"The Level-3A product provides a monthly synthesis of surface reflectances from Theia's L2A products. The synthesis is based on a weighted arithmetic mean of clear observations. The data processing is produced by WASP (Weighted Average Synthesis Processor), by MUSCATE data center at CNES, in the framework of THEIA data center. The full description of the product format is available at https://theia.cnes.fr/atdistrib/documents/THEIA-ST-411-0419-CNES_01-04_Format_Specification_of_MUSCATE_Level-3A_Products-signed.pdf ",MSI,SENTINEL2,"S2A,S2B",L3,"MSI,SENTINEL,sentinel2,S2,S2A,S2B,L3,L3A,WASP",OPTICAL,proprietary,SENTINEL2 Level-3A,2015-06-23T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+S3_EFR,,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,EFR",OPTICAL,proprietary,SENTINEL3 EFR,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_ERR,,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,ERR",OPTICAL,proprietary,SENTINEL3 ERR,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_LAN,LAN or SR_2_LAN___ (peps),SRAL,SENTINEL3,"S3A,S3B",L2,"SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,LAN",RADAR,proprietary,SENTINEL3 SRAL Level-2 LAN,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_OLCI_L2LFR,"The OLCI Level-2 Water Full Resolution (OL_2_WFR) products contain water and atmospheric geophysical products at Full resolution with a spatial sampling of approximately 300 m. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WFR,WFR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Full Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_OLCI_L2LRR,"The OLCI Level-2 Land Reduced Resolution (OL_2_LRR) products contain land and atmospheric geophysical products at Reduced resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-land ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2LRR,LRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Land Reduced Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_OLCI_L2WFR,"The OLCI Level-2 Water Full Resolution (OL_2_WRR) products contain water and atmospheric geophysical products at Full resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WRR,WRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Full Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,,available,,,
+S3_OLCI_L2WRR,"The OLCI Level-2 Water Reduced Resolution (OL_2_WRR) products contain water and atmospheric geophysical products at Reduced resolution with a spatial sampling of approximately 1.2 km. The products are assumed to be computed in Near Real Time (NRT) (i.e. delivered to users less than 3 hours after acquisition), in Non-Time Critical (NTC) (i.e. within 1 month after acquisition) or in re-processed NTC. Details at https://sentinel.esa.int/web/sentinel/user-guides/sentinel-3-olci/product-types/level-2-water ",OLCI,SENTINEL3,"S3A,S3B",L2,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WRR,WRR",OPTICAL,proprietary,SENTINEL3 OLCI Level-2 Water Reduced Resolution,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,,available,,,
+S3_RAC,Sentinel 3 OLCI products output during Radiometric Calibration mode ,OLCI,SENTINEL3,"S3A,S3B",L1,"OLCI,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,L2,RAC",OPTICAL,proprietary,SENTINEL3 RAC,2016-02-16T00:00:00Z,,,,,,,,,,,,,,,,available,,,
+S3_SLSTR_L1RBT,"SLSTR Level-1 observation mode products consisting of full resolution, geolocated, co-located nadir and along track view, Top of Atmosphere (TOA) brightness temperatures (in the case of thermal IR channels) or radiances (in the case of visible, NIR and SWIR channels) from all SLSTR channels, and quality flags, pixel classification information and meteorological annotations ",SLSTR,SENTINEL3,"S3A,S3B",L1,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L1,L1RBT,RBT",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SLSTR_L2AOD,"The Copernicus NRT S3 AOD processor quantifies the abundance of aerosol particles and monitors their global distribution and long-range transport, at the scale of 9.5 x 9.5 km2. All observations are made available in less than three hours from the SLSTR observation sensing time. It is only applicable during daytime. NOTE: The SLSTR L2 AOD product is generated by EUMETSAT in NRT only. An offline (NTC) AOD product is generated from SYN data by ESA, exploiting the synergy between the SLSTR and OLCI instruments. ",SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2AOD,AOD",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 AOD,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,,,,available,,,
+S3_SLSTR_L2FRP,"The SLSTR Level-2 FRP product is providing one measurement data file, FRP_in.nc, with Fire Radiative Power (FRP) values and associated parameters generated for each fire detected over land and projected on the SLSTR 1 km grid. The fire detection is based on a mixed thermal band, combining S7 radiometric measurements and, for pixels associated with a saturated value of S7 (i.e. above 311 K), F1 radiometric measurements. ",SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2FRP,FRP",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 FRP,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SLSTR_L2LST,The SLSTR Level-2 LST product provides land surface parameters generated on the wide 1 km measurement grid. It contains measurement file with Land Surface Temperature (LST) values with associated parameters (LST parameters are computed and provided for each pixel (re-gridded or orphan) included in the 1 km measurement grid) ,SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2LST,LST",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 LST,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SLSTR_L2WST,The SLSTR Level-2 WST product provides land surface parameters generated on the wide 1 km measurement grid. It contains measurement file with Water Surface Temperature (WST) values with associated parameters (WST parameters are computed and provided for each pixel (re-gridded or orphan) included in the 1 km measurement grid) ,SLSTR,SENTINEL3,"S3A,S3B",L2,"SLSTR,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,L2WST,WST",ATMOSPHERIC,proprietary,SENTINEL3 SLSTR Level-2 WST,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,,available,,,
+S3_SRA,,SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SRA_A,"A Level 1A SRAL product contains one ""measurement data file"" containing the L1A measurements parameters: ECHO_SAR_Ku: L1A Tracking measurements (sorted and calibrated) in SAR mode - Ku-band (80-Hz) ECHO_PLRM: L1A Tracking measurements (sorted and calibrated) in pseudo-LRM mode - Ku and C bands (80-Hz) ",SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1 SRA_A,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SRA_BS,"A Level 1B-S SRAL product contains one ""measurement data file"" containing the L1b measurements parameters: ECHO_SAR_Ku : L1b Tracking measurements in SAR mode - Ku band (20-Hz) as defined in the L1b MEAS product               completed with SAR expert information ECHO_PLRM : L1b Tracking measurements in pseudo-LRM mode - Ku and C bands (20-Hz) as defined in the L1b             MEAS product ",SRAL,SENTINEL3,"S3A,S3B",L1,"SRA,SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L1",RADAR,proprietary,SENTINEL3 SRAL Level-1 SRA_BS,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SY_AOD,"The Level-2 SYN AOD product (SY_2_AOD) is produced by a dedicated processor including the whole SYN L1 processing module and a global synergy level 2 processing module retrieving, over land and sea, aerosol optical thickness. The resolution of this product is wider than classic S3 products, as the dataset are provided on a 4.5 km² resolution ",SYNERGY,SENTINEL3,"S3A,S3B",L2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,AOD","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 AOD,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,,available,,,
+S3_SY_SYN,"The Level-2 SYN product (SY_2_SYN) is produced by the Synergy Level-1/2 SDR software and contains surface reflectance and aerosol parameters over land. All measurement datasets are provided on the OLCI image grid, similar to the one included in the OLCI L1b product. Some sub-sampled annotations and atmospheric datasets are provided on the OLCI tie-points grid. Several associated variables are also provided in annotation data files. ",SYNERGY,SENTINEL3,"S3A,S3B",L2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,SYN","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 SYN,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SY_V10,"The Level-2 VG1 and V10 SYN products (SY_2_VG1 and SY_2_V10 respectively) are produced by the SYNERGY Level-2 processor and contain 1 km VEGETATION-like product, 1 and 10 days synthesis surface reflectances and NDVI. The product grid and the four spectral bands are similar to the SYN Level-2 VGP product. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2W,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,V10","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 V10,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SY_VG1,"The Level-2 VG1 and V10 SYN products (SY_2_VG1 and SY_2_V10 respectively) are produced by the SYNERGY Level-2 processor and contain 1 km VEGETATION-like product, 1 and 10 days synthesis surface reflectances and NDVI. The product grid and the four spectral bands are similar to the SYN Level-2 VGP product. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,VG1","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 VG1,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_SY_VGP,"The Level-2 VGP SYN product (SY_2_VGP) is produced by the Global Synergy Level-1/2 software and contains 1 km VEGETATION-like product TOA reflectances. The ""1 km VEGETATION-like product"" label means that measurements are provided on a regular latitude-longitude grid, with an equatorial sampling distance of approximately 1 km. This product is restricted in longitude, including only filled ones. ",SYNERGY,SENTINEL3,"S3A,S3B",LEVEL-2,"SYNERGY,SY,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,VGP","OPTICAL,RADAR",proprietary,SENTINEL3 SYNERGY Level-2 VGP,2016-02-16T00:00:00Z,,,,,available,available,,,,,,available,available,,,available,,,
+S3_WAT,,SRAL,SENTINEL3,"S3A,S3B",L2,"SRAL,SENTINEL,SENTINEL3,S3,S3A,S3B,L2,WAT",RADAR,proprietary,SENTINEL3 SRAL Level-2 WAT,2016-02-16T00:00:00Z,,,,,available,available,,,,,,,available,,,available,,,
+S5P_L1B_IR_SIR,"Solar irradiance spectra for the SWIR bands (band 7 and band 8). TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,IR,SIR,SWIR,Irradiances",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Irradiances for the SWIR bands,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,,
+S5P_L1B_IR_UVN,"Solar irradiance spectra for the UVN bands (band 1 through band 6). TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,IR,UVN,Irradiances",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Irradiances for the UVN bands,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,,
+S5P_L1B_RA_BD1,"Sentinel-5 Precursor Level 1B Radiances for spectral band 1. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD1,BAND1,B01",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 1,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD2,"Sentinel-5 Precursor Level 1B Radiances for spectral band 2. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD2,BAND2,B02",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 2,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD3,"Sentinel-5 Precursor Level 1B Radiances for spectral band 3. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD3,BAND3,B03",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 3,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD4,"Sentinel-5 Precursor Level 1B Radiances for spectral band 4. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD4,BAND4,B04",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 4,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD5,"Sentinel-5 Precursor Level 1B Radiances for spectral band 5. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD5,BAND5,B05",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 5,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD6,"Sentinel-5 Precursor Level 1B Radiances for spectral band 6. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD6,BAND6,B06",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 6,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD7,"Sentinel-5 Precursor Level 1B Radiances for spectral band 7. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD7,BAND7,B07",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 7,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L1B_RA_BD8,"Sentinel-5 Precursor Level 1B Radiances for spectral band 8. TROPOMI utilises a single telescope to form an image of the target area onto a rectangular slit that acts as the entrance slit of the spectrometer system. There are four different spectrometers, each with its own optics and detector: mediumwave ultraviolet (UV), longwave ultraviolet combined with visible (UVIS), near infrared (NIR), and shortwave infrared (SWIR). The spectrometers for UV, UVIS and NIR are jointly referred to as UVN. Radiation for the SWIR spectrometer is transferred by an optical relay part in the UVN system from the telescope to an interface position (the pupil stop) for the SWIR spectrometer. This is done because of the more stringent thermal requirements on the SWIR part of the instrument. Each of the detectors is divided in two halves, which yields a total of eight spectral bands. ",TROPOMI,SENTINEL5P,S5P,L1B,"SENTINEL,SENTINEL5P,S5P,L1,L1B,TROPOMI,RA,Radiances,BD8,BAND8,B08",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 1B Radiances for spectral band 8,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_AER_AI,"TROPOMI aerosol index is referred to as the Ultraviolet Aerosol Index (UVAI). The relatively simple calculation of the Aerosol Index is based on wavelength dependent changes in Rayleigh scattering in the UV spectral range where ozone absorption is very small. UVAI can also be calculated in the presence of clouds so that daily, global coverage is possible. This is ideal for tracking the evolution of episodic aerosol plumes from dust outbreaks, volcanic ash, and biomass burning. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,AER,AI,Ultraviolet,Aerosol,Index",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ultraviolet Aerosol Index,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_AER_LH,"The TROPOMI Aerosol Layer Height product focuses on retrieval of vertically localised aerosol layers in the free troposphere, such as desert dust, biomass burning aerosol, or volcanic ash plumes. The height of such layers is retrieved for cloud-free conditions. Height information for aerosols in the free troposphere is particularly important for aviation safety. Scientific applications include radiative forcing studies, long-range transport modelling and studies of cloud formation processes. Aerosol height information also helps to interpret the UV Aerosol Index (UVAI) in terms of aerosol absorption as the index is strongly height-dependent. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,AER,LH,Aerosol,Layer,Height",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Aerosol Layer Height,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_CH4,"Methane (CH4) is, after carbon dioxide (CO2), the most important contributor to the anthropogenically enhanced greenhouse effect. Roughly three-quarters of methane emissions are anthropogenic and as such it is important to continue the record of satellite-based measurements. TROPOMI aims at providing CH4 column concentrations with high sensitivity to the Earth's surface, good spatio/temporal coverage, and sufficient accuracy to facilitate inverse modelling of sources and sinks. The output product consists of the retrieved methane column and a row vector referred to as the column averaging kernel A. The column averaging kernel describes how the retrieved column relates to the true profile and should be used in validation exercises (when possible) or use of the product in source/sink inverse modelling. The output product also contains altitude levels of the layer interfaces to which the column averaging kernel corresponds. Additional output for Level-2 data products: viewing geometry, precision of retrieved methane, residuals of the fit, quality flags (cloudiness, terrain roughness etc.) and retrieved albedo and aerosol properties. The latter properties are required for a posteriori filtering and for estimation of total retrieval error. The Sentinel-5 Precursor mission flies in loose formation (about 3.5 - 5 minutes behind) with the S-NPP (SUOMI-National Polar-orbiting Partnership) mission to use VIIRS (Visible Infrared Imaging Radiometer Suite) cloud information to select cloud free TROPOMI pixels for high quality methane retrieval. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CH4,Methane",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Methane,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_CLOUD,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves operationally the most important quantities for cloud correction of satellite trace gas retrievals: cloud fraction, cloud optical thickness (albedo), and cloud-top pressure (height). Cloud parameters from TROPOMI are not only used for enhancing the accuracy of trace gas retrievals, but also to extend the satellite data record of cloud information derived from oxygen A-band measurements initiated with GOME. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CLOUD",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Cloud,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_CO,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves the CO global abundance exploiting clear-sky and cloudy-sky Earth radiance measurements in the 2.3 µm spectral range of the shortwave infrared (SWIR) part of the solar spectrum. TROPOMI clear sky observations provide CO total columns with sensitivity to the tropospheric boundary layer. For cloudy atmospheres, the column sensitivity changes according to the light path. The TROPOMI CO retrieval uses the same method employed by SCIAMACHY. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,CO,Carbon,Monoxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Carbon Monoxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_HCHO,"Formaldehyde is an intermediate gas in almost all oxidation chains of Non-Methane Volatile Organic Compounds (NMVOC), leading eventually to CO2. NMVOCs are, together with NOx, CO and CH4, among the most important precursors of tropospheric O3. The major HCHO source in the remote atmosphere is CH4 oxidation. Over the continents, the oxidation of higher NMVOCs emitted from vegetation, fires, traffic and industrial sources results in important and localised enhancements of the HCHO levels. In addition to the main product results, such as HCHO slant column, vertical column and air mass factor, the level 2 data files contain several additional parameters and diagnostic information. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,HCHO,Formaldehyde",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Formaldehyde,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_NO2,"The TROPOMI instrument, single payload onboard Sentinel-5 Precursor, retrieves operationally tropospheric and stratospheric NO2 column products. The TROPOMI NO2 data products pose an improvement over previous NO2 data sets, particularly in their unprecedented spatial resolution, but also in the separation of the stratospheric and tropospheric contributions of the retrieved slant columns, and in the calculation of the air-mass factors used to convert slant to total columns. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NO2,Nitrogen,Dioxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Nitrogen Dioxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_NP_BD3,"S5P-NPP Cloud for spectral band 3. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD3,B03,BAND3",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 3,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_NP_BD6,"S5P-NPP Cloud for spectral band 6. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD6,B06,BAND6",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 6,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_NP_BD7,"S5P-NPP Cloud for spectral band 7. The S5P level 2 methane product is dependent on having information on cloud occurrence at spatial resolution finer than that achievable from TROPOMI itself. This information is also useful for other purposes, including assessing the influence of cloud on other L2 products and issues related to spatial co-registration. A level 2 auxiliary product was therefore developed to describe cloud in the TROPOMI field of view (FOV), using co-located observations of VIIRS (Visible Infra-red Imaging Radiometer Suite) on the U.S. S-NPP (Suomi - National Polar-orbiting Partnership). S5P flies in a so-called loose formation with the S-NPP with a temporal separation between them of less than 5 minutes. The main information contained in the S5P-NPP product is: 1. A statistical summary for each S5P FOV of the NPP-VIIRS L2 Cloud Mask (VCM). 2. The mean and standard deviation of the sun-normalised radiance in a number of VIIRS moderate resolution bands. This information is provided for three S5P spectral bands (to account for differences in spatial sampling). ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,NP,NPP,Cloud,BD7,B07,BAND7",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 NPP Cloud for band 7,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_O3,"Ozone (O3) is of crucial importance for the equilibrium of the Earth's atmosphere. In the stratosphere, the ozone layer shields the biosphere from dangerous solar ultraviolet radiation. In the troposphere, it acts as an efficient cleansing agent, but at high concentration it also becomes harmful to the health of humans, animals, and vegetation. Ozone is also an important greenhouse-gas contributor to ongoing climate change. These products are provided in NetCDF-CF format and contain total ozone, ozone temperature, and error information including averaging kernels. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,Ozone",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ozone,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_O3_PR,"Retrieved ozone profiles are used to monitor the evolution of stratospheric and tropospheric ozone. Such monitoring is important as the ozone layer protects life on Earth against harmful UV radiation. The ozone layer is recovering from depletion due to manmade Chlorofluorocarbons (CFCs). Tropospheric ozone is toxic and it plays an important role in tropospheric chemistry. Also, ozone is a greenhouse gas and is therefore also relevant for climate change. The main parameters in the file are the retrieved ozone profile at 33 levels and the retrieved sub-columns of ozone in 6 layers. In addition, the total ozone column and tropospheric ozone columns are provided. For the ozone profile, the precision and smoothing errors, the a-priori profile and the averaging kernel are also provided. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,PR,Ozone,Profile",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Ozone Profile,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+S5P_L2_O3_TCL,"Ozone in the tropical troposphere plays various important roles. The intense UV radiation and high humidity in the tropics stimulate the formation of the hydroxyl radical (OH) by the photolysis of ozone. OH is the most important oxidant in the troposphere because it reacts with virtually all trace gases, such as CO, CH4 and other hydrocarbons. The tropics are also characterized by large emissions of nitrogen oxides (NOx), carbon monoxide (CO) and hydrocarbons, both from natural and anthropogenic sources. Ozone that is formed over regions where large amounts of these ozone precursors are emitted, can be transported over great distances and affects areas far from the source. The TROPOMI tropospheric ozone product is a level-2c product that represents three day averaged tropospheric ozone columns on a 0.5° by 1° latitude-longitude grid for the tropical region between 20°N and 20°S. The TROPOMI tropospheric ozone column product uses the TROPOMI Level-2 total OZONE and CLOUD products as input. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,O3,TCL,Tropospheric,Ozone",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Tropospheric Ozone,2017-10-13T00:00:00Z,,,,,,available,,,,,,available,,,,,,,
+S5P_L2_SO2,"Sulphur dioxide (SO2) enters the Earth's atmosphere through both natural (~30%) and anthropogenic processes (~70%). It plays a role in chemistry on a local and global scale and its impact ranges from short term pollution to effects on climate. Beside the total column of SO2, enhanced levels of SO2 are flagged within the products. The recognition of enhanced SO2 values is essential in order to detect and monitor volcanic eruptions and anthropogenic pollution sources. Volcanic SO2 emissions may also pose a threat to aviation, along with volcanic ash. ",TROPOMI,SENTINEL5P,S5P,L2,"SENTINEL,SENTINEL5P,S5P,L2,TROPOMI,SO2,Sulphur,Dioxide",ATMOSPHERIC,proprietary,Sentinel-5 Precursor Level 2 Sulphur Dioxide,2017-10-13T00:00:00Z,,,,,available,available,,,,,,available,available,,,,,,
+SPOT5_SPIRIT,SPOT 5 stereoscopic survey of Polar Ice. ,,SPOT5,SPOT5,L1A,"SPOT,SPOT5,L1A",OPTICAL,proprietary,Spot 5 SPIRIT,2002-05-04T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+SPOT_SWH,The Spot World Heritage (SWH) programme objective is the free availability for non-commercial use of orthorectified products derived from multispectral images of more than 5 years old from the Spot 1-5 satellites family. More informations on https://www.theia-land.fr/en/product/spot-world-heritage/ ,,SPOT1-5,SPOT1-5,L1C,"SPOT,SPOT1,SPOT2,SPOT3,SPOT4,SPOT5,L1C",OPTICAL,proprietary,Spot World Heritage,1986-02-22T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+SPOT_SWH_OLD,Spot world heritage Old format. ,,SPOT1-5,SPOT1-5,L1C,"SPOT,SPOT1,SPOT2,SPOT3,SPOT4,SPOT5,L1C",OPTICAL,proprietary,Spot World Heritage,1986-02-22T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+TIGGE_CF_SFC,TIGGE (THORPEX Interactive Grand Global Ensemble) Surface Control forecast from ECMWF ,,TIGGE,TIGGE,,"THORPEX,TIGGE,CF,SFC,ECMWF",ATMOSPHERIC,proprietary,TIGGE ECMWF Surface Control forecast,2003-01-01T00:00:00Z,,,,,,,,,,available,,,,,,,,,
+VENUS_L1C,A light description of Venus L1 data is available at http://www.cesbio.ups-tlse.fr/multitemp/?page_id=12984 ,,VENUS,VENUS,L1C,"VENUS,L1,L1C",OPTICAL,proprietary,Venus Level1-C,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+VENUS_L2A_MAJA,"Level2 products provide surface reflectances after atmospheric correction, along with masks of clouds and their shadows. Data is processed by MAJA (before called MACCS) for THEIA land data center. ",,VENUS,VENUS,L2A,"VENUS,L2,L2A",OPTICAL,proprietary,Venus Level2-A,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,,available,,
+VENUS_L3A_MAJA,,,VENUS,VENUS,L3A,"VENUS,L3,L3A",OPTICAL,proprietary,Venus Level3-A,2017-08-02T00:00:00Z,,,,,,,,,,,,,,,,,available,,
```

### Comparing `eodag-2.9.1/docs/_static/progress_1.png` & `eodag-2.9.2/docs/_static/progress_1.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/progress_1_none.png` & `eodag-2.9.2/docs/_static/progress_1_none.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/progress_2.png` & `eodag-2.9.2/docs/_static/progress_2.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/progress_2_none.png` & `eodag-2.9.2/docs/_static/progress_2_none.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/stac_browser_example.png` & `eodag-2.9.2/docs/_static/stac_browser_example.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/_static/stac_browser_example_600.png` & `eodag-2.9.2/docs/_static/stac_browser_example_600.png`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/add_provider.rst` & `eodag-2.9.2/docs/add_provider.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/api_reference/call_graphs.rst` & `eodag-2.9.2/docs/api_reference/call_graphs.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/api_reference/core.rst` & `eodag-2.9.2/docs/api_reference/core.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/api_reference/searchresult.rst` & `eodag-2.9.2/docs/api_reference/searchresult.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/api_user_guide.rst` & `eodag-2.9.2/docs/api_user_guide.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/cli_user_guide.rst` & `eodag-2.9.2/docs/cli_user_guide.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/conf.py` & `eodag-2.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/configure.rst` & `eodag-2.9.2/docs/getting_started_guide/configure.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/install.rst` & `eodag-2.9.2/docs/getting_started_guide/install.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/overview.rst` & `eodag-2.9.2/docs/getting_started_guide/overview.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/product_storage_status.rst` & `eodag-2.9.2/docs/getting_started_guide/product_storage_status.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/product_types.rst` & `eodag-2.9.2/docs/getting_started_guide/product_types.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/getting_started_guide/providers.rst` & `eodag-2.9.2/docs/getting_started_guide/providers.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,12 +21,13 @@
 * `earth_search_gcs <https://cloud.google.com/storage/docs/public-datasets>`_: Element84 Earth Search and Google Cloud Storage download
 * `ecmwf <https://www.ecmwf.int/>`_: European Centre for Medium-Range Weather Forecasts
 * `cop_ads <https://ads.atmosphere.copernicus.eu>`_: Copernicus Atmosphere Data Store
 * `cop_cds <https://cds.climate.copernicus.eu>`_: Copernicus Climate Data Store
 * `sara <https://copernicus.nci.org.au>`_: Sentinel Australasia Regional Acces
 * `meteoblue <https://content.meteoblue.com/en/business-solutions/weather-apis/dataset-api>`_: Meteoblue forecast
 * `cop_dataspace <https://dataspace.copernicus.eu/>`_: Copernicus Data Space
+* `planetary_computer <https://planetarycomputer.microsoft.com/>`_: Microsoft Planetary Computer
 
 Providers available through an external plugin:
 
 * `SciHub / Copernicus Open Access Hub <https://scihub.copernicus.eu/userguide/WebHome>`_: available using
   `eodag-sentinelsat <https://github.com/CS-SI/eodag-sentinelsat>`_
```

### Comparing `eodag-2.9.1/docs/getting_started_guide/register.rst` & `eodag-2.9.2/docs/getting_started_guide/register.rst`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
 * `meteoblue`: eodag uses `dataset API <https://content.meteoblue.com/en/business-solutions/weather-apis/dataset-api>`_
   which requires the access level `Access Gold <https://content.meteoblue.com/en/business-solutions/weather-apis/pricing>`_.
   Contact `support@meteoblue.com <mailto:support@meteoblue.com>`_ to apply for a free API key trial.
 
 * `cop_dataspace`: create an account `here <https://identity.dataspace.copernicus.eu/auth/realms/CDSE/protocol/openid-connect/auth?client_id=cdse-public&redirect_uri=https%3A%2F%2Fdataspace.copernicus.eu%2Fbrowser%2F&response_type=code&scope=openid>`__
 
+* `planetary_computer`: most datasets are anonymously accessible, but a subscription key may be needed to increase `rate limits and access private datasets <https://planetarycomputer.microsoft.com/docs/concepts/sas/#rate-limits-and-access-restrictions>`_.
+  Create an account `here <https://planetarycomputer.microsoft.com/account/request>`__, then view your keys by signing in with your Microsoft account `here <https://planetarycomputer.developer.azure-api.net/>`__.
+
 * `aws_eos`: you need credentials for both EOS (search) and AWS (download):
 
   * Create an account on `EOS <https://auth.eos.com>`__
 
   * Get your EOS api key from `here <https://console.eos.com>`__
 
   * Create an account on `AWS <https://aws.amazon.com/>`__
```

### Comparing `eodag-2.9.1/docs/getting_started_guide/side_projects.rst` & `eodag-2.9.2/docs/getting_started_guide/side_projects.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/index.rst` & `eodag-2.9.2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
       `earth_search_gcs <https://cloud.google.com/storage/docs/public-datasets>`_,
       `usgs <https://earthexplorer.usgs.gov/>`_, `theia <https://theia.cnes.fr/atdistrib/rocket/>`_,
       `peps <https://peps.cnes.fr/rocket/#/home>`_, `aws_eos <https://eos.com/>`_, `creodias <https://creodias.eu/>`_,
       `mundi <https://mundiwebservices.com/>`_, `onda <https://www.onda-dias.eu/cms/>`_, `ecmwf <https://www.ecmwf.int/>`_,
       `cop_ads <https://ads.atmosphere.copernicus.eu>`_, `cop_cds <https://cds.climate.copernicus.eu>`_,
       `sara <https://copernicus.nci.org.au>`_,
       `meteoblue <https://content.meteoblue.com/en/business-solutions/weather-apis/dataset-api>`_,
-      `cop_dataspace <https://dataspace.copernicus.eu/>`_
+      `cop_dataspace <https://dataspace.copernicus.eu/>`_,
+      `planetary_computer <https://planetarycomputer.microsoft.com/>`_
 
 EODAG has the following primary features:
 
 * Search and download Earth Observation products from different providers with **a unified API**
 * It is both a `Command Line Tool <cli_user_guide.rst>`_ and a `Python Package <api_user_guide.rst>`_
 * It supports `STAC and Static STAC <notebooks/tutos/tuto_stac_client.ipynb>`_ catalogs
 * It can run as a `STAC API REST server <stac_rest.rst>`_ to give access to a provider's catalog
```

### Comparing `eodag-2.9.1/docs/make.bat` & `eodag-2.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/1_overview.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/1_overview.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/2_providers_products_available.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/2_providers_products_available.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994088963394062%*

 * *Differences: {"'cells'": "{1: {'execution_count': 23}, 4: {'execution_count': 24, 'outputs': {0: {'data': "*

 * *            '{\'text/plain\': {insert: [(14, " \'planetary_computer\',\\n")]}}, '*

 * *            "'execution_count': 24}}}, 5: {'execution_count': 25, 'outputs': {0: {'text': ['eodag "*

 * *            "has 19 providers already configured.\\n']}}}, 7: {'execution_count': 26}, 11: "*

 * *            "{'execution_count': 27}, 12: {'execution_count': 28}, 14: {'execution_count': 29}, "*

 * *            "15: {'execution_count': 30}, 16 […]*

```diff
@@ -5,15 +5,15 @@
             "metadata": {},
             "source": [
                 "# Providers and products"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from eodag import EODataAccessGateway\n",
                 "dag = EODataAccessGateway()"
             ]
         },
@@ -29,15 +29,15 @@
             "metadata": {},
             "source": [
                 "The method [available_providers()](../../api_reference/core.rst#eodag.api.core.EODataAccessGateway.available_providers) returns a list of the pre-configured providers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['astraea_eod',\n",
                             " 'aws_eos',\n",
@@ -49,40 +49,41 @@
                             " 'earth_search_cog',\n",
                             " 'earth_search_gcs',\n",
                             " 'ecmwf',\n",
                             " 'meteoblue',\n",
                             " 'mundi',\n",
                             " 'onda',\n",
                             " 'peps',\n",
+                            " 'planetary_computer',\n",
                             " 'sara',\n",
                             " 'theia',\n",
                             " 'usgs',\n",
                             " 'usgs_satapi_aws']"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "available_providers = dag.available_providers()\n",
                 "available_providers"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "eodag has 18 providers already configured.\n"
+                        "eodag has 19 providers already configured.\n"
                     ]
                 }
             ],
             "source": [
                 "print(f\"eodag has {len(available_providers)} providers already configured.\")"
             ]
         },
@@ -91,15 +92,15 @@
             "metadata": {},
             "source": [
                 "It can take a product type as an argument and will return the providers known to `eodag` that offer this product."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 26,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['astraea_eod',\n",
                             " 'aws_eos',\n",
@@ -148,15 +149,15 @@
             "metadata": {},
             "source": [
                 "The method [list_product_types()](../../api_reference/core.rst#eodag.api.core.EODataAccessGateway.list_product_types) returns a dictionary that represents `eodag`'s internal product type catalog if used with `fetch_providers=False`. It will fetch providers for new product types and return an extended list if used with `fetch_providers=True` (default behavior)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "EODAG has 103 product types stored in its internal catalog.\n"
@@ -166,15 +167,15 @@
             "source": [
                 "internal_catalog = dag.list_product_types(fetch_providers=False)\n",
                 "print(f\"EODAG has {len(internal_catalog)} product types stored in its internal catalog.\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 28,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "EODAG has 126 product types stored in its extended catalog, after having fetched providers.\n"
@@ -191,15 +192,15 @@
             "metadata": {},
             "source": [
                 "When providers are fetched for new product types, `eodag`'s product types configuration is updated in `EODataAccessGateway` instance. Extended product types list is then returned independantly of `fetch_providers` option in [list_product_types()](../../api_reference/core.rst#eodag.api.core.EODataAccessGateway.list_product_types):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 29,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "list_product_types() keeps returning 126 product types.\n"
@@ -209,15 +210,15 @@
             "source": [
                 "called_again_catalog = dag.list_product_types(fetch_providers=False)\n",
                 "print(f\"list_product_types() keeps returning {len(called_again_catalog)} product types.\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 30,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'ID': 'CAMS_EAC4',\n",
                             " 'abstract': 'CAMS (Copernicus Atmosphere Monitoring Service) ECMWF Atmospheric Composition Reanalysis 4\\nfrom Copernicus ADS\\n',\n",
@@ -239,15 +240,15 @@
             ],
             "source": [
                 "internal_catalog[0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['CAMS_EAC4',\n",
                             " 'CAMS_GACF_AOT',\n",
@@ -369,15 +370,15 @@
             "metadata": {},
             "source": [
                 "The method can take a provider name as an argument and will return the product types known to `eodag` that are offered by this provider."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 32,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['S1_SAR_GRD', 'S1_SAR_OCN', 'S1_SAR_SLC', 'S2_MSI_L1C', 'S2_MSI_L2A']"
                         ]
@@ -404,15 +405,15 @@
             "metadata": {},
             "source": [
                 "These two methods can be combined to find which product type is the most common in `eodag`'s catalog among all the providers."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 33,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "The most common product type is 'S2_MSI_L1C' with 11 providers offering it.\n"
@@ -434,15 +435,15 @@
             "metadata": {},
             "source": [
                 "These can be also used to find out which provider (as configured by `eodag`) offers the hights number of different product types."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 34,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "The provider with the largest number of product types is 'creodias' with 61.\n"
```

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/3_configuration.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/3_configuration.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999974300986842%*

 * *Differences: {"'cells'": '{4: {\'outputs\': {0: {\'data\': {\'text/plain\': {insert: [(14, " '*

 * *            '\'planetary_computer\',\\n")]}}}}}}'}*

```diff
@@ -48,14 +48,15 @@
                             " 'earth_search_cog',\n",
                             " 'earth_search_gcs',\n",
                             " 'ecmwf',\n",
                             " 'meteoblue',\n",
                             " 'mundi',\n",
                             " 'onda',\n",
                             " 'peps',\n",
+                            " 'planetary_computer',\n",
                             " 'sara',\n",
                             " 'theia',\n",
                             " 'usgs',\n",
                             " 'usgs_satapi_aws']"
                         ]
                     },
                     "execution_count": 2,
```

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/4_search.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/4_search.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/5_serialize_deserialize.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/5_serialize_deserialize.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/6_crunch.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/6_crunch.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/7_download.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/7_download.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/8_post_process.ipynb` & `eodag-2.9.2/docs/notebooks/api_user_guide/8_post_process.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/data/crunch_search_results.geojson` & `eodag-2.9.2/docs/notebooks/api_user_guide/data/crunch_search_results.geojson`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/api_user_guide/data/download_search_results.geojson` & `eodag-2.9.2/docs/notebooks/api_user_guide/data/download_search_results.geojson`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/intro_notebooks.ipynb` & `eodag-2.9.2/docs/notebooks/intro_notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qpj` & `eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.qpj`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shp` & `eodag-2.9.2/docs/notebooks/tutos/auxdata/Gulf_of_Trieste_seamask_UTM33.shp`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/auxdata/sentinel2_tiling_grid_centroids.zip` & `eodag-2.9.2/docs/notebooks/tutos/auxdata/sentinel2_tiling_grid_centroids.zip`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_burnt_areas_snappy.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_burnt_areas_snappy.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_cds.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_cds.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_cop_dem.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_cop_dem.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_ecmwf.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_ecmwf.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_meteoblue.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_meteoblue.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_search_location_tile.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_search_location_tile.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_ship_detection.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_ship_detection.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/notebooks/tutos/tuto_stac_client.ipynb` & `eodag-2.9.2/docs/notebooks/tutos/tuto_stac_client.ipynb`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/plugins.rst` & `eodag-2.9.2/docs/plugins.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,51 +25,53 @@
    plugins_reference/crunch
    plugins_reference/auth
    plugins_reference/download
    plugins_reference/api
 
 The providers are implemented with a triplet of *Search/Authentication/Download* plugins or with an *Api* plugin:
 
-+------------------+-----------------------+--------------------------+----------------+
-| Provider         | Search                | Authentication           | Download       |
-+==================+=======================+==========================+================+
-| aws_eos          | PostJsonSearch        | AwsAuth                  | AwsDownload    |
-+------------------+-----------------------+--------------------------+----------------+
-| theia            | QueryStringSearch     | TokenAuth                | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| peps             | QueryStringSearch     | GenericAuth              | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| creodias         | ODataV4Search         | KeycloakOIDCPasswordAuth | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| mundi            | QueryStringSearch     | HTTPHeaderAuth           | S3RestDownload |
-+------------------+-----------------------+--------------------------+----------------+
-| onda             | ODataV4Search         | GenericAuth              | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| astraea_eod      | StacSearch            | AwsAuth                  | AwsDownload    |
-+------------------+-----------------------+--------------------------+----------------+
-| usgs_satapi_aws  | StacSearch            | AwsAuth                  | AwsDownload    |
-+------------------+-----------------------+--------------------------+----------------+
-| earth_search     | StacSearch            | AwsAuth                  | AwsDownload    |
-+------------------+-----------------------+--------------------------+----------------+
-| earth_search_cog | StacSearch            | None                     | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| earth_search_gcs | StacSearch            | AwsAuth                  | AwsDownload    |
-+------------------+-----------------------+--------------------------+----------------+
-| usgs             | UsgsApi               | UsgsApi                  | UsgsApi        |
-+------------------+-----------------------+--------------------------+----------------+
-| ecmwf            | EcmwfApi              | EcmwfApi                 | EcmwfApi       |
-+------------------+-----------------------+--------------------------+----------------+
-| cop_ads          | CdsApi                | CdsApi                   | CdsApi         |
-+------------------+-----------------------+--------------------------+----------------+
-| cop_cds          | CdsApi                | CdsApi                   | CdsApi         |
-+------------------+-----------------------+--------------------------+----------------+
-| meteoblue        | BuildPostSearchResult | HttpQueryStringAuth      | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
-| cop_dataspace    | ODataV4Search         | KeycloakOIDCPasswordAuth | HTTPDownload   |
-+------------------+-----------------------+--------------------------+----------------+
++--------------------+-----------------------+--------------------------+----------------+
+| Provider           | Search                | Authentication           | Download       |
++====================+=======================+==========================+================+
+| aws_eos            | PostJsonSearch        | AwsAuth                  | AwsDownload    |
++--------------------+-----------------------+--------------------------+----------------+
+| theia              | QueryStringSearch     | TokenAuth                | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| peps               | QueryStringSearch     | GenericAuth              | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| creodias           | ODataV4Search         | KeycloakOIDCPasswordAuth | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| mundi              | QueryStringSearch     | HTTPHeaderAuth           | S3RestDownload |
++--------------------+-----------------------+--------------------------+----------------+
+| onda               | ODataV4Search         | GenericAuth              | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| astraea_eod        | StacSearch            | AwsAuth                  | AwsDownload    |
++--------------------+-----------------------+--------------------------+----------------+
+| usgs_satapi_aws    | StacSearch            | AwsAuth                  | AwsDownload    |
++--------------------+-----------------------+--------------------------+----------------+
+| earth_search       | StacSearch            | AwsAuth                  | AwsDownload    |
++--------------------+-----------------------+--------------------------+----------------+
+| earth_search_cog   | StacSearch            | None                     | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| earth_search_gcs   | StacSearch            | AwsAuth                  | AwsDownload    |
++--------------------+-----------------------+--------------------------+----------------+
+| usgs               | UsgsApi               | UsgsApi                  | UsgsApi        |
++--------------------+-----------------------+--------------------------+----------------+
+| ecmwf              | EcmwfApi              | EcmwfApi                 | EcmwfApi       |
++--------------------+-----------------------+--------------------------+----------------+
+| cop_ads            | CdsApi                | CdsApi                   | CdsApi         |
++--------------------+-----------------------+--------------------------+----------------+
+| cop_cds            | CdsApi                | CdsApi                   | CdsApi         |
++--------------------+-----------------------+--------------------------+----------------+
+| meteoblue          | BuildPostSearchResult | HttpQueryStringAuth      | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| cop_dataspace      | ODataV4Search         | KeycloakOIDCPasswordAuth | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
+| planetary_computer | StacSearch            | SASAuth                  | HTTPDownload   |
++--------------------+-----------------------+--------------------------+----------------+
 
 .. _creating_plugins:
 
 Creating Plugins
 ^^^^^^^^^^^^^^^^
 
 EODAG plugins can be separated from the core eodag package. They live in your Python site-packages as standalone Python
```

### Comparing `eodag-2.9.1/docs/plugins_reference/auth.rst` & `eodag-2.9.2/docs/plugins_reference/auth.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/plugins_reference/crunch.rst` & `eodag-2.9.2/docs/plugins_reference/crunch.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/plugins_reference/download.rst` & `eodag-2.9.2/docs/plugins_reference/download.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/plugins_reference/search.rst` & `eodag-2.9.2/docs/plugins_reference/search.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/stac.rst` & `eodag-2.9.2/docs/stac.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/stac_rest.rst` & `eodag-2.9.2/docs/stac_rest.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/docs/tutos.rst` & `eodag-2.9.2/docs/tutos.rst`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/__init__.py` & `eodag-2.9.2/eodag/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/__init__.py` & `eodag-2.9.2/eodag/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/core.py` & `eodag-2.9.2/eodag/api/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
 import os
 import re
 import shutil
-from copy import deepcopy
 from operator import itemgetter
 
 import geojson
 import pkg_resources
 import yaml.parser
 from pkg_resources import resource_filename
 from whoosh import analysis, fields
 from whoosh.fields import Schema
 from whoosh.index import create_in, exists_in, open_dir
 from whoosh.qparser import QueryParser
 
-from eodag.api.product.metadata_mapping import mtd_cfg_as_jsonpath
+from eodag.api.product.metadata_mapping import mtd_cfg_as_conversion_and_querypath
 from eodag.api.search_result import SearchResult
 from eodag.config import (
     SimpleYamlProxyConfig,
     get_ext_product_types_conf,
     load_default_config,
     load_stac_provider_config,
     load_yml_config,
@@ -46,17 +45,19 @@
 )
 from eodag.plugins.download.base import DEFAULT_DOWNLOAD_TIMEOUT, DEFAULT_DOWNLOAD_WAIT
 from eodag.plugins.manager import PluginManager
 from eodag.utils import (
     GENERIC_PRODUCT_TYPE,
     MockResponse,
     _deprecated,
+    deepcopy,
     get_geometry_from_various,
     makedirs,
     obj_md5sum,
+    string_to_jsonpath,
     uri_to_path,
 )
 from eodag.utils.exceptions import (
     AuthenticationError,
     MisconfiguredError,
     NoMatchingProductType,
     PluginImplementationError,
@@ -223,15 +224,15 @@
                 | analysis.LowercaseFilter()
                 | analysis.SubstitutionFilter("-", "")
                 | analysis.SubstitutionFilter("_", "")
             )
 
             product_types_schema = Schema(
                 ID=fields.STORED,
-                abstract=fields.TEXT,
+                abstract=fields.STORED,
                 instrument=fields.IDLIST,
                 platform=fields.ID,
                 platformSerialIdentifier=fields.IDLIST,
                 processingLevel=fields.ID,
                 sensorType=fields.ID,
                 md5=fields.ID,
                 license=fields.ID,
@@ -318,15 +319,15 @@
             # check if the configured value has already been built as jsonpath
             if (
                 isinstance(some_configured_value, list)
                 and isinstance(some_configured_value[1], tuple)
                 or isinstance(some_configured_value, tuple)
             ):
                 # also build as jsonpath the incoming conf
-                mtd_cfg_as_jsonpath(
+                mtd_cfg_as_conversion_and_querypath(
                     deepcopy(
                         conf_update[provider][search_plugin_key]["metadata_mapping"]
                     ),
                     conf_update[provider][search_plugin_key]["metadata_mapping"],
                 )
 
         override_config_from_mapping(self.providers_config, conf_update)
@@ -514,17 +515,18 @@
                     provider_to_fetch
                 ] = discovery_conf
                 if not getattr(provider_config, "product_types_fetched", False):
                     already_fetched = False
 
         if not already_fetched:
             # get ext_product_types conf
-            if "EODAG_EXT_PRODUCT_TYPES_CFG_FILE" in os.environ:
+            ext_product_types_cfg_file = os.getenv("EODAG_EXT_PRODUCT_TYPES_CFG_FILE")
+            if ext_product_types_cfg_file is not None:
                 ext_product_types_conf = get_ext_product_types_conf(
-                    os.environ["EODAG_EXT_PRODUCT_TYPES_CFG_FILE"]
+                    ext_product_types_cfg_file
                 )
             else:
                 ext_product_types_conf = get_ext_product_types_conf()
 
                 if not ext_product_types_conf:
                     # empty ext_product_types conf
                     discover_kwargs = dict(provider=provider) if provider else {}
@@ -553,15 +555,52 @@
                     default_provider_search_config = default_provider_config.api
                 else:
                     continue
                 default_discovery_conf = getattr(
                     default_provider_search_config, "discover_product_types", {}
                 )
                 # compare confs
-                if default_discovery_conf == user_discovery_conf and (
+                if default_discovery_conf["result_type"] == "json" and isinstance(
+                    default_discovery_conf["results_entry"], str
+                ):
+                    default_discovery_conf_parsed = dict(
+                        default_discovery_conf,
+                        **{
+                            "results_entry": string_to_jsonpath(
+                                default_discovery_conf["results_entry"], force=True
+                            )
+                        },
+                        **mtd_cfg_as_conversion_and_querypath(
+                            dict(
+                                generic_product_type_id=default_discovery_conf[
+                                    "generic_product_type_id"
+                                ]
+                            )
+                        ),
+                        **dict(
+                            generic_product_type_parsable_properties=mtd_cfg_as_conversion_and_querypath(
+                                default_discovery_conf[
+                                    "generic_product_type_parsable_properties"
+                                ]
+                            )
+                        ),
+                        **dict(
+                            generic_product_type_parsable_metadata=mtd_cfg_as_conversion_and_querypath(
+                                default_discovery_conf[
+                                    "generic_product_type_parsable_metadata"
+                                ]
+                            )
+                        ),
+                    )
+                else:
+                    default_discovery_conf_parsed = default_discovery_conf
+                if (
+                    user_discovery_conf == default_discovery_conf
+                    or user_discovery_conf == default_discovery_conf_parsed
+                ) and (
                     not default_discovery_conf.get("fetch_url", None)
                     or "ext_product_types_conf" not in locals()
                     or "ext_product_types_conf" in locals()
                     and (
                         provider in ext_product_types_conf
                         or len(ext_product_types_conf.keys()) == 0
                     )
@@ -639,15 +678,15 @@
     def update_product_types_list(self, ext_product_types_conf):
         """Update eodag product types list
 
         :param ext_product_types_conf: external product types configuration
         :type ext_product_types_conf: dict
         """
         for provider, new_product_types_conf in ext_product_types_conf.items():
-            if new_product_types_conf:
+            if new_product_types_conf and provider in self.providers_config:
                 try:
                     if hasattr(self.providers_config[provider], "search"):
                         search_plugin_config = self.providers_config[provider].search
                     elif hasattr(self.providers_config[provider], "api"):
                         search_plugin_config = self.providers_config[provider].api
                     else:
                         continue
@@ -657,14 +696,15 @@
                     provider_products_config = self.providers_config[provider].products
                 except UnsupportedProvider:
                     logger.debug(
                         "Ignoring external product types for unknown provider %s",
                         provider,
                     )
                     continue
+                new_product_types = []
                 for (
                     new_product_type,
                     new_product_type_conf,
                 ) in new_product_types_conf["providers_config"].items():
                     if new_product_type not in provider_products_config:
                         for existing_product_type in provider_products_config.copy():
                             # compare parsed extracted conf (without metadata_mapping entry)
@@ -700,18 +740,23 @@
                                     ][new_product_type]
                                 }
                             )
                             self.product_types_config_md5 = obj_md5sum(
                                 self.product_types_config.source
                             )
                             ext_product_types_conf[provider] = new_product_types_conf
-                            logger.debug(
-                                f"Added product type {new_product_type} for {provider}"
-                            )
+                            new_product_types.append(new_product_type)
+                if new_product_types:
+                    logger.debug(
+                        f"Added product types {str(new_product_types)} for {provider}"
+                    )
 
+            elif provider not in self.providers_config:
+                # unknown provider
+                continue
             self.providers_config[provider].product_types_fetched = True
 
         # re-create _plugins_manager using up-to-date providers_config
         self._plugins_manager.build_product_type_to_provider_config_map()
 
         # rebuild index after product types list update
         self.build_index()
```

### Comparing `eodag-2.9.1/eodag/api/product/__init__.py` & `eodag-2.9.2/eodag/api/product/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/product/_product.py` & `eodag-2.9.2/eodag/api/product/_product.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/product/drivers/__init__.py` & `eodag-2.9.2/eodag/api/product/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/product/drivers/base.py` & `eodag-2.9.2/eodag/api/product/drivers/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/api/product/metadata_mapping.py` & `eodag-2.9.2/eodag/api/product/metadata_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import ast
 import logging
 import re
-from copy import deepcopy
 from datetime import datetime, timedelta
-from functools import partial
 from string import Formatter
 
 import geojson
 import pyproj
 from dateutil.parser import isoparse
 from dateutil.tz import UTC, tzutc
-from jsonpath_ng.jsonpath import Child, Fields, Index
+from jsonpath_ng.jsonpath import Child
 from lxml import etree
 from lxml.etree import XPathEvalError
 from shapely import wkt
 from shapely.geometry import MultiPolygon, Polygon
 from shapely.ops import transform
 
 from eodag.utils import (
     DEFAULT_PROJ,
-    cached_parse,
+    deepcopy,
     get_timestamp,
     items_recursive_apply,
     nested_pairs2dict,
+    string_to_jsonpath,
 )
 
 logger = logging.getLogger("eodag.api.product.metadata_mapping")
 
 SEP = r"#"
 INGEST_CONVERSION_REGEX = re.compile(
     r"^{(?P<path>[^#]*)" + SEP + r"(?P<converter>[^\d\W]\w*)(\((?P<args>.*)\))*}$"
@@ -318,20 +317,22 @@
             ewkt_regex = re.compile(r"^(?P<proj>[A-Za-z]+=[0-9]+);(?P<wkt>.*)$")
             ewkt_match = ewkt_regex.match(ewkt_string)
             if ewkt_match:
                 g = ewkt_match.groupdict()
                 from_proj = g["proj"].replace("SRID", "EPSG").replace("=", ":")
                 input_geom = wkt.loads(g["wkt"])
 
-                from_proj = pyproj.Proj(from_proj)
-                to_proj = pyproj.Proj(DEFAULT_PROJ)
+                from_proj = pyproj.CRS(from_proj)
+                to_proj = pyproj.CRS(DEFAULT_PROJ)
 
                 if from_proj != to_proj:
                     # reproject
-                    project = partial(pyproj.transform, from_proj, to_proj)
+                    project = pyproj.Transformer.from_crs(
+                        from_proj, to_proj, always_xy=True
+                    ).transform
                     return transform(project, input_geom)
                 else:
                     return input_geom
             else:
                 logger.warning(f"Could not read {ewkt_string} as EWKT")
                 return ewkt_string
 
@@ -356,17 +357,19 @@
                     for i in range(int(len(coords_list) / 2))
                 ]
                 return Polygon(polygon_args)
             elif len(georss) == 1 and "multisurface" in georss[0].tag.lower():
                 # Multipolygon
                 from_proj = getattr(georss[0], "attrib", {}).get("srsName", None)
                 if from_proj:
-                    from_proj = pyproj.Proj(from_proj)
-                    to_proj = pyproj.Proj(DEFAULT_PROJ)
-                    project = partial(pyproj.transform, from_proj, to_proj)
+                    from_proj = pyproj.CRS(from_proj)
+                    to_proj = pyproj.CRS(DEFAULT_PROJ)
+                    project = pyproj.Transformer.from_crs(
+                        from_proj, to_proj, always_xy=True
+                    ).transform
 
                 # function to get deepest elements
                 def flatten_elements(nested):
 
                     for e in nested:
                         if len(e) > 0:
                             yield from flatten_elements(e)
@@ -582,39 +585,41 @@
 
     # adds missing discovered properties
     if not discovery_config:
         discovery_config = {}
     discovery_pattern = discovery_config.get("metadata_pattern", None)
     discovery_path = discovery_config.get("metadata_path", None)
     if discovery_pattern and discovery_path:
-        discovered_properties = cached_parse(discovery_path).find(json)
+        discovered_properties = string_to_jsonpath(discovery_path).find(json)
         for found_jsonpath in discovered_properties:
             if "metadata_path_id" in discovery_config.keys():
-                found_key_paths = cached_parse(
-                    discovery_config["metadata_path_id"]
+                found_key_paths = string_to_jsonpath(
+                    discovery_config["metadata_path_id"], force=True
                 ).find(found_jsonpath.value)
                 if not found_key_paths:
                     continue
                 found_key = found_key_paths[0].value
                 used_jsonpath = Child(
                     found_jsonpath.full_path,
-                    cached_parse(discovery_config["metadata_path_value"]),
+                    string_to_jsonpath(
+                        discovery_config["metadata_path_value"], force=True
+                    ),
                 )
             else:
                 # default key got from metadata_path
                 found_key = found_jsonpath.path.fields[-1]
                 used_jsonpath = found_jsonpath.full_path
             if (
                 re.compile(discovery_pattern).match(found_key)
                 and found_key not in properties.keys()
                 and used_jsonpath not in used_jsonpaths
             ):
                 if "metadata_path_value" in discovery_config.keys():
-                    found_value_path = cached_parse(
-                        discovery_config["metadata_path_value"]
+                    found_value_path = string_to_jsonpath(
+                        discovery_config["metadata_path_value"], force=True
                     ).find(found_jsonpath.value)
                     properties[found_key] = (
                         found_value_path[0].value if found_value_path else NOT_AVAILABLE
                     )
                 else:
                     # default value got from metadata_path
                     properties[found_key] = found_jsonpath.value
@@ -775,84 +780,46 @@
                 and found_xpath.tag not in used_xpaths
             ):
                 properties[found_key] = found_xpath.text
 
     return properties
 
 
-def mtd_cfg_as_jsonpath(
-    src_dict, dest_dict={}, common_jsonpath=None, keep_conversion=True
-):
-    """Metadata configuration dictionary to jsonpath objects dictionnay
-    Transform every src_dict value from jsonpath str to jsonpath object
+def mtd_cfg_as_conversion_and_querypath(src_dict, dest_dict={}, result_type="json"):
+    """Metadata configuration dictionary to querypath with conversion dictionnary
+    Transform every src_dict value from jsonpath_str to tuple `(conversion, jsonpath_object)`
+    or from xpath_str to tuple `(conversion, xpath_str)`
 
     :param src_dict: Input dict containing jsonpath str as values
     :type src_dict: dict
     :param dest_dict: (optional) Output dict containing jsonpath objects as values
     :type dest_dict: dict
-    :param common_jsonpath: (optional) common jsonpath used optimize jsonpath build process
-    :type common_jsonpath: str
-    :param keep_conversion: (optional) whether to keep conversion on parse error or not
-    :type keep_conversion: bool
     :returns: dest_dict
     :rtype: dict
     """
-    if common_jsonpath:
-        common_jsonpath_parsed = cached_parse(common_jsonpath)
-        common_jsonpath_match = re.compile(
-            rf"^{re.escape(common_jsonpath)}\.[a-zA-Z0-9-_:\.\[\]\"]+$"
-        )
-        array_field_match = re.compile(r"^[a-zA-Z0-9-_:]+\[[0-9]+\]$")
-    else:
-        common_jsonpath_match = None
     if not dest_dict:
         dest_dict = deepcopy(src_dict)
     for metadata in src_dict:
         if metadata not in dest_dict:
             dest_dict[metadata] = (None, NOT_MAPPED)
         else:
             conversion, path = get_metadata_path(dest_dict[metadata])
-            try:
-                # combine with common jsonpath if possible
-                if common_jsonpath_match and common_jsonpath_match.match(path):
-                    path_suffix = path[len(common_jsonpath) + 1 :]
-                    path_splits = path_suffix.split(".")
-                    parsed_path = common_jsonpath_parsed
-                    for path_split in path_splits:
-                        path_split = path_split.strip("'").strip('"')
-                        if "[" in path_split and array_field_match.match(path_split):
-                            # simple array field
-                            indexed_path, index = path_split[:-1].split("[")
-                            index = int(index)
-                            parsed_path = Child(
-                                Child(parsed_path, Fields(indexed_path)),
-                                Index(index=index),
-                            )
-                            continue
-                        elif "[" in path_split:
-                            # nested array field
-                            parsed_path = cached_parse(path)
-                            break
-                        else:
-                            parsed_path = Child(parsed_path, Fields(path_split))
-                else:
-                    parsed_path = cached_parse(path)
-                # If the metadata is queryable (i.e a list of 2 elements), replace the value of the last item
-                if len(dest_dict[metadata]) == 2:
-                    dest_dict[metadata][1] = (conversion, parsed_path)
-                else:
-                    dest_dict[metadata] = (conversion, parsed_path)
-            except Exception:  # jsonpath_ng does not provide a proper exception
-                # Keep path as this and its associated conversion (or None if not keep_conversion)
-                if not keep_conversion:
+            if result_type == "json":
+                parsed_path = string_to_jsonpath(path)
+                if isinstance(parsed_path, str):
+                    # not a jsonpath: assume the mapping is to be passed as is. Ignore any transformation specified.
+                    # If a value is to be passed as is, we don't want to transform it further
                     conversion = None
-                if len(dest_dict[metadata]) == 2:
-                    dest_dict[metadata][1] = (conversion, path)
-                else:
-                    dest_dict[metadata] = (conversion, path)
+            else:
+                parsed_path = path
+
+            if len(dest_dict[metadata]) == 2:
+                dest_dict[metadata][1] = (conversion, parsed_path)
+            else:
+                dest_dict[metadata] = (conversion, parsed_path)
 
             # Put the updated mapping at the end
             dest_dict[metadata] = dest_dict.pop(metadata)
 
     return dest_dict
```

### Comparing `eodag-2.9.1/eodag/api/search_result.py` & `eodag-2.9.2/eodag/api/search_result.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/cli.py` & `eodag-2.9.2/eodag/cli.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/config.py` & `eodag-2.9.2/eodag/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
+# import copy
 import logging
 import os
 import tempfile
-from copy import deepcopy
 
+import orjson
 import requests
 import yaml
 import yaml.constructor
 import yaml.parser
 from pkg_resources import resource_filename
 
 from eodag.utils import (
     USER_AGENT,
+    cached_yaml_load,
+    cached_yaml_load_all,
+    deepcopy,
     dict_items_recursive_apply,
     merge_mappings,
     slugify,
     string_to_jsonpath,
     update_nested_dict,
     uri_to_path,
 )
@@ -47,20 +50,20 @@
 
 
 class SimpleYamlProxyConfig(object):
     """A simple configuration class acting as a proxy to an underlying dict object
     as returned by yaml.load"""
 
     def __init__(self, conf_file_path):
-        with open(os.path.abspath(os.path.realpath(conf_file_path)), "r") as fh:
-            try:
-                self.source = yaml.load(fh, Loader=yaml.SafeLoader)
-            except yaml.parser.ParserError as e:
-                print("Unable to load user configuration file")
-                raise e
+        try:
+            self.source = cached_yaml_load(conf_file_path)
+            # self.source = deepcopy(cached_yaml_load(conf_file_path))
+        except yaml.parser.ParserError as e:
+            print("Unable to load user configuration file")
+            raise e
 
     def __getitem__(self, item):
         return self.source[item]
 
     def __contains__(self, item):
         return item in self.source
 
@@ -238,27 +241,27 @@
 
     :param config_path: The path to the provider config file
     :type config_path: str
     :returns: The default provider's configuration
     :rtype: dict
     """
     config = {}
-    with open(config_path, "r") as fh:
-        try:
-            # Providers configs are stored in this file as separated yaml documents
-            # Load all of it
-            providers_configs = yaml.load_all(fh, Loader=yaml.Loader)
-        except yaml.parser.ParserError as e:
-            logger.error("Unable to load configuration")
-            raise e
-        stac_provider_config = load_stac_provider_config()
-        for provider_config in providers_configs:
-            provider_config_init(provider_config, stac_provider_config)
-            config[provider_config.name] = provider_config
-        return config
+    try:
+        # Providers configs are stored in this file as separated yaml documents
+        # Load all of it
+        providers_configs = cached_yaml_load_all(config_path)
+    except yaml.parser.ParserError as e:
+        logger.error("Unable to load configuration")
+        raise e
+    stac_provider_config = load_stac_provider_config()
+    for provider_config in providers_configs:
+        # for provider_config in copy.deepcopy(providers_configs):
+        provider_config_init(provider_config, stac_provider_config)
+        config[provider_config.name] = provider_config
+    return config
 
 
 def provider_config_init(provider_config, stac_search_default_conf=None):
     """Applies some default values to provider config
 
     :param provider_config: An eodag provider configuration
     :type provider_config: :class:`~eodag.config.ProviderConfig`
@@ -491,15 +494,15 @@
             )
             return {}
     elif conf_uri.lower().startswith("file"):
         conf_uri = uri_to_path(conf_uri)
 
     # read from local
     try:
-        with open(conf_uri) as f:
-            return json.load(f)
-    except (json.JSONDecodeError, FileNotFoundError) as e:
+        with open(conf_uri, "rb") as f:
+            return orjson.loads(f.read())
+    except (orjson.JSONDecodeError, FileNotFoundError) as e:
         logger.debug(e)
         logger.warning(
             "Could not read local external product types conf from %s", conf_uri
         )
         return {}
```

### Comparing `eodag-2.9.1/eodag/crunch.py` & `eodag-2.9.2/eodag/crunch.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/__init__.py` & `eodag-2.9.2/eodag/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/apis/__init__.py` & `eodag-2.9.2/eodag/plugins/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/apis/base.py` & `eodag-2.9.2/eodag/plugins/apis/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/apis/cds.py` & `eodag-2.9.2/eodag/plugins/apis/cds.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,149 +11,102 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import hashlib
 import logging
 from datetime import datetime
 
 import cdsapi
+import geojson
 import requests
 
-from eodag import EOProduct
-from eodag.api.product.metadata_mapping import NOT_AVAILABLE, properties_from_json
 from eodag.plugins.apis.base import Api
 from eodag.plugins.download.base import (
     DEFAULT_DOWNLOAD_TIMEOUT,
     DEFAULT_DOWNLOAD_WAIT,
     Download,
 )
-from eodag.plugins.search.qssearch import QueryStringSearch
-from eodag.utils import (
-    datetime_range,
-    get_geometry_from_various,
-    parse_qsl,
-    path_to_uri,
-    urlsplit,
-)
-from eodag.utils.exceptions import (
-    AuthenticationError,
-    DownloadError,
-    RequestError,
-    ValidationError,
-)
+from eodag.plugins.search.base import Search
+from eodag.plugins.search.build_search_result import BuildPostSearchResult
+from eodag.rest.stac import DEFAULT_MISSION_START_DATE
+from eodag.utils import datetime_range, get_geometry_from_various, path_to_uri, urlsplit
+from eodag.utils.exceptions import AuthenticationError, DownloadError, RequestError
 from eodag.utils.logging import get_logging_verbose
 
 logger = logging.getLogger("eodag.plugins.apis.cds")
 
 CDS_KNOWN_FORMATS = {"grib": "grib", "netcdf": "nc"}
 
 
-class CdsApi(Download, Api, QueryStringSearch):
+class CdsApi(Download, Api, BuildPostSearchResult):
     """A plugin that enables to build download-request and download data on CDS API.
 
     Builds a single ready-to-download :class:`~eodag.api.product._product.EOProduct`
     during the search stage.
 
     This class inherits from :class:`~eodag.plugins.apis.base.Api` for compatibility,
     :class:`~eodag.plugins.download.base.Download` for download methods, and
     :class:`~eodag.plugins.search.qssearch.QueryStringSearch` for metadata-mapping and
     query build methods.
     """
 
     def __init__(self, provider, config):
         # init self.config.metadata_mapping using Search Base plugin
-        super(QueryStringSearch, self).__init__(provider, config)
+        Search.__init__(self, provider, config)
 
         # needed by QueryStringSearch.build_query_string / format_free_text_search
         self.config.__dict__.setdefault("free_text_search_operations", {})
         # needed for compatibility
-        self.config.__dict__.setdefault("pagination", {})
+        self.config.__dict__.setdefault("pagination", {"next_page_query_obj": "{{}}"})
+
+    def do_search(self, *args, **kwargs):
+        """Should perform the actual search request."""
+        return [{}]
 
     def query(
         self, product_type=None, items_per_page=None, page=None, count=True, **kwargs
     ):
         """Build ready-to-download SearchResult"""
 
-        # check some mandatory parameters
+        # check productType, dates, geometry, use defaults if not specified
+        # productType
+        if not kwargs.get("productType"):
+            kwargs["productType"] = kwargs.get("dataset", None)
         # start date
         if "startTimeFromAscendingNode" not in kwargs:
-            raise ValidationError("Required start date is missing")
+            kwargs["startTimeFromAscendingNode"] = (
+                getattr(self.config, "product_type_config", {}).get(
+                    "missionStartDate", None
+                )
+                or DEFAULT_MISSION_START_DATE
+            )
         # end date
         if "completionTimeFromAscendingNode" not in kwargs:
-            raise ValidationError("Required end date is missing")
-
-        product_type = kwargs.get("productType")
-
-        # Map query args to properties
-        product_properties = kwargs
-        product_properties.pop("auth", None)
+            kwargs["completionTimeFromAscendingNode"] = getattr(
+                self.config, "product_type_config", {}
+            ).get("missionEndDate", None) or datetime.utcnow().isoformat(
+                timespec="seconds"
+            )
         # geometry
-        search_geometry = product_properties.get("geometry", None) or [
-            -180,
-            -90,
-            180,
-            90,
-        ]
-        product_geometry = get_geometry_from_various(geometry=search_geometry)
-        product_properties["geometry"] = product_geometry
-
-        # add product_type specific properties from provider configuration (overriden by query args)
-        product_properties = dict(
-            self.config.products.get(product_type, {}), **product_properties
-        )
-
-        # properties mapped using provider configuration
-        product_properties = properties_from_json(
-            product_properties, self.config.metadata_mapping
-        )
+        if not kwargs.get("geometry", None):
+            kwargs["geometry"] = [
+                -180,
+                -90,
+                180,
+                90,
+            ]
+        kwargs["geometry"] = get_geometry_from_various(geometry=kwargs["geometry"])
 
-        # build query string & parameters dict using from available mapped properties
-        product_available_properties = {
-            k: v for (k, v) in product_properties.items() if v != NOT_AVAILABLE
-        }
-        qp, qs = self.build_query_string(product_type, **product_available_properties)
-
-        # query hash, will be used to build a product id
-        query_hash = hashlib.sha1(str(qs).encode("UTF-8")).hexdigest()
-
-        # build product id
-        if product_type is not None:
-            id_prefix = product_type
-        else:
-            id_prefix = ("%s" % (qp.get("dataset", ""))).upper()
-
-        product_id = "%s_%s_%s" % (
-            id_prefix,
-            qp["date"][0].split("/")[0].replace("-", ""),
-            query_hash,
-        )
-        product_properties["id"] = product_properties["title"] = product_id
-
-        # update downloadLink
-        product_properties["downloadLink"] += f"?{qs}"
-
-        product = EOProduct(
-            provider=self.provider,
-            productType=product_type,
-            properties=product_properties,
-        )
-        # use product_type_config as default properties
-        product.properties = dict(
-            getattr(self.config, "product_type_config", {}), **product.properties
+        return BuildPostSearchResult.query(
+            self, items_per_page=items_per_page, page=page, count=count, **kwargs
         )
 
-        results_count = 1
-        return [
-            product,
-        ], results_count
-
     def _get_cds_client(self, **auth_dict):
         """Returns cdsapi client."""
         # eodag logging info
         eodag_verbosity = get_logging_verbose()
         eodag_logger = logging.getLogger("eodag")
 
         client = cdsapi.Client(
@@ -223,16 +176,17 @@
 
         if not fs_path or not record_filename:
             if fs_path:
                 product.location = path_to_uri(fs_path)
             return fs_path
 
         # get download request dict from product.location/downloadLink url query string
+        # separate url & parameters
         query_str = "".join(urlsplit(product.location).fragment.split("?", 1)[1:])
-        download_request = dict(parse_qsl(query_str))
+        download_request = geojson.loads(query_str)
 
         date_range = download_request.pop("date_range", False)
         if date_range:
             date = download_request.pop("date")
             start, end, *_ = date.split("/")
             _start = datetime.fromisoformat(start)
             _end = datetime.fromisoformat(end)
```

### Comparing `eodag-2.9.1/eodag/plugins/apis/ecmwf.py` & `eodag-2.9.2/eodag/plugins/apis/ecmwf.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import hashlib
 import logging
+from datetime import datetime
 
+import geojson
 from ecmwfapi import ECMWFDataServer, ECMWFService
 from ecmwfapi.api import APIException, Connection, get_apikey_values
 
-from eodag import EOProduct
-from eodag.api.product.metadata_mapping import NOT_AVAILABLE, properties_from_json
 from eodag.plugins.apis.base import Api
 from eodag.plugins.download.base import (
     DEFAULT_DOWNLOAD_TIMEOUT,
     DEFAULT_DOWNLOAD_WAIT,
     Download,
 )
-from eodag.plugins.search.qssearch import QueryStringSearch
-from eodag.utils import get_geometry_from_various, parse_qsl, path_to_uri, urlsplit
-from eodag.utils.exceptions import AuthenticationError, DownloadError, ValidationError
+from eodag.plugins.search.base import Search
+from eodag.plugins.search.build_search_result import BuildPostSearchResult
+from eodag.rest.stac import DEFAULT_MISSION_START_DATE
+from eodag.utils import get_geometry_from_various, path_to_uri, urlsplit
+from eodag.utils.exceptions import AuthenticationError, DownloadError
 from eodag.utils.logging import get_logging_verbose
 
 logger = logging.getLogger("eodag.plugins.apis.ecmwf")
 
 ECMWF_MARS_KNOWN_FORMATS = {"grib": "grib", "netcdf": "nc"}
 
 
-class EcmwfApi(Download, Api, QueryStringSearch):
+class EcmwfApi(Download, Api, BuildPostSearchResult):
     """A plugin that enables to build download-request and download data on ECMWF MARS.
 
     Builds a single ready-to-download :class:`~eodag.api.product._product.EOProduct`
     during the search stage.
 
     Download will then be performed on ECMWF Public Datasets (if ``dataset`` parameter
     is in query), or on MARS Operational Archive (if ``dataset`` parameter is not in
@@ -53,105 +54,66 @@
     :class:`~eodag.plugins.download.base.Download` for download methods, and
     :class:`~eodag.plugins.search.qssearch.QueryStringSearch` for metadata-mapping and
     query build methods.
     """
 
     def __init__(self, provider, config):
         # init self.config.metadata_mapping using Search Base plugin
-        super(QueryStringSearch, self).__init__(provider, config)
+        Search.__init__(self, provider, config)
 
         # needed by QueryStringSearch.build_query_string / format_free_text_search
         self.config.__dict__.setdefault("free_text_search_operations", {})
         # needed for compatibility
-        self.config.__dict__.setdefault("pagination", {})
+        self.config.__dict__.setdefault("pagination", {"next_page_query_obj": "{{}}"})
+
+    def do_search(self, *args, **kwargs):
+        """Should perform the actual search request."""
+        return [{}]
 
     def query(
         self, product_type=None, items_per_page=None, page=None, count=True, **kwargs
     ):
         """Build ready-to-download SearchResult"""
 
-        # check some mandatory parameters
+        # check productType, dates, geometry, use defaults if not specified
+        # productType
+        if not kwargs.get("productType"):
+            kwargs["productType"] = "%s_%s_%s" % (
+                kwargs.get("dataset", "mars"),
+                kwargs.get("type", ""),
+                kwargs.get("levtype", ""),
+            )
         # start date
         if "startTimeFromAscendingNode" not in kwargs:
-            raise ValidationError("Required start date is missing")
+            kwargs["startTimeFromAscendingNode"] = (
+                getattr(self.config, "product_type_config", {}).get(
+                    "missionStartDate", None
+                )
+                or DEFAULT_MISSION_START_DATE
+            )
         # end date
         if "completionTimeFromAscendingNode" not in kwargs:
-            raise ValidationError("Required end date is missing")
-
-        product_type = kwargs.get("productType")
-
-        # Map query args to properties
-        product_properties = kwargs
-        product_properties.pop("auth", None)
+            kwargs["completionTimeFromAscendingNode"] = getattr(
+                self.config, "product_type_config", {}
+            ).get("missionEndDate", None) or datetime.utcnow().isoformat(
+                timespec="seconds"
+            )
         # geometry
-        search_geometry = product_properties.get("geometry", None) or [
-            -180,
-            -90,
-            180,
-            90,
-        ]
-        product_geometry = get_geometry_from_various(geometry=search_geometry)
-        product_properties["geometry"] = product_geometry
-
-        # add product_type specific properties from provider configuration (overriden by query args)
-        product_properties = dict(
-            self.config.products.get(product_type, {}), **product_properties
-        )
-
-        # properties mapped using provider configuration
-        product_properties = properties_from_json(
-            product_properties, self.config.metadata_mapping
-        )
+        if not kwargs.get("geometry", None):
+            kwargs["geometry"] = [
+                -180,
+                -90,
+                180,
+                90,
+            ]
+        kwargs["geometry"] = get_geometry_from_various(geometry=kwargs["geometry"])
 
-        # build query string & parameters dict using from available mapped properties
-        product_available_properties = {
-            k: v for (k, v) in product_properties.items() if v != NOT_AVAILABLE
-        }
-        qp, qs = self.build_query_string(product_type, **product_available_properties)
-
-        # query hash, will be used to build a product id
-        query_hash = hashlib.sha1(str(qs).encode("UTF-8")).hexdigest()
-
-        # build product id
-        if product_type is not None:
-            id_prefix = product_type
-        else:
-            id_prefix = (
-                "%s_%s_%s"
-                % (
-                    qp.get("dataset", "mars"),
-                    qp.get("type", ""),
-                    qp.get("levtype", ""),
-                )
-            ).upper()
-
-        product_id = "%s_%s_%s" % (
-            id_prefix,
-            qp["date"][0].split("/")[0].replace("-", ""),
-            query_hash,
+        return BuildPostSearchResult.query(
+            self, items_per_page=items_per_page, page=page, count=count, **kwargs
         )
-        product_properties["id"] = product_properties["title"] = product_id
-
-        # update downloadLink
-        product_properties["downloadLink"] += f"?{qs}"
-
-        product = EOProduct(
-            provider=self.provider,
-            productType=product_type,
-            properties=product_properties,
-        )
-        # use product_type_config as default properties
-        product.properties = dict(
-            getattr(self.config, "product_type_config", {}), **product.properties
-        )
-
-        results_count = 1
-        return [
-            product,
-        ], results_count
 
     def authenticate(self):
         """Check credentials and returns information needed for auth
 
         :returns: {key, url, email} dictionary
         :rtype: dict
         :raises: :class:`~eodag.utils.exceptions.AuthenticationError`
@@ -195,15 +157,16 @@
 
         if not fs_path or not record_filename:
             if fs_path:
                 product.location = path_to_uri(fs_path)
             return fs_path
 
         # get download request dict from product.location/downloadLink url query string
-        download_request = dict(parse_qsl(urlsplit(product.location).query))
+        # separate url & parameters
+        download_request = geojson.loads(urlsplit(product.location).query)
 
         # Set verbosity
         eodag_verbosity = get_logging_verbose()
         if eodag_verbosity is not None and eodag_verbosity >= 3:
             # debug verbosity
             ecmwf_verbose = True
             ecmwf_log = logger.debug
@@ -213,25 +176,28 @@
             ecmwf_log = logger.info
 
         auth_dict = self.authenticate()
 
         # Send download request to ECMWF web API
         logger.info("Request download on ECMWF: %s" % download_request)
         try:
-            if "dataset" in download_request:
+            if "dataset" in download_request and not download_request[
+                "dataset"
+            ].startswith("mars_"):
                 # Public dataset
                 ecmwf_server = ECMWFDataServer(
                     verbose=ecmwf_verbose, log=ecmwf_log, **auth_dict
                 )
                 ecmwf_server.retrieve(dict(download_request, **{"target": fs_path}))
             else:
                 # Operational Archive
                 ecmwf_server = ECMWFService(
                     service="mars", verbose=ecmwf_verbose, log=ecmwf_log, **auth_dict
                 )
+                download_request.pop("dataset", None)
                 ecmwf_server.execute(download_request, fs_path)
         except APIException as e:
             logger.error(e)
             raise DownloadError(e)
 
         with open(record_filename, "w") as fh:
             fh.write(product.properties["downloadLink"])
```

### Comparing `eodag-2.9.1/eodag/plugins/apis/usgs.py` & `eodag-2.9.2/eodag/plugins/apis/usgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 import logging
 import shutil
 import tarfile
 import zipfile
 
 import requests
 from jsonpath_ng.ext import parse
 from requests import RequestException
 from usgs import USGSAuthExpiredError, USGSError, api
 
 from eodag.api.product import EOProduct
 from eodag.api.product.metadata_mapping import (
     DEFAULT_METADATA_MAPPING,
-    mtd_cfg_as_jsonpath,
+    mtd_cfg_as_conversion_and_querypath,
     properties_from_json,
 )
 from eodag.plugins.apis.base import Api
 from eodag.plugins.download.base import (
     DEFAULT_DOWNLOAD_TIMEOUT,
     DEFAULT_DOWNLOAD_WAIT,
     Download,
@@ -49,14 +48,30 @@
 
 logger = logging.getLogger("eodag.plugins.apis.usgs")
 
 
 class UsgsApi(Download, Api):
     """A plugin that enables to query and download data on the USGS catalogues"""
 
+    def __init__(self, provider, config):
+        super(UsgsApi, self).__init__(provider, config)
+
+        # Same method as in base.py, Search.__init__()
+        # Prepare the metadata mapping
+        # Do a shallow copy, the structure is flat enough for this to be sufficient
+        metas = DEFAULT_METADATA_MAPPING.copy()
+        # Update the defaults with the mapping value. This will add any new key
+        # added by the provider mapping that is not in the default metadata.
+        metas.update(self.config.metadata_mapping)
+        self.config.metadata_mapping = mtd_cfg_as_conversion_and_querypath(
+            metas,
+            self.config.metadata_mapping,
+            result_type=getattr(self.config, "result_type", "json"),
+        )
+
     def authenticate(self):
         """Login to usgs api
 
         :raises: :class:`~eodag.utils.exceptions.AuthenticationError`
         """
         for i in range(2):
             try:
@@ -155,36 +170,21 @@
                         and download_option["available"]
                     ):
                         results_by_entity_id[download_option["entityId"]].update(
                             download_option
                         )
             results["data"]["results"] = list(results_by_entity_id.values())
 
-            # Same method as in base.py, Search.__init__()
-            # Prepare the metadata mapping
-            # Do a shallow copy, the structure is flat enough for this to be sufficient
-            metas = DEFAULT_METADATA_MAPPING.copy()
-            # Update the defaults with the mapping value. This will add any new key
-            # added by the provider mapping that is not in the default metadata.
-            # A deepcopy is done to prevent self.config.metadata_mapping from being modified when metas[metadata]
-            # is a list and is modified
-            metas.update(copy.deepcopy(self.config.metadata_mapping))
-            # common_jsonpath usage to optimize jsonpath build process
-            mtd_cfg_as_jsonpath_options = {}
-            if hasattr(self.config, "common_metadata_mapping_path"):
-                mtd_cfg_as_jsonpath_options[
-                    "common_jsonpath"
-                ] = self.config.common_metadata_mapping_path
-            metas = mtd_cfg_as_jsonpath(metas, **mtd_cfg_as_jsonpath_options)
-
             for result in results["data"]["results"]:
 
                 result["productType"] = usgs_dataset
 
-                product_properties = properties_from_json(result, metas)
+                product_properties = properties_from_json(
+                    result, self.config.metadata_mapping
+                )
 
                 final.append(
                     EOProduct(
                         productType=product_type,
                         provider=self.provider,
                         properties=product_properties,
                         geometry=footprint,
```

### Comparing `eodag-2.9.1/eodag/plugins/authentication/__init__.py` & `eodag-2.9.2/eodag/plugins/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/aws_auth.py` & `eodag-2.9.2/eodag/plugins/authentication/aws_auth.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/base.py` & `eodag-2.9.2/eodag/plugins/authentication/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/generic.py` & `eodag-2.9.2/eodag/plugins/authentication/generic.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/header.py` & `eodag-2.9.2/eodag/plugins/authentication/header.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/keycloak.py` & `eodag-2.9.2/eodag/plugins/authentication/keycloak.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,18 @@
             )
             response.raise_for_status()
         except requests.RequestException as e:
             # check if error is identified as auth_error in provider conf
             auth_errors = getattr(self.config, "auth_error_code", [None])
             if not isinstance(auth_errors, list):
                 auth_errors = [auth_errors]
-            if e.response.status_code in auth_errors:
+            if (
+                hasattr(e.response, "status_code")
+                and e.response.status_code in auth_errors
+            ):
                 raise AuthenticationError(
                     "HTTP Error %s returned, %s\nPlease check your credentials for %s"
                     % (e.response.status_code, e.response.text.strip(), self.provider)
                 )
             # other error
             else:
                 import traceback as tb
```

### Comparing `eodag-2.9.1/eodag/plugins/authentication/oauth.py` & `eodag-2.9.2/eodag/plugins/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/openid_connect.py` & `eodag-2.9.2/eodag/plugins/authentication/openid_connect.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/qsauth.py` & `eodag-2.9.2/eodag/plugins/authentication/qsauth.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/authentication/token.py` & `eodag-2.9.2/eodag/plugins/authentication/token.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/base.py` & `eodag-2.9.2/eodag/plugins/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/__init__.py` & `eodag-2.9.2/eodag/plugins/crunch/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/base.py` & `eodag-2.9.2/eodag/plugins/crunch/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/filter_date.py` & `eodag-2.9.2/eodag/plugins/crunch/filter_date.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/filter_latest_intersect.py` & `eodag-2.9.2/eodag/plugins/crunch/filter_latest_intersect.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/filter_latest_tpl_name.py` & `eodag-2.9.2/eodag/plugins/crunch/filter_latest_tpl_name.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/filter_overlap.py` & `eodag-2.9.2/eodag/plugins/crunch/filter_overlap.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/crunch/filter_property.py` & `eodag-2.9.2/eodag/plugins/crunch/filter_property.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/download/__init__.py` & `eodag-2.9.2/eodag/plugins/download/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/download/aws.py` & `eodag-2.9.2/eodag/plugins/download/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import boto3
 import requests
 from botocore.exceptions import ClientError, ProfileNotFound
 from botocore.handlers import disable_signing
 from lxml import etree
 
 from eodag.api.product.metadata_mapping import (
-    mtd_cfg_as_jsonpath,
+    mtd_cfg_as_conversion_and_querypath,
     properties_from_json,
     properties_from_xml,
 )
 from eodag.plugins.download.base import Download
 from eodag.utils import (
     USER_AGENT,
     ProgressCallback,
@@ -252,15 +252,15 @@
             fetch_format = product_conf["fetch_metadata"]["fetch_format"]
             update_metadata = product_conf["fetch_metadata"]["update_metadata"]
             fetch_url = product_conf["fetch_metadata"]["fetch_url"].format(
                 **product.properties
             )
             logger.info("Fetching extra metadata from %s" % fetch_url)
             resp = requests.get(fetch_url, headers=USER_AGENT, timeout=HTTP_REQ_TIMEOUT)
-            update_metadata = mtd_cfg_as_jsonpath(update_metadata)
+            update_metadata = mtd_cfg_as_conversion_and_querypath(update_metadata)
             if fetch_format == "json":
                 json_resp = resp.json()
                 update_metadata = properties_from_json(json_resp, update_metadata)
                 product.properties.update(update_metadata)
             elif fetch_format == "xml":
                 update_metadata = properties_from_xml(resp.content, update_metadata)
                 product.properties.update(update_metadata)
```

### Comparing `eodag-2.9.1/eodag/plugins/download/base.py` & `eodag-2.9.2/eodag/plugins/download/base.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/download/http.py` & `eodag-2.9.2/eodag/plugins/download/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import shutil
 import zipfile
-from cgi import parse_header
 from urllib.parse import parse_qs, urlparse
 
 import geojson
 import requests
 from lxml import etree
 from requests import HTTPError, RequestException
 
 from eodag.api.product.metadata_mapping import (
     OFFLINE_STATUS,
     ONLINE_STATUS,
-    mtd_cfg_as_jsonpath,
+    mtd_cfg_as_conversion_and_querypath,
     properties_from_json,
     properties_from_xml,
 )
 from eodag.plugins.download.base import (
     DEFAULT_DOWNLOAD_TIMEOUT,
     DEFAULT_DOWNLOAD_WAIT,
     DEFAULT_STREAM_REQUESTS_TIMEOUT,
     Download,
 )
 from eodag.utils import (
     USER_AGENT,
     ProgressCallback,
     flatten_top_directories,
+    parse_header,
     path_to_uri,
     uri_to_path,
 )
 from eodag.utils.exceptions import (
     AuthenticationError,
     DownloadError,
     MisconfiguredError,
@@ -135,15 +135,15 @@
 
         order_metadata_mapping = getattr(self.config, "order_on_response", {}).get(
             "metadata_mapping", {}
         )
         if order_metadata_mapping:
             logger.debug("Parsing order response to update product metada-mapping")
             order_metadata_mapping_jsonpath = {}
-            order_metadata_mapping_jsonpath = mtd_cfg_as_jsonpath(
+            order_metadata_mapping_jsonpath = mtd_cfg_as_conversion_and_querypath(
                 order_metadata_mapping, order_metadata_mapping_jsonpath
             )
             properties_update = properties_from_json(
                 response.json(),
                 order_metadata_mapping_jsonpath,
             )
             product.properties.update(properties_update)
@@ -272,17 +272,19 @@
                             # single result
                             result = results[0]
                             # parse result
                             new_search_metadata_mapping = (
                                 self.config.order_status_on_success["metadata_mapping"]
                             )
                             order_metadata_mapping_jsonpath = {}
-                            order_metadata_mapping_jsonpath = mtd_cfg_as_jsonpath(
-                                new_search_metadata_mapping,
-                                order_metadata_mapping_jsonpath,
+                            order_metadata_mapping_jsonpath = (
+                                mtd_cfg_as_conversion_and_querypath(
+                                    new_search_metadata_mapping,
+                                    order_metadata_mapping_jsonpath,
+                                )
                             )
                             properties_update = properties_from_xml(
                                 result,
                                 order_metadata_mapping_jsonpath,
                             )
                         except Exception as e:
                             logger.debug(e)
@@ -552,31 +554,30 @@
                 # HEAD request for size & filename
                 asset_headers = requests.head(
                     asset["href"],
                     auth=auth,
                     headers=USER_AGENT,
                     timeout=HTTP_REQ_TIMEOUT,
                 ).headers
-                header_content_disposition_dict = {}
 
                 if not asset.get("size", 0):
                     # size from HEAD header / Content-length
                     asset["size"] = int(asset_headers.get("Content-length", 0))
 
                 if not asset.get("size", 0) or not asset.get("filename", 0):
                     # header content-disposition
-                    header_content_disposition_dict = parse_header(
+                    header_content_disposition = parse_header(
                         asset_headers.get("content-disposition", "")
-                    )[-1]
+                    )
                 if not asset.get("size", 0):
                     # size from HEAD header / content-disposition / size
-                    asset["size"] = int(header_content_disposition_dict.get("size", 0))
+                    asset["size"] = int(header_content_disposition.get_param("size", 0))
                 if not asset.get("filename", 0):
                     # filename from HEAD header / content-disposition / size
-                    asset["filename"] = header_content_disposition_dict.get(
+                    asset["filename"] = header_content_disposition.get_param(
                         "filename", None
                     )
 
                 if not asset.get("size", 0):
                     # GET request for size
                     with requests.get(
                         asset["href"],
@@ -589,15 +590,15 @@
                         # size from GET header / Content-length
                         asset["size"] = int(stream.headers.get("Content-length", 0))
                         if not asset.get("size", 0):
                             # size from GET header / content-disposition / size
                             asset["size"] = int(
                                 parse_header(
                                     stream.headers.get("content-disposition", "")
-                                )[-1].get("size", 0)
+                                ).get_param("size", 0)
                             )
 
                 total_size += asset["size"]
 
         progress_callback.reset(total=total_size)
         error_messages = set()
 
@@ -643,21 +644,21 @@
                     error_messages.add(str(e))
                 else:
                     asset_rel_path = urlparse(asset["href"]).path.strip("/")
                     asset_rel_dir = os.path.dirname(asset_rel_path)
 
                     if not asset.get("filename", None):
                         # try getting filename in GET header if was not found in HEAD result
-                        asset_content_disposition_dict = stream.headers.get(
+                        asset_content_disposition = stream.headers.get(
                             "content-disposition", None
                         )
-                        if asset_content_disposition_dict:
+                        if asset_content_disposition:
                             asset["filename"] = parse_header(
-                                asset_content_disposition_dict
-                            )[-1].get("filename", None)
+                                asset_content_disposition
+                            ).get_param("filename", None)
 
                     if not asset.get("filename", None):
                         # default filename extracted from path
                         asset["filename"] = os.path.basename(asset_rel_path)
 
                     asset_abs_path = os.path.join(
                         fs_dir_path, asset_rel_dir, asset["filename"]
```

### Comparing `eodag-2.9.1/eodag/plugins/download/s3rest.py` & `eodag-2.9.2/eodag/plugins/download/s3rest.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/manager.py` & `eodag-2.9.2/eodag/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/search/__init__.py` & `eodag-2.9.2/eodag/plugins/search/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/search/base.py` & `eodag-2.9.2/eodag/plugins/search/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from eodag.api.product.metadata_mapping import (
     DEFAULT_METADATA_MAPPING,
-    mtd_cfg_as_jsonpath,
+    mtd_cfg_as_conversion_and_querypath,
 )
 from eodag.plugins.base import PluginTopic
 
 
 class Search(PluginTopic):
     """Base Search Plugin.
 
@@ -36,22 +36,18 @@
         super(Search, self).__init__(provider, config)
         # Prepare the metadata mapping
         # Do a shallow copy, the structure is flat enough for this to be sufficient
         metas = DEFAULT_METADATA_MAPPING.copy()
         # Update the defaults with the mapping value. This will add any new key
         # added by the provider mapping that is not in the default metadata
         metas.update(self.config.metadata_mapping)
-        # common_jsonpath usage to optimize jsonpath build process
-        mtd_cfg_as_jsonpath_options = {}
-        if hasattr(self.config, "common_metadata_mapping_path"):
-            mtd_cfg_as_jsonpath_options[
-                "common_jsonpath"
-            ] = self.config.common_metadata_mapping_path
-        self.config.metadata_mapping = mtd_cfg_as_jsonpath(
-            metas, self.config.metadata_mapping, **mtd_cfg_as_jsonpath_options
+        self.config.metadata_mapping = mtd_cfg_as_conversion_and_querypath(
+            metas,
+            self.config.metadata_mapping,
+            result_type=getattr(self.config, "result_type", "json"),
         )
 
     def clear(self):
         """Method used to clear a search context between two searches."""
         pass
 
     def query(self, *args, count=True, **kwargs):
```

### Comparing `eodag-2.9.1/eodag/plugins/search/build_search_result.py` & `eodag-2.9.2/eodag/plugins/search/build_search_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
-import json
 import logging
 
 import geojson
+import orjson
 from jsonpath_ng import Fields
 
 from eodag.api.product import EOProduct
 from eodag.api.product.metadata_mapping import (
     NOT_AVAILABLE,
     NOT_MAPPED,
     properties_from_json,
@@ -99,15 +99,15 @@
 
         # update result with query parameters without pagination (or search-only params)
         if isinstance(self.config.pagination["next_page_query_obj"], str) and hasattr(
             self, "query_params_unpaginated"
         ):
             unpaginated_query_params = self.query_params_unpaginated
         elif isinstance(self.config.pagination["next_page_query_obj"], str):
-            next_page_query_obj = json.loads(
+            next_page_query_obj = orjson.loads(
                 self.config.pagination["next_page_query_obj"].format()
             )
             unpaginated_query_params = {
                 k: v
                 for k, v in self.query_params.items()
                 if (k, v) not in next_page_query_obj.items()
             }
```

### Comparing `eodag-2.9.1/eodag/plugins/search/csw.py` & `eodag-2.9.2/eodag/plugins/search/csw.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/plugins/search/qssearch.py` & `eodag-2.9.2/eodag/plugins/search/qssearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
 import logging
 import re
-from urllib.error import HTTPError as urllib_HTTPError
+from urllib.error import URLError
 from urllib.request import Request, urlopen
 
+import orjson
 import requests
 from lxml import etree
 
 from eodag.api.product import EOProduct
 from eodag.api.product.metadata_mapping import (
     NOT_AVAILABLE,
     NOT_MAPPED,
     format_metadata,
-    get_metadata_path_value,
     get_search_param,
-    mtd_cfg_as_jsonpath,
+    mtd_cfg_as_conversion_and_querypath,
     properties_from_json,
     properties_from_xml,
 )
 from eodag.plugins.search.base import Search
 from eodag.utils import (
     GENERIC_PRODUCT_TYPE,
     USER_AGENT,
-    cached_parse,
+    _deprecated,
     dict_items_recursive_apply,
     format_dict_items,
     quote,
+    string_to_jsonpath,
     update_nested_dict,
     urlencode,
 )
 from eodag.utils.exceptions import AuthenticationError, MisconfiguredError, RequestError
 from eodag.utils.stac_reader import HTTP_REQ_TIMEOUT
 
 logger = logging.getLogger("eodag.plugins.search.qssearch")
@@ -162,14 +162,87 @@
         self.config.__dict__.setdefault("free_text_search_operations", {})
         self.search_urls = []
         self.query_params = dict()
         self.query_string = ""
         self.next_page_url = None
         self.next_page_query_obj = None
         self.next_page_merge = None
+        # parse jsonpath on init: pagination
+        if (
+            self.config.result_type == "json"
+            and "total_items_nb_key_path" in self.config.pagination
+        ):
+            self.config.pagination["total_items_nb_key_path"] = string_to_jsonpath(
+                self.config.pagination["total_items_nb_key_path"]
+            )
+        if (
+            self.config.result_type == "json"
+            and "next_page_url_key_path" in self.config.pagination
+        ):
+            self.config.pagination["next_page_url_key_path"] = string_to_jsonpath(
+                self.config.pagination.get("next_page_url_key_path", None)
+            )
+        if (
+            self.config.result_type == "json"
+            and "next_page_query_obj_key_path" in self.config.pagination
+        ):
+            self.config.pagination["next_page_query_obj_key_path"] = string_to_jsonpath(
+                self.config.pagination.get("next_page_query_obj_key_path", None)
+            )
+        if (
+            self.config.result_type == "json"
+            and "next_page_merge_key_path" in self.config.pagination
+        ):
+            self.config.pagination["next_page_merge_key_path"] = string_to_jsonpath(
+                self.config.pagination.get("next_page_merge_key_path", None)
+            )
+
+        # parse jsonpath on init: product types discovery
+        if (
+            getattr(self.config, "discover_product_types", {}).get(
+                "results_entry", None
+            )
+            and getattr(self.config, "discover_product_types", {}).get(
+                "result_type", None
+            )
+            == "json"
+        ):
+            self.config.discover_product_types["results_entry"] = string_to_jsonpath(
+                self.config.discover_product_types["results_entry"], force=True
+            )
+            self.config.discover_product_types[
+                "generic_product_type_id"
+            ] = mtd_cfg_as_conversion_and_querypath(
+                {"foo": self.config.discover_product_types["generic_product_type_id"]}
+            )[
+                "foo"
+            ]
+            self.config.discover_product_types[
+                "generic_product_type_parsable_properties"
+            ] = mtd_cfg_as_conversion_and_querypath(
+                self.config.discover_product_types[
+                    "generic_product_type_parsable_properties"
+                ]
+            )
+            self.config.discover_product_types[
+                "generic_product_type_parsable_metadata"
+            ] = mtd_cfg_as_conversion_and_querypath(
+                self.config.discover_product_types[
+                    "generic_product_type_parsable_metadata"
+                ]
+            )
+
+        # parse jsonpath on init: product type specific metadata-mapping
+        for product_type in self.config.products.keys():
+            if "metadata_mapping" in self.config.products[product_type].keys():
+                self.config.products[product_type][
+                    "metadata_mapping"
+                ] = mtd_cfg_as_conversion_and_querypath(
+                    self.config.products[product_type]["metadata_mapping"]
+                )
 
     def clear(self):
         """Clear search context"""
         super().clear()
         self.search_urls.clear()
         self.query_params.clear()
         self.query_string = ""
@@ -199,66 +272,59 @@
         else:
             try:
                 if self.config.discover_product_types["result_type"] == "json":
                     resp_as_json = response.json()
                     # extract results from response json
                     result = [
                         match.value
-                        for match in cached_parse(
-                            self.config.discover_product_types["results_entry"]
-                        ).find(resp_as_json)
+                        for match in self.config.discover_product_types[
+                            "results_entry"
+                        ].find(resp_as_json)
                     ]
 
                     conf_update_dict = {
                         "providers_config": {},
                         "product_types_config": {},
                     }
 
                     for product_type_result in result:
                         # providers_config extraction
-                        mapping_config = {}
-                        mapping_config = mtd_cfg_as_jsonpath(
+                        extracted_mapping = properties_from_json(
+                            product_type_result,
                             dict(
                                 self.config.discover_product_types[
                                     "generic_product_type_parsable_properties"
                                 ],
                                 **{
                                     "generic_product_type_id": self.config.discover_product_types[
                                         "generic_product_type_id"
                                     ]
                                 },
                             ),
-                            mapping_config,
-                        )
-
-                        extracted_mapping = properties_from_json(
-                            product_type_result, mapping_config
                         )
                         generic_product_type_id = extracted_mapping.pop(
                             "generic_product_type_id"
                         )
                         conf_update_dict["providers_config"][
                             generic_product_type_id
                         ] = dict(
                             extracted_mapping,
                             **self.config.discover_product_types.get(
                                 "generic_product_type_unparsable_properties", {}
                             ),
                         )
                         # product_types_config extraction
-                        mapping_config = {}
-                        mapping_config = mtd_cfg_as_jsonpath(
+                        conf_update_dict["product_types_config"][
+                            generic_product_type_id
+                        ] = properties_from_json(
+                            product_type_result,
                             self.config.discover_product_types[
                                 "generic_product_type_parsable_metadata"
                             ],
-                            mapping_config,
                         )
-                        conf_update_dict["product_types_config"][
-                            generic_product_type_id
-                        ] = properties_from_json(product_type_result, mapping_config)
 
                         # update keywords
                         keywords_fields = [
                             "instrument",
                             "platform",
                             "platformSerialIdentifier",
                             "processingLevel",
@@ -347,26 +413,22 @@
         other_product_for_mapping = self.product_type_def_params.get(
             "metadata_mapping_from_product", ""
         )
         if other_product_for_mapping:
             other_product_type_def_params = self.get_product_type_def_params(
                 other_product_for_mapping, **kwargs
             )
-            self.update_metadata_mapping(
+            self.config.metadata_mapping.update(
                 other_product_type_def_params.get("metadata_mapping", {})
             )
         # from current product
-        self.update_metadata_mapping(
+        self.config.metadata_mapping.update(
             self.product_type_def_params.get("metadata_mapping", {})
         )
 
-        # Add to the query, the queryable parameters set in the provider product type definition
-        self.product_type_def_params = self.get_product_type_def_params(
-            product_type, **kwargs
-        )
         # if product_type_def_params is set, remove product_type as it may conflict with this conf
         if self.product_type_def_params:
             keywords.pop("productType", None)
         keywords.update(
             {
                 k: v
                 for k, v in self.product_type_def_params.items()
@@ -391,35 +453,21 @@
         provider_results = self.do_search(items_per_page=items_per_page, **kwargs)
         if count and total_items is None and hasattr(self, "total_items_nb"):
             total_items = self.total_items_nb
         eo_products = self.normalize_results(provider_results, **kwargs)
         total_items = len(eo_products) if total_items == 0 else total_items
         return eo_products, total_items
 
+    @_deprecated(
+        reason="Simply run `self.config.metadata_mapping.update(metadata_mapping)` instead",
+        version="2.10.0",
+    )
     def update_metadata_mapping(self, metadata_mapping):
         """Update plugin metadata_mapping with input metadata_mapping configuration"""
         self.config.metadata_mapping.update(metadata_mapping)
-        unparsed_metadata = {
-            k: v
-            for k, v in metadata_mapping.items()
-            if isinstance(get_metadata_path_value(self.config.metadata_mapping[k]), str)
-        }
-        # common_jsonpath usage to optimize jsonpath build process
-        # On error, assume the mapping is to be passed as is. Ignore any transformation specified.
-        #   If a value is to be passed as is, we don't want to transform it further
-        mtd_cfg_as_jsonpath_options = {"keep_conversion": False}
-        if hasattr(self.config, "common_metadata_mapping_path"):
-            mtd_cfg_as_jsonpath_options[
-                "common_jsonpath"
-            ] = self.config.common_metadata_mapping_path
-        self.config.metadata_mapping = mtd_cfg_as_jsonpath(
-            unparsed_metadata,
-            self.config.metadata_mapping,
-            **mtd_cfg_as_jsonpath_options,
-        )
 
     def build_query_string(self, product_type, **kwargs):
         """Build The query string using the search parameters"""
         logger.debug("Building the query string that will be used for search")
 
         if "raise_errors" in kwargs.keys():
             del kwargs["raise_errors"]
@@ -439,15 +487,15 @@
                 if len(parts) == 1:
                     formatted_query_param = format_metadata(
                         provider_search_key, product_type, **kwargs
                     )
                     if "{{" in provider_search_key:
                         # json query string (for POST request)
                         update_nested_dict(
-                            query_params, json.loads(formatted_query_param)
+                            query_params, orjson.loads(formatted_query_param)
                         )
                     else:
                         query_params[eodag_search_key] = formatted_query_param
                 else:
                     provider_search_key, provider_value = parts
                     query_params.setdefault(provider_search_key, []).append(
                         format_metadata(provider_value, product_type, **kwargs)
@@ -626,17 +674,17 @@
         :param items_per_page: (optional) The number of items to return for one page
         :type items_per_page: int
         """
         if getattr(self, "need_count", False):
             # extract total_items_nb from search results
             total_items_nb = 0
             if self.config.result_type == "json":
-                total_items_nb_key_path_parsed = cached_parse(
-                    self.config.pagination["total_items_nb_key_path"]
-                )
+                total_items_nb_key_path_parsed = self.config.pagination[
+                    "total_items_nb_key_path"
+                ]
 
         results = []
         for search_url in self.search_urls:
             response = self._request(
                 search_url,
                 info_message="Sending search request: {}".format(search_url),
                 exception_message="Skipping error while searching for {} {} "
@@ -683,35 +731,35 @@
                     except IndexError:
                         logger.debug(
                             "Could not extract total_items_nb from search results"
                         )
             else:
                 resp_as_json = response.json()
                 if next_page_url_key_path:
-                    path_parsed = cached_parse(next_page_url_key_path)
+                    path_parsed = next_page_url_key_path
                     try:
                         self.next_page_url = path_parsed.find(resp_as_json)[0].value
                         logger.debug(
                             "Next page URL collected and set for the next search",
                         )
                     except IndexError:
                         logger.debug("Next page URL could not be collected")
                 if next_page_query_obj_key_path:
-                    path_parsed = cached_parse(next_page_query_obj_key_path)
+                    path_parsed = next_page_query_obj_key_path
                     try:
                         self.next_page_query_obj = path_parsed.find(resp_as_json)[
                             0
                         ].value
                         logger.debug(
                             "Next page Query-object collected and set for the next search",
                         )
                     except IndexError:
                         logger.debug("Next page Query-object could not be collected")
                 if next_page_merge_key_path:
-                    path_parsed = cached_parse(next_page_merge_key_path)
+                    path_parsed = next_page_merge_key_path
                     try:
                         self.next_page_merge = path_parsed.find(resp_as_json)[0].value
                         logger.debug(
                             "Next page merge collected and set for the next search",
                         )
                     except IndexError:
                         logger.debug("Next page merge could not be collected")
@@ -788,17 +836,15 @@
                 self.config.pagination["total_items_nb_key_path"],
                 namespaces={k or "ns": v for k, v in root_node.nsmap.items()},
             )[0]
             total_results = int(total_nb_results)
         else:
             count_results = response.json()
             if isinstance(count_results, dict):
-                path_parsed = cached_parse(
-                    self.config.pagination["total_items_nb_key_path"]
-                )
+                path_parsed = self.config.pagination["total_items_nb_key_path"]
                 total_results = path_parsed.find(count_results)[0].value
             else:  # interpret the result as a raw int
                 total_results = int(count_results)
         return total_results
 
     def get_collections(self, **kwargs):
         """Get the collection to which the product belongs"""
@@ -851,15 +897,15 @@
             logger.debug(
                 "Getting provider product type definition parameters for %s",
                 product_type,
             )
             return self.config.products[product_type]
         elif GENERIC_PRODUCT_TYPE in self.config.products.keys():
             logger.debug(
-                "Getting genric provider product type definition parameters for %s",
+                "Getting generic provider product type definition parameters for %s",
                 product_type,
             )
             return {
                 k: v
                 for k, v in format_dict_items(
                     self.config.products[GENERIC_PRODUCT_TYPE], **kwargs
                 ).items()
@@ -912,15 +958,15 @@
             else:
                 if info_message:
                     logger.info(info_message)
                 response = requests.get(
                     url, timeout=HTTP_REQ_TIMEOUT, headers=USER_AGENT, **kwargs
                 )
                 response.raise_for_status()
-        except (requests.RequestException, urllib_HTTPError) as err:
+        except (requests.RequestException, URLError) as err:
             err_msg = err.readlines() if hasattr(err, "readlines") else ""
             if exception_message:
                 logger.exception("%s %s" % (exception_message, err_msg))
             else:
                 logger.exception(
                     "Skipping error while requesting: %s (provider:%s, plugin:%s): %s",
                     url,
@@ -958,14 +1004,27 @@
         return normalized
 
 
 class ODataV4Search(QueryStringSearch):
     """A specialisation of a QueryStringSearch that does a two step search to retrieve
     all products metadata"""
 
+    def __init__(self, provider, config):
+        super(ODataV4Search, self).__init__(provider, config)
+
+        # parse jsonpath on init
+        metadata_pre_mapping = getattr(self.config, "metadata_pre_mapping", {})
+        metadata_path = metadata_pre_mapping.get("metadata_path", None)
+        metadata_path_id = metadata_pre_mapping.get("metadata_path_id", None)
+        metadata_path_value = metadata_pre_mapping.get("metadata_path_value", None)
+        if metadata_path and metadata_path_id and metadata_path_value:
+            self.config.metadata_pre_mapping["metadata_path"] = string_to_jsonpath(
+                metadata_path
+            )
+
     def do_search(self, *args, **kwargs):
         """A two step search can be performed if the metadata are not given into the search result"""
 
         if getattr(self.config, "per_product_metadata_query", False):
             final_result = []
             # Query the products entity set for basic metadata about the product
             for entity in super(ODataV4Search, self).do_search(*args, **kwargs):
@@ -1005,15 +1064,16 @@
         """
         metadata_pre_mapping = getattr(self.config, "metadata_pre_mapping", {})
         metadata_path = metadata_pre_mapping.get("metadata_path", None)
         metadata_path_id = metadata_pre_mapping.get("metadata_path_id", None)
         metadata_path_value = metadata_pre_mapping.get("metadata_path_value", None)
 
         if metadata_path and metadata_path_id and metadata_path_value:
-            parsed_metadata_path = cached_parse(metadata_path)
+            # metadata_path already parsed on init
+            parsed_metadata_path = metadata_path
             for result in results:
                 found_metadata = parsed_metadata_path.find(result)
                 if found_metadata:
                     metadata_update = {}
                     for metadata_dict in found_metadata[0].value:
                         metada_id = metadata_dict[metadata_path_id]
                         metada_value = metadata_dict[metadata_path_value]
@@ -1052,19 +1112,19 @@
         other_product_for_mapping = self.product_type_def_params.get(
             "metadata_mapping_from_product", ""
         )
         if other_product_for_mapping:
             other_product_type_def_params = self.get_product_type_def_params(
                 other_product_for_mapping, **kwargs
             )
-            self.update_metadata_mapping(
+            self.config.metadata_mapping.update(
                 other_product_type_def_params.get("metadata_mapping", {})
             )
         # from current product
-        self.update_metadata_mapping(
+        self.config.metadata_mapping.update(
             self.product_type_def_params.get("metadata_mapping", {})
         )
 
         # Add to the query, the queryable parameters set in the provider product type definition
         keywords.update(
             {
                 k: v
@@ -1137,15 +1197,15 @@
 
         if "count_endpoint" not in self.config.pagination:
             # if count_endpoint is not set, total_results should be extracted from search result
             total_results = None
             self.need_count = True
             self.total_items_nb = None
 
-        if hasattr(kwargs["auth"], "config"):
+        if "auth" in kwargs and hasattr(kwargs["auth"], "config"):
             auth_conf_dict = getattr(kwargs["auth"].config, "credentials", {})
         else:
             auth_conf_dict = {}
         for collection in self.get_collections(**kwargs):
             try:
                 search_endpoint = self.config.api_endpoint.rstrip("/").format(
                     **dict(collection=collection, **auth_conf_dict)
@@ -1175,15 +1235,15 @@
                     ].format(
                         items_per_page=items_per_page,
                         page=page,
                         skip=(page - 1) * items_per_page,
                         skip_base_1=(page - 1) * items_per_page + 1,
                     )
                     update_nested_dict(
-                        self.query_params, json.loads(next_page_query_obj)
+                        self.query_params, orjson.loads(next_page_query_obj)
                     )
 
             urls.append(search_endpoint)
         return urls, total_results
 
     def _request(self, url, info_message=None, exception_message=None):
         try:
@@ -1206,15 +1266,15 @@
                 url,
                 json=self.query_params,
                 headers=USER_AGENT,
                 timeout=HTTP_REQ_TIMEOUT,
                 **kwargs,
             )
             response.raise_for_status()
-        except (requests.RequestException, urllib_HTTPError) as err:
+        except (requests.RequestException, URLError) as err:
             # check if error is identified as auth_error in provider conf
             auth_errors = getattr(self.config, "auth_error_code", [None])
             if not isinstance(auth_errors, list):
                 auth_errors = [auth_errors]
             if (
                 hasattr(err.response, "status_code")
                 and err.response.status_code in auth_errors
```

### Comparing `eodag-2.9.1/eodag/plugins/search/static_stac_search.py` & `eodag-2.9.2/eodag/plugins/search/static_stac_search.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/locations_conf_template.yml` & `eodag-2.9.2/eodag/resources/locations_conf_template.yml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/product_types.yml` & `eodag-2.9.2/eodag/resources/product_types.yml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/providers.yml` & `eodag-2.9.2/eodag/resources/providers.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
   api: !plugin
     type: UsgsApi
     need_auth: true
     google_base_url: 'http://storage.googleapis.com/earthengine-public/landsat/'
     pagination:
       max_items_per_page: 5000
       total_items_nb_key_path: '$.totalHits'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       id: '$.displayId'
       geometry: '$.spatialBounds'
       productType: '$.productType'
       title: '$.displayId'
       abstract: '$.summary'
       cloudCover: '$.cloudCover'
@@ -106,15 +105,14 @@
       max_items_per_page: 500
     query_params_key: 'search'
     discover_metadata:
       auto_discovery: true
       metadata_pattern: '^[a-zA-Z0-9_]+$'
       search_param: '{{{{"search":{{{{"{metadata}":"{{{metadata}}}" }}}} }}}}'
       metadata_path: '$.*'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       # landsat8_downloadLink : 's3://landsat-pds/c{storedInCollection}/L8/{path}/{row}/{productID}'
       geometry:
         - '{{"search":{{"shape": {geometry#to_geojson} }} }}'
         - '$.dataGeometry'
       # storageStatus set to ONLINE for consistency between providers
       storageStatus: '{$.null#replace_str("Not Available","ONLINE")}'
@@ -556,15 +554,14 @@
       # 2021/03/19: Returns a 400 error code if greater than 500.
       max_items_per_page: 500
     discover_metadata:
       auto_discovery: true
       metadata_pattern: '^(?!collection)[a-zA-Z0-9_]+$'
       search_param: '{metadata}={{{metadata}}}'
       metadata_path: '$.properties.*'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       # Opensearch resource identifier within the search engine context (in our case
       # within the context of the data provider)
       uid: '$.id'
       # OpenSearch Parameters for Collection Search (Table 3)
       productType:
         - productType
@@ -732,15 +729,14 @@
       # 2021/03/19: 500 is the max, no error if greater
       max_items_per_page: 500
     discover_metadata:
       auto_discovery: true
       metadata_pattern: '^(?!collection)[a-zA-Z0-9_]+$'
       search_param: '{metadata}={{{metadata}}}'
       metadata_path: '$.properties.*'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       # Opensearch resource identifier within the search engine context (in our case
       # within the context of the data provider)
       uid: '$.id'
       # OpenSearch Parameters for Collection Search (Table 3)
       productType:
         - productType
@@ -821,15 +817,15 @@
         - '$.geometry'
       # The url of the quicklook
       quicklook: '$.properties.quicklook'
       # The url to download the product "as is" (literal or as a template to be completed either after the search result
       # is obtained from the provider or during the eodag download phase)
       downloadLink: '$.properties.services.download.url'
       # storageStatus: must be one of ONLINE, STAGING, OFFLINE
-      storageStatus: '{$.properties.storage.mode#get_group_name((?P<ONLINE>disk)|(?P<STAGING>staging)|(?P<OFFLINE>tape))}'
+      storageStatus: '{$.properties.storage.mode#get_group_name((?P<ONLINE>disk|tier2)|(?P<STAGING>staging)|(?P<OFFLINE>unknown|tape|tier3))}'
 
       # Additional metadata provided by the providers but that don't appear in the reference spec
       thumbnail: '$.properties.thumbnail'
 
   products:
     S1_SAR_OCN:
       productType: OCN
@@ -918,19 +914,18 @@
       search_param:
         free_text_search_operations:
           $filter:
             operations:
               and:
                 -  "Attributes/OData.CSC.StringAttribute/any(att:att/Name eq '{metadata}' and att/OData.CSC.StringAttribute/Value eq '{{{metadata}}}')"
       metadata_path: '$.Attributes.*'
-    common_metadata_mapping_path: '$'
     discover_product_types:
       fetch_url: 'https://datahub.creodias.eu/stac/collections'
       result_type: json
-      results_entry: 'collections[*]'
+      results_entry: '$.collections[*]'
       generic_product_type_id: '$.id'
       generic_product_type_parsable_properties:
         collection: '$.id'
       generic_product_type_parsable_metadata:
         abstract: '$.description'
         instrument: '{$.summaries.instruments#csv_list}'
         platform: '{$.summaries.constellation#csv_list}'
@@ -1621,15 +1616,14 @@
                 - '{metadata}:{{{metadata}}}'
       metadata_path: '$.Metadata.*'
     per_product_metadata_query: false
     metadata_pre_mapping:
       metadata_path: '$.Metadata'
       metadata_path_id: 'id'
       metadata_path_value: 'value'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       # Opensearch resource identifier within the search engine context (in our case
       # within the context of the data provider)
       # Queryable parameters are set with null as 1st configuration list value to mark them as queryable,
       #   but `free_text_search_operations.$search.operations.AND` entries are then used instead.
       uid: '$.id'
       # OpenSearch Parameters for Collection Search (Table 3)
@@ -2018,15 +2012,15 @@
   description: Earth Search
   url: https://www.element84.com/earth-search/
   search: !plugin
     type: StacSearch
     api_endpoint: https://earth-search.aws.element84.com/v0/search
     need_auth: false
     discover_product_types:
-      results_entry: 'collections[?id!="sentinel-s2-l2a-cogs"]'
+      results_entry: '$.collections[?id!="sentinel-s2-l2a-cogs"]'
     pagination:
       # Override the default next page url key path of StacSearch because the next link returned
       # by Earth Search is invalid (as of 2021/04/29). Entry set to null (None) to avoid using the
       # next page retrieval mechanism, `next_page_url_tpl` will be used instead (inherited from StacSearch)
       # Remove that entry if Earth Search updates that and returns a valid link.
       next_page_url_key_path: null
       # 2021/04/28: Earth-Search relies on Sat-API whose docs (http://sat-utils.github.io/sat-api/#search-stac-items-by-simple-filtering-)
@@ -2173,15 +2167,14 @@
   roles:
     - host
   url: https://www.ecmwf.int
   api: !plugin
     type: EcmwfApi
     api_endpoint: https://api.ecmwf.int/v1
     extract: false
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       productType: '$.productType'
       title: '$.id'
       startTimeFromAscendingNode: '{$.startTimeFromAscendingNode#to_iso_date}'
       completionTimeFromAscendingNode:
         - 'date={startTimeFromAscendingNode#to_iso_date}/to/{completionTimeFromAscendingNode#to_iso_date(-1,)}'
         - '{$.completionTimeFromAscendingNode#to_iso_date}'
@@ -2396,15 +2389,14 @@
   roles:
     - host
   url: https://ads.atmosphere.copernicus.eu/
   api: !plugin
     type: CdsApi
     api_endpoint: https://ads.atmosphere.copernicus.eu/api/v2
     extract: false
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       productType: '$.productType'
       title: '$.id'
       startTimeFromAscendingNode: '{$.startTimeFromAscendingNode#to_iso_date}'
       completionTimeFromAscendingNode:
         - 'date={startTimeFromAscendingNode#to_iso_date}/{completionTimeFromAscendingNode#to_iso_date(-1,)}'
         - '{$.completionTimeFromAscendingNode#to_iso_date}'
@@ -2714,15 +2706,14 @@
   roles:
     - host
   url: https://cds.climate.copernicus.eu/
   api: !plugin
     type: CdsApi
     api_endpoint: https://cds.climate.copernicus.eu/api/v2
     extract: false
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       productType: '$.productType'
       title: '$.id'
       startTimeFromAscendingNode: '{$.startTimeFromAscendingNode#to_iso_date}'
       completionTimeFromAscendingNode:
         - 'date={startTimeFromAscendingNode#to_iso_date}/{completionTimeFromAscendingNode#to_iso_date(-1,)}'
         - '{$.completionTimeFromAscendingNode#to_iso_date}'
@@ -2966,15 +2957,14 @@
       # 2021/03/19: 500 is the max, no error if greater
       max_items_per_page: 500
     discover_metadata:
       auto_discovery: true
       metadata_pattern: '^(?!collection)[a-zA-Z0-9_]+$'
       search_param: '{metadata}={{{metadata}}}'
       metadata_path: '$.properties.*'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       # Opensearch resource identifier within the search engine context (in our case
       # within the context of the data provider)
       uid: '$.id'
       # OpenSearch Parameters for Collection Search (Table 3)
       productType:
         - productType
@@ -3230,15 +3220,14 @@
     pagination:
       next_page_query_obj: '{{"checkOnly":true}}'
     discover_metadata:
       auto_discovery: true
       metadata_pattern: '^[a-zA-Z0-9_]+$'
       search_param: '{{{{"{metadata}":{{{metadata}#to_geojson}} }}}}'
       metadata_path: '$.*'
-    common_metadata_mapping_path: '$'
     metadata_mapping:
       startTimeFromAscendingNode: '{$.startTimeFromAscendingNode#to_iso_utc_datetime}'
       completionTimeFromAscendingNode:
         - '{{"timeIntervals": [ "{startTimeFromAscendingNode#to_iso_date}/{completionTimeFromAscendingNode#to_iso_date(-1,)}" ] }}'
         - '{$.completionTimeFromAscendingNode#to_iso_utc_datetime}'
       geometry:
         - '{{"geometry": {geometry#to_geojson} }}'
@@ -3351,15 +3340,14 @@
       search_param:
         free_text_search_operations:
           $filter:
             operations:
               and:
                 -  "Attributes/OData.CSC.StringAttribute/any(att:att/Name eq '{metadata}' and att/OData.CSC.StringAttribute/Value eq '{{{metadata}}}')"
       metadata_path: '$.Attributes.*'
-    common_metadata_mapping_path: '$'
     per_product_metadata_query: false
     metadata_pre_mapping:
       metadata_path: '$.Attributes'
       metadata_path_id: 'Name'
       metadata_path_value: 'Value'
     metadata_mapping:
       # Opensearch resource identifier within the search engine context (in our case
@@ -3619,7 +3607,47 @@
       collection: SENTINEL-5P
     S5P_L2_SO2:
       productType: L2__SO2___
       collection: SENTINEL-5P
     GENERIC_PRODUCT_TYPE:
       productType: '{productType}'
       collection: '{collection}'
+---
+!provider
+  name: planetary_computer
+  priority: 0
+  roles:
+    - host
+  description: Planetary Computer
+  url:  https://planetarycomputer.microsoft.com
+  search: !plugin
+    type: StacSearch
+    api_endpoint: https://planetarycomputer.microsoft.com/api/stac/v1/search
+    need_auth: false
+    pagination:
+      max_items_per_page: 1000
+  products:
+    S1_SAR_GRD:
+      productType: sentinel-1-grd
+    S2_MSI_L2A:
+      productType: sentinel-2-l2a
+    LANDSAT_C2L1:
+      productType: landsat-c2-l1
+    LANDSAT_C2L2:
+      productType: landsat-c2-l2
+    MODIS_MCD43A4:
+      productType: modis-43A4-061
+    NAIP:
+      productType: naip
+    GENERIC_PRODUCT_TYPE:
+      productType: '{productType}'
+  download: !plugin
+    type: HTTPDownload
+    base_uri: 'https://planetarycomputer.microsoft.com/api/stac/download'
+    flatten_top_dirs: True
+    auth_error_code: 403
+  auth: !plugin
+    type: SASAuth
+    auth_uri: 'https://planetarycomputer.microsoft.com/api/sas/v1/sign?href={url}'
+    signed_url_key: href
+    headers:
+      Ocp-Apim-Subscription-Key: "{apikey}"
```

### Comparing `eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.dbf` & `eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.dbf`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.shp` & `eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.shp`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/shp/ne_110m_admin_0_map_units.shx` & `eodag-2.9.2/eodag/resources/shp/ne_110m_admin_0_map_units.shx`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/stac.yml` & `eodag-2.9.2/eodag/resources/stac.yml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/stac_api.yml` & `eodag-2.9.2/eodag/resources/stac_api.yml`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/resources/stac_provider.yml` & `eodag-2.9.2/eodag/resources/stac_provider.yml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     auto_discovery: true
     metadata_pattern: '^[a-zA-Z0-9_:-]+$'
     search_param: '{{{{"query":{{{{"{metadata}":{{{{"eq":"{{{metadata}}}" }}}} }}}} }}}}'
     metadata_path: '$.properties.*'
   discover_product_types:
       fetch_url: '{api_endpoint}/../collections'
       result_type: json
-      results_entry: 'collections[*]'
+      results_entry: '$.collections[*]'
       generic_product_type_id: '$.id'
       generic_product_type_parsable_properties:
         productType: '$.id'
       generic_product_type_parsable_metadata:
         abstract: '$.description'
         instrument: '{$.summaries.instruments#csv_list}'
         platform: '{$.summaries.constellation#csv_list}'
```

### Comparing `eodag-2.9.1/eodag/resources/user_conf_template.yml` & `eodag-2.9.2/eodag/resources/user_conf_template.yml`

 * *Files 2% similar despite different names*

```diff
@@ -178,7 +178,15 @@
     download:
         extract:
         outputs_prefix:
     auth:
         credentials:
             username:
             password:
+planetary_computer:
+    priority: # Lower value means lower priority (Default: 0)
+    search:   # Search parameters configuration
+    auth:
+        credentials:
+            apikey:
+    download:
+        outputs_prefix:
```

### Comparing `eodag-2.9.1/eodag/rest/__init__.py` & `eodag-2.9.2/eodag/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/rest/server.py` & `eodag-2.9.2/eodag/rest/server.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/rest/stac.py` & `eodag-2.9.2/eodag/rest/stac.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import copy
 import datetime
 import logging
 import os
 import re
 from collections import defaultdict
 
 import dateutil.parser
@@ -31,14 +30,15 @@
 
 from eodag.api.product.metadata_mapping import (
     DEFAULT_METADATA_MAPPING,
     format_metadata,
     get_metadata_path,
 )
 from eodag.utils import (
+    deepcopy,
     dict_items_recursive_apply,
     format_dict_items,
     jsonpath_parse_dict_items,
     string_to_jsonpath,
     update_nested_dict,
 )
 from eodag.utils.exceptions import (
@@ -46,15 +46,15 @@
     NoMatchingProductType,
     NotAvailableError,
     ValidationError,
 )
 
 logger = logging.getLogger("eodag.rest.stac")
 
-default_min_date = "2015-01-01"
+DEFAULT_MISSION_START_DATE = "2015-01-01T00:00:00Z"
 
 
 class StacCommon(object):
     """Stac common object
 
     :param url: Requested URL
     :type url: str
@@ -132,20 +132,18 @@
         :param extension: Extension name
         :type extension: str
         :param kwargs: Additional variables needed for parsing extension
         :type kwargs: Any
         :returns: STAC extension as dictionnary
         :rtype: dict
         """
-        extension_model = (
-            copy.deepcopy(stac_config).get("extensions", {}).get(extension, {})
-        )
+        extension_model = deepcopy(stac_config).get("extensions", {}).get(extension, {})
 
         # parse f-strings
-        format_args = copy.deepcopy(stac_config)
+        format_args = deepcopy(stac_config)
         format_args["extension"] = {
             "url": url,
             "properties": kwargs.get("properties", {}),
         }
         extension = format_dict_items(extension_model, **format_args)
 
         return extension
@@ -239,15 +237,15 @@
                 else:
                     product_item["properties"][prop_key] = format_metadata(
                         "{%s#%s}" % (formatable_prop_key, conv_func),
                         **{formatable_prop_key: product_item["properties"][prop_key]},
                     )
 
             # parse f-strings
-            format_args = copy.deepcopy(self.stac_config)
+            format_args = deepcopy(self.stac_config)
             format_args["catalog"] = catalog
             format_args["item"] = product_item
             product_item = format_dict_items(product_item, **format_args)
             product_item["bbox"] = [float(i) for i in product_item["bbox"]]
 
             # remove empty properties
             product_item = self.__filter_item_properties_values(product_item)
@@ -262,15 +260,15 @@
         :param search_results: EODAG search results
         :type search_results: :class:`~eodag.api.search_result.SearchResult`
         :param catalog: STAC catalog dict used for parsing item metadata
         :type catalog: dict
         :returns: Items dictionnary
         :rtype: dict
         """
-        items_model = copy.deepcopy(self.stac_config["items"])
+        items_model = deepcopy(self.stac_config["items"])
 
         search_results.numberMatched = search_results.properties["totalResults"]
         search_results.numberReturned = len(search_results)
 
         # next page link
         if "?" in self.url:
             # search endpoint: use page url as self link
@@ -302,15 +300,15 @@
         )
 
         # parse jsonpath
         items = jsonpath_parse_dict_items(
             items_model, {"search_results": search_results.__dict__}
         )
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = catalog
         items = format_dict_items(items, **format_args)
 
         # last page: remove next page link
         if (
             search_results.properties["itemsPerPage"]
             * search_results.properties["page"]
@@ -355,15 +353,15 @@
         except IndexError:
             raise MisconfiguredError(
                 "Product type {} not available for {}".format(
                     product_type, self.provider
                 )
             )
 
-        result_item_model = copy.deepcopy(item_model)
+        result_item_model = deepcopy(item_model)
         result_item_model["stac_extensions"] = list(
             self.stac_config["stac_extensions"].values()
         )
 
         # build jsonpath for eodag product default properties and adapt path
         eodag_properties_dict = {
             k: string_to_jsonpath(k, v.replace("$.", "$.product."))
@@ -401,15 +399,15 @@
         """Removes empty properties, unused extensions, and add missing extensions
 
         :param item: STAC item data
         :type item: dict
         :returns: Filtered item model
         :rtype: dict
         """
-        all_extensions_dict = copy.deepcopy(self.stac_config["stac_extensions"])
+        all_extensions_dict = deepcopy(self.stac_config["stac_extensions"])
         # parse f-strings with root
         all_extensions_dict = format_dict_items(
             all_extensions_dict, **{"catalog": {"root": self.root}}
         )
 
         item["stac_extensions"] = []
         # dict to list of keys to permit pop() while iterating
@@ -452,15 +450,15 @@
         )
 
         # parse jsonpath
         product_item = jsonpath_parse_dict_items(
             item_model, {"product": product.__dict__}
         )
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         # format_args["collection"] = dict(catalog.as_dict(), **{"url": catalog.url})
         format_args["catalog"] = dict(
             catalog.as_dict(), **{"url": catalog.url, "root": catalog.root}
         )
         format_args["item"] = product_item
         product_item = format_dict_items(product_item, **format_args)
         product_item["bbox"] = [float(i) for i in product_item["bbox"]]
@@ -534,15 +532,15 @@
         """Build STAC collections list
 
         :param filters: (optional) Additional filters for collections search
         :type filters: dict
         :returns: STAC collection dicts list
         :rtype: list
         """
-        collection_model = copy.deepcopy(self.stac_config["collection"])
+        collection_model = deepcopy(self.stac_config["collection"])
 
         product_types = self.__get_product_types(filters)
 
         collection_list = []
         for product_type in product_types:
             # get default provider for each product_type
             product_type_provider = (
@@ -565,15 +563,15 @@
                     "product_type": product_type,
                     "provider": self.eodag_api.providers_config[
                         product_type_provider
                     ].__dict__,
                 },
             )
             # parse f-strings
-            format_args = copy.deepcopy(self.stac_config)
+            format_args = deepcopy(self.stac_config)
             format_args["collection"] = dict(
                 product_type_collection, **{"url": self.url, "root": self.root}
             )
             product_type_collection = format_dict_items(
                 product_type_collection, **format_args
             )
 
@@ -585,15 +583,15 @@
         """Build STAC collections
 
         :param filters: (optional) Additional filters for collections search
         :type filters: dict
         :returns: Collections dictionnary
         :rtype: dict
         """
-        collections = copy.deepcopy(self.stac_config["collections"])
+        collections = deepcopy(self.stac_config["collections"])
         collections["collections"] = self.__get_collection_list(filters)
 
         collections["links"] += [
             {
                 "rel": "child",
                 "title": collec["id"],
                 "href": [
@@ -668,15 +666,15 @@
         )
         self.shp_location_config = eodag_api.locations_config
         self.search_args = {}
 
         self.data = {}
         self.children = []
 
-        self.catalog_config = copy.deepcopy(stac_config["catalog"])
+        self.catalog_config = deepcopy(stac_config["catalog"])
 
         self.__update_data_from_catalog_config({"model": {}})
 
         # expand links
         self.parent = "/".join(self.url.rstrip("/").split("/")[:-1])
         if self.parent != self.root:
             self.data["links"].append({"rel": "parent", "href": self.parent})
@@ -694,15 +692,15 @@
         """
         model = catalog_config["model"]
 
         self.catalog_config = update_nested_dict(self.catalog_config, catalog_config)
 
         # parse f-strings
         # defaultdict usage will return "" for missing keys in format_args
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = defaultdict(
             str, dict(model, **{"root": self.root, "url": self.url})
         )
         parsed_model = format_dict_items(self.catalog_config["model"], **format_args)
 
         self.update_data(parsed_model)
 
@@ -731,17 +729,17 @@
             url=self.url,
             stac_config=self.stac_config,
             provider=self.provider,
             eodag_api=self.eodag_api,
             root=self.root,
         ).get_collection_by_id(product_type)
 
-        cat_model = copy.deepcopy(self.stac_config["catalogs"]["product_type"]["model"])
+        cat_model = deepcopy(self.stac_config["catalogs"]["product_type"]["model"])
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = defaultdict(str, **self.data)
         format_args["collection"] = collection
         try:
             parsed_dict = format_dict_items(cat_model, **format_args)
         except Exception:
             logger.error("Could not format product_type catalog")
             raise
@@ -811,15 +809,15 @@
             [
                 extent_date_max,
                 dateutil.parser.parse("{}-01-01T00:00:00Z".format((year)))
                 + relativedelta(years=1),
             ]
         )
 
-        catalog_model = copy.deepcopy(self.stac_config["catalogs"]["year"]["model"])
+        catalog_model = deepcopy(self.stac_config["catalogs"]["year"]["model"])
 
         parsed_dict = self.set_stac_date(datetime_min, datetime_max, catalog_model)
 
         return parsed_dict
 
     def set_stac_month_by_id(self, month, **kwargs):
         """Updates and returns catalog with given month
@@ -842,15 +840,15 @@
             [
                 extent_date_max,
                 dateutil.parser.parse("{}-{}-01T00:00:00Z".format(year, month))
                 + relativedelta(months=1),
             ]
         )
 
-        catalog_model = copy.deepcopy(self.stac_config["catalogs"]["month"]["model"])
+        catalog_model = deepcopy(self.stac_config["catalogs"]["month"]["model"])
 
         parsed_dict = self.set_stac_date(datetime_min, datetime_max, catalog_model)
 
         return parsed_dict
 
     def set_stac_day_by_id(self, day, **kwargs):
         """Updates and returns catalog with given day
@@ -874,27 +872,29 @@
             [
                 extent_date_max,
                 dateutil.parser.parse("{}-{}-{}T00:00:00Z".format(year, month, day))
                 + relativedelta(days=1),
             ]
         )
 
-        catalog_model = copy.deepcopy(self.stac_config["catalogs"]["day"]["model"])
+        catalog_model = deepcopy(self.stac_config["catalogs"]["day"]["model"])
 
         parsed_dict = self.set_stac_date(datetime_min, datetime_max, catalog_model)
 
         return parsed_dict
 
     def get_datetime_extent(self):
         """Returns catalog temporal extent as datetime objs
 
         :returns: Start & stop dates
         :rtype: tuple
         """
-        extent_date_min = dateutil.parser.parse(default_min_date).replace(tzinfo=tz.UTC)
+        extent_date_min = dateutil.parser.parse(DEFAULT_MISSION_START_DATE).replace(
+            tzinfo=tz.UTC
+        )
         extent_date_max = datetime.datetime.now(datetime.timezone.utc).replace(
             tzinfo=tz.UTC
         )
         for interval in self.data["extent"]["temporal"]["interval"]:
             extent_date_min_str, extent_date_max_str = interval
             # date min
             if extent_date_min_str:
@@ -921,15 +921,15 @@
         :type datetime_max: :class:`datetime.datetime`
         :param catalog_model: Catalog model to use, from yml stac_config[catalogs]
         :type catalog_model: dict
         :returns: Updated catalog
         :rtype: dict
         """
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = defaultdict(str, **self.data)
         format_args["date"] = defaultdict(
             str,
             {
                 "year": datetime_min.year,
                 "month": datetime_min.month,
                 "day": datetime_min.day,
@@ -964,17 +964,17 @@
         """Updates and returns catalog with given max cloud_cover
 
         :param cloud_cover: Cloud_cover number
         :type cloud_cover: str
         :returns: Updated catalog
         :rtype: dict
         """
-        cat_model = copy.deepcopy(self.stac_config["catalogs"]["cloud_cover"]["model"])
+        cat_model = deepcopy(self.stac_config["catalogs"]["cloud_cover"]["model"])
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = defaultdict(str, **self.data)
         format_args["cloud_cover"] = cloud_cover
         parsed_dict = format_dict_items(cat_model, **format_args)
 
         self.update_data(parsed_dict)
 
         # update search args
@@ -1060,17 +1060,17 @@
             logger.warning(
                 "no feature found in %s matching %s=%s" % (path, attr, location)
             )
             return {}
 
         geom = unary_union(geom_hits)
 
-        cat_model = copy.deepcopy(self.stac_config["catalogs"]["country"]["model"])
+        cat_model = deepcopy(self.stac_config["catalogs"]["country"]["model"])
         # parse f-strings
-        format_args = copy.deepcopy(self.stac_config)
+        format_args = deepcopy(self.stac_config)
         format_args["catalog"] = defaultdict(str, **self.data)
         format_args["feature"] = defaultdict(str, {"geometry": geom, "id": location})
         parsed_dict = format_dict_items(cat_model, **format_args)
 
         self.update_data(parsed_dict)
 
         # update search args
@@ -1082,15 +1082,15 @@
         """Build locations config from stac_conf[locations_catalogs] & eodag_api.locations_config
 
         :returns: Locations configuration dict
         :rtype: dict
         """
         user_config_locations_list = self.eodag_api.locations_config
 
-        locations_config_model = copy.deepcopy(self.stac_config["locations_catalogs"])
+        locations_config_model = deepcopy(self.stac_config["locations_catalogs"])
 
         locations_config = {}
         for loc in user_config_locations_list:
             # parse jsonpath
             parsed = jsonpath_parse_dict_items(
                 locations_config_model, {"shp_location": loc}
             )
@@ -1114,27 +1114,26 @@
         :returns: This catalog obj
         :rtype: :class:`eodag.stac.StacCatalog`
         """
         # update conf with user shp locations
         locations_config = self.build_locations_config()
 
         self.stac_config["catalogs"] = dict(
-            copy.deepcopy(self.stac_config["catalogs"]), **locations_config
+            deepcopy(self.stac_config["catalogs"]), **locations_config
         )
 
         if len(catalogs) == 0:
             # Build root catalog combined with landing page
             self.__update_data_from_catalog_config(
                 {
                     "model": dict(
-                        copy.deepcopy(self.stac_config["landing_page"]),
+                        deepcopy(self.stac_config["landing_page"]),
                         **{"provider": self.provider},
                     )
                 }
-                # {"model": copy.deepcopy(self.stac_config["landing_page"])}
             )
 
             # build children : product_types
             product_types_list = [
                 pt
                 for pt in self.eodag_api.list_product_types(
                     provider=self.provider, fetch_providers=fetch_providers
@@ -1149,15 +1148,15 @@
                     }
                     for product_type in product_types_list
                 ]
             )
         else:
             # use product_types_list as base for building nested catalogs
             self.__update_data_from_catalog_config(
-                copy.deepcopy(self.stac_config["catalogs"]["product_types_list"])
+                deepcopy(self.stac_config["catalogs"]["product_types_list"])
             )
 
         for idx, cat in enumerate(catalogs):
             if idx % 2 == 0:
                 # even: cat is a filtering value ----------------------------------
                 cat_data_name = self.catalog_config["child_key"]
                 cat_data_value = cat
@@ -1232,15 +1231,15 @@
                         for c in self.stac_config["catalogs"].keys()
                         if self.stac_config["catalogs"][c]["model"]["id"] == cat
                     ][0]
                 except IndexError:
                     raise ValidationError(
                         "Bad settings for %s in stac_config catalogs" % cat
                     )
-                cat_config = copy.deepcopy(self.stac_config["catalogs"][cat_key])
+                cat_config = deepcopy(self.stac_config["catalogs"][cat_key])
                 # update data
                 self.__update_data_from_catalog_config(cat_config)
 
                 # get filtering values list
                 get_data_method_name = (
                     "get_stac_%s" % cat_key
                     if "catalog_type"
```

### Comparing `eodag-2.9.1/eodag/rest/utils.py` & `eodag-2.9.2/eodag/rest/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from eodag.api.product.metadata_mapping import OSEO_METADATA_MAPPING
 from eodag.api.search_result import SearchResult
 from eodag.config import load_stac_config, load_stac_provider_config
 from eodag.plugins.crunch.filter_latest_intersect import FilterLatestIntersect
 from eodag.plugins.crunch.filter_latest_tpl_name import FilterLatestByName
 from eodag.plugins.crunch.filter_overlap import FilterOverlap
 from eodag.rest.stac import StacCatalog, StacCollection, StacCommon, StacItem
-from eodag.utils import _deprecated, cached_parse, dict_items_recursive_apply
+from eodag.utils import _deprecated, dict_items_recursive_apply, string_to_jsonpath
 from eodag.utils.exceptions import (
     MisconfiguredError,
     NoMatchingProductType,
     UnsupportedProductType,
     ValidationError,
 )
 
@@ -313,17 +313,17 @@
                 # We create the dict corresponding to the metadata query of the metadata
                 metadata_query_dict = ast.literal_eval(
                     metadata_query_template.format(**{metadata_name: None})
                 )
                 # We check if our query path pattern matches one or more of the dict path
                 matches = [
                     (str(match.full_path))
-                    for match in cached_parse(STAC_QUERY_PATTERN).find(
-                        metadata_query_dict
-                    )
+                    for match in string_to_jsonpath(
+                        STAC_QUERY_PATTERN, force=True
+                    ).find(metadata_query_dict)
                 ]
                 if matches:
                     metadata_query_path = matches[0]
                     metadata_query_paths[metadata_query_path] = metadata_name
             except KeyError:
                 pass
     return metadata_query_paths
@@ -339,15 +339,15 @@
     :param arguments: Request args
     :type arguments: dict
     :returns: Mapping of query paths with their corresponding values
     :rtype: dict
     """
     return dict(
         (str(match.full_path), match.value)
-        for match in cached_parse(STAC_QUERY_PATTERN).find(arguments)
+        for match in string_to_jsonpath(STAC_QUERY_PATTERN, force=True).find(arguments)
     )
 
 
 def get_criterias_from_metadata_mapping(metadata_mapping, arguments):
     """Get criterias from the search arguments with the metadata mapping config
 
     :param metadata_mapping: STAC metadata mapping (see 'resources/stac_provider.yml')
```

### Comparing `eodag-2.9.1/eodag/utils/__init__.py` & `eodag-2.9.2/eodag/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 # limitations under the License.
 """Miscellaneous utilities to be used throughout eodag.
 
 Everything that does not fit into one of the specialised categories of utilities in
 this package should go here
 """
 import ast
-import copy
 import datetime
 import errno
 import functools
 import hashlib
 import inspect
-import json
 import logging as py_logging
 import os
 import re
 import shutil
 import string
 import types
 import unicodedata
 import warnings
 from collections import defaultdict
+from copy import deepcopy as copy_deepcopy
+from email.message import Message
 from glob import glob
 from itertools import repeat, starmap
 from pathlib import Path
 from tempfile import mkdtemp
 
 # All modules using these should import them from utils package
 from urllib.parse import (  # noqa; noqa
@@ -53,20 +53,23 @@
     urlparse,
     urlsplit,
     urlunparse,
 )
 from urllib.request import url2pathname
 
 import click
+import orjson
 import shapefile
 import shapely.wkt
+import yaml
 from dateutil.parser import isoparse
 from dateutil.tz import UTC
 from jsonpath_ng import jsonpath
 from jsonpath_ng.ext import parse
+from jsonpath_ng.jsonpath import Child, Fields, Index, Root, Slice
 from requests.auth import AuthBase
 from shapely.geometry import Polygon, shape
 from shapely.geometry.base import BaseGeometry
 from tqdm.auto import tqdm
 
 from eodag.utils import logging as eodag_logging
 
@@ -81,14 +84,18 @@
 logger = py_logging.getLogger("eodag.utils")
 
 GENERIC_PRODUCT_TYPE = "GENERIC_PRODUCT_TYPE"
 
 eodag_version = metadata("eodag")["Version"]
 USER_AGENT = {"User-Agent": f"eodag/{eodag_version}"}
 
+JSONPATH_MATCH = re.compile(r"^[\{\(]*\$(\..*)*$")
+WORKABLE_JSONPATH_MATCH = re.compile(r"^\$(\.[a-zA-Z0-9-_:\.\[\]\"\(\)=\?\*]+)*$")
+ARRAY_FIELD_MATCH = re.compile(r"^[a-zA-Z0-9-_:]+(\[[0-9\*]+\])+$")
+
 
 def _deprecated(reason="", version=None):
     """Simple decorator to mark functions/methods/classes as deprecated.
 
     Warning: Does not work with staticmethods!
 
     @deprecate(reason="why", version="1.2")
@@ -751,15 +758,15 @@
     :param apply_method: Method to be applied to dict elements
     :type apply_method: :func:`apply_method`
     :param apply_method_parameters: Optional parameters passed to the method
     :type apply_method_parameters: dict
     :returns: Updated dict
     :rtype: dict
     """
-    result_dict = copy.deepcopy(config_dict)
+    result_dict = deepcopy(config_dict)
     for dict_k, dict_v in result_dict.items():
         if isinstance(dict_v, dict):
             result_dict[dict_k] = dict_items_recursive_apply(
                 dict_v, apply_method, **apply_method_parameters
             )
         elif any(isinstance(dict_v, t) for t in (list, tuple)):
             result_dict[dict_k] = list_items_recursive_apply(
@@ -787,15 +794,15 @@
     :param apply_method: Method to be applied to list elements
     :type apply_method: :func:`apply_method`
     :param apply_method_parameters: Optional parameters passed to the method
     :type apply_method_parameters: dict
     :returns: Updated list
     :rtype: list
     """
-    result_list = copy.deepcopy(config_list)
+    result_list = deepcopy(config_list)
     for list_idx, list_v in enumerate(result_list):
         if isinstance(list_v, dict):
             result_list[list_idx] = dict_items_recursive_apply(
                 list_v, apply_method, **apply_method_parameters
             )
         elif any(isinstance(list_v, t) for t in (list, tuple)):
             result_list[list_idx] = list_items_recursive_apply(
@@ -844,15 +851,15 @@
     True
 
     :param config_dict: Input nested dictionnary
     :type config_dict: dict
     :returns: Updated dict
     :rtype: dict
     """
-    result_dict = copy.deepcopy(config_dict)
+    result_dict = deepcopy(config_dict)
     for dict_k, dict_v in result_dict.items():
         if isinstance(dict_v, dict):
             result_dict[dict_k] = dict_items_recursive_sort(dict_v)
         elif any(isinstance(dict_v, t) for t in (list, tuple)):
             result_dict[dict_k] = list_items_recursive_sort(dict_v)
         else:
             result_dict[dict_k] = dict_v
@@ -867,47 +874,104 @@
     ['b', {0: 1, 1: 2, 2: 0}]
 
     :param config_list: Input list containing nested lists/dicts
     :type config_list: list
     :returns: Updated list
     :rtype: list
     """
-    result_list = copy.deepcopy(config_list)
+    result_list = deepcopy(config_list)
     for list_idx, list_v in enumerate(result_list):
         if isinstance(list_v, dict):
             result_list[list_idx] = dict_items_recursive_sort(list_v)
         elif any(isinstance(list_v, t) for t in (list, tuple)):
             result_list[list_idx] = list_items_recursive_sort(list_v)
         else:
             result_list[list_idx] = list_v
 
     return result_list
 
 
-def string_to_jsonpath(key, str_value):
+def string_to_jsonpath(*args, force=False):
     """Get jsonpath for "$.foo.bar" like string
 
     >>> string_to_jsonpath(None, "$.foo.bar")
     Child(Child(Root(), Fields('foo')), Fields('bar'))
+    >>> string_to_jsonpath("$.foo.bar")
+    Child(Child(Root(), Fields('foo')), Fields('bar'))
+    >>> string_to_jsonpath('$.foo[0][*]')
+    Child(Child(Child(Root(), Fields('foo')), Index(index=0)), Slice(start=None,end=None,step=None))
+    >>> string_to_jsonpath("foo")
+    'foo'
+    >>> string_to_jsonpath("foo", force=True)
+    Fields('foo')
 
-    :param key: Input item key
-    :type key: str
-    :param str_value: Input item value, to be converted
-    :type str_value: str
+    :param args: Last arg as input string value, to be converted
+    :type args: str
+    :param force: force conversion even if input string is not detected as a jsonpath
+    :type force: bool
     :returns: Parsed value
     :rtype: str
     """
-    if "$." in str(str_value):
+    path_str = args[-1]
+    if JSONPATH_MATCH.match(str(path_str)) or force:
         try:
-            return cached_parse(str_value)
+            common_jsonpath = "$"
+            common_jsonpath_parsed = Root()
+
+            # combine with common jsonpath if possible
+            if WORKABLE_JSONPATH_MATCH.match(path_str):
+                path_suffix = path_str[len(common_jsonpath) + 1 :]
+                path_splits = path_suffix.split(".") if path_suffix else []
+                parsed_path = common_jsonpath_parsed
+                for path_split in path_splits:
+                    path_split = path_split.strip("'").strip('"')
+                    if "[" in path_split and ARRAY_FIELD_MATCH.match(path_split):
+                        # handle nested array
+                        indexed_path_and_indexes = path_split[:-1].split("[")
+                        indexed_path = indexed_path_and_indexes[0]
+                        parsed_path = Child(parsed_path, Fields(indexed_path))
+                        for idx in range(len(indexed_path_and_indexes) - 1):
+                            index = (
+                                indexed_path_and_indexes[idx + 1][:-1]
+                                if idx < len(indexed_path_and_indexes) - 2
+                                else indexed_path_and_indexes[idx + 1]
+                            )
+                            # wildcard index
+                            if index == "*":
+                                parsed_path = Child(
+                                    parsed_path,
+                                    Slice(start=None, end=None, step=None),
+                                )
+                                continue
+                            try:
+                                index = int(index)
+                            except ValueError:
+                                # unsupported index
+                                parsed_path = cached_parse(path_str)
+                                break
+                            # integer index
+                            parsed_path = Child(
+                                parsed_path,
+                                Index(index=index),
+                            )
+                    elif "[" in path_split:
+                        # unsupported array field
+                        parsed_path = cached_parse(path_str)
+                        break
+                    else:
+                        parsed_path = Child(parsed_path, Fields(path_split))
+                return parsed_path
+            else:
+                return cached_parse(path_str)
+
         except Exception:  # jsonpath_ng does not provide a proper exception
             # If str_value does not contain a jsonpath, return it as is
-            return str_value
+            return path_str
     else:
-        return str_value
+        return path_str
 
 
 def format_string(key, str_to_format, **format_variables):
     """Format "{foo}" like string
 
     >>> format_string(None, "foo {bar}, {baz} ?", **{"bar": "qux", "baz": "quux"})
     'foo qux, quux ?'
@@ -1114,15 +1178,15 @@
     '37a6259cc0c1dae299a7866489dff0bd'
 
     :param data: JSON serializable input object
     :type data: Any
     :returns: MD5 checksum
     :rtype: str
     """
-    return hashlib.md5(json.dumps(data, sort_keys=True).encode("utf-8")).hexdigest()
+    return hashlib.md5(orjson.dumps(data, option=orjson.OPT_SORT_KEYS)).hexdigest()
 
 
 @functools.lru_cache()
 def cached_parse(str_to_parse):
     """Cached jsonpath_ng.ext.parse
 
     >>> cached_parse.cache_clear()
@@ -1143,14 +1207,50 @@
     :type str_to_parse: str
     :returns: parsed jsonpath
     :rtype: :class:`jsonpath_ng.JSONPath`
     """
     return parse(str_to_parse)
 
 
+@functools.lru_cache()
+def _mutable_cached_yaml_load(config_path):
+    with open(os.path.abspath(os.path.realpath(config_path)), "r") as fh:
+        return yaml.load(fh, Loader=yaml.SafeLoader)
+
+
+def cached_yaml_load(config_path):
+    """Cached yaml.load
+
+    :param config_path: path to the yaml configuration file
+    :type config_path: str
+    :returns: loaded yaml configuration
+    :rtype: dict
+    """
+    return copy_deepcopy(_mutable_cached_yaml_load(config_path))
+
+
+@functools.lru_cache()
+def _mutable_cached_yaml_load_all(config_path):
+    with open(config_path, "r") as fh:
+        return list(yaml.load_all(fh, Loader=yaml.Loader))
+
+
+def cached_yaml_load_all(config_path):
+    """Cached yaml.load_all
+
+    Load all configurations stored in the configuration file as separated yaml documents
+
+    :param config_path: path to the yaml configuration file
+    :type config_path: str
+    :returns: list of configurations
+    :rtype: list
+    """
+    return copy_deepcopy(_mutable_cached_yaml_load_all(config_path))
+
+
 def get_bucket_name_and_prefix(url=None, bucket_path_level=None):
     """Extract bucket name and prefix from URL
 
     :param url: (optional) URL to use as product.location
     :type url: str
     :param bucket_path_level: (optional) bucket location index in path.split('/')
     :type bucket_path_level: int
@@ -1196,7 +1296,62 @@
         logger.debug(f"Flatten {common_subdirs_path} to {nested_dir_root}")
         tmp_path = mkdtemp()
         # need to delete tmp_path to prevent FileExistsError with copytree. Use dirs_exist_ok with py > 3.7
         shutil.rmtree(tmp_path)
         shutil.copytree(common_subdirs_path, tmp_path)
         shutil.rmtree(nested_dir_root)
         shutil.move(tmp_path, nested_dir_root)
+
+
+def deepcopy(sth):
+    """Customized and faster deepcopy inspired by https://stackoverflow.com/a/45858907
+    `_copy_list` and `_copy_dict` available for the moment
+
+    :param sth: Object to copy
+    :type sth: Any
+    :returns: Copied object
+    :rtype: Any
+    """
+    _dispatcher = {}
+
+    def _copy_list(input_list, dispatch):
+        ret = input_list.copy()
+        for idx, item in enumerate(ret):
+            cp = dispatch.get(type(item))
+            if cp is not None:
+                ret[idx] = cp(item, dispatch)
+        return ret
+
+    def _copy_dict(input_dict, dispatch):
+        ret = input_dict.copy()
+        for key, value in ret.items():
+            cp = dispatch.get(type(value))
+            if cp is not None:
+                ret[key] = cp(value, dispatch)
+        return ret
+
+    _dispatcher[list] = _copy_list
+    _dispatcher[dict] = _copy_dict
+
+    cp = _dispatcher.get(type(sth))
+    if cp is None:
+        return sth
+    else:
+        return cp(sth, _dispatcher)
+
+
+def parse_header(header):
+    """Parse HTTP header
+
+    >>> parse_header(
+    ...     'Content-Disposition: form-data; name="field2"; filename="example.txt"'
+    ... ).get_param("filename")
+    'example.txt'
+
+    :param header: header to parse
+    :type header: str
+    :returns: parsed header
+    :rtype: :class:`~email.message.Message`
+    """
+    m = Message()
+    m["content-type"] = header
+    return m
```

### Comparing `eodag-2.9.1/eodag/utils/exceptions.py` & `eodag-2.9.2/eodag/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/utils/import_system.py` & `eodag-2.9.2/eodag/utils/import_system.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/utils/logging.py` & `eodag-2.9.2/eodag/utils/logging.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/utils/notebook.py` & `eodag-2.9.2/eodag/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/eodag/utils/stac_reader.py` & `eodag-2.9.2/eodag/utils/stac_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
 import logging
 import re
 import socket
 from urllib.error import HTTPError, URLError
 from urllib.request import urlopen
 
 import concurrent.futures
+import orjson
 import pystac
 
 from eodag.utils.exceptions import STACOpenerError
 
 logger = logging.getLogger("eodag.utils.stac_reader")
 
 HTTP_REQ_TIMEOUT = 5
@@ -41,18 +41,19 @@
         # Only used by read_http_remote_json
         self.timeout = timeout
 
     @staticmethod
     def read_local_json(url, as_json):
         """Read JSON local file"""
         try:
-            with open(url) as f:
-                if as_json:
-                    return json.load(f)
-                else:
+            if as_json:
+                with open(url, "rb") as f:
+                    return orjson.loads(f.read())
+            else:
+                with open(url) as f:
                     return f.read()
         except OSError:
             logger.debug("read_local_json is not the right STAC opener")
             raise STACOpenerError
 
     def read_http_remote_json(self, url, as_json):
         """Read JSON remote HTTP file"""
@@ -64,15 +65,15 @@
             else:
                 m = re.search(r"charset\s*=\s*(\S+)", content_type, re.I)
                 if m is None:
                     encoding = "utf-8"
                 else:
                     encoding = m.group(1)
             content = res.read().decode(encoding)
-            return json.loads(content) if as_json else content
+            return orjson.loads(content) if as_json else content
         except URLError as e:
             if isinstance(e.reason, socket.timeout):
                 logger.error("%s: %s", url, e)
                 raise socket.timeout(
                     f"{url} with a timeout of {self.timeout} seconds"
                 ) from None
             else:
```

### Comparing `eodag-2.9.1/eodag.egg-info/PKG-INFO` & `eodag-2.9.2/eodag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodag
-Version: 2.9.1
+Version: 2.9.2
 Summary: Earth Observation Data Access Gateway
 Home-page: https://github.com/CS-SI/eodag
 Author: CS GROUP - France (CSSI)
 Author-email: admin@geostorm.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/CS-SI/eodag/issues/
 Project-URL: Documentation, https://eodag.readthedocs.io
```

### Comparing `eodag-2.9.1/eodag.egg-info/SOURCES.txt` & `eodag-2.9.2/eodag.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 eodag/plugins/authentication/base.py
 eodag/plugins/authentication/generic.py
 eodag/plugins/authentication/header.py
 eodag/plugins/authentication/keycloak.py
 eodag/plugins/authentication/oauth.py
 eodag/plugins/authentication/openid_connect.py
 eodag/plugins/authentication/qsauth.py
+eodag/plugins/authentication/sas_auth.py
 eodag/plugins/authentication/token.py
 eodag/plugins/crunch/__init__.py
 eodag/plugins/crunch/base.py
 eodag/plugins/crunch/filter_date.py
 eodag/plugins/crunch/filter_latest_intersect.py
 eodag/plugins/crunch/filter_latest_tpl_name.py
 eodag/plugins/crunch/filter_overlap.py
```

### Comparing `eodag-2.9.1/eodag.egg-info/entry_points.txt` & `eodag-2.9.2/eodag.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 AwsAuth = eodag.plugins.authentication.aws_auth:AwsAuth
 GenericAuth = eodag.plugins.authentication.generic:GenericAuth
 HTTPHeaderAuth = eodag.plugins.authentication.header:HTTPHeaderAuth
 HttpQueryStringAuth = eodag.plugins.authentication.qsauth:HttpQueryStringAuth
 KeycloakOIDCPasswordAuth = eodag.plugins.authentication.keycloak:KeycloakOIDCPasswordAuth
 OAuth = eodag.plugins.authentication.oauth:OAuth
 OIDCAuthorizationCodeFlowAuth = eodag.plugins.authentication.openid_connect:OIDCAuthorizationCodeFlowAuth
+SASAuth = eodag.plugins.authentication.sas_auth:SASAuth
 TokenAuth = eodag.plugins.authentication.token:TokenAuth
 
 [eodag.plugins.crunch]
 FilterDate = eodag.plugins.crunch.filter_date:FilterDate
 FilterLatestByName = eodag.plugins.crunch.filter_latest_tpl_name:FilterLatestByName
 FilterLatestIntersect = eodag.plugins.crunch.filter_latest_intersect:FilterLatestIntersect
 FilterOverlap = eodag.plugins.crunch.filter_overlap:FilterOverlap
```

### Comparing `eodag-2.9.1/eodag.egg-info/requires.txt` & `eodag-2.9.2/eodag.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 click
 requests
 python-dateutil
 PyYAML
 tqdm
 shapely
 pyshp
+orjson
 geojson
-pyproj
+pyproj>=2.1.0
 usgs>=0.3.1
 boto3
 flasgger
 jsonpath-ng
 lxml
 flask!=2.2.0,!=2.2.1,>=1.0.2
 whoosh
@@ -39,15 +40,15 @@
 wheel
 flake8
 pre-commit
 responses
 
 [docs]
 sphinx
-sphinx-book-theme>=0.1.0
+sphinx-book-theme<1.0.0
 sphinx-copybutton
 sphinxcontrib-jquery
 nbsphinx
 ipython!=8.7.0
 
 [notebook]
 tqdm[notebook]
```

### Comparing `eodag-2.9.1/setup.cfg` & `eodag-2.9.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,17 @@
 	python-dateutil
 	PyYAML
 	tqdm
 	shapely
 	pyshp
 	owslib < 0.26;python_version>='3.10'
 	owslib;python_version<'3.10'
+	orjson
 	geojson
-	pyproj
+	pyproj >= 2.1.0
 	usgs >= 0.3.1
 	boto3
 	flasgger
 	jsonpath-ng
 	lxml
 	flask >= 1.0.2, != 2.2.0, != 2.2.1
 	whoosh
@@ -85,15 +86,15 @@
 	matplotlib
 	folium
 	imageio
 	rasterio
 	netcdf4
 docs = 
 	sphinx
-	sphinx-book-theme >= 0.1.0
+	sphinx-book-theme < 1.0.0
 	sphinx-copybutton
 	sphinxcontrib-jquery
 	nbsphinx
 	ipython!=8.7.0
 
 [options.packages.find]
 exclude = 
@@ -119,14 +120,15 @@
 	HTTPHeaderAuth = eodag.plugins.authentication.header:HTTPHeaderAuth
 	AwsAuth = eodag.plugins.authentication.aws_auth:AwsAuth
 	OAuth = eodag.plugins.authentication.oauth:OAuth
 	TokenAuth = eodag.plugins.authentication.token:TokenAuth
 	OIDCAuthorizationCodeFlowAuth = eodag.plugins.authentication.openid_connect:OIDCAuthorizationCodeFlowAuth
 	KeycloakOIDCPasswordAuth = eodag.plugins.authentication.keycloak:KeycloakOIDCPasswordAuth
 	HttpQueryStringAuth = eodag.plugins.authentication.qsauth:HttpQueryStringAuth
+	SASAuth = eodag.plugins.authentication.sas_auth:SASAuth
 eodag.plugins.crunch = 
 	FilterLatestIntersect = eodag.plugins.crunch.filter_latest_intersect:FilterLatestIntersect
 	FilterLatestByName = eodag.plugins.crunch.filter_latest_tpl_name:FilterLatestByName
 	FilterOverlap = eodag.plugins.crunch.filter_overlap:FilterOverlap
 	FilterProperty = eodag.plugins.crunch.filter_property:FilterProperty
 	FilterDate = eodag.plugins.crunch.filter_date:FilterDate
 eodag.plugins.download =
```

### Comparing `eodag-2.9.1/setup.py` & `eodag-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/tox.ini` & `eodag-2.9.2/tox.ini`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/utils/params_mapping_to_csv.py` & `eodag-2.9.2/utils/params_mapping_to_csv.py`

 * *Files identical despite different names*

### Comparing `eodag-2.9.1/utils/product_types_information_to_csv.py` & `eodag-2.9.2/utils/product_types_information_to_csv.py`

 * *Files identical despite different names*

