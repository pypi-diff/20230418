# Comparing `tmp/pymarkdownlnt-0.9.8.tar.gz` & `tmp/pymarkdownlnt-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymarkdownlnt-0.9.8.tar", last modified: Wed Sep 21 03:16:31 2022, max compression
+gzip compressed data, was "pymarkdownlnt-0.9.9.tar", last modified: Sun Feb 26 21:48:15 2023, max compression
```

## Comparing `pymarkdownlnt-0.9.8.tar` & `pymarkdownlnt-0.9.9.tar`

### file list

```diff
@@ -1,140 +1,147 @@
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:31.001901 pymarkdownlnt-0.9.8/
--rw-rw-rw-   0        0        0     1066 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/LICENSE.txt
--rw-rw-rw-   0        0        0       78 2021-05-30 03:14:28.000000 pymarkdownlnt-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0    17317 2022-09-21 03:16:31.002904 pymarkdownlnt-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0    16444 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/README.md
--rw-rw-rw-   0        0        0       74 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/install-requirements.txt
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:29.856800 pymarkdownlnt-0.9.8/pymarkdown/
--rw-rw-rw-   0        0        0      184 2021-10-07 03:00:02.000000 pymarkdownlnt-0.9.8/pymarkdown/__init__.py
--rw-rw-rw-   0        0        0      390 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/__main__.py
--rw-rw-rw-   0        0        0      436 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/bad_tokenization_error.py
--rw-rw-rw-   0        0        0      454 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/block_quote_data.py
--rw-rw-rw-   0        0        0    80642 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/pymarkdown/block_quote_processor.py
--rw-rw-rw-   0        0        0     5819 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/coalesce_processor.py
--rw-rw-rw-   0        0        0    10783 2022-09-16 02:23:07.000000 pymarkdownlnt-0.9.8/pymarkdown/constants.py
--rw-rw-rw-   0        0        0    44165 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/pymarkdown/container_block_leaf_processor.py
--rw-rw-rw-   0        0        0    78084 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/pymarkdown/container_block_processor.py
--rw-rw-rw-   0        0        0    22633 2022-09-05 05:46:39.000000 pymarkdownlnt-0.9.8/pymarkdown/container_grab_bag.py
--rw-rw-rw-   0        0        0      541 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/container_indices.py
--rw-rw-rw-   0        0        0    12203 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/container_markdown_token.py
--rw-rw-rw-   0        0        0    20120 2022-09-16 02:23:07.000000 pymarkdownlnt-0.9.8/pymarkdown/emphasis_helper.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:29.883822 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/
--rw-rw-rw-   0        0        0        0 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/__init__.py
--rw-rw-rw-   0        0        0      656 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/extension_impl.py
--rw-rw-rw-   0        0        0    12197 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/extension_manager.py
--rw-rw-rw-   0        0        0      364 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/extension_manager_constants.py
--rw-rw-rw-   0        0        0      896 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extension_manager/parser_extension.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:29.949880 pymarkdownlnt-0.9.8/pymarkdown/extensions/
--rw-rw-rw-   0        0        0        0 2022-07-24 03:14:42.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/__init__.py
--rw-rw-rw-   0        0        0     1688 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/disallowed_raw_html.py
--rw-rw-rw-   0        0        0     1710 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/extended_autolinks.py
--rw-rw-rw-   0        0        0     1756 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/extension_one.py
--rw-rw-rw-   0        0        0     9575 2022-09-01 03:11:50.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/front_matter_extension.py
--rw-rw-rw-   0        0        0     3194 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/front_matter_markdown_token.py
--rw-rw-rw-   0        0        0     1680 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/markdown_strikethrough.py
--rw-rw-rw-   0        0        0     1636 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/markdown_tables.py
--rw-rw-rw-   0        0        0     7885 2022-08-29 05:00:20.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/pragma_token.py
--rw-rw-rw-   0        0        0     1685 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/extensions/task_list_items.py
--rw-rw-rw-   0        0        0    34535 2022-08-29 05:00:20.000000 pymarkdownlnt-0.9.8/pymarkdown/html_helper.py
--rw-rw-rw-   0        0        0    48506 2022-09-11 23:34:02.000000 pymarkdownlnt-0.9.8/pymarkdown/inline_helper.py
--rw-rw-rw-   0        0        0    26139 2022-09-11 01:14:22.000000 pymarkdownlnt-0.9.8/pymarkdown/inline_markdown_token.py
--rw-rw-rw-   0        0        0    80195 2022-09-11 19:24:36.000000 pymarkdownlnt-0.9.8/pymarkdown/inline_processor.py
--rw-rw-rw-   0        0        0      926 2022-09-11 20:01:08.000000 pymarkdownlnt-0.9.8/pymarkdown/inline_request.py
--rw-rw-rw-   0        0        0      673 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/inline_response.py
--rw-rw-rw-   0        0        0    42609 2022-09-05 15:11:20.000000 pymarkdownlnt-0.9.8/pymarkdown/leaf_block_processor.py
--rw-rw-rw-   0        0        0    11628 2022-09-11 01:14:22.000000 pymarkdownlnt-0.9.8/pymarkdown/leaf_block_processor_paragraph.py
--rw-rw-rw-   0        0        0    23135 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/leaf_markdown_token.py
--rw-rw-rw-   0        0        0    68505 2022-08-29 05:00:21.000000 pymarkdownlnt-0.9.8/pymarkdown/link_helper.py
--rw-rw-rw-   0        0        0    32752 2022-09-01 03:11:50.000000 pymarkdownlnt-0.9.8/pymarkdown/link_reference_definition_helper.py
--rw-rw-rw-   0        0        0      510 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/link_reference_info.py
--rw-rw-rw-   0        0        0      315 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/link_reference_titles.py
--rw-rw-rw-   0        0        0    97336 2022-09-04 02:32:31.000000 pymarkdownlnt-0.9.8/pymarkdown/list_block_processor.py
--rw-rw-rw-   0        0        0    26697 2022-08-25 03:20:36.000000 pymarkdownlnt-0.9.8/pymarkdown/main.py
--rw-rw-rw-   0        0        0    21952 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/markdown_token.py
--rw-rw-rw-   0        0        0     1038 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/parse_block_pass_properties.py
--rw-rw-rw-   0        0        0    36881 2022-09-07 02:34:52.000000 pymarkdownlnt-0.9.8/pymarkdown/parser_helper.py
--rw-rw-rw-   0        0        0     4449 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/parser_logger.py
--rw-rw-rw-   0        0        0     9897 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/parser_state.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:29.982909 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/
--rw-rw-rw-   0        0        0        0 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/__init__.py
--rw-rw-rw-   0        0        0     4180 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/bad_plugin_error.py
--rw-rw-rw-   0        0        0      939 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/found_plugin.py
--rw-rw-rw-   0        0        0      637 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_details.py
--rw-rw-rw-   0        0        0    33890 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_manager.py
--rw-rw-rw-   0        0        0     1815 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_scan_context.py
--rw-rw-rw-   0        0        0     1212 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_scan_failure.py
--rw-rw-rw-   0        0        0     5954 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/rule_plugin.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:30.959866 pymarkdownlnt-0.9.8/pymarkdown/plugins/
--rw-rw-rw-   0        0        0        0 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/__init__.py
--rw-rw-rw-   0        0        0     3140 2022-07-24 03:14:43.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/plugin_one.py
--rw-rw-rw-   0        0        0     3003 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_001.py
--rw-rw-rw-   0        0        0     2921 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_002.py
--rw-rw-rw-   0        0        0     7250 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_003.py
--rw-rw-rw-   0        0        0     4621 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_004.py
--rw-rw-rw-   0        0        0     9713 2022-09-20 23:44:55.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_005.py
--rw-rw-rw-   0        0        0     3368 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_006.py
--rw-rw-rw-   0        0        0    12047 2022-08-14 16:28:01.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_007.py
--rw-rw-rw-   0        0        0     6549 2022-08-27 17:18:14.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_009.py
--rw-rw-rw-   0        0        0     1948 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_010.py
--rw-rw-rw-   0        0        0     3030 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_011.py
--rw-rw-rw-   0        0        0     3115 2022-07-24 03:14:44.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_012.py
--rw-rw-rw-   0        0        0     6822 2022-08-27 21:46:32.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_013.py
--rw-rw-rw-   0        0        0     2194 2022-07-24 03:14:45.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_014.py
--rw-rw-rw-   0        0        0    11348 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_018.py
--rw-rw-rw-   0        0        0     2462 2022-07-24 03:14:45.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_019.py
--rw-rw-rw-   0        0        0     4086 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_020.py
--rw-rw-rw-   0        0        0     2823 2022-07-24 03:14:45.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_021.py
--rw-rw-rw-   0        0        0     6563 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_022.py
--rw-rw-rw-   0        0        0     4466 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_023.py
--rw-rw-rw-   0        0        0     4693 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_024.py
--rw-rw-rw-   0        0        0     3555 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_025.py
--rw-rw-rw-   0        0        0     4105 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_026.py
--rw-rw-rw-   0        0        0    35936 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_027.py
--rw-rw-rw-   0        0        0     3296 2022-07-24 03:14:46.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_028.py
--rw-rw-rw-   0        0        0     7388 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_029.py
--rw-rw-rw-   0        0        0     7503 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_030.py
--rw-rw-rw-   0        0        0     5235 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_031.py
--rw-rw-rw-   0        0        0     3225 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_032.py
--rw-rw-rw-   0        0        0     5193 2022-08-27 16:10:45.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_033.py
--rw-rw-rw-   0        0        0     4167 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_034.py
--rw-rw-rw-   0        0        0     3550 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_035.py
--rw-rw-rw-   0        0        0     4029 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_036.py
--rw-rw-rw-   0        0        0     4312 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_037.py
--rw-rw-rw-   0        0        0     2053 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_038.py
--rw-rw-rw-   0        0        0     1518 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_039.py
--rw-rw-rw-   0        0        0     1654 2022-09-04 18:16:03.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_040.py
--rw-rw-rw-   0        0        0     4489 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_041.py
--rw-rw-rw-   0        0        0     1573 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_042.py
--rw-rw-rw-   0        0        0    19982 2022-08-27 17:08:01.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_043.py
--rw-rw-rw-   0        0        0    13443 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_044.py
--rw-rw-rw-   0        0        0     1534 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_045.py
--rw-rw-rw-   0        0        0     3136 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_046.py
--rw-rw-rw-   0        0        0     1716 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_047.py
--rw-rw-rw-   0        0        0     3330 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_048.py
--rw-rw-rw-   0        0        0      382 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/position_marker.py
--rw-rw-rw-   0        0        0      352 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/requeue_line_info.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:30.962869 pymarkdownlnt-0.9.8/pymarkdown/resources/
--rw-rw-rw-   0        0        0   148128 2020-02-05 05:31:16.000000 pymarkdownlnt-0.9.8/pymarkdown/resources/entities.json
--rw-rw-rw-   0        0        0     3015 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/source_providers.py
--rw-rw-rw-   0        0        0    16664 2022-07-24 03:14:47.000000 pymarkdownlnt-0.9.8/pymarkdown/stack_token.py
--rw-rw-rw-   0        0        0    34726 2022-09-04 03:49:04.000000 pymarkdownlnt-0.9.8/pymarkdown/tokenized_markdown.py
--rw-rw-rw-   0        0        0     5566 2022-09-09 03:46:04.000000 pymarkdownlnt-0.9.8/pymarkdown/transform_state.py
--rw-rw-rw-   0        0        0    42157 2022-09-10 22:27:12.000000 pymarkdownlnt-0.9.8/pymarkdown/transform_to_gfm.py
--rw-rw-rw-   0        0        0    11890 2022-07-24 03:14:48.000000 pymarkdownlnt-0.9.8/pymarkdown/transform_to_gfm_list_looseness.py
--rw-rw-rw-   0        0        0       70 2022-09-20 23:41:11.000000 pymarkdownlnt-0.9.8/pymarkdown/version.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:30.976880 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/
--rw-rw-rw-   0        0        0    17317 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4437 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-21 03:16:28.000000 pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      741 2022-09-21 03:16:31.003903 pymarkdownlnt-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     2500 2022-07-24 03:14:48.000000 pymarkdownlnt-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-21 03:16:31.000901 pymarkdownlnt-0.9.8/test/
--rw-rw-rw-   0        0        0    13161 2022-08-25 03:20:37.000000 pymarkdownlnt-0.9.8/test/test_listfiles.py
--rw-rw-rw-   0        0        0    60164 2022-08-27 16:10:45.000000 pymarkdownlnt-0.9.8/test/test_main.py
--rw-rw-rw-   0        0        0    84395 2022-09-19 04:12:11.000000 pymarkdownlnt-0.9.8/test/test_markdown_extra.py
--rw-rw-rw-   0        0        0     1549 2022-07-24 03:14:50.000000 pymarkdownlnt-0.9.8/test/test_markdown_transform_to_gfm.py
--rw-rw-rw-   0        0        0     2488 2022-07-24 03:14:50.000000 pymarkdownlnt-0.9.8/test/test_perf.py
--rw-rw-rw-   0        0        0     1378 2022-07-24 03:14:51.000000 pymarkdownlnt-0.9.8/test/test_transform_markdown.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.095407 pymarkdownlnt-0.9.9/
+-rw-rw-rw-   0        0        0     1066 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       78 2021-05-30 03:14:28.000000 pymarkdownlnt-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    17317 2023-02-26 21:48:15.095407 pymarkdownlnt-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16444 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/README.md
+-rw-rw-rw-   0        0        0       74 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/install-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:14.987798 pymarkdownlnt-0.9.9/pymarkdown/
+-rw-rw-rw-   0        0        0      184 2021-10-07 03:00:02.000000 pymarkdownlnt-0.9.9/pymarkdown/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/__main__.py
+-rw-rw-rw-   0        0        0    10161 2023-02-26 16:31:52.000000 pymarkdownlnt-0.9.9/pymarkdown/application_file_scanner.py
+-rw-rw-rw-   0        0        0     5500 2023-02-12 17:15:25.000000 pymarkdownlnt-0.9.9/pymarkdown/application_logging.py
+-rw-rw-rw-   0        0        0      436 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/bad_tokenization_error.py
+-rw-rw-rw-   0        0        0      454 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/block_quote_data.py
+-rw-rw-rw-   0        0        0    85218 2023-02-26 18:38:54.000000 pymarkdownlnt-0.9.9/pymarkdown/block_quote_processor.py
+-rw-rw-rw-   0        0        0     6512 2023-02-26 16:31:52.000000 pymarkdownlnt-0.9.9/pymarkdown/coalesce_processor.py
+-rw-rw-rw-   0        0        0    10783 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/constants.py
+-rw-rw-rw-   0        0        0    39567 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/container_block_leaf_processor.py
+-rw-rw-rw-   0        0        0    78211 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/container_block_processor.py
+-rw-rw-rw-   0        0        0    22802 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/container_grab_bag.py
+-rw-rw-rw-   0        0        0     3734 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/container_helper.py
+-rw-rw-rw-   0        0        0      541 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/container_indices.py
+-rw-rw-rw-   0        0        0    16215 2023-02-25 16:07:59.000000 pymarkdownlnt-0.9.9/pymarkdown/container_markdown_token.py
+-rw-rw-rw-   0        0        0    20114 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/emphasis_helper.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:14.994048 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/
+-rw-rw-rw-   0        0        0        0 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/extension_impl.py
+-rw-rw-rw-   0        0        0    12553 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/extension_manager.py
+-rw-rw-rw-   0        0        0      364 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/extension_manager_constants.py
+-rw-rw-rw-   0        0        0      896 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extension_manager/parser_extension.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.006264 pymarkdownlnt-0.9.9/pymarkdown/extensions/
+-rw-rw-rw-   0        0        0        0 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1688 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/disallowed_raw_html.py
+-rw-rw-rw-   0        0        0     1710 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/extended_autolinks.py
+-rw-rw-rw-   0        0        0     2006 2023-02-11 16:41:20.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/extension_one.py
+-rw-rw-rw-   0        0        0     9571 2023-02-26 16:31:52.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/front_matter_extension.py
+-rw-rw-rw-   0        0        0     3194 2023-02-11 16:39:55.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/front_matter_markdown_token.py
+-rw-rw-rw-   0        0        0     1680 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/markdown_strikethrough.py
+-rw-rw-rw-   0        0        0     1636 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/markdown_tables.py
+-rw-rw-rw-   0        0        0     8601 2023-02-19 04:47:03.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/pragma_token.py
+-rw-rw-rw-   0        0        0     1685 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/extensions/task_list_items.py
+-rw-rw-rw-   0        0        0    38685 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/html_helper.py
+-rw-rw-rw-   0        0        0    50137 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/inline_helper.py
+-rw-rw-rw-   0        0        0    28100 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/inline_markdown_token.py
+-rw-rw-rw-   0        0        0   109407 2023-02-26 16:31:55.000000 pymarkdownlnt-0.9.9/pymarkdown/inline_processor.py
+-rw-rw-rw-   0        0        0      977 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/inline_request.py
+-rw-rw-rw-   0        0        0      673 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/inline_response.py
+-rw-rw-rw-   0        0        0   106961 2023-02-26 18:38:54.000000 pymarkdownlnt-0.9.9/pymarkdown/leaf_block_processor.py
+-rw-rw-rw-   0        0        0    17354 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/leaf_block_processor_paragraph.py
+-rw-rw-rw-   0        0        0    23275 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/leaf_markdown_token.py
+-rw-rw-rw-   0        0        0    72308 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/link_helper.py
+-rw-rw-rw-   0        0        0     1199 2023-02-24 02:45:09.000000 pymarkdownlnt-0.9.9/pymarkdown/link_helper_properties.py
+-rw-rw-rw-   0        0        0    52262 2023-02-26 18:38:54.000000 pymarkdownlnt-0.9.9/pymarkdown/link_reference_definition_helper.py
+-rw-rw-rw-   0        0        0      510 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/link_reference_info.py
+-rw-rw-rw-   0        0        0      315 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/link_reference_titles.py
+-rw-rw-rw-   0        0        0   109971 2023-02-26 16:31:55.000000 pymarkdownlnt-0.9.9/pymarkdown/list_block_processor.py
+-rw-rw-rw-   0        0        0    17784 2023-02-26 17:46:40.000000 pymarkdownlnt-0.9.9/pymarkdown/main.py
+-rw-rw-rw-   0        0        0     1802 2023-02-12 16:00:15.000000 pymarkdownlnt-0.9.9/pymarkdown/main_presentation.py
+-rw-rw-rw-   0        0        0    22217 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/markdown_token.py
+-rw-rw-rw-   0        0        0     1038 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/parse_block_pass_properties.py
+-rw-rw-rw-   0        0        0    33925 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/parser_helper.py
+-rw-rw-rw-   0        0        0     4695 2023-02-11 16:41:20.000000 pymarkdownlnt-0.9.9/pymarkdown/parser_logger.py
+-rw-rw-rw-   0        0        0     9907 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/parser_state.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.016273 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/
+-rw-rw-rw-   0        0        0        0 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/__init__.py
+-rw-rw-rw-   0        0        0     4178 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/bad_plugin_error.py
+-rw-rw-rw-   0        0        0      939 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/found_plugin.py
+-rw-rw-rw-   0        0        0      637 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_details.py
+-rw-rw-rw-   0        0        0    35033 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_manager.py
+-rw-rw-rw-   0        0        0     1815 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_scan_context.py
+-rw-rw-rw-   0        0        0     1212 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_scan_failure.py
+-rw-rw-rw-   0        0        0     6040 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/rule_plugin.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.075389 pymarkdownlnt-0.9.9/pymarkdown/plugins/
+-rw-rw-rw-   0        0        0        0 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-02-11 16:41:20.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/plugin_one.py
+-rw-rw-rw-   0        0        0     3003 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_001.py
+-rw-rw-rw-   0        0        0     2921 2023-02-11 16:39:56.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_002.py
+-rw-rw-rw-   0        0        0     7234 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_003.py
+-rw-rw-rw-   0        0        0     4621 2023-02-11 16:39:58.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_004.py
+-rw-rw-rw-   0        0        0     9659 2023-02-26 21:38:55.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_005.py
+-rw-rw-rw-   0        0        0     3370 2023-02-11 16:39:58.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_006.py
+-rw-rw-rw-   0        0        0    12842 2023-02-18 15:46:46.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_007.py
+-rw-rw-rw-   0        0        0     6639 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_009.py
+-rw-rw-rw-   0        0        0     1948 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_010.py
+-rw-rw-rw-   0        0        0     3030 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_011.py
+-rw-rw-rw-   0        0        0     3115 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_012.py
+-rw-rw-rw-   0        0        0     6818 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_013.py
+-rw-rw-rw-   0        0        0     2194 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_014.py
+-rw-rw-rw-   0        0        0    11348 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_018.py
+-rw-rw-rw-   0        0        0     2462 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_019.py
+-rw-rw-rw-   0        0        0     4086 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_020.py
+-rw-rw-rw-   0        0        0     2823 2023-02-11 16:39:59.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_021.py
+-rw-rw-rw-   0        0        0     6953 2023-02-25 15:59:31.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_022.py
+-rw-rw-rw-   0        0        0     4466 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_023.py
+-rw-rw-rw-   0        0        0     4693 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_024.py
+-rw-rw-rw-   0        0        0     3555 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_025.py
+-rw-rw-rw-   0        0        0     4105 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_026.py
+-rw-rw-rw-   0        0        0    36527 2023-02-25 16:12:37.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_027.py
+-rw-rw-rw-   0        0        0     3296 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_028.py
+-rw-rw-rw-   0        0        0     7388 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_029.py
+-rw-rw-rw-   0        0        0     7501 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_030.py
+-rw-rw-rw-   0        0        0     5235 2023-02-11 16:40:00.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_031.py
+-rw-rw-rw-   0        0        0     3223 2023-02-26 16:31:53.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_032.py
+-rw-rw-rw-   0        0        0     5193 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_033.py
+-rw-rw-rw-   0        0        0     4167 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_034.py
+-rw-rw-rw-   0        0        0     3550 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_035.py
+-rw-rw-rw-   0        0        0     5144 2023-02-25 16:02:03.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_036.py
+-rw-rw-rw-   0        0        0     4442 2023-02-18 15:58:07.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_037.py
+-rw-rw-rw-   0        0        0     2053 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_038.py
+-rw-rw-rw-   0        0        0     1518 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_039.py
+-rw-rw-rw-   0        0        0     1654 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_040.py
+-rw-rw-rw-   0        0        0     4489 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_041.py
+-rw-rw-rw-   0        0        0     1573 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_042.py
+-rw-rw-rw-   0        0        0    21594 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_043.py
+-rw-rw-rw-   0        0        0    13435 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_044.py
+-rw-rw-rw-   0        0        0     1534 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_045.py
+-rw-rw-rw-   0        0        0     3136 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_046.py
+-rw-rw-rw-   0        0        0     1716 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_047.py
+-rw-rw-rw-   0        0        0     3330 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_048.py
+-rw-rw-rw-   0        0        0      382 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/position_marker.py
+-rw-rw-rw-   0        0        0      352 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/requeue_line_info.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.076389 pymarkdownlnt-0.9.9/pymarkdown/resources/
+-rw-rw-rw-   0        0        0   148128 2020-02-05 05:31:16.000000 pymarkdownlnt-0.9.9/pymarkdown/resources/entities.json
+-rw-rw-rw-   0        0        0     3015 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/source_providers.py
+-rw-rw-rw-   0        0        0    17127 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/stack_token.py
+-rw-rw-rw-   0        0        0    21077 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/tab_helper.py
+-rw-rw-rw-   0        0        0    36034 2023-02-26 16:31:54.000000 pymarkdownlnt-0.9.9/pymarkdown/tokenized_markdown.py
+-rw-rw-rw-   0        0        0     5566 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/pymarkdown/transform_state.py
+-rw-rw-rw-   0        0        0    43777 2023-02-26 16:31:55.000000 pymarkdownlnt-0.9.9/pymarkdown/transform_to_gfm.py
+-rw-rw-rw-   0        0        0    11840 2023-02-25 03:42:23.000000 pymarkdownlnt-0.9.9/pymarkdown/transform_to_gfm_list_looseness.py
+-rw-rw-rw-   0        0        0       70 2023-02-26 21:38:38.000000 pymarkdownlnt-0.9.9/pymarkdown/version.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.084397 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/
+-rw-rw-rw-   0        0        0    17317 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4673 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-02-26 21:48:14.000000 pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      570 2023-02-26 21:48:15.096408 pymarkdownlnt-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     2500 2023-02-11 16:40:01.000000 pymarkdownlnt-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-26 21:48:15.093405 pymarkdownlnt-0.9.9/test/
+-rw-rw-rw-   0        0        0     7614 2023-02-11 16:40:05.000000 pymarkdownlnt-0.9.9/test/test_application_file_scanner.py
+-rw-rw-rw-   0        0        0    13300 2023-02-11 16:40:05.000000 pymarkdownlnt-0.9.9/test/test_listfiles.py
+-rw-rw-rw-   0        0        0    61655 2023-02-12 17:35:50.000000 pymarkdownlnt-0.9.9/test/test_main.py
+-rw-rw-rw-   0        0        0    92878 2023-02-11 16:40:06.000000 pymarkdownlnt-0.9.9/test/test_markdown_extra.py
+-rw-rw-rw-   0        0        0     1549 2023-02-11 16:40:06.000000 pymarkdownlnt-0.9.9/test/test_markdown_transform_to_gfm.py
+-rw-rw-rw-   0        0        0     2484 2023-02-26 16:31:56.000000 pymarkdownlnt-0.9.9/test/test_perf.py
+-rw-rw-rw-   0        0        0     1378 2023-02-11 16:40:06.000000 pymarkdownlnt-0.9.9/test/test_transform_markdown.py
```

### Comparing `pymarkdownlnt-0.9.8/LICENSE.txt` & `pymarkdownlnt-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/PKG-INFO` & `pymarkdownlnt-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymarkdownlnt
-Version: 0.9.8
+Version: 0.9.9
 Summary: A GitHub Flavored Markdown compliant Markdown linter.
 Home-page: https://github.com/jackdewinter/pymarkdown
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/pymarkdown/blob/main/changelog.md
```

### Comparing `pymarkdownlnt-0.9.8/README.md` & `pymarkdownlnt-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/block_quote_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/block_quote_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     HtmlBlockStackToken,
     IndentedCodeBlockStackToken,
     LinkDefinitionStackToken,
     ListStackToken,
     ParagraphStackToken,
     StackToken,
 )
+from pymarkdown.tab_helper import TabHelper
 
 # pylint: disable=too-many-lines
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 
 class BlockQuoteProcessor:
@@ -48,15 +49,15 @@
         adj_ws: Optional[str] = None,
     ) -> bool:
         """
         Determine if we have the start of a block quote section.
         """
 
         assert extracted_whitespace is not None
-        return ParserHelper.is_length_less_than_or_equal_to(
+        return TabHelper.is_length_less_than_or_equal_to(
             extracted_whitespace if adj_ws is None else adj_ws, 3
         ) and ParserHelper.is_character_at_index(
             line_to_parse, start_index, BlockQuoteProcessor.__block_quote_character
         )
 
     @staticmethod
     def __adjust_lazy_handling(
@@ -150,90 +151,82 @@
                 block_quote_data = BlockQuoteData(
                     block_quote_data.current_count, stack_count
                 )
         return container_level_tokens, block_quote_data, was_paragraph_continuation
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-locals
     @staticmethod
     def __handle_block_quote_block_really_start(
         parser_state: ParserState,
         position_marker: PositionMarker,
         extracted_whitespace: Optional[str],
         grab_bag: ContainerGrabBag,
     ) -> Tuple[
         Optional[RequeueLineInfo],
         bool,
         int,
         bool,
         List[MarkdownToken],
         List[MarkdownToken],
     ]:
-        container_start_bq_count: Optional[int] = grab_bag.container_start_bq_count
-        block_quote_data: BlockQuoteData = grab_bag.block_quote_data
-
-        assert container_start_bq_count is not None
+        assert grab_bag.container_start_bq_count is not None
         POGGER.debug("handle_block_quote_block>>block-start")
+        POGGER.debug("original_line:>:$:<", grab_bag.original_line)
         (
             adjusted_text_to_parse,
             adjusted_index_number,
             leaf_tokens,
             container_level_tokens,
-            block_quote_data,
-            removed_chars_at_start,
-            did_blank,
+            grab_bag.block_quote_data,
+            grab_bag.removed_chars_at_start_of_line,
+            grab_bag.did_blank,
             last_block_quote_index,
             text_removed_by_container,
             avoid_block_starts,
             requeue_line_info,
-            force_list_continuation,
+            grab_bag.do_force_list_continuation,
         ) = BlockQuoteProcessor.__handle_block_quote_section(
             parser_state,
             position_marker,
-            block_quote_data,
+            grab_bag.block_quote_data,
             extracted_whitespace,
-            container_start_bq_count,
+            grab_bag.container_start_bq_count,
+            grab_bag.original_line,
         )
-        POGGER.debug("force_list_continuation=$", force_list_continuation)
+        POGGER.debug("force_list_continuation=$", grab_bag.do_force_list_continuation)
         POGGER.debug("adjusted_index_number>>:$:", adjusted_index_number)
         POGGER.debug(">>avoid_block_starts>>$", avoid_block_starts)
         POGGER.debug(">>text_removed_by_container>>:$:", text_removed_by_container)
 
         (
             did_process,
             end_of_bquote_start_index,
         ) = BlockQuoteProcessor.__handle_block_quote_block_kludges(
             parser_state,
-            block_quote_data,
+            grab_bag.block_quote_data,
             leaf_tokens,
             container_level_tokens,
             adjusted_text_to_parse,
             last_block_quote_index,
             adjusted_index_number,
         )
-        grab_bag.did_blank = did_blank
-        grab_bag.do_force_list_continuation = force_list_continuation
-        grab_bag.removed_chars_at_start_of_line = removed_chars_at_start
         grab_bag.start_index = adjusted_index_number
         grab_bag.line_to_parse = adjusted_text_to_parse
         grab_bag.text_removed_by_container = text_removed_by_container
         grab_bag.last_block_quote_index = last_block_quote_index
-        grab_bag.block_quote_data = block_quote_data
         return (
             requeue_line_info,
             did_process,
             end_of_bquote_start_index,
             avoid_block_starts,
             leaf_tokens,
             container_level_tokens,
         )
 
-    # pylint: enable=too-many-locals
-
     @staticmethod
     def handle_block_quote_block(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[bool, int, List[MarkdownToken], List[MarkdownToken], bool]:
         """
@@ -243,20 +236,18 @@
         extracted_whitespace: Optional[str] = grab_bag.extracted_whitespace
         adj_ws: Optional[str] = grab_bag.adj_ws
 
         (
             did_process,
             avoid_block_starts,
             end_of_bquote_start_index,
-            requeue_line_info,
         ) = (
             False,
             False,
             -1,
-            None,
         )
         grab_bag.do_force_list_continuation = False
         grab_bag.did_blank = False
         grab_bag.removed_chars_at_start_of_line = 0
         grab_bag.start_index = position_marker.index_number
         grab_bag.line_to_parse = position_marker.text_to_parse
         grab_bag.text_removed_by_container = None
@@ -325,15 +316,15 @@
                 "handle_block w/ no open>>found>>$",
                 last_block_token,
             )
             POGGER.debug("hbqblk>>last_block_token>>$", last_block_token)
             POGGER.debug(
                 "hbqblk>>leading_text_index>>$", last_block_token.leading_text_index
             )
-            last_block_token.add_leading_spaces("")
+            last_block_token.add_bleading_spaces("")
             POGGER.debug("hbqblk>>last_block_token>>$", last_block_token)
             POGGER.debug(
                 "hbqblk>>leading_text_index>>$", last_block_token.leading_text_index
             )
 
     # pylint: disable=too-many-arguments
     @staticmethod
@@ -378,15 +369,14 @@
     @staticmethod
     def __check_if_really_start(
         parser_state: ParserState,
         position_marker: PositionMarker,
         extracted_whitespace: Optional[str],
         adj_ws: Optional[str],
     ) -> Tuple[bool, Optional[RequeueLineInfo]]:
-
         assert extracted_whitespace is not None
         POGGER.debug(
             "handle_block_quote_block>>text>:$:<", position_marker.text_to_parse
         )
         POGGER.debug(
             "handle_block_quote_block>>extracted_whitespace>:$:<",
             extracted_whitespace,
@@ -421,15 +411,14 @@
                 )
         return really_start, requeue_line_info
 
     @staticmethod
     def __check_if_really_start_paragraph(
         parser_state: ParserState, position_marker: PositionMarker
     ) -> Tuple[bool, Optional[RequeueLineInfo]]:
-
         current_indent, eligible_stack, eligible_stack_index = (
             0,
             parser_state.token_stack[1:-1],
             0,
         )
 
         POGGER.debug("handle_block_quote_block>>eligible_stack>:$:<", eligible_stack)
@@ -458,41 +447,43 @@
     @staticmethod
     def __check_if_really_start_list(
         parser_state: ParserState,
         position_marker: PositionMarker,
         eligible_stack: List[StackToken],
         eligible_stack_index: int,
     ) -> Tuple[int, Optional[RequeueLineInfo]]:
-
         assert eligible_stack[eligible_stack_index].is_list
         list_token = cast(ListStackToken, eligible_stack[eligible_stack_index])
         current_indent = list_token.indent_level
         if current_indent <= position_marker.index_number:
             return current_indent, None
         POGGER.debug("BOOYAH")
         POGGER.debug("current_indent=$", current_indent)
         POGGER.debug("index_number=$", position_marker.index_number)
         POGGER.debug("eligible_stack=$", eligible_stack)
         POGGER.debug("eligible_stack_index=$", eligible_stack_index)
 
         while eligible_stack_index >= 0:
             assert eligible_stack[eligible_stack_index].is_list
             list_token = cast(ListStackToken, eligible_stack[eligible_stack_index])
-            if not list_token.indent_level > position_marker.index_number:
+            if list_token.indent_level <= position_marker.index_number:
                 break
             eligible_stack_index -= 1
         POGGER.debug("eligible_stack_index=$", eligible_stack_index)
         if eligible_stack_index >= 0:
             root_index = (
                 parser_state.token_stack.index(eligible_stack[eligible_stack_index]) + 1
             )
         else:
             root_index = 0
         POGGER.debug("root_index=$", root_index)
-        (container_level_tokens, _,) = parser_state.close_open_blocks_fn(
+        (
+            container_level_tokens,
+            _,
+        ) = parser_state.close_open_blocks_fn(
             parser_state,
             include_block_quotes=True,
             include_lists=True,
             until_this_index=root_index,
             was_forced=True,
         )
         parser_state.token_document.extend(container_level_tokens)
@@ -509,15 +500,19 @@
         is_top_of_stack_is_html_block: bool,
     ) -> Tuple[BlockQuoteData, int, str, int, bool]:
         """
         Having detected a block quote character (">") on a line, continue to consume
         and count while the block quote pattern is there.
         """
 
-        (last_block_quote_index, avoid_block_starts, adjusted_line,) = (
+        (
+            last_block_quote_index,
+            avoid_block_starts,
+            adjusted_line,
+        ) = (
             -1,
             False,
             line_to_parse,
         )
         if block_quote_data.stack_count == 0 and is_top_of_stack_fenced_code_block:
             start_index -= 1
         else:
@@ -597,15 +592,14 @@
         start_index: int,
         osi: int,
         oltp: str,
         is_top_of_stack_fenced_code_block: bool,
         avoid_block_starts: bool,
         last_block_quote_index: int,
     ) -> Tuple[bool, bool, int, str, int, int]:
-
         continue_processing = True
         POGGER.debug(
             "current_count--$--stack_count--$--is_top_of_stack_is_html_block--$",
             current_count,
             stack_count,
             is_top_of_stack_is_html_block,
         )
@@ -617,15 +611,16 @@
                 avoid_block_starts = ParserHelper.is_character_at_index(
                     adjusted_line,
                     start_index,
                     BlockQuoteProcessor.__block_quote_character,
                 )
                 POGGER.debug("avoid_block_starts=$", avoid_block_starts)
                 continue_processing = False
-            elif current_count > stack_count:
+            else:
+                assert current_count > stack_count
                 (
                     start_index,
                     adjusted_line,
                     last_block_quote_index,
                     avoid_block_starts,
                     current_count,
                     continue_processing,
@@ -637,15 +632,15 @@
                     stack_count,
                     False,
                 )
 
         if continue_processing:
             continue_processing = False
             if is_top_of_stack_fenced_code_block and (current_count >= stack_count):
-                pass
+                POGGER.debug("out of stack")
             elif start_index == len(adjusted_line):
                 POGGER.debug("ran out of line")
             elif ParserHelper.is_character_at_index_not(
                 adjusted_line,
                 start_index,
                 BlockQuoteProcessor.__block_quote_character,
             ):
@@ -714,22 +709,23 @@
                     BlockQuoteProcessor.__block_quote_character, start_index
                 )
                 POGGER.debug("+1>>next_bq_index:$:", next_bq_index)
                 if next_bq_index != -1 and (next_bq_index - start_index) <= 3:
                     continue_processing, start_index = True, next_bq_index
         return continue_processing, start_index
 
-    # pylint: disable=too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_block_quote_section(
         parser_state: ParserState,
         position_marker: PositionMarker,
         block_quote_data: BlockQuoteData,
         extracted_whitespace: Optional[str],
         container_start_bq_count: int,
+        original_line: str,
     ) -> Tuple[
         str,
         int,
         List[MarkdownToken],
         List[MarkdownToken],
         BlockQuoteData,
         int,
@@ -789,91 +785,77 @@
         POGGER.debug(">>block_quote_data.stack_count>>$", block_quote_data.stack_count)
         POGGER.debug(">>start_index>>$", start_index)
         POGGER.debug(">>original_start_index>>$", position_marker.index_number)
         POGGER.debug(">>avoid_block_starts>>$", avoid_block_starts)
 
         if last_block_quote_index != -1:
             POGGER.debug("start_index>>:$:", start_index)
-            (
-                line_to_parse,
-                start_index,
-                leaf_tokens,
-                container_level_tokens,
-                block_quote_data,
-                removed_chars_at_start,
-                did_blank,
-                text_removed_by_container,
-                requeue_line_info,
-                force_list_continuation,
-            ) = BlockQuoteProcessor.__handle_existing_block_quote(
+            return BlockQuoteProcessor.__handle_existing_block_quote(
                 parser_state,
                 block_quote_data,
                 start_index,
                 line_to_parse,
                 extracted_whitespace,
                 position_marker.index_number,
                 container_start_bq_count,
                 position_marker,
                 leaf_tokens,
                 container_level_tokens,
+                original_line,
+                last_block_quote_index,
+                avoid_block_starts,
             )
-            POGGER.debug("force_list_continuation=$", force_list_continuation)
-            POGGER.debug("start_index>>:$:", start_index)
-        else:
-            (
-                text_removed_by_container,
-                did_blank,
-                removed_chars_at_start,
-                requeue_line_info,
-                force_list_continuation,
-            ) = (None, False, 0, None, False)
 
         return (
             line_to_parse,
             start_index,
             leaf_tokens,
             container_level_tokens,
             block_quote_data,
-            removed_chars_at_start,
-            did_blank,
+            0,
+            False,
             last_block_quote_index,
-            text_removed_by_container,
+            None,
             avoid_block_starts,
-            requeue_line_info,
-            force_list_continuation,
+            None,
+            False,
         )
 
-    # pylint: enable=too-many-locals
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_existing_block_quote(
         parser_state: ParserState,
         block_quote_data: BlockQuoteData,
         start_index: int,
         line_to_parse: str,
         extracted_whitespace: Optional[str],
         original_start_index: int,
         container_start_bq_count: int,
         position_marker: PositionMarker,
         leaf_tokens: List[MarkdownToken],
         container_level_tokens: List[MarkdownToken],
+        original_line: str,
+        last_block_quote_index: int,
+        avoid_block_starts: bool,
     ) -> Tuple[
         str,
         int,
         List[MarkdownToken],
         List[MarkdownToken],
         BlockQuoteData,
         int,
         bool,
+        int,
         Optional[str],
+        bool,
         Optional[RequeueLineInfo],
         bool,
     ]:
-
         POGGER.debug(
             "__handle_block_quote_section---block_quote_data.current_count--$--$--$--",
             block_quote_data.current_count,
             start_index,
             line_to_parse,
         )
         POGGER.debug(
@@ -889,67 +871,62 @@
                 ">>block_quote_data.current_count>>$", block_quote_data.current_count
             )
             block_quote_data = BlockQuoteData(
                 block_quote_data.current_count + container_start_bq_count,
                 block_quote_data.stack_count,
             )
 
-        force_list_continuation = False
         if not parser_state.token_stack[-1].is_fenced_code_block:
-            (
-                container_level_tokens,
-                requeue_line_info,
-                line_to_parse,
-                removed_chars_at_start,
-                text_removed_by_container,
-                did_blank,
-                leaf_tokens,
-                force_list_continuation,
-            ) = BlockQuoteProcessor.__handle_non_fenced_code_section(
+            return BlockQuoteProcessor.__handle_non_fenced_code_section(
                 parser_state,
                 block_quote_data,
                 extracted_whitespace,
                 position_marker,
                 original_start_index,
                 container_start_bq_count,
                 line_to_parse,
                 start_index,
                 leaf_tokens,
+                original_line,
+                last_block_quote_index,
+                avoid_block_starts,
             )
-            POGGER.debug("force_list_continuation=$", force_list_continuation)
-        else:
-            did_blank, requeue_line_info, removed_chars_at_start = False, None, 0
-            (
-                block_quote_data,
-                line_to_parse,
-                container_level_tokens,
-                text_removed_by_container,
-            ) = BlockQuoteProcessor.__handle_fenced_code_section(
-                parser_state,
-                block_quote_data,
-                start_index,
-                line_to_parse,
-                container_level_tokens,
-            )
+
+        (
+            block_quote_data,
+            line_to_parse,
+            container_level_tokens,
+            text_removed_by_container,
+        ) = BlockQuoteProcessor.__handle_fenced_code_section(
+            parser_state,
+            block_quote_data,
+            start_index,
+            line_to_parse,
+            container_level_tokens,
+        )
 
         POGGER.debug(
             "OUT>__handle_block_quote_section---$<<<",
             line_to_parse,
         )
+        POGGER.debug("force_list_continuation=false")
+        POGGER.debug("start_index>>:$:", start_index)
         return (
             line_to_parse,
             start_index,
             leaf_tokens,
             container_level_tokens,
             block_quote_data,
-            removed_chars_at_start,
-            did_blank,
+            0,
+            False,
+            last_block_quote_index,
             text_removed_by_container,
-            requeue_line_info,
-            force_list_continuation,
+            avoid_block_starts,
+            None,
+            False,
         )
 
     # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __handle_non_fenced_code_section(
@@ -958,26 +935,31 @@
         extracted_whitespace: Optional[str],
         position_marker: PositionMarker,
         original_start_index: int,
         container_start_bq_count: int,
         line_to_parse: str,
         start_index: int,
         leaf_tokens: List[MarkdownToken],
+        original_line: str,
+        last_block_quote_index: int,
+        avoid_block_starts: bool,
     ) -> Tuple[
-        List[MarkdownToken],
-        Optional[RequeueLineInfo],
         str,
         int,
+        List[MarkdownToken],
+        List[MarkdownToken],
+        BlockQuoteData,
+        int,
+        bool,
+        int,
         Optional[str],
         bool,
-        List[MarkdownToken],
+        Optional[RequeueLineInfo],
         bool,
     ]:
-
-        did_blank, removed_chars_at_start, text_removed_by_container = False, 0, None
         POGGER.debug("handle_block_quote_section>>not fenced")
         (
             container_level_tokens,
             requeue_line_info,
             extra_consumed_whitespace,
             force_list_continuation,
         ) = BlockQuoteProcessor.__ensure_stack_at_level(
@@ -985,114 +967,188 @@
             block_quote_data,
             extracted_whitespace,
             position_marker,
             original_start_index,
             container_start_bq_count,
         )
         POGGER.debug("force_list_continuation=$", force_list_continuation)
-        if not requeue_line_info:
-            POGGER.debug("extracted_whitespace:$:", extracted_whitespace)
-            POGGER.debug("line_to_parse:$:", line_to_parse)
-            POGGER.debug("start_index:$:", start_index)
-            POGGER.debug(
-                "position_marker.index_number:$:", position_marker.index_number
-            )
-            POGGER.debug(
-                "position_marker.index_indent:$:", position_marker.index_indent
-            )
-            removed_text = f"{extracted_whitespace}{line_to_parse[position_marker.index_number : start_index]}"
-            POGGER.debug(
-                "==EWS[$],OSI[$],SI[$],LTP[$],RT=[$]",
-                extracted_whitespace,
-                original_start_index,
-                position_marker.index_number,
-                position_marker.text_to_parse,
-                removed_text,
-            )
-            (
+        if requeue_line_info:
+            return (
                 line_to_parse,
-                removed_chars_at_start,
-                stack_index,
-                text_removed_by_container,
-            ) = (
-                line_to_parse[start_index:],
                 start_index,
-                parser_state.find_last_block_quote_on_stack(),
-                removed_text,
-            )
-            POGGER.debug("==REM[$],LTP[$]", removed_text, line_to_parse)
-
-            assert stack_index != -1
-            found_bq_stack_token = cast(
-                BlockQuoteStackToken, parser_state.token_stack[stack_index]
-            )
-            assert found_bq_stack_token
-
-            BlockQuoteProcessor.__do_block_quote_leading_spaces_adjustments(
-                parser_state,
-                stack_index,
-                container_start_bq_count,
-                block_quote_data,
-                text_removed_by_container,
-                found_bq_stack_token,
-                removed_text,
-                original_start_index,
-                extra_consumed_whitespace,
+                leaf_tokens,
                 container_level_tokens,
+                block_quote_data,
+                0,
+                False,
+                last_block_quote_index,
+                None,
+                avoid_block_starts,
+                requeue_line_info,
+                force_list_continuation,
             )
-            POGGER.debug("text_removed_by_container=[$]", text_removed_by_container)
-            POGGER.debug("removed_text=[$]", removed_text)
-            if not line_to_parse.strip():
-                did_blank, leaf_tokens = BlockQuoteProcessor.__handle_normal_blank_line(
-                    parser_state,
-                    block_quote_data,
-                    position_marker,
-                    text_removed_by_container,
-                    line_to_parse,
-                )
-        return (
-            container_level_tokens,
-            requeue_line_info,
+        # POGGER.debug("extracted_whitespace:$:", extracted_whitespace)
+        # POGGER.debug("line_to_parse:$:", line_to_parse)
+        # POGGER.debug("start_index:$:", start_index)
+        # POGGER.debug(
+        #     "position_marker.index_number:$:", position_marker.index_number
+        # )
+        # POGGER.debug(
+        #     "position_marker.index_indent:$:", position_marker.index_indent
+        # )
+        removed_text = f"{extracted_whitespace}{line_to_parse[position_marker.index_number : start_index]}"
+        # POGGER.debug(
+        #     "==EWS[$],OSI[$],SI[$],LTP[$],RT=[$]",
+        #     extracted_whitespace,
+        #     original_start_index,
+        #     position_marker.index_number,
+        #     position_marker.text_to_parse,
+        #     removed_text,
+        # )
+
+        (
             line_to_parse,
             removed_chars_at_start,
             text_removed_by_container,
             did_blank,
             leaf_tokens,
+        ) = BlockQuoteProcessor.__handle_non_fenced_code_section_no_requeue(
+            parser_state,
+            position_marker,
+            line_to_parse,
+            start_index,
+            removed_text,
+            container_start_bq_count,
+            block_quote_data,
+            original_start_index,
+            extra_consumed_whitespace,
+            container_level_tokens,
+            original_line,
+        )
+        return (
+            line_to_parse,
+            start_index,
+            leaf_tokens,
+            container_level_tokens,
+            block_quote_data,
+            removed_chars_at_start,
+            did_blank,
+            last_block_quote_index,
+            text_removed_by_container,
+            avoid_block_starts,
+            None,
             force_list_continuation,
         )
 
     # pylint: enable=too-many-arguments, too-many-locals
 
     # pylint: disable=too-many-arguments
     @staticmethod
+    def __handle_non_fenced_code_section_no_requeue(
+        parser_state: ParserState,
+        position_marker: PositionMarker,
+        line_to_parse: str,
+        start_index: int,
+        removed_text: str,
+        container_start_bq_count: int,
+        block_quote_data: BlockQuoteData,
+        original_start_index: int,
+        extra_consumed_whitespace: Optional[int],
+        container_level_tokens: List[MarkdownToken],
+        original_line: str,
+    ) -> Tuple[str, int, str, bool, List[MarkdownToken]]:
+        (
+            line_to_parse,
+            stack_index,
+        ) = (
+            line_to_parse[start_index:],
+            parser_state.find_last_block_quote_on_stack(),
+        )
+        POGGER.debug("==REM[$],LTP[$]", removed_text, line_to_parse)
+
+        assert stack_index != -1
+        found_bq_stack_token = cast(
+            BlockQuoteStackToken, parser_state.token_stack[stack_index]
+        )
+        assert found_bq_stack_token
+
+        BlockQuoteProcessor.__do_block_quote_leading_spaces_adjustments(
+            parser_state,
+            stack_index,
+            container_start_bq_count,
+            block_quote_data,
+            removed_text,
+            found_bq_stack_token,
+            removed_text,
+            original_start_index,
+            extra_consumed_whitespace,
+            container_level_tokens,
+            original_line,
+        )
+        POGGER.debug("text_removed_by_container=[$]", removed_text)
+        POGGER.debug("removed_text=[$]", removed_text)
+        if line_to_parse.strip():
+            return (
+                line_to_parse,
+                start_index,
+                removed_text,
+                False,
+                [],
+            )
+        did_blank, leaf_tokens = BlockQuoteProcessor.__handle_normal_blank_line(
+            parser_state,
+            block_quote_data,
+            position_marker,
+            removed_text,
+            line_to_parse,
+        )
+        return (
+            line_to_parse,
+            start_index,
+            removed_text,
+            did_blank,
+            leaf_tokens,
+        )
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
     def __adjust_1(
         parser_state: ParserState,
         container_start_bq_count: int,
         adjusted_removed_text: str,
         text_removed_by_container: str,
         stack_index: int,
         block_quote_data: BlockQuoteData,
-    ) -> str:
+        original_line: str,
+    ) -> Tuple[str, Optional[str]]:
+        POGGER.debug("__hbqs>>container_start_bq_count>>$", container_start_bq_count)
+        POGGER.debug(
+            "__hbqs>>token_stack[stack_index - 1]>>$",
+            parser_state.token_stack[stack_index - 1],
+        )
         if (
             container_start_bq_count
             and parser_state.token_stack[stack_index - 1].is_block_quote
         ):
             block_stack_token = cast(
                 BlockQuoteStackToken, parser_state.token_stack[stack_index - 1]
             )
             count_of_actual_starts = ParserHelper.count_characters_in_text(
                 adjusted_removed_text, ">"
             )
             assert count_of_actual_starts != block_quote_data.current_count
             block_quote_token = cast(
                 BlockQuoteMarkdownToken, block_stack_token.matching_markdown_token
             )
-            adj_leading_spaces = block_quote_token.leading_spaces
+            adj_leading_spaces = block_quote_token.bleading_spaces
             assert adj_leading_spaces is not None
             POGGER.debug("__hbqs>>count_of_actual_starts>>$", count_of_actual_starts)
+            POGGER.debug("__hbqs>>original_line>:$:<", original_line)
             POGGER.debug(
                 "__hbqs>>adj_leading_spaces>>:$:$:<",
                 len(adj_leading_spaces),
                 adj_leading_spaces,
             )
             POGGER.debug(
                 "__hbqs>>adjusted_removed_text>>:$:$:<",
@@ -1101,30 +1157,74 @@
             )
             POGGER.debug(
                 "__hbqs>>text_removed_by_container>>:$:$:<",
                 len(text_removed_by_container),
                 text_removed_by_container,
             )
             last_line_index = adj_leading_spaces.rfind("\n")
-            if last_line_index != -1:
-                adj_leading_spaces = adj_leading_spaces[last_line_index + 1 :]
+            assert last_line_index == -1
+            # if last_line_index != -1:
+            #     adj_leading_spaces = adj_leading_spaces[last_line_index + 1 :]
 
             delta = len(text_removed_by_container) - len(
                 adj_leading_spaces + adjusted_removed_text
             )
             adj_leading_spaces = adj_leading_spaces + ParserHelper.repeat_string(
                 ParserHelper.space_character, delta
             )
             adjusted_removed_text = adj_leading_spaces + adjusted_removed_text
+
             POGGER.debug("__hbqs>>adjusted_removed_text>>:$:<", adjusted_removed_text)
-        return adjusted_removed_text
+
+        POGGER.debug("__hbqs>>adjusted_removed_text>>:$:<", adjusted_removed_text)
+        tabbed_removed_text = BlockQuoteProcessor.__adjust_1_with_tab(
+            original_line, adjusted_removed_text
+        )
+        return (adjusted_removed_text, tabbed_removed_text)
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
+    def __adjust_1_with_tab(
+        original_line: str, adjusted_removed_text: str
+    ) -> Optional[str]:
+        tabbed_removed_text = None
+
+        if "\t" in original_line:
+            POGGER.debug("original_line>>:$:<", original_line)
+            detabified_original_line = TabHelper.detabify_string(original_line)
+            POGGER.debug("detabified_original_line>>:$:<", detabified_original_line)
+            assert detabified_original_line.startswith(adjusted_removed_text)
+            original_line_index = 1
+            while original_line_index < len(original_line):
+                original_line_prefix = original_line[:original_line_index]
+                POGGER.debug("original_line_prefix>>:$:<", original_line_prefix)
+                detabified_original_line_prefix = TabHelper.detabify_string(
+                    original_line_prefix
+                )
+                POGGER.debug(
+                    "detabified_original_line_prefix>>:$:<",
+                    detabified_original_line_prefix,
+                )
+                if detabified_original_line_prefix == adjusted_removed_text:
+                    break
+                original_line_index += 1
+            POGGER.debug(
+                "original_line_prefix>>:$:< == detabified_original_line_prefix>>:$:<",
+                original_line_prefix,
+                detabified_original_line_prefix,
+            )
+            if (
+                adjusted_removed_text != original_line_prefix
+                and detabified_original_line_prefix == adjusted_removed_text
+            ):
+                tabbed_removed_text = original_line_prefix
+        return tabbed_removed_text
+
+    @staticmethod
     def __find_original_token(
         parser_state: ParserState, found_bq_stack_token: StackToken
     ) -> Optional[MarkdownToken]:
         original_token = None
         for block_copy_token in parser_state.block_copy:
             if not block_copy_token:
                 continue
@@ -1137,81 +1237,90 @@
                 and found_bq_stack_token.matching_markdown_token.column_number
                 == block_copy_token.column_number
             ):
                 original_token = block_copy_token
                 break
         return original_token
 
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __adjust_2(
         parser_state: ParserState,
         found_bq_stack_token: StackToken,
         original_removed_text: str,
         adjusted_removed_text: str,
         extra_consumed_whitespace: Optional[int],
+        tabbed_removed_text: Optional[str],
     ) -> Tuple[bool, str]:
         POGGER.debug("original_removed_text>>:$:", original_removed_text)
         POGGER.debug("extra_consumed_whitespace>>:$:", extra_consumed_whitespace)
         POGGER.debug("parser_state.block_copy>>$", parser_state.block_copy)
         special_case = False
+        olad = adjusted_removed_text
         if parser_state.block_copy and found_bq_stack_token:
-
             POGGER.debug("parser_state.block_copy>>search")
             if original_token := BlockQuoteProcessor.__find_original_token(
                 parser_state, found_bq_stack_token
             ):
                 original_block_quote_token = cast(
                     BlockQuoteMarkdownToken, original_token
                 )
                 assert found_bq_stack_token.matching_markdown_token is not None
                 POGGER.debug("original_token>>$", original_block_quote_token)
-                assert original_block_quote_token.leading_spaces is not None
+                assert original_block_quote_token.bleading_spaces is not None
                 POGGER.debug(
-                    "original_token.leading_spaces>>:$:<<",
-                    original_block_quote_token.leading_spaces,
+                    "original_token.bleading_spaces>>:$:<<",
+                    original_block_quote_token.bleading_spaces,
                 )
                 block_quote_markdown_token = cast(
                     BlockQuoteMarkdownToken,
                     found_bq_stack_token.matching_markdown_token,
                 )
-                current_leading_spaces = block_quote_markdown_token.leading_spaces
+                current_leading_spaces = block_quote_markdown_token.bleading_spaces
                 assert current_leading_spaces is not None
                 POGGER.debug("found_bq_stack_token.ls>>:$:<<", current_leading_spaces)
                 assert current_leading_spaces.startswith(
-                    original_block_quote_token.leading_spaces
+                    original_block_quote_token.bleading_spaces
                 )
                 (
                     special_case,
                     adjusted_removed_text,
                 ) = BlockQuoteProcessor.__adjust_2_fix_leading_spaces(
                     special_case,
                     adjusted_removed_text,
                     original_removed_text,
                     original_block_quote_token,
                     current_leading_spaces,
                     extra_consumed_whitespace,
                 )
+
+        if tabbed_removed_text:
+            assert olad == adjusted_removed_text
         return special_case, adjusted_removed_text
 
+    # pylint: enable=too-many-arguments
+
     # pylint: disable=too-many-arguments
     @staticmethod
     def __adjust_2_fix_leading_spaces(
         special_case: bool,
         adjusted_removed_text: str,
         original_removed_text: str,
         original_block_quote_token: BlockQuoteMarkdownToken,
         current_leading_spaces: str,
         extra_consumed_whitespace: Optional[int],
     ) -> Tuple[bool, str]:
         POGGER.debug("original_removed_text>>:$:", original_removed_text)
         POGGER.debug("adjusted_removed_text>>:$:", adjusted_removed_text)
-        assert original_block_quote_token.leading_spaces is not None
-        if len(current_leading_spaces) > len(original_block_quote_token.leading_spaces):
+        assert original_block_quote_token.bleading_spaces is not None
+        if len(current_leading_spaces) > len(
+            original_block_quote_token.bleading_spaces
+        ):
             current_leading_spaces = current_leading_spaces[
-                len(original_block_quote_token.leading_spaces) :
+                len(original_block_quote_token.bleading_spaces) :
             ]
             POGGER.debug("current_leading_spaces>>:$:", current_leading_spaces)
             assert current_leading_spaces[0] == "\n"
             current_leading_spaces = current_leading_spaces[1:]
             POGGER.debug(
                 "current_leading_spaces>>:$:($)",
                 current_leading_spaces,
@@ -1272,16 +1381,16 @@
         block_quote_data: BlockQuoteData,
         text_removed_by_container: str,
         found_bq_stack_token: BlockQuoteStackToken,
         removed_text: str,
         original_start_index: int,
         extra_consumed_whitespace: Optional[int],
         container_level_tokens: List[MarkdownToken],
+        original_line: str,
     ) -> None:
-
         POGGER.debug("__hbqs>>removed_text>>:$:<", removed_text)
         POGGER.debug("__hbqs>>container_start_bq_count>>$", container_start_bq_count)
         POGGER.debug("__hbqs>>original_start_index>>$", original_start_index)
         POGGER.debug("token_stack--$", parser_state.token_stack)
         original_start_index = BlockQuoteProcessor.__block_quote_start_adjust(
             parser_state, original_start_index, container_level_tokens
         )
@@ -1289,60 +1398,87 @@
         adjusted_removed_text = (
             removed_text[original_start_index:]
             if container_start_bq_count and original_start_index
             else removed_text
         )
 
         POGGER.debug("dbqlsa>>adjusted_removed_text>>:$:<", adjusted_removed_text)
-        adjusted_removed_text = BlockQuoteProcessor.__adjust_1(
+        (
+            adjusted_removed_text,
+            tabbed_removed_text,
+        ) = BlockQuoteProcessor.__adjust_1(
             parser_state,
             container_start_bq_count,
             adjusted_removed_text,
             text_removed_by_container,
             stack_index,
             block_quote_data,
+            original_line,
         )
-
-        assert found_bq_stack_token.matching_markdown_token is not None
-        block_quote_token = cast(
-            BlockQuoteMarkdownToken, found_bq_stack_token.matching_markdown_token
-        )
+        POGGER.debug("dbqlsa>>adjusted_removed_text>>:$:<", adjusted_removed_text)
+        POGGER.debug("dbqlsa>>tabbed_removed_text>>:$:<", tabbed_removed_text)
 
         POGGER.debug("__hbqs>>adjusted_removed_text>>:$:<", adjusted_removed_text)
+        POGGER.debug("__hbqs>>tabbed_removed_text>>:$:<", tabbed_removed_text)
         POGGER.debug("token_stack--$", parser_state.token_stack)
         POGGER.debug("token_document--$", parser_state.token_document)
         POGGER.debug("dbqlsa>>found_bq_stack_token>>$", found_bq_stack_token)
-        POGGER.debug("dbqlsa>>bq>>$", block_quote_token)
 
         POGGER.debug("dbqlsa>>adjusted_removed_text>>:$:<<", adjusted_removed_text)
         special_case, adjusted_removed_text = BlockQuoteProcessor.__adjust_2(
             parser_state,
             found_bq_stack_token,
             original_removed_text,
             adjusted_removed_text,
             extra_consumed_whitespace,
+            tabbed_removed_text,
         )
         POGGER.debug("dbqlsa>>adjusted_removed_text>>:$:<<", adjusted_removed_text)
         POGGER.debug("dbqlsa>>special_case>>$", special_case)
 
+        BlockQuoteProcessor.__do_block_quote_leading_spaces_adjustments_adjust_bleading(
+            found_bq_stack_token,
+            tabbed_removed_text,
+            adjusted_removed_text,
+            special_case,
+        )
+
+    # pylint: enable=too-many-arguments
+
+    @staticmethod
+    def __do_block_quote_leading_spaces_adjustments_adjust_bleading(
+        found_bq_stack_token: BlockQuoteStackToken,
+        tabbed_removed_text: Optional[str],
+        adjusted_removed_text: str,
+        special_case: bool,
+    ) -> None:
+        assert found_bq_stack_token.matching_markdown_token is not None
+        block_quote_token = cast(
+            BlockQuoteMarkdownToken, found_bq_stack_token.matching_markdown_token
+        )
         POGGER.debug("dbqlsa>>last_block_token>>$", block_quote_token)
         POGGER.debug(
             "dbqlsa>>leading_text_index>>$", block_quote_token.leading_text_index
         )
-        block_quote_token.add_leading_spaces(adjusted_removed_text, special_case)
+        POGGER.debug("dbqlsa>>bq>>$", block_quote_token)
+        POGGER.debug("dbqlsa>>tabbed_removed_text>>$", tabbed_removed_text)
+
+        block_quote_token.add_bleading_spaces(
+            adjusted_removed_text,
+            special_case,
+            tabbed_removed_text,
+        )
         block_quote_token.leading_text_index += 1
         POGGER.debug("dbqlsa>>last_block_token>>$", block_quote_token)
         POGGER.debug(
             "dbqlsa>>leading_text_index>>$", block_quote_token.leading_text_index
         )
 
         POGGER.debug("__hbqs>>bq>>$", block_quote_token)
 
-    # pylint: enable=too-many-arguments
-
     @staticmethod
     def __handle_normal_blank_line(
         parser_state: ParserState,
         block_quote_data: BlockQuoteData,
         position_marker: PositionMarker,
         text_removed_by_container: str,
         line_to_parse: str,
@@ -1376,25 +1512,25 @@
         ):
             list_token = cast(
                 ListStartMarkdownToken,
                 parser_state.token_stack[1].matching_markdown_token,
             )
             list_token.add_leading_spaces("")
 
+        assert leaf_tokens is not None
         return True, leaf_tokens
 
     @staticmethod
     def __handle_fenced_code_section(
         parser_state: ParserState,
         block_quote_data: BlockQuoteData,
         start_index: int,
         line_to_parse: str,
         container_level_tokens: List[MarkdownToken],
     ) -> Tuple[BlockQuoteData, str, List[MarkdownToken], str]:
-
         POGGER.debug("handle_block_quote_section>>fenced")
         assert start_index >= 0
         removed_text, line_to_parse = (
             line_to_parse[:start_index],
             line_to_parse[start_index:],
         )
 
@@ -1404,15 +1540,18 @@
             "__hbqs>>block_quote_data.current_count>>$", block_quote_data.current_count
         )
         POGGER.debug(
             "__hbqs>>block_quote_data.stack_count>>$", block_quote_data.stack_count
         )
 
         if block_quote_data.current_count < block_quote_data.stack_count:
-            (container_level_tokens, _,) = parser_state.close_open_blocks_fn(
+            (
+                container_level_tokens,
+                _,
+            ) = parser_state.close_open_blocks_fn(
                 parser_state,
                 only_these_blocks=[
                     FencedCodeBlockStackToken,
                 ],
                 was_forced=True,
             )
             block_quote_data = BlockQuoteProcessor.__decrease_stack_to_level(
@@ -1429,15 +1568,15 @@
             found_bq_stack_token,
         )
         found_bq_token = cast(
             BlockQuoteMarkdownToken, found_bq_stack_token.matching_markdown_token
         )
         POGGER.debug("hfcs>>last_block_token>>$", found_bq_token)
         POGGER.debug("hfcs>>leading_text_index>>$", found_bq_token.leading_text_index)
-        found_bq_token.add_leading_spaces(removed_text)
+        found_bq_token.add_bleading_spaces(removed_text)
         found_bq_token.leading_text_index += 1
         POGGER.debug("hfcs>>last_block_token>>$", found_bq_token)
         POGGER.debug("hfcs>>leading_text_index>>$", found_bq_token.leading_text_index)
         text_removed_by_container = removed_text
 
         return (
             block_quote_data,
@@ -1453,15 +1592,14 @@
         current_stack_index: int,
         indent_text_count: int,
         length_of_available_whitespace: int,
         extra_consumed_whitespace: int,
         adjust_current_block_quote: bool,
         last_bq_index: int,
     ) -> Tuple[int, int, int, int]:
-
         assert parser_state.token_stack[current_stack_index].is_list
         list_stack_token = cast(
             ListStackToken, parser_state.token_stack[current_stack_index]
         )
         POGGER.debug(
             "indent_level:$:indent_text_count:$:",
             list_stack_token.indent_level,
@@ -1491,15 +1629,15 @@
                 "__calculate_stack_hard_limit>>last_block_token>>$",
                 parser_state.token_stack[last_bq_index].matching_markdown_token,
             )
             block_token = cast(
                 BlockQuoteMarkdownToken,
                 parser_state.token_stack[last_bq_index].matching_markdown_token,
             )
-            block_token.add_leading_spaces(
+            block_token.add_bleading_spaces(
                 ParserHelper.repeat_string(ParserHelper.space_character, delta), True
             )
             POGGER.debug(
                 "__calculate_stack_hard_limit>>last_block_token>>$", block_token
             )
 
         return (
@@ -2040,15 +2178,18 @@
         container_level_tokens: List[MarkdownToken],
     ) -> BlockQuoteData:
         while current_count < stack_count:
             POGGER.debug(
                 "decreasing block quotes by one>>",
             )
             stack_count -= 1
-            (new_tokens, _,) = parser_state.close_open_blocks_fn(
+            (
+                new_tokens,
+                _,
+            ) = parser_state.close_open_blocks_fn(
                 parser_state,
                 include_block_quotes=True,
                 until_this_index=len(parser_state.token_stack) - 1,
                 was_forced=True,
             )
             container_level_tokens.extend(new_tokens)
         return BlockQuoteData(current_count, stack_count)
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/coalesce_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/coalesce_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 from pymarkdown.inline_markdown_token import TextMarkdownToken
 from pymarkdown.leaf_markdown_token import (
     IndentedCodeBlockMarkdownToken,
     ParagraphMarkdownToken,
 )
 from pymarkdown.markdown_token import MarkdownToken
+from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 
 # pylint: disable=too-few-public-methods
 class CoalesceProcessor:
     """
@@ -25,36 +27,42 @@
     def coalesce_text_blocks(
         first_pass_results: List[MarkdownToken],
     ) -> List[MarkdownToken]:
         """
         Take a pass and combine any two adjacent text blocks into one.
         """
         coalesced_list = [first_pass_results[0]]
+        # POGGER.debug("coalesced_list:$:", coalesced_list)
         for coalesce_index in range(1, len(first_pass_results)):
             POGGER.debug(
                 "coalesce_text_blocks>>>>$<<",
                 first_pass_results[coalesce_index],
             )
             if coalesced_list[-1].is_text:
+                # POGGER.debug("__coalesce_with_previous")
                 did_process = CoalesceProcessor.__coalesce_with_previous(
                     first_pass_results, coalesced_list, coalesce_index
                 )
             else:
                 did_process = (
                     first_pass_results[coalesce_index].is_blank_line
                     and coalesced_list[-1].is_code_block
                 )
                 if did_process:
+                    # POGGER.debug("__coalesce_with_blank_line")
                     CoalesceProcessor.__coalesce_with_blank_line(
                         first_pass_results, coalesced_list, coalesce_index
                     )
             if not did_process:
                 coalesced_list.append(first_pass_results[coalesce_index])
+                # POGGER.debug("coalesced_list:$:", coalesced_list)
 
+        # POGGER.debug("--Final--coalesced_list:$:", coalesced_list)
         CoalesceProcessor.__calculate_final_whitespaces(coalesced_list)
+        # POGGER.debug("coalesced_list:$:", coalesced_list)
 
         return coalesced_list
 
     @staticmethod
     def __calculate_final_whitespaces(coalesced_list: List[MarkdownToken]) -> None:
         for coalesce_index in range(1, len(coalesced_list)):
             if coalesced_list[coalesce_index].is_text and (
@@ -63,14 +71,16 @@
             ):
                 text_token = cast(TextMarkdownToken, coalesced_list[coalesce_index])
                 POGGER.debug("full_paragraph_text>$<", text_token)
                 POGGER.debug(
                     "full_paragraph_text>$<",
                     text_token.token_text,
                 )
+                # POGGER.debug("text_token.tabified_text=:$:", text_token.tabified_text)
+                # POGGER.debug("text_token.token_text=:$:", text_token.token_text)
                 removed_ws = text_token.remove_final_whitespace()
                 POGGER.debug(
                     "full_paragraph_text>$<",
                     text_token.token_text,
                 )
 
                 paragraph_or_setext_token = cast(
@@ -82,58 +92,53 @@
 
     @staticmethod
     def __coalesce_with_previous(
         first_pass_results: List[MarkdownToken],
         coalesced_list: List[MarkdownToken],
         coalesce_index: int,
     ) -> bool:
-
-        POGGER.debug(">>coalesce_text_blocks>>>>$<<", coalesced_list[-1])
-        if first_pass_results[coalesce_index].is_text or (
-            first_pass_results[coalesce_index].is_blank_line
-            and coalesced_list[-2].is_code_block
+        # POGGER.debug(">>coalesce_text_blocks>>>>$<<", coalesced_list[-1])
+        if not first_pass_results[coalesce_index].is_text and (
+            not first_pass_results[coalesce_index].is_blank_line
+            or not coalesced_list[-2].is_code_block
         ):
-
-            POGGER.debug("text-text>>$<<", coalesced_list[-2])
-            if coalesced_list[-2].is_indented_code_block:
-                indented_token = cast(
-                    IndentedCodeBlockMarkdownToken, coalesced_list[-2]
-                )
-                remove_leading_spaces = len(indented_token.extracted_whitespace)
-            elif (
-                coalesced_list[-2].is_paragraph or coalesced_list[-2].is_setext_heading
-            ):
-                remove_leading_spaces = -1
-            else:
-                remove_leading_spaces = 0
-
-            text_token = cast(TextMarkdownToken, coalesced_list[-1])
-            POGGER.debug("remove_leading_spaces>>$", remove_leading_spaces)
-            POGGER.debug("combine1>>$", text_token)
-            POGGER.debug("combine2>>$", first_pass_results[coalesce_index])
-            indented_whitespace = text_token.combine(
-                first_pass_results[coalesce_index], remove_leading_spaces
+            return False
+            # POGGER.debug("text-text>>$<<", coalesced_list[-2])
+        if coalesced_list[-2].is_indented_code_block:
+            indented_token = cast(IndentedCodeBlockMarkdownToken, coalesced_list[-2])
+            remove_leading_spaces = (
+                TabHelper.calculate_length(indented_token.extracted_whitespace)
+                if ParserHelper.tab_character in indented_token.extracted_whitespace
+                else len(indented_token.extracted_whitespace)
             )
-            POGGER.debug("combined>>$", text_token)
-            POGGER.debug("indented_whitespace>>$<<", indented_whitespace)
-            if coalesced_list[-2].is_indented_code_block:
-                indented_token = cast(
-                    IndentedCodeBlockMarkdownToken, coalesced_list[-2]
-                )
-                indented_token.add_indented_whitespace(indented_whitespace)
-            return True
-        return False
+        elif coalesced_list[-2].is_paragraph or coalesced_list[-2].is_setext_heading:
+            remove_leading_spaces = -1
+        else:
+            remove_leading_spaces = 0
+
+        text_token = cast(TextMarkdownToken, coalesced_list[-1])
+        # POGGER.debug("remove_leading_spaces>>$", remove_leading_spaces)
+        # POGGER.debug("combine1>>$", text_token)
+        # POGGER.debug("combine2>>$", first_pass_results[coalesce_index])
+        indented_whitespace = text_token.combine(
+            first_pass_results[coalesce_index], remove_leading_spaces
+        )
+        # POGGER.debug("combined>>$", text_token)
+        # POGGER.debug("indented_whitespace>>$<<", indented_whitespace)
+        if coalesced_list[-2].is_indented_code_block:
+            indented_token = cast(IndentedCodeBlockMarkdownToken, coalesced_list[-2])
+            indented_token.add_indented_whitespace(indented_whitespace)
+        return True
 
     @staticmethod
     def __coalesce_with_blank_line(
         first_pass_results: List[MarkdownToken],
         coalesced_list: List[MarkdownToken],
         coalesce_index: int,
     ) -> None:
-
         POGGER.debug("was>>$", first_pass_results[coalesce_index])
         text_token = cast(TextMarkdownToken, first_pass_results[coalesce_index])
         replacement_token = TextMarkdownToken(
             "",
             text_token.extracted_whitespace,
             line_number=text_token.line_number,
             column_number=text_token.column_number,
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/constants.py` & `pymarkdownlnt-0.9.9/pymarkdown/constants.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/container_block_leaf_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/container_block_leaf_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 from pymarkdown.block_quote_data import BlockQuoteData
 from pymarkdown.container_grab_bag import ContainerGrabBag
 from pymarkdown.container_markdown_token import (
     BlockQuoteMarkdownToken,
     ListStartMarkdownToken,
 )
-from pymarkdown.html_helper import HtmlHelper
-from pymarkdown.inline_markdown_token import TextMarkdownToken
 from pymarkdown.leaf_block_processor import LeafBlockProcessor
 from pymarkdown.leaf_block_processor_paragraph import LeafBlockProcessorParagraph
 from pymarkdown.link_reference_definition_helper import LinkReferenceDefinitionHelper
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.parser_state import ParserState
 from pymarkdown.position_marker import PositionMarker
 from pymarkdown.stack_token import ListStackToken
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 # pylint: disable=too-many-lines
+# pylint: disable=too-few-public-methods
 
 
 class ContainerBlockLeafProcessor:
     """
     Class to provide processing for the handling of leaf elements within container blocks.
     """
 
@@ -181,46 +181,63 @@
         Parse the contents of a line for a leaf block.
 
         Note: This is one of the more heavily traffic functions in the
         parser.  Debugging should be uncommented only if needed.
         """
         POGGER.debug("parsing leaf tokens")
         POGGER.debug("Leaf Line:$:", position_marker.text_to_parse)
+        POGGER.debug("original_line:$:", grab_bag.original_line)
+        detabified_original_line = TabHelper.detabify_string(grab_bag.original_line)
+        detabified_original_start_index = detabified_original_line.find(
+            position_marker.text_to_parse
+        )
+        assert detabified_original_start_index != -1
+        POGGER.debug(
+            "detabified_original_start_index:$:", detabified_original_start_index
+        )
 
         (
             outer_processed,
             leaf_block_position_marker,
             leaf_token_whitespace,
         ) = ContainerBlockLeafProcessor.__handle_block_leaf_tokens(
-            parser_state, position_marker, grab_bag
+            parser_state, position_marker, detabified_original_start_index, grab_bag
         )
 
         if not outer_processed:
             new_tokens = (
                 LeafBlockProcessor.parse_atx_headings(
-                    parser_state, leaf_block_position_marker, leaf_token_whitespace
+                    parser_state,
+                    leaf_block_position_marker,
+                    leaf_token_whitespace,
+                    grab_bag.block_quote_data,
+                    grab_bag.original_line,
                 )
                 or LeafBlockProcessor.parse_indented_code_block(
                     parser_state,
                     leaf_block_position_marker,
                     leaf_token_whitespace,
                     grab_bag.removed_chars_at_start_of_line,
                     grab_bag.last_block_quote_index,
+                    grab_bag.last_list_start_index,
+                    grab_bag.original_line,
                 )
                 or LeafBlockProcessor.parse_setext_headings(
                     parser_state,
                     leaf_block_position_marker,
                     leaf_token_whitespace,
                     grab_bag.block_quote_data,
+                    grab_bag.original_line,
                 )
                 or LeafBlockProcessor.parse_thematic_break(
                     parser_state,
                     leaf_block_position_marker,
                     leaf_token_whitespace,
                     grab_bag.block_quote_data,
+                    grab_bag.original_line,
                 )
                 or LeafBlockProcessorParagraph.parse_paragraph(
                     parser_state,
                     leaf_block_position_marker,
                     leaf_token_whitespace,
                     grab_bag.block_quote_data,
                     grab_bag.text_removed_by_container,
@@ -230,17 +247,17 @@
             # POGGER.debug(">>leaf--adding>>$", new_tokens)
             grab_bag.extend_leaf_tokens(new_tokens)
 
     @staticmethod
     def __handle_block_leaf_tokens(
         parser_state: ParserState,
         incoming_position_marker: PositionMarker,
+        detabified_original_start_index: int,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[bool, PositionMarker, Optional[str]]:
-
         POGGER.debug(
             "line>>$>>index>>$>>",
             incoming_position_marker.text_to_parse,
             incoming_position_marker.index_number,
         )
         remaining_line_to_parse = incoming_position_marker.text_to_parse[
             incoming_position_marker.index_number :
@@ -255,27 +272,27 @@
         position_marker = PositionMarker(
             incoming_position_marker.line_number,
             new_index_number,
             incoming_position_marker.text_to_parse,
             index_indent=incoming_position_marker.index_indent,
         )
 
-        pre_tokens = (
-            ContainerBlockLeafProcessor.__close_indented_block_if_indent_not_there(
-                parser_state, leaf_token_whitespace
-            )
+        pre_tokens = LeafBlockProcessor.close_indented_block_if_indent_not_there(
+            parser_state, leaf_token_whitespace
         )
 
         new_tokens: List[MarkdownToken] = []
-        outer_processed = ContainerBlockLeafProcessor.__handle_fenced_code_block(
+        outer_processed = LeafBlockProcessor.handle_fenced_code_block(
             parser_state,
             position_marker,
             leaf_token_whitespace,
             new_tokens,
             grab_bag.original_line,
+            detabified_original_start_index,
+            grab_bag.block_quote_data,
         )
 
         ignore_lrd_start = (
             grab_bag.do_ignore_link_definition_start
             or parser_state.token_stack[-1].is_html_block
         )
 
@@ -286,174 +303,34 @@
             parser_state,
             outer_processed,
             position_marker,
             leaf_token_whitespace,
             remaining_line_to_parse,
             ignore_lrd_start,
             pre_tokens,
+            grab_bag.original_line,
         )
 
-        outer_processed = ContainerBlockLeafProcessor.__handle_html_block(
+        outer_processed = LeafBlockProcessor.handle_html_block(
             parser_state,
             position_marker,
             outer_processed,
             leaf_token_whitespace,
             new_tokens,
+            grab_bag,
         )
         grab_bag.extend_leaf_tokens(pre_tokens)
         grab_bag.extend_leaf_tokens(new_tokens)
         return (
             outer_processed,
             position_marker,
             leaf_token_whitespace,
         )
 
     @staticmethod
-    def __handle_html_block(
-        parser_state: ParserState,
-        position_marker: PositionMarker,
-        outer_processed: bool,
-        leaf_token_whitespace: Optional[str],
-        new_tokens: List[MarkdownToken],
-    ) -> bool:
-        """
-        Take care of the processing for html blocks.
-        """
-
-        POGGER.debug(">>position_marker>>ttp>>$>>", position_marker.text_to_parse)
-        POGGER.debug(">>position_marker>>in>>$>>", position_marker.index_number)
-        POGGER.debug(">>position_marker>>ln>>$>>", position_marker.line_number)
-        if not outer_processed and not parser_state.token_stack[-1].is_html_block:
-            POGGER.debug(">>html started?>>")
-            old_top_of_stack = parser_state.token_stack[-1]
-            html_tokens = HtmlHelper.parse_html_block(
-                parser_state,
-                position_marker,
-                leaf_token_whitespace,
-            )
-            if html_tokens:
-                POGGER.debug(">>html started>>")
-                LeafBlockProcessor.correct_for_leaf_block_start_in_list(
-                    parser_state,
-                    position_marker.index_indent,
-                    old_top_of_stack,
-                    html_tokens,
-                )
-            new_tokens.extend(html_tokens)
-        if parser_state.token_stack[-1].is_html_block:
-            POGGER.debug(">>html continued>>")
-            assert leaf_token_whitespace is not None
-            html_tokens = HtmlHelper.check_normal_html_block_end(
-                parser_state,
-                position_marker.text_to_parse,
-                position_marker.index_number,
-                leaf_token_whitespace,
-                position_marker,
-            )
-            assert html_tokens
-            new_tokens.extend(html_tokens)
-            outer_processed = True
-        else:
-            POGGER.debug(">>html not encountered>>")
-
-        return outer_processed
-
-    @staticmethod
-    def __handle_fenced_code_block(
-        parser_state: ParserState,
-        position_marker: PositionMarker,
-        leaf_token_whitespace: Optional[str],
-        new_tokens: List[MarkdownToken],
-        original_line: str,
-    ) -> bool:
-        """
-        Take care of the processing for fenced code blocks.
-        """
-        if parser_state.token_stack[-1].was_link_definition_started:
-            return False
-
-        POGGER.debug(">>__handle_fenced_code_block>>start")
-        (
-            fenced_tokens,
-            leaf_token_whitespace,
-        ) = LeafBlockProcessor.parse_fenced_code_block(
-            parser_state, position_marker, leaf_token_whitespace, original_line
-        )
-        if fenced_tokens:
-            new_tokens.extend(fenced_tokens)
-            POGGER.debug(">>new_tokens>>$", new_tokens)
-        elif parser_state.token_stack[-1].is_fenced_code_block:
-            assert leaf_token_whitespace is not None
-            new_tokens.append(
-                TextMarkdownToken(
-                    position_marker.text_to_parse[position_marker.index_number :],
-                    leaf_token_whitespace,
-                    position_marker=position_marker,
-                )
-            )
-            POGGER.debug(">>new_tokens>>$", new_tokens)
-        else:
-            return False
-        return True
-
-    @staticmethod
-    def __close_indented_block_if_indent_not_there(
-        parser_state: ParserState, leaf_token_whitespace: Optional[str]
-    ) -> List[MarkdownToken]:
-
-        POGGER.debug(
-            "__close_indented_block_if_indent_not_there>>$>",
-            parser_state.token_stack[-1],
-        )
-        POGGER.debug("leaf_token_whitespace>>$>", leaf_token_whitespace)
-        pre_tokens: List[MarkdownToken] = []
-        assert leaf_token_whitespace is not None
-        if parser_state.token_stack[
-            -1
-        ].is_indented_code_block and ParserHelper.is_length_less_than_or_equal_to(
-            leaf_token_whitespace, 3
-        ):
-            pre_tokens.append(
-                parser_state.token_stack[
-                    -1
-                ].generate_close_markdown_token_from_stack_token()
-            )
-            del parser_state.token_stack[-1]
-
-            extracted_blank_line_tokens = (
-                ContainerBlockLeafProcessor.extract_markdown_tokens_back_to_blank_line(
-                    parser_state, False
-                )
-            )
-            extracted_blank_line_tokens.reverse()
-            pre_tokens.extend(extracted_blank_line_tokens)
-        POGGER.debug(
-            "__close_indented_block_if_indent_not_there>>pre_tokens>$>", pre_tokens
-        )
-        return pre_tokens
-
-    @staticmethod
-    def extract_markdown_tokens_back_to_blank_line(
-        parser_state: ParserState, was_forced: bool
-    ) -> List[MarkdownToken]:
-        """
-        Extract tokens going back to the last blank line token.
-        """
-
-        pre_tokens: List[MarkdownToken] = []
-        while parser_state.token_document[-1].is_blank_line:
-            last_element = parser_state.token_document[-1]
-            if was_forced:
-                pre_tokens.insert(0, last_element)
-            else:
-                pre_tokens.append(last_element)
-            del parser_state.token_document[-1]
-        return pre_tokens
-
-    @staticmethod
     def __handle_special_block_quote_reduction(
         parser_state: ParserState,
         last_block_index: int,
         last_list_index: int,
         grab_bag: ContainerGrabBag,
     ) -> None:
         assert grab_bag.is_leaf_tokens_empty()
@@ -471,14 +348,16 @@
             and not last_list_index
         ):
             POGGER.debug("yes special_block_quote_reduction")
             stack_delta = (
                 grab_bag.block_quote_data.stack_count
                 - grab_bag.block_quote_data.current_count
             )
+            if parser_state.token_stack[-1].was_link_definition_started:
+                stack_delta += 1
             (
                 close_tokens,
                 grab_bag.requeue_line_info,
             ) = parser_state.close_open_blocks_fn(
                 parser_state,
                 include_block_quotes=True,
                 was_forced=True,
@@ -760,15 +639,14 @@
         parser_state: ParserState,
         xposition_marker: PositionMarker,
         last_block_index: int,
         total_ws: int,
         actual_removed_leading_space: Optional[str],
         grab_bag: ContainerGrabBag,
     ) -> PositionMarker:
-
         POGGER.debug("??? adjust_containers_before_leaf_blocks")
         if (
             xposition_marker.text_to_parse
             and not grab_bag.was_paragraph_continuation
             and not grab_bag.was_indent_already_processed
         ):
             (
@@ -820,15 +698,14 @@
 
     @staticmethod
     def __post_leaf_block_adjustment(
         parser_state: ParserState,
         orig_text_removed_by_container: Optional[str],
         line_number: int,
     ) -> None:
-
         last_block_index = parser_state.find_last_block_quote_on_stack()
         POGGER.debug("last_block_index>>:$:", last_block_index)
         if not last_block_index:
             return
 
         last_block_token = cast(
             BlockQuoteMarkdownToken,
@@ -841,15 +718,15 @@
             POGGER.debug(
                 "plt-c>>last_block_token>>$",
                 last_block_token,
             )
             POGGER.debug(
                 "plt-c>>leading_text_index>>$", last_block_token.leading_text_index
             )
-            last_block_token.add_leading_spaces("")
+            last_block_token.add_bleading_spaces("")
             last_block_token.leading_text_index += 1
             POGGER.debug("plt-c>>last_block_token>>$", last_block_token)
             POGGER.debug(
                 "plt-c>>leading_text_index>>$", last_block_token.leading_text_index
             )
 
     @staticmethod
@@ -895,25 +772,21 @@
         )
         assert parser_state.original_line_to_parse
         if grab_bag.weird_adjusted_text:
             new_index_indent = len(grab_bag.weird_adjusted_text)
             grab_bag.text_removed_by_container = grab_bag.weird_adjusted_text
             new_text_to_parse = parser_state.original_line_to_parse[new_index_indent:]
         else:
-            # POGGER.debug("total_ws>>:$:<", total_ws)
             POGGER.debug("current_indent_level>>:$:<", current_indent_level)
             current_indent_level -= xposition_marker.index_indent
-            # total_ws -= xposition_marker.index_indent
-            # POGGER.debug("total_ws>>:$:<", total_ws)
             POGGER.debug("current_indent_level>>:$:<", current_indent_level)
             assert current_indent_level >= 0
 
             prefix_text = xposition_marker.text_to_parse[:current_indent_level]
             new_text_to_parse = xposition_marker.text_to_parse[current_indent_level:]
-            new_index_indent = xposition_marker.index_indent + current_indent_level
 
             new_index_indent = len(parser_state.original_line_to_parse) - len(
                 new_text_to_parse
             )
 
             POGGER.debug("new_text_to_parse>>:$:<", new_text_to_parse)
             POGGER.debug("new_index_indent>>:$:<", new_index_indent)
@@ -1097,7 +970,10 @@
         proposed_indent_level = (
             len(text_removed_by_container) if text_removed_by_container else 0
         ) + base_indent_level
         POGGER.debug("last bq token, processing:$", proposed_indent_level)
         return proposed_indent_level, non_last_block_index
 
     # pylint: enable=too-many-arguments
+
+
+# pylint: enable=too-few-public-methods
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/container_block_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/container_block_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from pymarkdown.markdown_token import EndMarkdownToken, MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.parser_state import ParserState
 from pymarkdown.position_marker import PositionMarker
 from pymarkdown.requeue_line_info import RequeueLineInfo
 from pymarkdown.stack_token import ListStackToken
+from pymarkdown.tab_helper import TabHelper
 
 if TYPE_CHECKING:  # pragma: no cover
     from pymarkdown.parse_block_pass_properties import ParseBlockPassProperties
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 # pylint: disable=too-many-lines
@@ -43,15 +44,14 @@
 
     @staticmethod
     def __setup(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[PositionMarker, bool, bool]:
-
         POGGER.debug(">>")
         POGGER.debug(">>")
         if ContainerBlockProcessor.__look_for_pragmas(
             position_marker,
             grab_bag,
         ):
             return position_marker, True, False
@@ -90,14 +90,15 @@
         position_marker: PositionMarker,
         ignore_link_definition_start: bool,
         parser_properties: ParseBlockPassProperties,
         container_start_bq_count: int,
         container_depth: int = 0,
         adjusted_block_index: Optional[int] = None,
         initial_block_quote_count: Optional[int] = None,
+        original_line: Optional[str] = None,
     ) -> Tuple[
         List[MarkdownToken],
         Optional[str],
         Optional[int],
         Optional[RequeueLineInfo],
         bool,
         bool,
@@ -115,15 +116,17 @@
             parser_state,
             container_depth,
             initial_block_quote_count,
             adjusted_block_index,
             container_start_bq_count,
             parser_properties,
             ignore_link_definition_start,
-            position_marker.text_to_parse,
+            original_line
+            if original_line is not None
+            else position_marker.text_to_parse,
         )
         (
             position_marker,
             did_find_pragma,
             is_not_in_root_list,
         ) = ContainerBlockProcessor.__setup(
             parser_state,
@@ -203,16 +206,16 @@
             ]
             POGGER.debug("last_container_stack_token>>$", last_container_stack_token)
             if last_container_stack_token.is_block_quote:
                 block_token = cast(
                     BlockQuoteMarkdownToken,
                     last_container_stack_token.matching_markdown_token,
                 )
-                assert block_token.leading_spaces is not None
-                split_spaces = block_token.leading_spaces.split(
+                assert block_token.bleading_spaces is not None
+                split_spaces = block_token.bleading_spaces.split(
                     ParserHelper.newline_character
                 )
                 # POGGER.debug("split_spaces>>$", split_spaces)
                 last_leading_space = split_spaces[-1]
                 # POGGER.debug(
                 #     "last_leading_space>:$:($)",
                 #     last_leading_space,
@@ -326,15 +329,14 @@
 
     @staticmethod
     def __special_list_block_block(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> None:
-
         if not (
             parser_state.token_stack[1].is_list
             and parser_state.token_stack[2].is_block_quote
             and parser_state.token_stack[3].is_block_quote
             and parser_state.token_stack[4].is_paragraph
             and parser_state.token_stack[1].matching_markdown_token
             and parser_state.token_stack[3].matching_markdown_token
@@ -375,15 +377,14 @@
 
     @staticmethod
     def __determine_leading_whitespace_preprocessing(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> None:
-
         assert grab_bag.extracted_whitespace is not None
         grab_bag.indent_used_by_container = 0
         if grab_bag.is_para_continue and not grab_bag.container_depth:
             ContainerBlockProcessor.__special_list_block_block(
                 parser_state, position_marker, grab_bag
             )
         elif not grab_bag.is_para_continue:
@@ -453,15 +454,14 @@
             )
 
     @staticmethod
     def __handle_trailing_indent_with_block_quote(
         parser_state: ParserState,
         grab_bag: ContainerGrabBag,
     ) -> None:
-
         grab_bag.did_indent_processing = True
         assert grab_bag.extracted_whitespace is not None
         for stack_capture_index in range(1, len(parser_state.token_stack)):
             POGGER.debug(
                 "$>stack:$:",
                 stack_capture_index,
                 parser_state.token_stack[stack_capture_index],
@@ -473,16 +473,16 @@
             POGGER.debug(
                 "$>token:$:",
                 stack_capture_index,
                 inner_token,
             )
             if inner_token.is_block_quote_start:
                 block_quote_token = cast(BlockQuoteMarkdownToken, inner_token)
-                assert block_quote_token.leading_spaces is not None
-                split_spaces = block_quote_token.leading_spaces.split("\n")
+                assert block_quote_token.bleading_spaces is not None
+                split_spaces = block_quote_token.bleading_spaces.split("\n")
                 grab_bag.indent_already_processed = len(split_spaces[-1])
             else:
                 assert inner_token.is_list_start
                 list_token = cast(ListStartMarkdownToken, inner_token)
                 grab_bag.indent_already_processed = list_token.indent_level
         delta = len(grab_bag.extracted_whitespace) - grab_bag.indent_already_processed
         POGGER.debug("len(ws)=$", len(grab_bag.extracted_whitespace))
@@ -694,31 +694,28 @@
         if grab_bag.can_continue:
             did_process = ContainerBlockProcessor.__handle_block_continuations(
                 parser_state,
                 position_marker,
                 did_process,
                 grab_bag,
             )
-        return
 
     @staticmethod
     def __prepare_container_start_variables(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> PositionMarker:
         # POGGER.debug("Stack Depth:$:", parser_state.original_stack_depth)
         # POGGER.debug("Document Depth:$:", parser_state.original_document_depth)
         if grab_bag.container_depth:
             return position_marker
 
         if ParserHelper.tab_character in position_marker.text_to_parse:
-            detabified_line = ParserHelper.detabify_string(
-                position_marker.text_to_parse
-            )
+            detabified_line = TabHelper.detabify_string(position_marker.text_to_parse)
             POGGER.debug("Before tab replacement:$:", position_marker.text_to_parse)
             POGGER.debug("After tab replacement :$:", detabified_line)
             position_marker = PositionMarker(
                 position_marker.line_number,
                 position_marker.index_number,
                 detabified_line,
                 position_marker.index_indent,
@@ -801,15 +798,14 @@
 
     @staticmethod
     def __check_for_container_starts(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[bool, bool]:
-
         parser_state.nested_list_start = None
         ulist_index = -1
         olist_index = -1
         (
             did_process,
             block_index,
             avoid_block_starts,
@@ -858,15 +854,14 @@
     def __handle_nested_blocks(
         parser_state: ParserState,
         position_marker: PositionMarker,
         was_container_start: bool,
         avoid_block_starts: bool,
         grab_bag: ContainerGrabBag,
     ) -> bool:
-
         # POGGER.debug("was_container_start>>$", was_container_start)
 
         grab_bag.last_list_start_index = 0
         if grab_bag.end_container_indices.block_index != -1:
             assert grab_bag.last_block_quote_index in (
                 grab_bag.end_container_indices.block_index - 1,
                 grab_bag.end_container_indices.block_index,
@@ -1105,15 +1100,14 @@
             grab_bag,
         )
 
     @staticmethod
     def __look_back_in_document_for_block_quote(
         parser_state: ParserState, token_index: int
     ) -> Optional[BlockQuoteMarkdownToken]:
-
         # TODO Look back on stack instead?
         other_block_quote_token, other_token_index = None, token_index
         while other_token_index >= 0:
             if parser_state.token_document[other_token_index].is_block_quote_start:
                 block_quote_token = cast(
                     BlockQuoteMarkdownToken,
                     parser_state.token_document[other_token_index],
@@ -1156,15 +1150,15 @@
 
         if other_block_quote_token:
             POGGER.debug("PLFCB>>other_block_quote_token>>:$:", other_block_quote_token)
             POGGER.debug(
                 "PLFCB>>other_block_quote_token.leading_text_index>>:$:",
                 other_block_quote_token.leading_text_index,
             )
-            leading_spaces = other_block_quote_token.calculate_next_leading_space_part(
+            leading_spaces = other_block_quote_token.calculate_next_bleading_space_part(
                 increment_index=False, delta=-1
             )
             POGGER.debug("PLFCB>>leading_spaces>>:$:", leading_spaces)
             POGGER.debug("PLFCB>>other_block_quote_token>>:$:", other_block_quote_token)
             POGGER.debug(
                 "PLFCB>>other_block_quote_token.leading_text_index>>:$:",
                 other_block_quote_token.leading_text_index,
@@ -1210,35 +1204,33 @@
     @staticmethod
     def __calculate_adjusted_whitespace_kludge(
         parser_state: ParserState,
         token_index: int,
         found_block_quote_token: Optional[BlockQuoteMarkdownToken],
         grab_bag: ContainerGrabBag,
     ) -> None:
-
         assert grab_bag.extracted_whitespace is not None
         previous_ws_len = 0
         force_reline, ws_len = (
             False,
-            ParserHelper.calculate_length(grab_bag.extracted_whitespace)
-            + previous_ws_len,
+            TabHelper.calculate_length(grab_bag.extracted_whitespace) + previous_ws_len,
         )
         if (
             found_block_quote_token
             and ContainerBlockProcessor.__does_block_quote_token_have_end(
                 parser_state, found_block_quote_token
             )
         ):
             found_block_quote_token = None
         if found_block_quote_token:
             POGGER.debug(
                 "PLFCB>>found_block_quote_token>>:$:",
                 ParserHelper.make_value_visible(found_block_quote_token),
             )
-            leading_spaces = found_block_quote_token.calculate_next_leading_space_part(
+            leading_spaces = found_block_quote_token.calculate_next_bleading_space_part(
                 increment_index=False, delta=-1, allow_overflow=True
             )
             POGGER.debug("PLFCB>>leading_spaces>>:$:", leading_spaces)
             old_start_index = len(leading_spaces)
         else:
             (
                 force_reline,
@@ -1433,15 +1425,14 @@
 
     @staticmethod
     def __check_for_nested_list_start(
         parser_state: ParserState,
         nested_container_starts: ContainerIndices,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[int, bool, int]:
-
         active_container_index = max(
             grab_bag.end_container_indices.ulist_index,
             grab_bag.end_container_indices.olist_index,
             grab_bag.end_container_indices.block_index,
         )
         POGGER.debug(
             "check next container_start>max>>$>>bq>>$",
@@ -1459,15 +1450,14 @@
                 "parser_state.nested_list_start>>$<<",
                 parser_state.nested_list_start,
             )
             POGGER.debug(
                 "parser_state.token_document>>$<<", parser_state.token_document
             )
             if parser_state.nested_list_start and grab_bag.adj_line_to_parse.strip():
-
                 (
                     grab_bag.start_index,
                     indent_level,
                     indent_was_adjusted,
                     indent_level_delta,
                 ) = ContainerBlockProcessor.__calculate_initial_list_adjustments(
                     parser_state,
@@ -1489,15 +1479,14 @@
 
     @staticmethod
     def __calculate_initial_list_adjustments(
         parser_state: ParserState,
         adj_line_to_parse: str,
         end_container_indices: ContainerIndices,
     ) -> Tuple[int, int, bool, int]:
-
         start_index, _ = ParserHelper.extract_spaces(adj_line_to_parse, 0)
         assert start_index is not None
         POGGER.debug("start_index>>$<<", start_index)
 
         assert parser_state.nested_list_start is not None
         assert parser_state.nested_list_start.matching_markdown_token is not None
         POGGER.debug(
@@ -1579,15 +1568,14 @@
         elif (
             not nested_container_starts.block_index
             and grab_bag.adj_line_to_parse
             and grab_bag.adj_line_to_parse[0] == ParserHelper.space_character
             and indent_was_adjusted
             and parser_state.nested_list_start
         ):
-
             assert parser_state.nested_list_start is not None
         return False
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __do_nested_cleanup(
         parser_state: ParserState,
@@ -1618,15 +1606,14 @@
     def __check_for_next_container(
         parser_state: ParserState,
         position_marker: PositionMarker,
         nested_container_starts: ContainerIndices,
         adjusted_text_to_parse: str,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[str, Optional[str], bool, bool]:
-
         POGGER.debug("check next container_start>stack>>$", parser_state.token_stack)
         POGGER.debug(
             "check next container_start>tokenized_document>>$",
             parser_state.token_document,
         )
 
         if (
@@ -1750,30 +1737,30 @@
             ):
                 block_quote_token = cast(
                     BlockQuoteMarkdownToken,
                     parser_state.token_stack[
                         last_container_index
                     ].matching_markdown_token,
                 )
-                assert block_quote_token.leading_spaces is not None
-                split_spaces = block_quote_token.leading_spaces.split(
+                assert block_quote_token.bleading_spaces is not None
+                split_spaces = block_quote_token.bleading_spaces.split(
                     ParserHelper.newline_character
                 )
                 nested_removed_text = str(split_spaces[-1])
         POGGER.debug("__calculate_nested_removed_text<<:$:", nested_removed_text)
         return nested_removed_text
 
     @staticmethod
     def __calculate_nested_removed_text_block_quote(
         parser_state: ParserState,
         block_quote_token: BlockQuoteMarkdownToken,
         grab_bag: ContainerGrabBag,
     ) -> str:
-        assert block_quote_token.leading_spaces is not None
-        split_spaces = block_quote_token.leading_spaces.split(
+        assert block_quote_token.bleading_spaces is not None
+        split_spaces = block_quote_token.bleading_spaces.split(
             ParserHelper.newline_character
         )
         nested_removed_text = str(split_spaces[-1])
         POGGER.debug("nested_removed_text:$:", nested_removed_text)
         if (
             len(parser_state.token_document) > 1
             and parser_state.token_document[-2].is_new_list_item
@@ -1847,14 +1834,15 @@
             position_marker,
             False,
             grab_bag.parser_properties,
             grab_bag.block_quote_data.current_count,
             container_depth=new_container_depth,
             adjusted_block_index=adj_block,
             initial_block_quote_count=grab_bag.block_quote_data.current_count,
+            original_line=grab_bag.original_line,
         )
         assert (
             not grab_bag.requeue_line_info
             or not grab_bag.requeue_line_info.lines_to_requeue
         )
         assert adjusted_text_to_parse is not None
 
@@ -1898,15 +1886,14 @@
         )
 
     @staticmethod
     def __process_list_in_progress(
         parser_state: ParserState,
         grab_bag: ContainerGrabBag,
     ) -> bool:
-
         did_process, ind = LeafBlockProcessorParagraph.check_for_list_in_process(
             parser_state
         )
         if did_process:
             assert not grab_bag.container_tokens
             POGGER.debug("clt>>list-in-progress")
             resultant_tokens = ListBlockProcessor.list_in_process(
@@ -1920,15 +1907,14 @@
 
     @staticmethod
     def __process_lazy_lines(
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> None:
-
         assert grab_bag.is_leaf_tokens_empty()
         POGGER.debug("clt>>lazy-check")
 
         after_ws_index, ex_whitespace = ParserHelper.extract_spaces(
             grab_bag.line_to_parse, 0
         )
         remaining_line = grab_bag.line_to_parse[after_ws_index:]
@@ -1950,15 +1936,14 @@
         grab_bag.extend_container_tokens(lazy_tokens)
 
     @staticmethod
     def __look_for_pragmas(
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> bool:
-
         _, pragma_whitespace = ParserHelper.extract_spaces(
             position_marker.text_to_parse, 0
         )
         return (
             PragmaExtension.look_for_pragmas(
                 position_marker,
                 position_marker.text_to_parse,
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/container_grab_bag.py` & `pymarkdownlnt-0.9.9/pymarkdown/container_grab_bag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Class to provide a "grab bag" for commonly used properties for the Container Block Processor.
 """
-# pylint: disable=too-many-statements
 # pylint: disable=too-many-instance-attributes
 import logging
 from typing import Any, List, Optional
 
 from pymarkdown.block_quote_data import BlockQuoteData
 from pymarkdown.container_indices import ContainerIndices
 from pymarkdown.markdown_token import MarkdownToken
@@ -33,148 +32,158 @@
         initial_block_quote_count: Optional[int],
         adjusted_block_index: Optional[int],
         container_start_bq_count: int,
         parser_properties: ParseBlockPassProperties,
         ignore_link_definition_start: bool,
         original_line: str,
     ) -> None:
-
         # Booleans
         self.__did_blank: bool = False
-        self.__log_read_write_value("did_blank", self.__did_blank)
         self.__was_paragraph_continuation: bool = False
+        self.__do_skip_containers_before_leaf_blocks: bool = False
+        self.__was_indent_already_processed: bool = False
+        self.__do_force_leaf_token_parse: bool = False
+        self.__did_indent_processing: bool = False
+        self.__have_pre_processed_indent: bool = False
+        self.__can_continue: bool = False
+        self.__do_force_list_continuation = False
+
+        # Integers
+        self.__indent_used_by_container: int = -1
+        self.__indent_already_processed: int = -1
+        self.__last_block_quote_index: int = -1
+        self.__last_list_start_index: int = -1
+        self.__start_index: int = -1
+
+        # Optional integers
+        self.__removed_chars_at_start_of_line: Optional[int] = None
+
+        # Strings
+        self.__adj_line_to_parse: str = ""
+        self.__line_to_parse: str = ""
+
+        # Optional strings
+        self.__weird_adjusted_text: Optional[str] = None
+        self.__indent_used_by_list: Optional[str] = None
+        self.__text_removed_by_container: Optional[str] = None
+        self.__extracted_whitespace: Optional[str] = None
+        self.__adj_ws: Optional[str] = None
+
+        # Others
+        self.__block_quote_data = BlockQuoteData(-1, -1)
+        self.__end_container_indices = ContainerIndices(-1, -1, -1)
+        self.__requeue_line_info: Optional[RequeueLineInfo] = None
+        self.__current_container_blocks: List[StackToken] = []
+        self.__leaf_tokens: List[MarkdownToken] = []
+        self.__container_level_tokens: List[MarkdownToken] = []
+
+        # Read only values
+        self.__container_depth = container_depth
+        self.__initial_block_quote_count = initial_block_quote_count
+        self.__adjusted_block_index = adjusted_block_index
+        self.__container_start_bq_count = container_start_bq_count
+        self.__parser_properties = parser_properties
+        self.__do_ignore_link_definition_start = ignore_link_definition_start
+        self.__original_line = original_line
+        self.__is_para_continue = (
+            bool(
+                parser_state
+                and parser_state.token_stack
+                and len(parser_state.token_stack) >= 2
+                and parser_state.token_stack[-1].is_paragraph
+            )
+            and not parser_state.token_document[-1].is_blank_line
+        )
+        self.__log_initial_values()
+
+    def __log_initial_values(self) -> None:
+        # Booleans
+        self.__log_read_write_value("did_blank", self.__did_blank)
         self.__log_read_write_value(
             "was_paragraph_continuation", self.__was_paragraph_continuation
         )
-        self.__do_skip_containers_before_leaf_blocks: bool = False
         self.__log_read_write_value(
             "do_skip_containers_before_leaf_blocks",
             self.__do_skip_containers_before_leaf_blocks,
         )
-        self.__was_indent_already_processed: bool = False
         self.__log_read_write_value(
             "was_indent_already_processed", self.__was_indent_already_processed
         )
-        self.__do_force_leaf_token_parse: bool = False
         self.__log_read_write_value(
             "do_force_leaf_token_parse", self.__do_force_leaf_token_parse
         )
-        self.__did_indent_processing: bool = False
         self.__log_read_write_value(
             "did_indent_processing", self.__did_indent_processing
         )
-        self.__have_pre_processed_indent: bool = False
         self.__log_read_write_value(
             "have_pre_processed_indent", self.__have_pre_processed_indent
         )
-        self.__can_continue: bool = False
         self.__log_read_write_value("can_continue", self.__can_continue)
-        self.__do_force_list_continuation = False
         self.__log_read_write_value(
             "do_force_list_continuation", self.__do_force_list_continuation
         )
 
         # Integers
-        self.__indent_used_by_container: int = -1
         self.__log_read_write_value(
             "indent_used_by_container", self.__indent_used_by_container
         )
-        self.__indent_already_processed: int = -1
         self.__log_read_write_value(
             "indent_already_processed", self.__indent_already_processed
         )
-        self.__last_block_quote_index: int = -1
         self.__log_read_write_value(
             "last_block_quote_index", self.__last_block_quote_index
         )
-        self.__last_list_start_index: int = -1
         self.__log_read_write_value(
             "last_list_start_index", self.__last_list_start_index
         )
-        self.__start_index: int = -1
         self.__log_read_write_value("start_index", self.__start_index)
 
         # Optional integers
-        self.__removed_chars_at_start_of_line: Optional[int] = None
         self.__log_read_write_value(
             "removed_chars_at_start_of_line", self.__removed_chars_at_start_of_line
         )
 
         # Strings
-        self.__adj_line_to_parse: str = ""
         self.__log_read_write_value("adj_line_to_parse", self.__adj_line_to_parse)
-        self.__line_to_parse: str = ""
         self.__log_read_write_value("line_to_parse", self.__line_to_parse)
 
         # Optional strings
-        self.__weird_adjusted_text: Optional[str] = None
         self.__log_read_write_value("weird_adjusted_text", self.__weird_adjusted_text)
-        self.__indent_used_by_list: Optional[str] = None
         self.__log_read_write_value("indent_used_by_list", self.__indent_used_by_list)
-        self.__text_removed_by_container: Optional[str] = None
         self.__log_read_write_value(
             "text_removed_by_container", self.__text_removed_by_container
         )
-        self.__extracted_whitespace: Optional[str] = None
         self.__log_read_write_value("extracted_whitespace", self.__extracted_whitespace)
-        self.__adj_ws: Optional[str] = None
         self.__log_read_write_value("adj_ws", self.__adj_ws)
 
         # Others
-        self.__block_quote_data = BlockQuoteData(-1, -1)
         self.__log_read_write_value("block_quote_data", self.__block_quote_data)
-        self.__end_container_indices = ContainerIndices(-1, -1, -1)
         self.__log_read_write_value(
             "end_container_indices", self.__end_container_indices
         )
-
-        self.__requeue_line_info: Optional[RequeueLineInfo] = None
         self.__log_read_write_value("requeue_line_info", self.__requeue_line_info)
-
-        self.__current_container_blocks: List[StackToken] = []
-
-        self.__leaf_tokens: List[MarkdownToken] = []
         self.__log_read_write_value("leaf_tokens", self.__leaf_tokens)
-
-        self.__container_level_tokens: List[MarkdownToken] = []
         self.__log_read_write_value(
             "container_level_tokens", self.__container_level_tokens
         )
 
         # Read only values
-        self.__container_depth = container_depth
-        self.__initial_block_quote_count = initial_block_quote_count
-        self.__adjusted_block_index = adjusted_block_index
-        self.__container_start_bq_count = container_start_bq_count
-        self.__parser_properties = parser_properties
-        self.__do_ignore_link_definition_start = ignore_link_definition_start
-        self.__original_line = original_line
         self.__log_read_only_value("container_depth", self.__container_depth)
         self.__log_read_only_value(
             "initial_block_quote_count", self.__initial_block_quote_count
         )
         self.__log_read_only_value("adjusted_block_index", self.__adjusted_block_index)
         self.__log_read_only_value(
             "container_start_bq_count", self.__container_start_bq_count
         )
         self.__log_read_only_value("parser_properties", self.__parser_properties)
         self.__log_read_only_value(
             "do_ignore_link_definition_start", self.__do_ignore_link_definition_start
         )
         self.__log_read_only_value("original_line", self.__original_line)
-
-        self.__is_para_continue = (
-            bool(
-                parser_state
-                and parser_state.token_stack
-                and len(parser_state.token_stack) >= 2
-                and parser_state.token_stack[-1].is_paragraph
-            )
-            and not parser_state.token_document[-1].is_blank_line
-        )
         self.__log_read_only_value("is_para_continue", self.__is_para_continue)
 
     @staticmethod
     def __log_read_only_value(value_name: str, value_object: Any) -> None:
         POGGER.debug("CGB(ReadOnly): '$'=:$:", value_name, value_object)
 
     @staticmethod
@@ -698,8 +707,7 @@
         Xxx
         """
         return self.__container_level_tokens
 
 
 # pylint: enable=too-many-public-methods
 # pylint: enable=too-many-instance-attributes
-# pylint: enable=too-many-statements
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/container_indices.py` & `pymarkdownlnt-0.9.9/pymarkdown/container_indices.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/container_markdown_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/container_markdown_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module to provide for a container element that can be added to markdown parsing stream.
 """
 import logging
-from typing import Optional
+from typing import Dict, Optional
 
 from pymarkdown.markdown_token import MarkdownToken, MarkdownTokenClass
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.position_marker import PositionMarker
 
 POGGER = ParserLogger(logging.getLogger(__name__))
@@ -100,34 +100,42 @@
     def __init__(
         self,
         token_name: str,
         position_marker: PositionMarker,
         list_start_sequence: str,
         list_start_content: str,
         indent_level: int,
+        tabbed_adjust: int,
         extracted_whitespace: str,
+        tabbed_whitespace_to_add: Optional[str],
     ) -> None:
         ContainerMarkdownToken.__init__(
             self,
             token_name,
             "",
             position_marker=position_marker,
         )
+        POGGER.debug("tabbed_adjust>:$:<", tabbed_adjust)
+        POGGER.debug("type(tabbed_adjust)>:$:<", type(tabbed_adjust))
         self.leading_spaces_index = 0
         self.is_loose = True
         (
             self.__list_start_sequence,
             self.__list_start_content,
             self.__indent_level,
             self.__extracted_whitespace,
+            self.__tabbed_whitespace_to_add,
+            self.__tabbed_adjust,
         ) = (
             list_start_sequence,
             list_start_content,
             indent_level,
             extracted_whitespace,
+            tabbed_whitespace_to_add,
+            tabbed_adjust,
         )
         self.__last_new_list_token: Optional[NewListItemMarkdownToken] = None
         self.__leading_spaces: Optional[str] = None
         self.__compose_extra_data_field()
 
     # pylint: enable=too-many-arguments
 
@@ -156,14 +164,28 @@
     def extracted_whitespace(self) -> str:
         """
         Returns any whitespace that was extracted before the processing of this element occurred.
         """
         return self.__extracted_whitespace
 
     @property
+    def tabbed_extracted_whitespace(self) -> Optional[str]:
+        """
+        extracted_whitespace, but with any tabs.
+        """
+        return self.__tabbed_whitespace_to_add
+
+    @property
+    def tabbed_adjust(self) -> int:
+        """
+        Adjustments for tabbed.
+        """
+        return self.__tabbed_adjust
+
+    @property
     def leading_spaces(self) -> Optional[str]:
         """
         Returns the leading spaces that occur before the list element.
         """
         return self.__leading_spaces
 
     def adjust_for_new_list_item(
@@ -188,18 +210,47 @@
 
         item_list = [
             self.__list_start_sequence,
             self.__list_start_content,
             str(self.__indent_level),
             self.__extracted_whitespace,
         ]
-        if self.__leading_spaces is not None:
-            item_list.append(self.__leading_spaces)
+        is_leading_spaces_valid = self.__leading_spaces is not None
+        is_tabbed_whitespace_valid = self.__tabbed_whitespace_to_add is not None
+        is_tabbed_adjust_valid = (
+            isinstance(self.__tabbed_adjust, int) and self.__tabbed_adjust >= 0
+        )
+
+        if (
+            is_leading_spaces_valid
+            or is_tabbed_whitespace_valid
+            or is_tabbed_adjust_valid
+        ):
+            item_list.append(self.__leading_spaces or "")
+        if is_tabbed_whitespace_valid or is_tabbed_adjust_valid:
+            item_list.append(self.__tabbed_whitespace_to_add or "")
+        if is_tabbed_adjust_valid:
+            item_list.append(str(self.__tabbed_adjust))
         self._set_extra_data(MarkdownToken.extra_data_separator.join(item_list))
 
+    def remove_last_leading_space(self) -> Optional[str]:
+        """
+        Remove the last leading space and return it.
+        """
+        assert self.__leading_spaces is not None
+        last_separator_index = self.__leading_spaces.rfind("\n")
+        assert last_separator_index == -1
+        extracted_text = self.__leading_spaces
+        self.__leading_spaces = None
+        # else:
+        #     extracted_text = self.__leading_spaces[last_separator_index:]
+        #     self.__leading_spaces = self.__leading_spaces[:last_separator_index]
+        self.__compose_extra_data_field()
+        return extracted_text
+
     def add_leading_spaces(self, ws_add: str) -> None:
         """
         Add any leading spaces to the token, separating them with line feeds.
         """
         POGGER.debug("__leading_spaces>>:$:<<", self.__leading_spaces)
         POGGER.debug("add_leading_spaces>>:$:<<", ws_add)
         self.__leading_spaces = (
@@ -235,66 +286,78 @@
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         list_start_sequence: str,
         list_start_content: str,
         indent_level: int,
+        tabbed_adjust: int,
         extracted_whitespace: str,
+        tabbed_whitespace_to_add: Optional[str],
         position_marker: PositionMarker,
     ) -> None:
         ListStartMarkdownToken.__init__(
             self,
             MarkdownToken._token_ordered_list_start,
             position_marker,
             list_start_sequence,
             list_start_content,
             indent_level,
+            tabbed_adjust,
             extracted_whitespace,
+            tabbed_whitespace_to_add,
         )
 
     # pylint: enable=too-many-arguments
 
 
 class UnorderedListStartMarkdownToken(ListStartMarkdownToken):
     """
     Class to provide for an encapsulation of the unordered list start element.
     """
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         list_start_sequence: str,
         indent_level: int,
+        tabbed_adjust: int,
         extracted_whitespace: str,
+        tabbed_whitespace_to_add: Optional[str],
         position_marker: PositionMarker,
     ) -> None:
         ListStartMarkdownToken.__init__(
             self,
             MarkdownToken._token_unordered_list_start,
             position_marker,
             list_start_sequence,
             "",
             indent_level,
+            tabbed_adjust,
             extracted_whitespace,
+            tabbed_whitespace_to_add,
         )
 
+    # pylint: enable=too-many-arguments
+
 
 class BlockQuoteMarkdownToken(ContainerMarkdownToken):
     """
     Class to provide for an encapsulation of the block quote element.
     """
 
     def __init__(
         self, extracted_whitespace: str, position_marker: PositionMarker
     ) -> None:
         self.__extracted_whitespace, self.__leading_spaces, self.leading_text_index = (
             extracted_whitespace,
             "",
             0,
         )
+        self.__tabbed_leading_spaces: Dict[int, str] = {}
         ContainerMarkdownToken.__init__(
             self,
             MarkdownToken._token_block_quote,
             "",
             position_marker=position_marker,
         )
         self.__compose_extra_data_field()
@@ -303,74 +366,117 @@
     def extracted_whitespace(self) -> str:
         """
         Returns any whitespace that was extracted before the processing of this element occurred.
         """
         return self.__extracted_whitespace
 
     @property
-    def leading_spaces(self) -> Optional[str]:
+    def bleading_spaces(self) -> Optional[str]:
         """
         Returns any leading spaces that preface the block quote.
         """
         return self.__leading_spaces
 
-    def add_leading_spaces(
-        self, leading_spaces_to_add: str, skip_adding_newline: bool = False
+    @property
+    def tabbed_bleading_spaces(self) -> Dict[int, str]:
+        """
+        Returns the tabbed information for any leading spaces
+        """
+        return self.__tabbed_leading_spaces
+
+    def add_bleading_spaces(
+        self,
+        leading_spaces_to_add: str,
+        skip_adding_newline: bool = False,
+        tabbed_leading_spaces: Optional[str] = None,
     ) -> None:
         """
         Add any leading spaces to the token, separating them with line feeds.
         """
         POGGER.debug(
             "__leading_spaces>>:$:<<",
             self.__leading_spaces,
         )
         POGGER.debug("add_leading_spaces>>:$:<<", leading_spaces_to_add)
-        self.__leading_spaces = (
-            f"{self.__leading_spaces}{leading_spaces_to_add}"
-            if skip_adding_newline
-            else (
+        if skip_adding_newline:
+            self.__leading_spaces = f"{self.__leading_spaces}{leading_spaces_to_add}"
+        else:
+            self.__leading_spaces = (
                 f"{self.__leading_spaces}{ParserHelper.newline_character}{leading_spaces_to_add}"
                 if self.__leading_spaces
                 else leading_spaces_to_add
             )
-        )
         POGGER.debug(
             "__leading_spaces>>:$:<<",
             self.__leading_spaces,
         )
+        if not skip_adding_newline and tabbed_leading_spaces:
+            POGGER.debug(
+                "__tabbed_leading_spaces>>:$:<<",
+                self.__tabbed_leading_spaces,
+            )
+            newline_count = ParserHelper.count_newlines_in_text(self.__leading_spaces)
+            self.__tabbed_leading_spaces[newline_count] = tabbed_leading_spaces
+            POGGER.debug(
+                "__tabbed_leading_spaces>>:$:<<",
+                self.__tabbed_leading_spaces,
+            )
         self.__compose_extra_data_field()
 
-    def remove_last_leading_space(self) -> str:
+    def remove_last_bleading_space(self) -> str:
         """
         Remove the last leading space and return it.
         """
-        last_separator_index = self.__leading_spaces.rindex("\n")
-        extracted_text = self.__leading_spaces[last_separator_index:]
-        self.__leading_spaces = self.__leading_spaces[:last_separator_index]
+        last_separator_index = self.__leading_spaces.rfind("\n")
+        if last_separator_index == -1:
+            extracted_text = self.__leading_spaces
+            self.__leading_spaces = ""
+        else:
+            extracted_text = self.__leading_spaces[last_separator_index:]
+            self.__leading_spaces = self.__leading_spaces[:last_separator_index]
         self.leading_text_index -= 1
         self.__compose_extra_data_field()
         return extracted_text
 
     def __compose_extra_data_field(self) -> None:
         """
         Compose the object's self.extra_data field from the local object's variables.
         """
         item_list = [self.__extracted_whitespace, self.__leading_spaces]
+        if self.__tabbed_leading_spaces:
+            item_list.append(
+                ParserHelper.make_value_visible(self.__tabbed_leading_spaces).replace(
+                    "'", '"'
+                )
+            )
         self._set_extra_data(MarkdownToken.extra_data_separator.join(item_list))
 
-    def calculate_next_leading_space_part(
+    def calculate_next_bleading_space_part(
         self, increment_index: bool = True, delta: int = 0, allow_overflow: bool = False
     ) -> str:
         """
         Calculate the next leading space based on the leading_text_index,
         optonally incrementing it as well.
         """
-        assert self.leading_spaces is not None
-        split_leading_spaces = self.leading_spaces.split(ParserHelper.newline_character)
+        assert self.bleading_spaces is not None
+
+        # print(f"increment_index>>:{increment_index}:<<")
+        tabbed_leading = None
+        if increment_index and self.__tabbed_leading_spaces:
+            tabbed_leading = self.__tabbed_leading_spaces[self.leading_text_index]
+            # print(f"dg>>:{ParserHelper.make_value_visible(dg)}:<<")
+
+        split_leading_spaces = self.bleading_spaces.split(
+            ParserHelper.newline_character
+        )
         absolute_index = self.leading_text_index + delta
         if allow_overflow and absolute_index >= len(split_leading_spaces):
             leading_text = ""
         else:
             leading_text = split_leading_spaces[self.leading_text_index + delta]
             if increment_index:
                 self.leading_text_index += 1
+
+        if tabbed_leading is not None:
+            leading_text = tabbed_leading
+
         return leading_text
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/emphasis_helper.py` & `pymarkdownlnt-0.9.9/pymarkdown/emphasis_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     @staticmethod
     def __find_potential_opener(
         delimiter_stack: List[SpecialTextMarkdownToken],
         current_position: int,
         stack_bottom: int,
         openers_bottom: int,
     ) -> Tuple[SpecialTextMarkdownToken, Optional[SpecialTextMarkdownToken]]:
-
         # POGGER.debug("delimiter_stack-->$",delimiter_stack)
         scan_index = current_position - 1
         found_opener: Optional[SpecialTextMarkdownToken] = None
         close_token = delimiter_stack[current_position]
         # POGGER.debug("potential closer-->$", current_position)
         while (
             scan_index >= 0
@@ -89,15 +88,14 @@
 
     @staticmethod
     def __process_this_delimiter_item(
         is_debug_enabled: bool,
         delimiter_stack: List[SpecialTextMarkdownToken],
         current_position: int,
     ) -> bool:
-
         special_token = delimiter_stack[current_position]
 
         if is_debug_enabled:
             POGGER.debug(
                 "Block($)-->$",
                 current_position,
                 special_token.show_process_emphasis(),
@@ -126,15 +124,14 @@
         )
 
         current_position, stack_size = (
             stack_bottom + 1,
             len(delimiter_stack),
         )
         if current_position < stack_size:
-
             openers_bottom = stack_bottom
             if is_debug_enabled:
                 POGGER.debug("BLOCK($) of ($)", current_position, stack_size)
                 POGGER.debug(
                     "BLOCK($)-->$",
                     current_position,
                     delimiter_stack[current_position].show_process_emphasis(),
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extension_manager/extension_impl.py` & `pymarkdownlnt-0.9.9/pymarkdown/extension_manager/extension_impl.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extension_manager/extension_manager.py` & `pymarkdownlnt-0.9.9/pymarkdown/extension_manager/extension_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pymarkdown.extensions.extended_autolinks import MarkdownExtendedAutolinksExtension
 from pymarkdown.extensions.extension_one import DebugExtension
 from pymarkdown.extensions.front_matter_extension import FrontMatterExtension
 from pymarkdown.extensions.markdown_strikethrough import MarkdownStrikeThroughExtension
 from pymarkdown.extensions.markdown_tables import MarkdownTablesExtension
 from pymarkdown.extensions.pragma_token import PragmaExtension
 from pymarkdown.extensions.task_list_items import MarkdownTaskListItemsExtension
+from pymarkdown.main_presentation import MainPresentation
 from pymarkdown.parser_helper import ParserHelper
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ExtensionManager:
     """
@@ -36,15 +37,20 @@
     __extensions_prefix = "extensions"
     __argparse_subparser: Optional[argparse.ArgumentParser] = None
     __root_subparser_name = "em_subcommand"
     __id_regex = re.compile("^[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9]$")
 
     __DEBUG_EXTENSION = DebugExtension()
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        presentation: MainPresentation,
+    ) -> None:
+        self.__presentation = presentation
+
         self.__extension_objects: Dict[str, ParserExtension] = {}
         self.__extension_details: Dict[str, ExtensionDetails] = {}
         self.__enabled_extensions: List[str] = []
         self.__properties: Optional[ApplicationProperties] = None
         self.__is_front_matter_enabled: bool = False
         self.__is_linter_pragmas_enabled: bool = False
 
@@ -136,24 +142,24 @@
         """
         Handle the parsing for this subparser.
         """
         return_code, subparser_value = 0, getattr(
             args, ExtensionManager.__root_subparser_name
         )
         if subparser_value == "list":
-            self.__handle_argparse_subparser_list(args)
+            return_code = self.__handle_argparse_subparser_list(args)
         elif subparser_value == "info":
             return_code = self.__handle_argparse_subparser_info(args)
         else:
             assert ExtensionManager.__argparse_subparser
             ExtensionManager.__argparse_subparser.print_help()
             sys.exit(2)
         return return_code
 
-    def __handle_argparse_subparser_list(self, args: argparse.Namespace) -> None:
+    def __handle_argparse_subparser_list(self, args: argparse.Namespace) -> int:
         list_re = None
         if args.list_filter:
             list_re = re.compile(
                 "^" + args.list_filter.replace("*", ".*").replace("?", ".") + "$"
             )
 
         names, show_rows = list(self.__extension_details.keys()), []
@@ -187,41 +193,49 @@
             headers = [
                 "id",
                 "name",
                 "enabled\n(default)",
                 "enabled\n(current)",
                 "version",
             ]
-            ExtensionManager.__print_column_output(headers, show_rows)
-        else:
-            print(f"No extension identifier matches the pattern '{args.list_filter}'.")
+            self.__print_column_output(headers, show_rows)
+            return 0
+        self.__presentation.print_system_error(
+            f"No extension identifier matches the pattern '{args.list_filter}'."
+        )
+        return 1
 
     def __handle_argparse_subparser_info(self, args: argparse.Namespace) -> int:
         if args.info_filter not in self.__extension_details:
-            print(f"Unable to find an extension with an id of '{args.info_filter}'.")
+            self.__presentation.print_system_error(
+                f"Unable to find an extension with an id of '{args.info_filter}'."
+            )
             return 1
 
         found_extension = self.__extension_details[args.info_filter]
         show_rows: List[List[str]] = [
             ["Id", found_extension.extension_id],
             ["Name", found_extension.extension_name],
             ["Short Description", found_extension.extension_description],
             ["Description Url", str(found_extension.extension_url)],
         ]
 
         headers = ["Item", "Description"]
-        ExtensionManager.__print_column_output(headers, show_rows)
+        self.__print_column_output(headers, show_rows)
         return 0
 
-    @staticmethod
-    def __print_column_output(headers: List[str], show_rows: List[List[str]]) -> None:
+    def __print_column_output(
+        self, headers: List[str], show_rows: List[List[str]]
+    ) -> None:
         table = columnar(show_rows, headers, no_borders=True)
         split_rows = table.split(ParserHelper.newline_character)
         new_rows = [next_row.rstrip() for next_row in split_rows]
-        print(ParserHelper.newline_character.join(new_rows))
+        self.__presentation.print_system_output(
+            ParserHelper.newline_character.join(new_rows)
+        )
 
     @staticmethod
     def __list_filter_type(argument: str) -> str:
         test_argument = argument.replace("*", "").replace("?", "")
         if ExtensionManager.__id_regex.match(test_argument):
             return argument
         raise argparse.ArgumentTypeError(
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extension_manager/parser_extension.py` & `pymarkdownlnt-0.9.9/pymarkdown/extension_manager/parser_extension.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/disallowed_raw_html.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/disallowed_raw_html.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/extended_autolinks.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/extended_autolinks.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/extension_one.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/markdown_strikethrough.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 """
-Module to provide for a debug extension.
+Module to provide for recognizing a strikethrough sequence.
 """
 
 from application_properties import ApplicationPropertiesFacade
 
 from pymarkdown.extension_manager.extension_impl import ExtensionDetails
 from pymarkdown.extension_manager.extension_manager_constants import (
     ExtensionManagerConstants,
 )
 from pymarkdown.extension_manager.parser_extension import ParserExtension
 
 
-class DebugExtension(ParserExtension):
+class MarkdownStrikeThroughExtension(ParserExtension):
     """
-    Extension to provide for a debug extension.
+    Extension to implement the strikethrough extension.
     """
 
     def get_identifier(self) -> str:
         """
         Get the identifier associated with this extension.
         """
-        return "debug-extension"
+        return "markdown-strikethrough"
 
     def get_details(self) -> ExtensionDetails:
         """
         Get the details for the extension.
         """
         return ExtensionDetails(
             extension_id=self.get_identifier(),
-            extension_name="Debug Extension",
-            extension_description="Allows testing through debug.",
+            extension_name="Markdown Strikethrough",
+            extension_description="Allows parsing of Markdown strikethrough.",
             extension_enabled_by_default=False,
             extension_version=ExtensionManagerConstants.EXTENSION_VERSION_NOT_IMPLEMENTED,
             extension_interface_version=ExtensionManagerConstants.EXTENSION_INTERFACE_VERSION_BASIC,
-            extension_url=None,
+            extension_url="https://github.github.com/gfm/#strikethrough-extension-",
             extension_configuration=None,
         )
 
     def apply_configuration(
         self, extension_specific_facade: ApplicationPropertiesFacade
     ) -> None:
         """
         Apply any configuration required by the extension.
         """
-        debug_mode = extension_specific_facade.get_integer_property(
-            "debug_mode", default_value=0
-        )
-        if debug_mode == 1:
-            raise Exception("blah")
-        if debug_mode == 2:
-            raise ValueError("blah")
+        _ = extension_specific_facade  # pragma: no cover
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/front_matter_extension.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/front_matter_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
 
     @staticmethod
     def __handle_document_front_matter(
         token_to_use: str, source_provider: SourceProvider
     ) -> Tuple[
         Optional[str], Optional[FrontMatterMarkdownToken], int, Optional[List[str]]
     ]:
-
         starting_line = token_to_use
         clean_starting_line = starting_line.rstrip()
         repeat_again = True
         have_closing = False
         collected_lines: List[str] = []
         POGGER.info("Metadata prefix detected, scanning for metadata header.")
         next_line = None
@@ -187,15 +186,14 @@
             None,
         )
 
     @staticmethod
     def __is_front_matter_valid(
         collected_lines: List[str],
     ) -> Union[Dict[str, str], str]:
-
         ascii_letters_and_digits = f"{string.ascii_letters}{string.digits}_-"
 
         current_title = ""
         current_value = ""
         value_map: Dict[str, str] = {}
 
         for next_line in collected_lines:
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/front_matter_markdown_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/front_matter_markdown_token.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/markdown_strikethrough.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/task_list_items.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 """
-Module to provide for recognizing a strikethrough sequence.
+Module to provide for a list item that can be check off.
 """
-
 from application_properties import ApplicationPropertiesFacade
 
 from pymarkdown.extension_manager.extension_impl import ExtensionDetails
 from pymarkdown.extension_manager.extension_manager_constants import (
     ExtensionManagerConstants,
 )
 from pymarkdown.extension_manager.parser_extension import ParserExtension
 
 
-class MarkdownStrikeThroughExtension(ParserExtension):
+class MarkdownTaskListItemsExtension(ParserExtension):
     """
-    Extension to implement the strikethrough extension.
+    Extension to implement the task list items extension.
     """
 
     def get_identifier(self) -> str:
         """
         Get the identifier associated with this extension.
         """
-        return "markdown-strikethrough"
+        return "markdown-task-list-items"
 
     def get_details(self) -> ExtensionDetails:
         """
         Get the details for the extension.
         """
         return ExtensionDetails(
             extension_id=self.get_identifier(),
-            extension_name="Markdown Strikethrough",
-            extension_description="Allows parsing of Markdown strikethrough.",
+            extension_name="Markdown Task List Items",
+            extension_description="Allows parsing of Markdown task list items.",
             extension_enabled_by_default=False,
             extension_version=ExtensionManagerConstants.EXTENSION_VERSION_NOT_IMPLEMENTED,
             extension_interface_version=ExtensionManagerConstants.EXTENSION_INTERFACE_VERSION_BASIC,
-            extension_url="https://github.github.com/gfm/#strikethrough-extension-",
+            extension_url="https://github.github.com/gfm/#task-list-items-extension-",
             extension_configuration=None,
         )
 
     def apply_configuration(
         self, extension_specific_facade: ApplicationPropertiesFacade
     ) -> None:
         """
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/markdown_tables.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/markdown_tables.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/extensions/pragma_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/extensions/pragma_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 )
                 parser_properties.pragma_lines[index_number] = line_to_parse
                 POGGER.debug("pragma $ extracted - >$<", index_number, line_to_parse)
                 return True
         POGGER.debug("pragma not extracted - >$<", line_to_parse)
         return False
 
-    # pylint: disable=too-many-locals, too-many-arguments
+    # pylint: disable=too-many-arguments
     @staticmethod
     def compile_single_pragma(
         scan_file: str,
         next_line_number: int,
         pragma_lines: Dict[int, str],
         all_ids: Dict[str, FoundPlugin],
         document_pragmas: Dict[int, Set[str]],
@@ -131,52 +131,78 @@
             after_whitespace_index
             + len(PragmaToken.pragma_title) : -len(PragmaToken.pragma_suffix)
         ]
         after_command_index, command = ParserHelper.extract_until_spaces(
             command_data, 0
         )
         assert command is not None
+        assert after_command_index is not None
         command = command.lower()
         if not command:
             log_pragma_failure(
                 scan_file,
                 actual_line_number,
                 "Inline configuration specified without command.",
             )
         elif command == "disable-next-line":
-            ids_to_disable = command_data[after_command_index:].split(",")
-            processed_ids = set()
-            for next_id in ids_to_disable:
-                next_id = next_id.strip().lower()
-                if not next_id:
-                    log_pragma_failure(
-                        scan_file,
-                        actual_line_number,
-                        f"Inline configuration command '{command}' specified a plugin with a blank id.",
-                    )
-                elif next_id in all_ids:
-                    normalized_id = all_ids[next_id].plugin_id
-                    processed_ids.add(normalized_id)
-                else:
-                    log_pragma_failure(
-                        scan_file,
-                        actual_line_number,
-                        f"Inline configuration command '{command}' unable to find a plugin with the id '{next_id}'.",
-                    )
-
-            if processed_ids:
-                document_pragmas[actual_line_number + 1] = processed_ids
+            PragmaExtension.__handle_disable_next_line(
+                command_data,
+                after_command_index,
+                log_pragma_failure,
+                scan_file,
+                actual_line_number,
+                document_pragmas,
+                all_ids,
+                command,
+            )
         else:
             log_pragma_failure(
                 scan_file,
                 actual_line_number,
                 f"Inline configuration command '{command}' not understood.",
             )
 
-    # pylint: enable=too-many-locals, too-many-arguments
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_disable_next_line(
+        command_data: str,
+        after_command_index: int,
+        log_pragma_failure: Callable[[str, int, str], None],
+        scan_file: str,
+        actual_line_number: int,
+        document_pragmas: Dict[int, Set[str]],
+        all_ids: Dict[str, FoundPlugin],
+        command: str,
+    ) -> None:
+        ids_to_disable = command_data[after_command_index:].split(",")
+        processed_ids = set()
+        for next_id in ids_to_disable:
+            next_id = next_id.strip().lower()
+            if not next_id:
+                log_pragma_failure(
+                    scan_file,
+                    actual_line_number,
+                    f"Inline configuration command '{command}' specified a plugin with a blank id.",
+                )
+            elif next_id in all_ids:
+                normalized_id = all_ids[next_id].plugin_id
+                processed_ids.add(normalized_id)
+            else:
+                log_pragma_failure(
+                    scan_file,
+                    actual_line_number,
+                    f"Inline configuration command '{command}' unable to find a plugin with the id '{next_id}'.",
+                )
+
+        if processed_ids:
+            document_pragmas[actual_line_number + 1] = processed_ids
+
+    # pylint: enable=too-many-arguments
 
 
 class PragmaToken(MarkdownToken):
     """
     Token that contains the pragmas for the document.
     """
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/html_helper.py` & `pymarkdownlnt-0.9.9/pymarkdown/html_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Module to provide helper functions for parsing html.
 """
 import logging
 import string
 from typing import List, Optional, Tuple, cast
 
+from pymarkdown.block_quote_data import BlockQuoteData
 from pymarkdown.constants import Constants
+from pymarkdown.container_helper import ContainerHelper
 from pymarkdown.inline_markdown_token import RawHtmlMarkdownToken, TextMarkdownToken
 from pymarkdown.inline_request import InlineRequest
 from pymarkdown.leaf_markdown_token import HtmlBlockMarkdownToken
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.parser_state import ParserState
 from pymarkdown.position_marker import PositionMarker
 from pymarkdown.stack_token import HtmlBlockStackToken, ParagraphStackToken, StackToken
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
+# pylint: disable=too-many-lines
+
 
 class HtmlHelper:
     """
     Class to provide helper functions for parsing html.
     """
 
     html_block_1 = "1"
@@ -205,28 +210,28 @@
         assert non_whitespace_index is not None
         if non_whitespace_index < line_to_parse_size:
             first_character_of_value = line_to_parse[non_whitespace_index]
             extracted_text: Optional[str] = None
             if first_character_of_value == HtmlHelper.__html_attribute_value_double:
                 (
                     non_whitespace_index,
-                    extracted_text,
+                    _,
                 ) = ParserHelper.collect_until_character(
                     line_to_parse,
                     non_whitespace_index + 1,
                     HtmlHelper.__html_attribute_value_double,
                 )
                 assert non_whitespace_index is not None
                 if non_whitespace_index == line_to_parse_size:
                     return -1
                 non_whitespace_index += 1
             elif first_character_of_value == HtmlHelper.__html_attribute_value_single:
                 (
                     non_whitespace_index,
-                    extracted_text,
+                    _,
                 ) = ParserHelper.collect_until_character(
                     line_to_parse,
                     non_whitespace_index + 1,
                     HtmlHelper.__html_attribute_value_single,
                 )
                 assert non_whitespace_index is not None
                 if non_whitespace_index == line_to_parse_size:
@@ -298,15 +303,14 @@
             is_tag_valid
             and extracted_whitespace
             and are_attributes_valid
             and 0 <= non_whitespace_index < line_to_parse_size
             and line_to_parse[non_whitespace_index]
             not in [HtmlHelper.__html_tag_end, HtmlHelper.__html_tag_start]
         ):
-
             non_whitespace_index = HtmlHelper.extract_html_attribute_name(
                 line_to_parse, non_whitespace_index
             )
             assert non_whitespace_index is not None
             are_attributes_valid = non_whitespace_index != -1
             if not are_attributes_valid:
                 break
@@ -379,15 +383,15 @@
         if ParserHelper.is_character_at_index(
             text_to_parse,
             end_name_index,
             HtmlHelper.__html_attribute_name_value_separator,
         ):
             (
                 value_start_index,
-                extracted_whitespace,
+                _,
             ) = ParserHelper.extract_ascii_whitespace(text_to_parse, end_name_index + 1)
             assert value_start_index is not None
             value_end_index: Optional[int] = None
             if ParserHelper.is_character_at_index_one_of(
                 text_to_parse,
                 value_start_index,
                 HtmlHelper.__html_attribute_value_single,
@@ -663,15 +667,14 @@
 
         return html_block_type
 
     @staticmethod
     def __check_for_normal_html_blocks_adjust_tag(
         remaining_html_tag: str, line_to_parse: str, character_index: int
     ) -> Tuple[str, int, bool]:
-
         adjusted_remaining_html_tag, line_to_parse_size = remaining_html_tag, len(
             line_to_parse
         )
         is_end_tag = (
             bool(adjusted_remaining_html_tag)
             and adjusted_remaining_html_tag[0] == HtmlHelper.__html_tag_start
         )
@@ -790,15 +793,15 @@
     ) -> Tuple[Optional[str], Optional[str]]:
         """
         Determine if the current sequence of characters would start a html block element.
         """
 
         assert extracted_whitespace is not None
         if (
-            ParserHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
+            TabHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
         ) and ParserHelper.is_character_at_index(
             line_to_parse,
             start_index,
             HtmlHelper.__html_block_start_character,
         ):
             (
                 html_block_type,
@@ -813,39 +816,74 @@
         return html_block_type, remaining_html_tag
 
     @staticmethod
     def parse_html_block(
         parser_state: ParserState,
         position_marker: PositionMarker,
         extracted_whitespace: Optional[str],
-    ) -> List[MarkdownToken]:
+        block_quote_data: BlockQuoteData,
+        original_line: str,
+    ) -> Tuple[List[MarkdownToken], bool]:
         """
         Determine if we have the criteria that we need to start an HTML block.
         """
 
         html_block_type, _ = HtmlHelper.is_html_block(
             position_marker.text_to_parse,
             position_marker.index_number,
             extracted_whitespace,
             parser_state.token_stack,
         )
+        did_adjust_block_quote = False
+        POGGER.debug("did_adjust_block_quote=$", did_adjust_block_quote)
         if html_block_type:
             new_tokens, _ = parser_state.close_open_blocks_fn(
                 parser_state,
                 only_these_blocks=[ParagraphStackToken],
             )
+            POGGER.debug("new_tokens=$", new_tokens)
+
+            split_tab = False
+            if ParserHelper.tab_character in original_line:
+                token_text = position_marker.text_to_parse[
+                    position_marker.index_number :
+                ]
+                POGGER.debug("original_line=:$:", original_line)
+                POGGER.debug("token_text=:$:", token_text)
+                POGGER.debug("extracted_whitespace=:$:", extracted_whitespace)
+                _, split_tab, _ = TabHelper.parse_thematic_break_with_tab(
+                    original_line, token_text, extracted_whitespace
+                )
+                POGGER.debug("split_tab=:$:", split_tab)
+
+            POGGER.debug("did_adjust_block_quote=$", did_adjust_block_quote)
+            POGGER.debug("split_tab=$", split_tab)
+            old_split_tab = split_tab
+            did_adjust_block_quote = False
+            if split_tab := ContainerHelper.reduce_containers_if_required(
+                parser_state, block_quote_data, new_tokens, split_tab
+            ):
+                TabHelper.adjust_block_quote_indent_for_tab(parser_state)
+                did_adjust_block_quote = True
+                POGGER.debug("did_adjust_block_quote=$", did_adjust_block_quote)
+            POGGER.debug("split_tab=$", split_tab)
+            did_adjust_block_quote = (
+                split_tab != old_split_tab or did_adjust_block_quote
+            )
+
             assert extracted_whitespace is not None
             new_token = HtmlBlockMarkdownToken(position_marker, extracted_whitespace)
             new_tokens.append(new_token)
             parser_state.token_stack.append(
                 HtmlBlockStackToken(html_block_type, new_token)
             )
         else:
             new_tokens = []
-        return new_tokens
+        POGGER.debug("did_adjust_block_quote=$", did_adjust_block_quote)
+        return new_tokens, did_adjust_block_quote
 
     @staticmethod
     def check_blank_html_block_end(parser_state: ParserState) -> List[MarkdownToken]:
         """
         Check to see if we have encountered the end of the current HTML block
         via an empty line or BLANK.
         """
@@ -856,35 +894,88 @@
             HtmlHelper.html_block_6,
             HtmlHelper.html_block_7,
         ]:
             new_tokens, _ = parser_state.close_open_blocks_fn(
                 parser_state,
                 only_these_blocks=[HtmlBlockStackToken],
             )
+            POGGER.debug("new_tokens=$", new_tokens)
         else:
             new_tokens = []
 
         return new_tokens
 
     @staticmethod
+    def __check_normal_html_block_end_with_tab(
+        parser_state: ParserState,
+        original_line: str,
+        extracted_whitespace: str,
+        token_text: str,
+        did_adjust_block_quote: bool,
+    ) -> Tuple[str, str]:
+        POGGER.debug("did_adjust_block_quote>:$:<", did_adjust_block_quote)
+        (
+            tabified_text,
+            split_tab,
+            tabified_whitespace,
+        ) = TabHelper.parse_thematic_break_with_tab(
+            original_line, token_text, extracted_whitespace
+        )
+
+        POGGER.debug("tabified_text>:$:<", tabified_text)
+        POGGER.debug("tabified_whitespace>:$:<", tabified_whitespace)
+        POGGER.debug("split_tab>:$:<", split_tab)
+
+        if split_tab:
+            POGGER.debug("extracted_whitespace>:$:<", extracted_whitespace)
+            assert tabified_whitespace is not None
+            tabified_whitespace = ParserHelper.create_replacement_markers(
+                tabified_whitespace, extracted_whitespace
+            )
+            POGGER.debug("tabified_whitespace>:$:<", tabified_whitespace)
+            if not did_adjust_block_quote:
+                TabHelper.adjust_block_quote_indent_for_tab(parser_state)
+        assert tabified_whitespace is not None
+        return tabified_whitespace, tabified_text
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
     def check_normal_html_block_end(
         parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: str,
         position_marker: PositionMarker,
+        original_line: str,
+        did_adjust_block_quote: bool,
     ) -> List[MarkdownToken]:
         """
         Check to see if we have encountered the end of the current HTML block
         via text on a normal line.
         """
 
+        token_text = line_to_parse[start_index:]
+        POGGER.debug("extracted_whitespace=:$:", extracted_whitespace)
+        POGGER.debug("token_text=:$:", token_text)
+        POGGER.debug("original_line=:$:", original_line)
+        if ParserHelper.tab_character in original_line:
+            (
+                extracted_whitespace,
+                token_text,
+            ) = HtmlHelper.__check_normal_html_block_end_with_tab(
+                parser_state,
+                original_line,
+                extracted_whitespace,
+                token_text,
+                did_adjust_block_quote,
+            )
+
         new_tokens: List[MarkdownToken] = [
             TextMarkdownToken(
-                line_to_parse[start_index:],
+                token_text,
                 extracted_whitespace,
                 position_marker=position_marker,
             )
         ]
 
         is_block_terminated, adj_line = False, line_to_parse[start_index:]
         assert parser_state.token_stack[-1].is_html_block
@@ -903,10 +994,13 @@
             is_block_terminated = HtmlHelper.__html_block_5_end in adj_line
 
         if is_block_terminated:
             terminated_block_tokens, _ = parser_state.close_open_blocks_fn(
                 parser_state,
                 only_these_blocks=[HtmlBlockStackToken],
             )
+            POGGER.debug("terminated_block_tokens=$", terminated_block_tokens)
             assert terminated_block_tokens
             new_tokens.extend(terminated_block_tokens)
         return new_tokens
+
+    # pylint: enable=too-many-arguments
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/inline_helper.py` & `pymarkdownlnt-0.9.9/pymarkdown/inline_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     UriAutolinkMarkdownToken,
 )
 from pymarkdown.inline_request import InlineRequest
 from pymarkdown.inline_response import InlineResponse
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 # pylint: disable=too-many-lines
 
 
 class InlineHelper:
@@ -56,15 +57,14 @@
     backslash_character = "\\"
     __entity_map: Dict[str, str] = {}
     character_reference_start_character = "&"
     __numeric_character_reference_start_character = "#"
     __hex_character_reference_start_character = "xX"
     __character_reference_end_character = ";"
     __invalid_reference_character_substitute = "\ufffd"
-    __line_end_whitespace = ParserHelper.space_character
     __valid_backslash_sequence_starts = (
         f"{backslash_character}{character_reference_start_character}"
     )
 
     __ascii_letters_and_digits = f"{string.ascii_letters}{string.digits}"
 
     __skip_html5_entities_ending_with = ";"
@@ -431,27 +431,14 @@
                     inline_response.delta_column_number,
                 ) = ParserHelper.calculate_deltas(
                     f"{original_between_text}{extracted_start_backticks}"
                 )
         return inline_response
 
     @staticmethod
-    def modify_end_string(
-        end_string: Optional[str], removed_end_whitespace: str
-    ) -> str:
-        """
-        Modify the string at the end of the paragraph.
-        """
-        return (
-            f"{removed_end_whitespace}{ParserHelper.newline_character}"
-            if end_string is None
-            else f"{end_string}{removed_end_whitespace}{ParserHelper.newline_character}"
-        )
-
-    @staticmethod
     def __backtick_split_lines(input_string: str) -> List[str]:
         current_index: Optional[int] = 0
         assert current_index is not None
         next_index, extracted_text = ParserHelper.collect_while_one_of_characters(
             input_string, current_index, " \t"
         )
         assert next_index is not None
@@ -480,61 +467,60 @@
     @staticmethod
     def __find_index_in_split_lines(
         split_array: List[str], index_to_find: int
     ) -> Tuple[int, int, int]:
         start_index = 0
         _array_index = 0
         for _array_index, array_element in enumerate(split_array):  # pragma: no cover
-            # POGGER.debug("$--$ >>:$:<<", array_index, start_index, split_array[array_index])
+            POGGER.debug(
+                "$--$ >>:$:<<", _array_index, start_index, split_array[_array_index]
+            )
             if start_index <= index_to_find < start_index + len(array_element):
                 break
             start_index += len(array_element)
-        assert start_index != len(split_array)
+        assert start_index != (start_index + len(split_array))
         delta = index_to_find - start_index
-        # POGGER.debug("i=$,start_index=$,delta=$", array_index, start_index, delta)
+        POGGER.debug("i=$,start_index=$,delta=$", _array_index, start_index, delta)
         return _array_index, delta, start_index
 
-    # pylint: disable=too-many-locals
     @staticmethod
     def __calculate_backtick_between_text(
         inline_request: InlineRequest, new_index: int, end_backtick_start_index: int
     ) -> Tuple[str, str, str, str]:
         POGGER.debug("inline_request.source_text>>$<<", inline_request.source_text)
         POGGER.debug("new_index>>$<<", new_index)
         POGGER.debug("end_backtick_start_index>>$<<", end_backtick_start_index)
 
         between_text = inline_request.source_text[new_index:end_backtick_start_index]
-        actual_between_text = between_text
-        if inline_request.tabified_text:
-            actual_between_text = (
-                InlineHelper.__calculate_backtick_between_tabified_text(
-                    inline_request, new_index, end_backtick_start_index
-                )
-            )
+
         original_between_text, leading_whitespace, trailing_whitespace = (
             between_text,
             "",
             "",
         )
+
+        if inline_request.tabified_text:
+            between_text = InlineHelper.__calculate_backtick_between_tabified_text(
+                inline_request, new_index, end_backtick_start_index
+            )
         POGGER.debug(
             "after_collect>$>>$>>$<<",
             between_text,
             end_backtick_start_index,
             inline_request.source_text[end_backtick_start_index:],
         )
         POGGER.debug("between_text>>$<<", between_text)
-        POGGER.debug("actual_between_text>>$<<", actual_between_text)
         if (
-            len(actual_between_text) > 2
-            and actual_between_text[0]
+            len(between_text) > 2
+            and between_text[0]
             in [
                 ParserHelper.space_character,
                 ParserHelper.newline_character,
             ]
-            and actual_between_text[-1]
+            and between_text[-1]
             in [
                 ParserHelper.space_character,
                 ParserHelper.newline_character,
             ]
         ):
             stripped_between_attempt = between_text[1:-1]
             if len(stripped_between_attempt.strip()) != 0:
@@ -570,30 +556,28 @@
         return (
             between_text,
             original_between_text,
             leading_whitespace,
             trailing_whitespace,
         )
 
-    # pylint: enable=too-many-locals
-
     @staticmethod
     def __calculate_backtick_between_tabified_text(
         inline_request: InlineRequest, new_index: int, end_backtick_start_index: int
     ) -> str:
         POGGER.debug("inline_request.tabified_text>>$<<", inline_request.tabified_text)
         split_source_lines = InlineHelper.__backtick_split_lines(
             inline_request.source_text
         )
-        POGGER.debug("rt>>$<<", split_source_lines)
+        POGGER.debug("split_source_lines>>$<<", split_source_lines)
         assert inline_request.tabified_text is not None
         split_tabified_lines = InlineHelper.__backtick_split_lines(
             inline_request.tabified_text
         )
-        POGGER.debug("rtx>>$<<", split_tabified_lines)
+        POGGER.debug("split_tabified_lines>>$<<", split_tabified_lines)
         assert len(split_tabified_lines) == len(split_source_lines)
 
         (
             start_array_index,
             start_delta,
             calculated_index,
         ) = InlineHelper.__find_index_in_split_lines(split_source_lines, new_index)
@@ -617,109 +601,124 @@
             end_array_index,
             end_delta,
             calculated_index,
         )
         assert calculated_index + end_delta == end_backtick_start_index
 
         if start_array_index == end_array_index:
+            POGGER.debug("same")
             actual_between_text = split_tabified_lines[start_array_index][
                 start_delta:end_delta
             ]
         else:
-            actual_between_text = "".join(
+            POGGER.debug("borders")
+            if start_delta:
+                actual_between_text = split_tabified_lines[start_array_index][
+                    start_delta:
+                ]
+                start_array_index += 1
+            else:
+                actual_between_text = ""
+            actual_between_text += "".join(
                 split_tabified_lines[i]
                 for i in range(start_array_index, end_array_index)
             )
+            if end_delta:
+                actual_between_text += split_tabified_lines[end_array_index][:end_delta]
         POGGER.debug("actual_between_text>:$:<", actual_between_text)
         return actual_between_text
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def handle_line_end(
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         end_string: Optional[str],
         current_string: str,
         inline_blocks: List[MarkdownToken],
         is_setext: bool,
         line_number: int,
         column_number: int,
         coalesced_stack: List[MarkdownToken],
         tabified_text: Optional[str],
+        inline_request: InlineRequest,
     ) -> Tuple[str, Optional[str], List[MarkdownToken], str, Optional[str], str]:
         """
         Handle the inline case of having the end of line character encountered.
         """
         new_tokens: List[MarkdownToken] = []
 
-        POGGER.debug(">>current_string>>$>>", current_string)
-        POGGER.debug(">>end_string>>$>>", end_string)
-        POGGER.debug(">>remaining_line>>$>>", remaining_line)
-        _, last_non_whitespace_index = ParserHelper.collect_backwards_while_spaces(
-            remaining_line, -1
-        )
-        POGGER.debug(">>last_non_whitespace_index>>$", last_non_whitespace_index)
-        removed_end_whitespace = remaining_line[last_non_whitespace_index:]
-        remaining_line = remaining_line[:last_non_whitespace_index]
-        POGGER.debug(">>removed_end_whitespace>>$>>", removed_end_whitespace)
-        POGGER.debug(">>remaining_line>>$>>", remaining_line)
-
-        POGGER.debug(">>current_string>>$>>", current_string)
-        (append_to_current_string, removed_end_whitespace_size, adj_hard_column,) = (
-            ParserHelper.newline_character,
-            len(removed_end_whitespace),
-            column_number + len(remaining_line),
-        )
-        whitespace_to_add: Optional[str] = None
-        POGGER.debug(
-            ">>len(r_e_w)>>$>>rem>>$>>",
-            removed_end_whitespace_size,
+        # POGGER.debug(">>current_string>>$>>", current_string)
+        # POGGER.debug(">>end_string>>$>>", end_string)
+        # POGGER.debug(">>remaining_line>>$>>", remaining_line)
+        # POGGER.debug(">>tabified_remaining_line>>$>>", tabified_remaining_line)
+        (
+            removed_end_whitespace,
             remaining_line,
+        ) = InlineHelper.__setup_for_select_line_ending(
+            tabified_remaining_line, is_setext, remaining_line
         )
-
-        is_proper_hard_break = InlineHelper.__is_proper_hard_break(
-            current_string, removed_end_whitespace_size
-        )
+        # POGGER.debug(">>line_to_use>>$>>", line_to_use)
+        # POGGER.debug(">>current_string>>$>>", current_string)
 
         (
             current_string,
             whitespace_to_add,
             append_to_current_string,
             end_string,
             remaining_line,
         ) = InlineHelper.__select_line_ending(
             new_tokens,
-            is_proper_hard_break,
             line_number,
-            adj_hard_column,
+            column_number + len(remaining_line),
             current_string,
             removed_end_whitespace,
-            removed_end_whitespace_size,
-            whitespace_to_add,
-            append_to_current_string,
             end_string,
             remaining_line,
             inline_blocks,
             is_setext,
             tabified_text,
+            inline_request,
         )
 
-        if coalesced_stack and coalesced_stack[-1].is_block_quote_start:
-            block_quote_token = cast(BlockQuoteMarkdownToken, coalesced_stack[-1])
-            block_quote_token.leading_text_index += 1
+        InlineHelper.__handle_line_end_adjust_block_quote(coalesced_stack)
 
         return (
             append_to_current_string,
             whitespace_to_add,
             new_tokens,
             remaining_line,
             end_string,
             current_string,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
+    @staticmethod
+    def __setup_for_select_line_ending(
+        tabified_remaining_line: Optional[str], is_setext: bool, remaining_line: str
+    ) -> Tuple[str, str]:
+        line_to_use = (
+            tabified_remaining_line
+            if tabified_remaining_line and is_setext
+            else remaining_line
+        )
+        _, last_non_whitespace_index = ParserHelper.collect_backwards_while_character(
+            line_to_use, -1, " "
+        )
+        removed_end_whitespace = line_to_use[last_non_whitespace_index:]
+        remaining_line = line_to_use[:last_non_whitespace_index]
+        return removed_end_whitespace, remaining_line
+
+    @staticmethod
+    def __handle_line_end_adjust_block_quote(
+        coalesced_stack: List[MarkdownToken],
+    ) -> None:
+        if coalesced_stack and coalesced_stack[-1].is_block_quote_start:
+            block_quote_token = cast(BlockQuoteMarkdownToken, coalesced_stack[-1])
+            block_quote_token.leading_text_index += 1
 
     @staticmethod
     def __is_proper_hard_break(
         current_string: str, removed_end_whitespace_size: int
     ) -> bool:
         POGGER.debug("__is_proper_hard_break>>current_string>>$>>", current_string)
         POGGER.debug("removed_end_whitespace_size>>$>>", removed_end_whitespace_size)
@@ -737,36 +736,53 @@
             POGGER.debug(">>$<<", is_proper_hard_break)
         else:
             is_proper_hard_break = False
 
         POGGER.debug("__is_proper_hard_break>>$>>", is_proper_hard_break)
         return is_proper_hard_break
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __select_line_ending(
         new_tokens: List[MarkdownToken],
-        is_proper_hard_break: bool,
         line_number: int,
         adj_hard_column: int,
         current_string: str,
         removed_end_whitespace: str,
-        removed_end_whitespace_size: int,
-        whitespace_to_add: Optional[str],
-        append_to_current_string: str,
         end_string: Optional[str],
         remaining_line: str,
         inline_blocks: List[MarkdownToken],
         is_setext: bool,
         tabified_text: Optional[str],
+        inline_request: InlineRequest,
     ) -> Tuple[str, Optional[str], str, Optional[str], str]:
-        POGGER.debug(">>removed_end_whitespace>:$:<", removed_end_whitespace)
-        POGGER.debug(">>tabified_text>:$:<", tabified_text)
+        # POGGER.debug(">>removed_end_whitespace>:$:<", removed_end_whitespace)
+        # POGGER.debug(">>tabified_text>:$:<", tabified_text)
+        # POGGER.debug(
+        #     ">>inline_request.tabified_text>:$:<", inline_request.tabified_text
+        # )
+        # POGGER.debug(
+        #     ">>inline_request.tabified_remaining_line>:$:<",
+        #     inline_request.tabified_remaining_line,
+        # )
+        append_to_current_string = ParserHelper.newline_character
+        whitespace_to_add: Optional[str] = None
+
+        removed_end_whitespace_size = len(removed_end_whitespace)
+        # POGGER.debug(
+        #     ">>len(r_e_w)>>$>>rem>>$>>",
+        #     removed_end_whitespace_size,
+        #     remaining_line,
+        # )
+
         is_proper_end = not tabified_text or tabified_text.endswith("  ")
-        if is_proper_hard_break:
+
+        if InlineHelper.__is_proper_hard_break(
+            current_string, removed_end_whitespace_size
+        ):
             POGGER.debug(">>proper hard break")
             new_tokens.append(
                 HardBreakMarkdownToken(
                     InlineHelper.backslash_character, line_number, adj_hard_column - 1
                 )
             )
             current_string, whitespace_to_add = current_string[:-1], None
@@ -778,95 +794,116 @@
                     removed_end_whitespace, line_number, adj_hard_column
                 )
             )
             whitespace_to_add = None
             append_to_current_string = ""
         else:
             POGGER.debug(">>normal end")
+            # POGGER.debug("current_string>:$:<", current_string)
+            # POGGER.debug("removed_end_whitespace>:$:<", removed_end_whitespace)
+            # POGGER.debug("end_string>:$:<", end_string)
+            # POGGER.debug("remaining_line>:$:<", remaining_line)
             end_string, remaining_line = InlineHelper.__select_line_ending_normal(
                 is_setext,
                 inline_blocks,
                 current_string,
                 removed_end_whitespace,
+                inline_request.tabified_remaining_line,
                 end_string,
                 remaining_line,
             )
 
-        POGGER.debug(
-            "<<append_to_current_string<<$<<",
-            append_to_current_string,
-        )
-        POGGER.debug(
-            "<<whitespace_to_add<<$<<",
-            whitespace_to_add,
-        )
-        POGGER.debug("<<remaining_line<<$<<", remaining_line)
-        POGGER.debug("<<end_string<<$<<", end_string)
-        POGGER.debug("<<current_string<<$<<", current_string)
+        # POGGER.debug(
+        #     "<<append_to_current_string<<$<<",
+        #     append_to_current_string,
+        # )
+        # POGGER.debug(
+        #     "<<whitespace_to_add<<$<<",
+        #     whitespace_to_add,
+        # )
+        # POGGER.debug("<<remaining_line<<$<<", remaining_line)
+        # POGGER.debug("<<end_string<<$<<", end_string)
+        # POGGER.debug("<<current_string<<$<<", current_string)
         return (
             current_string,
             whitespace_to_add,
             append_to_current_string,
             end_string,
             remaining_line,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __select_line_ending_normal(
         is_setext: bool,
         inline_blocks: List[MarkdownToken],
         current_string: str,
         removed_end_whitespace: str,
+        tabified_remaining_line: Optional[str],
         end_string: Optional[str],
         remaining_line: str,
     ) -> Tuple[str, str]:
         # POGGER.debug("<<is_setext<<$<<", is_setext)
         # POGGER.debug("<<inline_blocks<<$<<", inline_blocks)
         # POGGER.debug("<<current_string<<$<<", current_string)
-        # POGGER.debug("<<remaining_line<<$<<", remaining_line)
-        # POGGER.debug("<<end_string<<$<<", end_string)
-        # POGGER.debug("<<removed_end_whitespace<<$<<", removed_end_whitespace)
+        POGGER.debug("<<remaining_line<<$<<", remaining_line)
+        POGGER.debug("<<end_string<<$<<", end_string)
+        POGGER.debug("<<removed_end_whitespace<<$<<", removed_end_whitespace)
         if (
             is_setext
             and inline_blocks
             and inline_blocks[-1].is_inline_hard_break
             and not current_string
         ):
             new_index, ex_ws = ParserHelper.extract_spaces(remaining_line, 0)
             # POGGER.debug("<<new_index<<$<<", new_index)
             # POGGER.debug("<<ex_ws<<$<<", ex_ws)
             assert new_index
             end_string = f"{ex_ws}{ParserHelper.whitespace_split_character}"
             remaining_line = remaining_line[new_index:]
+        if not is_setext and tabified_remaining_line and removed_end_whitespace:
+            POGGER.debug("<<tabified_remaining_line>:$:<", tabified_remaining_line)
+            POGGER.debug("<<removed_end_whitespace>:$:<", removed_end_whitespace)
+            adj_original, _ = TabHelper.find_detabify_string_ex(
+                tabified_remaining_line, removed_end_whitespace
+            )
+            POGGER.debug("<<adj_original<<$<<", adj_original)
+            assert adj_original is not None
+            removed_end_whitespace = adj_original
 
-        end_string = InlineHelper.modify_end_string(end_string, removed_end_whitespace)
-        # POGGER.debug("<<end_string<<$<<", end_string)
+        POGGER.debug("<<end_string<<$<<", end_string)
+        end_string = (
+            f"{removed_end_whitespace}{ParserHelper.newline_character}"
+            if end_string is None
+            else f"{end_string}{removed_end_whitespace}{ParserHelper.newline_character}"
+        )
+        POGGER.debug("<<end_string<<$<<", end_string)
         return end_string, remaining_line
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
     def extract_bounded_string(
         source_text: str,
         new_index: int,
         close_character: str,
         start_character: Optional[str],
     ) -> Tuple[Optional[int], Optional[str]]:
         """
         Extract a string that is bounded by some manner of characters.
         """
+        nesting_level: int = 0
         break_characters = (
             f"{InlineHelper.backslash_character}{close_character}{start_character}"
             if start_character
             else f"{InlineHelper.backslash_character}{close_character}"
         )
-        nesting_level: int = 0
+
         POGGER.debug(
             "extract_bounded_string>>new_index>>$>>data>>$>>",
             new_index,
             source_text[new_index:],
         )
         next_index, data = ParserHelper.collect_until_one_of_characters(
             source_text, new_index, break_characters
@@ -875,16 +912,16 @@
         extracted_parts: List[str] = [data]
         POGGER.debug(
             ">>next_index1>>$>>data>>$>>",
             next_index,
             data,
         )
         assert next_index is not None
-        while next_index < len(source_text) and not (
-            source_text[next_index] == close_character and nesting_level == 0
+        while next_index < len(source_text) and (
+            source_text[next_index] != close_character or nesting_level != 0
         ):
             (
                 next_index,
                 nesting_level,
             ) = InlineHelper.__handle_next_extract_bounded_string_item(
                 source_text,
                 next_index,
@@ -924,15 +961,14 @@
         next_index: int,
         extracted_parts: List[str],
         start_character: Optional[str],
         nesting_level: int,
         close_character: str,
         break_characters: str,
     ) -> Tuple[int, int]:
-
         if ParserHelper.is_character_at_index(
             source_text, next_index, InlineHelper.backslash_character
         ):
             POGGER.debug("pre-back>>next_index>>$>>", next_index)
             old_index = next_index
 
             inline_request = InlineRequest(source_text, next_index)
@@ -1086,15 +1122,14 @@
                 f"Named character entity map file '{master_entities_file}' "
                 + f"was not loaded ({this_exception})."
             )
             raise BadTokenizationError(error_message) from this_exception
 
         approved_entity_map = {}
         for next_name, char_entity in results_dictionary.items():
-
             # Downloaded file is for HTML5, which includes some names that do
             # not end with ";".  These are excluded.
             if next_name[-1] != InlineHelper.__skip_html5_entities_ending_with:
                 continue
 
             entity_characters = char_entity["characters"]
             entity_codepoints = char_entity["codepoints"]
@@ -1165,15 +1200,14 @@
         """
         Given an open angle bracket, determine which of the three possibilities it is.
         """
         closing_angle_index = inline_request.source_text.find(
             InlineHelper.__angle_bracket_end, inline_request.next_index
         )
         if closing_angle_index not in (-1, inline_request.next_index + 1):
-
             between_brackets, remaining_line = (
                 inline_request.source_text[
                     inline_request.next_index + 1 : closing_angle_index
                 ],
                 inline_request.source_text[inline_request.next_index + 1 :],
             )
             closing_angle_index += 1
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/inline_markdown_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/inline_markdown_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Module to provide for an inline element that can be added to markdown parsing stream.
 """
 import logging
 from typing import Optional, Tuple, cast
 
 from pymarkdown.constants import Constants
+from pymarkdown.link_helper_properties import LinkHelperProperties
 from pymarkdown.markdown_token import MarkdownToken, MarkdownTokenClass
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.position_marker import PositionMarker
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
@@ -264,81 +265,74 @@
 
 # pylint: disable=too-many-instance-attributes
 class ReferenceMarkdownToken(InlineMarkdownToken):
     """
     Base class for images and links.
     """
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
+        lhp: LinkHelperProperties,
         token_name: str,
-        label_type: str,
-        link_uri: str,
-        link_title: Optional[str],
         extra_data: Optional[str],
-        pre_link_uri: str,
-        pre_link_title: Optional[str],
-        ex_label: Optional[str],
         text_from_blocks: str,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: Optional[str],
-        before_link_whitespace: Optional[str],
-        before_title_whitespace: Optional[str],
-        after_title_whitespace: Optional[str],
         line_number: int = 0,
         column_number: int = 0,
         requires_end_token: bool = False,
         can_force_close: bool = True,
     ):
+        assert lhp.inline_link is not None
+        assert lhp.label_type is not None
+        assert lhp.pre_inline_link is not None
         (
             self.__label_type,
             self.__link_uri,
             self.__link_title,
             self.__pre_link_uri,
             self.__pre_link_title,
             self.__ex_label,
             self.__text_from_blocks,
             self.__did_use_angle_start,
             self.__inline_title_bounding_character,
             self.__before_link_whitespace,
             self.__before_title_whitespace,
             self.__after_title_whitespace,
         ) = (
-            label_type,
-            link_uri,
-            link_title,
-            pre_link_uri,
-            pre_link_title,
-            ex_label,
+            lhp.label_type,
+            lhp.inline_link,
+            lhp.inline_title,
+            lhp.pre_inline_link,
+            lhp.pre_inline_title,
+            lhp.ex_label,
             text_from_blocks,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
+            lhp.did_use_angle_start,
+            lhp.bounding_character,
+            lhp.before_link_whitespace,
+            lhp.before_title_whitespace,
+            lhp.after_title_whitespace,
         )
 
         if token_name == MarkdownToken._token_inline_image:
             extra_data = f"{extra_data}{MarkdownToken.extra_data_separator}"
 
         # Purposefully split this way to accommodate the extra data
-        part_1, part_2 = self.__build_extra_data(extra_data, label_type)
+        part_1, part_2 = self.__build_extra_data(extra_data, lhp.label_type)
 
         InlineMarkdownToken.__init__(
             self,
             token_name,
             f"{part_1}{part_2}",
             line_number=line_number,
             column_number=column_number,
             requires_end_token=requires_end_token,
             can_force_close=can_force_close,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
     def __build_extra_data(
         self, extra_data: Optional[str], label_type: str
     ) -> Tuple[str, str]:
         assert self.__link_title is not None
         assert extra_data is not None
         part_1 = MarkdownToken.extra_data_separator.join(
@@ -411,15 +405,15 @@
     def text_from_blocks(self) -> str:
         """
         Returns the text extracted from the blocks of the link, before processing.
         """
         return self.__text_from_blocks
 
     @property
-    def did_use_angle_start(self) -> bool:
+    def did_use_angle_start(self) -> Optional[bool]:
         """
         Returns a value indicating whether an angle start was used around the URI.
         """
         return self.__did_use_angle_start
 
     @property
     def inline_title_bounding_character(self) -> Optional[str]:
@@ -454,103 +448,87 @@
 
 
 class LinkStartMarkdownToken(ReferenceMarkdownToken):
     """
     Class to provide for an encapsulation of the link element.
     """
 
-    # pylint: disable=too-many-arguments
     def __init__(
         self,
-        link_uri: str,
-        pre_link_uri: str,
-        link_title: str,
-        pre_link_title: str,
-        ex_label: str,
-        label_type: str,
         text_from_blocks: str,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: str,
-        before_link_whitespace: str,
-        before_title_whitespace: str,
-        after_title_whitespace: str,
         line_number: int,
         column_number: int,
+        lhp: LinkHelperProperties,
     ) -> None:
+        assert lhp.pre_inline_link is not None
+        assert lhp.label_type is not None
+        assert lhp.inline_link is not None
         ReferenceMarkdownToken.__init__(
             self,
-            MarkdownToken._token_inline_link,
-            label_type,
-            link_uri,
-            link_title,
+            lhp,
+            LinkStartMarkdownToken.get_markdown_token_type(),
             "",
-            pre_link_uri,
-            pre_link_title,
-            ex_label,
             text_from_blocks,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
             line_number=line_number,
             column_number=column_number,
             requires_end_token=True,
             can_force_close=False,
         )
 
-    # pylint: enable=too-many-arguments
+    # pylint: disable=protected-access
+    @staticmethod
+    def get_markdown_token_type() -> str:
+        """
+        Get the type of markdown token for rehydration purposes.
+        """
+        return MarkdownToken._token_inline_link
+
+    # pylint: enable=protected-access
 
 
 class ImageStartMarkdownToken(ReferenceMarkdownToken):
     """
     Class to provide for an encapsulation of the image element.
     """
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
-        image_uri: str,
-        pre_image_uri: str,
-        image_title: str,
-        pre_image_title: str,
         image_alt_text: str,
-        ex_label: str,
-        label_type: str,
         text_from_blocks: str,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: str,
-        before_link_whitespace: str,
-        before_title_whitespace: str,
-        after_title_whitespace: str,
         line_number: int,
         column_number: int,
+        lhp: LinkHelperProperties,
     ) -> None:
+        assert lhp.label_type is not None
+        assert lhp.pre_inline_link is not None
+        assert lhp.inline_link is not None
+
         self.__image_alt_text = image_alt_text
         ReferenceMarkdownToken.__init__(
             self,
-            MarkdownToken._token_inline_image,
-            label_type,
-            image_uri,
-            image_title,
+            lhp,
+            ImageStartMarkdownToken.get_markdown_token_type(),
             self.__image_alt_text,
-            pre_image_uri,
-            pre_image_title,
-            ex_label,
             text_from_blocks,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
             line_number=line_number,
             column_number=column_number,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=protected-access
+    @staticmethod
+    def get_markdown_token_type() -> str:
+        """
+        Get the type of markdown token for rehydration purposes.
+        """
+        return MarkdownToken._token_inline_image
+
+    # pylint: enable=protected-access
 
     @property
     def image_alt_text(self) -> str:
         """
         Returns the text extracted from the blocks of the link, after processing.
         """
         return self.__image_alt_text
@@ -652,57 +630,117 @@
     def remove_final_whitespace(self) -> str:
         """
         Remove any final whitespace.  Used by paragraph blocks so that they do not
         end with a hard break.
         """
 
         removed_whitespace = ""
+        # POGGER.debug("self.__tabified_text=:$:", self.__tabified_text)
+        # POGGER.debug("self.__token_text=:$:", self.__token_text)
         (
             collected_whitespace_length,
             first_non_whitespace_index,
         ) = ParserHelper.collect_backwards_while_one_of_characters(
             self.__token_text, -1, Constants.ascii_whitespace
         )
+        # POGGER.debug("collected_whitespace_length=:$:", collected_whitespace_length)
+        # POGGER.debug("first_non_whitespace_index=:$:", first_non_whitespace_index)
+
         assert first_non_whitespace_index is not None
         if collected_whitespace_length:
             removed_whitespace = self.__token_text[
                 first_non_whitespace_index : first_non_whitespace_index
                 + collected_whitespace_length
             ]
             self.__token_text = self.__token_text[:first_non_whitespace_index]
+            if self.__tabified_text:
+                (
+                    collected_whitespace_length,
+                    first_non_whitespace_index,
+                ) = ParserHelper.collect_backwards_while_one_of_characters(
+                    self.__tabified_text, -1, Constants.ascii_whitespace
+                )
+                # POGGER.debug("collected_whitespace_length=:$:", collected_whitespace_length)
+                # POGGER.debug("first_non_whitespace_index=:$:", first_non_whitespace_index)
+                assert collected_whitespace_length is not None
+                assert first_non_whitespace_index is not None
+                removed_whitespace = self.__tabified_text[
+                    first_non_whitespace_index : first_non_whitespace_index
+                    + collected_whitespace_length
+                ]
+                self.__tabified_text = self.__tabified_text[:first_non_whitespace_index]
+        self.__compose_extra_data_field()
         return removed_whitespace
 
     def combine(
         self, other_text_token: MarkdownToken, remove_leading_spaces: int
     ) -> str:
         """
         Combine the two text tokens together with a line feed between.
         If remove_leading_spaces > 0, then that many leading spaces will be
         removed from each line, if present.
         If remove_leading_spaces == -1, then.
         If remove_leading_spaces == 0, then.
         """
 
         if other_text_token.is_blank_line:
-            text_to_combine, whitespace_present, blank_line_sequence = (
-                "",
+            text_to_combine = ""
+            tabified_text_to_combine: Optional[str] = ""
+            (
+                whitespace_present,
+                blank_line_sequence,
+            ) = (
                 other_text_token.extra_data,
                 ParserHelper.replace_noop_character,
             )
         else:
             assert other_text_token.is_text
             text_other_token = cast(TextMarkdownToken, other_text_token)
-            text_to_combine, whitespace_present, blank_line_sequence = (
-                text_other_token.token_text,
+
+            text_to_combine = text_other_token.token_text
+            tabified_text_to_combine = text_other_token.tabified_text
+            (
+                whitespace_present,
+                blank_line_sequence,
+            ) = (
                 text_other_token.extracted_whitespace,
                 "",
             )
 
+        removed_whitespace, prefix_whitespace = self.__combine_handle_whitespace(
+            remove_leading_spaces, whitespace_present
+        )
+
+        if self.__tabified_text or tabified_text_to_combine:
+            other_token_text = tabified_text_to_combine or text_to_combine
+
+            this_token_text = self.__tabified_text or self.__token_text
+            # POGGER.debug("this_token_text>:$:<", this_token_text)
+            # POGGER.debug("blank_line_sequence>:$:<", blank_line_sequence)
+            # POGGER.debug("prefix_whitespace>:$:<", prefix_whitespace)
+            # POGGER.debug("other_token_text>:$:<", other_token_text)
+
+            self.__tabified_text = (
+                f"{this_token_text}{ParserHelper.newline_character}{blank_line_sequence}"
+                + f"{prefix_whitespace}{other_token_text}"
+            )
+        self.__token_text = (
+            f"{self.__token_text}{ParserHelper.newline_character}{blank_line_sequence}"
+            + f"{prefix_whitespace}{text_to_combine}"
+        )
+        self.__compose_extra_data_field()
+        return removed_whitespace
+
+    def __combine_handle_whitespace(
+        self, remove_leading_spaces: int, whitespace_present: Optional[str]
+    ) -> Tuple[str, str]:
+        prefix_whitespace = ""
         whitespace_to_append, removed_whitespace = None, ""
         if not remove_leading_spaces:
+            assert whitespace_present is not None
             prefix_whitespace = whitespace_present
         elif remove_leading_spaces == -1:
             whitespace_to_append, prefix_whitespace = whitespace_present, ""
         else:
             assert whitespace_present is not None
             whitespace_present_size = len(whitespace_present)
             POGGER.debug(
@@ -720,20 +758,15 @@
                 )
 
         if whitespace_to_append is not None:
             self.__extracted_whitespace = (
                 f"{self.__extracted_whitespace}"
                 + f"{ParserHelper.newline_character}{whitespace_to_append}"
             )
-        self.__token_text = (
-            f"{self.__token_text}{ParserHelper.newline_character}{blank_line_sequence}"
-            + f"{prefix_whitespace}{text_to_combine}"
-        )
-        self.__compose_extra_data_field()
-        return removed_whitespace
+        return removed_whitespace, prefix_whitespace
 
 
 class SpecialTextMarkdownToken(TextMarkdownToken):
     """
     Class to provide for special tokens that represent exceptional inline elements.
     """
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/inline_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/inline_processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     AtxHeadingMarkdownToken,
     ParagraphMarkdownToken,
 )
 from pymarkdown.link_helper import LinkHelper
 from pymarkdown.markdown_token import EndMarkdownToken, MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 # pylint: disable=too-many-lines
 
 
 class InlineProcessor:
@@ -254,14 +255,21 @@
         POGGER.debug(
             ">>before_add_ws>>$>>add>>$>>",
             coalesced_list[-1],
             text_token.extracted_whitespace,
         )
         paragraph_token.add_whitespace(text_token.extracted_whitespace)
         POGGER.debug(">>after_add_ws>>$", coalesced_list[-1])
+        POGGER.debug(
+            ">>text_token>>$", ParserHelper.make_whitespace_visible(str(text_token))
+        )
+        POGGER.debug(
+            "text_token.token_text>:$:<",
+            ParserHelper.make_whitespace_visible(str(text_token.token_text)),
+        )
         return InlineProcessor.__process_inline_text_block(
             text_token.token_text,
             coalesced_stack,
             is_para=True,
             para_space=text_token.extracted_whitespace,
             line_number=text_token.line_number,
             column_number=text_token.column_number,
@@ -272,84 +280,94 @@
     @staticmethod
     def __parse_atx_heading(
         coalesced_results: List[MarkdownToken],
         coalesce_index: int,
         coalesced_stack: List[MarkdownToken],
         coalesced_list: List[MarkdownToken],
     ) -> List[MarkdownToken]:
-
         assert coalesced_results[coalesce_index].is_text
         text_token = cast(TextMarkdownToken, coalesced_results[coalesce_index])
         POGGER.debug("atx-block>>$<<", text_token)
         POGGER.debug(
             "atx-block-text>>$<<",
             text_token.token_text,
         )
         POGGER.debug(
             "atx-block-ws>>$<<",
             text_token.extracted_whitespace,
         )
 
         assert coalesced_list[-1].is_atx_heading
         atx_token = cast(AtxHeadingMarkdownToken, coalesced_list[-1])
+        POGGER.debug(">>text_token>>$", text_token)
         return InlineProcessor.__process_inline_text_block(
             text_token.token_text,
             coalesced_stack,
             text_token.extracted_whitespace,
             line_number=text_token.line_number,
             column_number=text_token.column_number
             + len(text_token.extracted_whitespace)
             + atx_token.hash_count,
+            tabified_text=text_token.tabified_text,
         )
 
     @staticmethod
     def __parse_setext_heading(
         coalesced_results: List[MarkdownToken],
         coalesce_index: int,
         coalesced_stack: List[MarkdownToken],
     ) -> List[MarkdownToken]:
-
         assert coalesced_results[coalesce_index].is_text
         text_token = cast(TextMarkdownToken, coalesced_results[coalesce_index])
+        POGGER.debug(">>text_token>>$", text_token)
         processed_tokens = InlineProcessor.__process_inline_text_block(
             text_token.token_text,
             coalesced_stack,
             whitespace_to_recombine=text_token.extracted_whitespace,
             is_setext=True,
             para_space=text_token.extracted_whitespace,
             line_number=text_token.line_number,
             column_number=text_token.column_number,
+            tabified_text=text_token.tabified_text,
         )
         POGGER.debug(
             "processed_tokens>>$",
             processed_tokens,
         )
         return processed_tokens
 
     @staticmethod
     def __parse_code_block(
         coalesced_results: List[MarkdownToken],
         coalesce_index: int,
         coalesced_list: List[MarkdownToken],
         coalesced_stack: List[MarkdownToken],
     ) -> List[MarkdownToken]:
-
         assert coalesced_results[coalesce_index].is_text
         text_token = cast(TextMarkdownToken, coalesced_results[coalesce_index])
         encoded_text = InlineHelper.append_text("", text_token.token_text)
         if coalesced_list[-1].is_fenced_code_block:
             line_number_delta, new_column_number = 1, 1
 
             POGGER.info("coalesced_stack:$<", coalesced_stack)
             if coalesced_stack:
-                list_token = cast(ListStartMarkdownToken, coalesced_stack[-1])
-                assert list_token.leading_spaces
-                split_leading_spaces = list_token.leading_spaces.split(
-                    ParserHelper.newline_character
-                )
+                if coalesced_stack[-1].is_block_quote_start:
+                    block_quote_token = cast(
+                        BlockQuoteMarkdownToken, coalesced_stack[-1]
+                    )
+                    assert block_quote_token.bleading_spaces
+                    split_leading_spaces = block_quote_token.bleading_spaces.split(
+                        ParserHelper.newline_character
+                    )
+                else:
+                    list_token = cast(ListStartMarkdownToken, coalesced_stack[-1])
+                    assert list_token.leading_spaces
+                    split_leading_spaces = list_token.leading_spaces.split(
+                        ParserHelper.newline_character
+                    )
                 new_column_number += (
                     (len(split_leading_spaces[1]))
                     if len(split_leading_spaces) >= 2
                     else (len(split_leading_spaces[0]))
                 )
             else:
                 leading_whitespace = text_token.extracted_whitespace
@@ -389,18 +407,20 @@
     ) -> InlineResponse:
         return InlineProcessor.__handle_inline_special(
             inline_request.source_text,
             inline_request.next_index,
             inline_request.inline_blocks,
             1,
             inline_request.remaining_line,
+            inline_request.tabified_remaining_line,
             inline_request.current_string_unresolved,
             inline_request.line_number,
             inline_request.column_number,
             inline_request.para_owner,
+            inline_request.tabified_text,
         )
 
     @staticmethod
     def __handle_inline_image_link_start_character(
         inline_request: InlineRequest,
     ) -> InlineResponse:
         if ParserHelper.are_characters_at_index(
@@ -410,251 +430,326 @@
         ):
             inline_response = InlineProcessor.__handle_inline_special(
                 inline_request.source_text,
                 inline_request.next_index,
                 inline_request.inline_blocks,
                 2,
                 inline_request.remaining_line,
+                inline_request.tabified_remaining_line,
                 inline_request.current_string_unresolved,
                 inline_request.line_number,
                 inline_request.column_number,
                 inline_request.para_owner,
+                inline_request.tabified_text,
             )
             assert not inline_response.consume_rest_of_line
         else:
             inline_response = InlineResponse()
             (
                 inline_response.new_string,
                 inline_response.new_index,
                 inline_response.delta_column_number,
             ) = (LinkHelper.image_start_sequence[0], inline_request.next_index + 1, 1)
         return inline_response
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_inline_special(
         source_text: str,
         next_index: int,
         inline_blocks: List[MarkdownToken],
         special_length: int,
         remaining_line: Optional[str],
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: Optional[str],
         line_number: Optional[int],
         column_number: Optional[int],
         para_owner: Optional[ParagraphMarkdownToken],
+        tabified_text: Optional[str],
     ) -> InlineResponse:
         """
         Handle the collection of special inline characters for later processing.
         """
         assert remaining_line is not None
         assert column_number is not None
         assert current_string_unresolved is not None
 
-        remaining_line_size = len(remaining_line)
+        inline_response = InlineResponse()
+        inline_response.new_string = ""
+
+        POGGER.debug(">>tabified_text>:$:<", tabified_text)
         POGGER.debug(">>column_number>>$<<", column_number)
         POGGER.debug(">>remaining_line>>$<<", remaining_line)
-        column_number += remaining_line_size
+        column_number += len(remaining_line)
         POGGER.debug(">>column_number>>$<<", column_number)
 
         (
             special_sequence,
-            repeat_count,
-            new_index,
-            preceding_two,
-            following_two,
+            inline_response.delta_column_number,
+            inline_response.new_index,
+            surrounding_whitespace_pair,
             is_active,
-            new_token,
-            consume_rest_of_line,
-            delta_line,
+            inline_response.new_tokens,
+            inline_response.consume_rest_of_line,
+            inline_response.delta_line_number,
         ) = InlineProcessor.__handle_inline_special_character(
             special_length,
             inline_blocks,
             remaining_line,
+            tabified_remaining_line,
             current_string_unresolved,
             source_text,
             next_index,
             para_owner,
-            remaining_line_size,
+            len(remaining_line),
+            tabified_text,
         )
-
-        if not new_token:
+        if not inline_response.new_tokens:
             assert line_number is not None
-            assert repeat_count is not None
             POGGER.debug(">>create>>$,$<<", line_number, column_number)
-            new_token = SpecialTextMarkdownToken(
-                special_sequence,
-                repeat_count,
-                preceding_two,
-                following_two,
-                is_active,
-                line_number,
-                column_number,
-            )
+            inline_response.new_tokens = [
+                SpecialTextMarkdownToken(
+                    special_sequence,
+                    inline_response.delta_column_number,
+                    surrounding_whitespace_pair[0],
+                    surrounding_whitespace_pair[1],
+                    is_active,
+                    line_number,
+                    column_number,
+                )
+            ]
 
-        POGGER.debug(">>delta_line>>$<<", delta_line)
-        POGGER.debug(">>repeat_count>>$<<", repeat_count)
-        assert repeat_count is not None
-        inline_response = InlineResponse()
-        (
-            inline_response.new_string,
-            inline_response.new_index,
-            inline_response.new_tokens,
-            inline_response.consume_rest_of_line,
-            inline_response.delta_line_number,
-            inline_response.delta_column_number,
-        ) = ("", new_index, [new_token], consume_rest_of_line, delta_line, repeat_count)
+        POGGER.debug(">>delta_line>>$<<", inline_response.delta_line_number)
+        POGGER.debug(">>repeat_count>>$<<", inline_response.delta_column_number)
         return inline_response
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_inline_special_character(
         special_length: int,
         inline_blocks: List[MarkdownToken],
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: str,
         source_text: str,
         next_index: int,
         para_owner: Optional[ParagraphMarkdownToken],
         remaining_line_size: int,
-    ) -> Tuple[
-        str,
-        Optional[int],
-        int,
-        Optional[str],
-        Optional[str],
-        bool,
-        Optional[MarkdownToken],
-        bool,
-        int,
-    ]:
-        (
-            preceding_two,
-            following_two,
-            is_active,
-            new_token,
-            consume_rest_of_line,
-            delta_line,
-        ) = (None, None, True, None, False, 0)
-        repeat_count: Optional[int] = 1
+        tabified_text: Optional[str],
+    ) -> Tuple[str, int, int, Any, bool, List[MarkdownToken], bool, int]:
         special_sequence = source_text[next_index : next_index + special_length]
         if special_length == 1 and special_sequence in EmphasisHelper.inline_emphasis:
-            repeat_count, new_index = ParserHelper.collect_while_character(
-                source_text, next_index, special_sequence
-            )
-            assert new_index is not None
-            special_sequence, preceding_two, following_two = (
-                source_text[next_index:new_index],
-                source_text[max(0, next_index - 2) : next_index],
-                source_text[new_index : min(len(source_text), new_index + 2)],
+            return InlineProcessor.__handle_inline_special_character_emphasis(
+                source_text,
+                next_index,
+                special_sequence,
             )
-        elif special_sequence[0] == LinkHelper.link_label_end:
-            POGGER.debug(
-                "POSSIBLE LINK CLOSE_FOUND($)>>$>>",
+        if special_sequence[0] == LinkHelper.link_label_end:
+            return InlineProcessor.__handle_inline_special_character_label_end(
                 special_length,
                 special_sequence,
-            )
-            assert repeat_count is not None
-            (
-                new_index,
-                is_active,
-                new_token,
-                consume_rest_of_line,
-                repeat_count,
-                delta_line,
-            ) = InlineProcessor.__handle_link_label_end(
                 inline_blocks,
                 remaining_line,
+                tabified_remaining_line,
                 current_string_unresolved,
                 source_text,
                 next_index,
                 para_owner,
                 remaining_line_size,
-                delta_line,
-                repeat_count,
+                tabified_text,
             )
-        else:
-            repeat_count, new_index = special_length, next_index + special_length
         return (
             special_sequence,
+            special_length,
+            next_index + special_length,
+            (None, None),
+            True,
+            [],
+            False,
+            0,
+        )
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_inline_special_character_label_end(
+        special_length: int,
+        special_sequence: str,
+        inline_blocks: List[MarkdownToken],
+        remaining_line: str,
+        tabified_remaining_line: Optional[str],
+        current_string_unresolved: str,
+        source_text: str,
+        next_index: int,
+        para_owner: Optional[ParagraphMarkdownToken],
+        remaining_line_size: int,
+        tabified_text: Optional[str],
+    ) -> Tuple[str, int, int, Any, bool, List[MarkdownToken], bool, int]:
+        POGGER.debug(
+            "POSSIBLE LINK CLOSE_FOUND($)>>$>>",
+            special_length,
+            special_sequence,
+        )
+        return InlineProcessor.__handle_link_label_end(
+            inline_blocks,
+            remaining_line,
+            tabified_remaining_line,
+            current_string_unresolved,
+            source_text,
+            next_index,
+            para_owner,
+            remaining_line_size,
+            0,
+            tabified_text,
+            special_sequence,
+        )
+
+    # pylint: enable=too-many-arguments
+
+    @staticmethod
+    def __handle_inline_special_character_emphasis(
+        source_text: str,
+        next_index: int,
+        special_sequence: str,
+    ) -> Tuple[str, int, int, Any, bool, List[MarkdownToken], bool, int]:
+        repeat_count, new_index = ParserHelper.collect_while_character(
+            source_text, next_index, special_sequence
+        )
+        assert new_index is not None
+        assert repeat_count is not None
+        return (
+            source_text[next_index:new_index],
             repeat_count,
             new_index,
-            preceding_two,
-            following_two,
-            is_active,
-            new_token,
-            consume_rest_of_line,
-            delta_line,
+            (
+                source_text[max(0, next_index - 2) : next_index],
+                source_text[new_index : min(len(source_text), new_index + 2)],
+            ),
+            True,
+            [],
+            False,
+            0,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
-
     # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __handle_link_label_end(
         inline_blocks: List[MarkdownToken],
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: str,
         source_text: str,
         next_index: int,
         para_owner: Optional[ParagraphMarkdownToken],
         remaining_line_size: int,
         delta_line: int,
-        repeat_count: int,
-    ) -> Tuple[int, bool, Optional[MarkdownToken], bool, int, int]:
+        tabified_text: Optional[str],
+        special_sequence: str,
+    ) -> Tuple[str, int, int, Any, bool, List[MarkdownToken], bool, int]:
         POGGER.debug(
             ">>inline_blocks>>$<<",
             inline_blocks,
         )
         POGGER.debug(
             ">>remaining_line>>$<<",
             remaining_line,
         )
         POGGER.debug(
+            ">>tabified_remaining_line>>$<<",
+            tabified_remaining_line,
+        )
+        POGGER.debug(
             ">>current_string_unresolved>>$<<",
             current_string_unresolved,
         )
         POGGER.debug(
-            ">>source_text>>$<<",
+            ">>source_text[next_index=$:]>:$:<",
+            next_index,
             source_text[next_index:],
         )
+        POGGER.debug(
+            ">>source_text>:$:<",
+            source_text,
+        )
+        POGGER.debug(
+            ">>tabified_text>>$<<",
+            tabified_text,
+        )
         POGGER.debug("")
         old_inline_blocks_count, old_inline_blocks_last_token = (
             len(inline_blocks),
             inline_blocks[-1] if inline_blocks else None,
         )
+
         (
             new_index,
             is_active,
             new_token,
             consume_rest_of_line,
         ) = LinkHelper.look_for_link_or_image(
             inline_blocks,
             source_text,
             next_index,
             remaining_line,
+            tabified_remaining_line,
             current_string_unresolved,
             InlineProcessor.__process_simple_inline_fn,
+            tabified_text,
         )
         POGGER.debug(">>next_index>>$<<", next_index)
         POGGER.debug(">>new_index>>$<<", new_index)
         POGGER.debug(
             ">>source_text:new_index>>$<<",
             source_text[new_index:],
         )
         POGGER.debug(">>inline_blocks>>$<<", inline_blocks)
         POGGER.debug(">>new_token>>$<<", new_token)
         POGGER.debug(">>source_text>>$<<", source_text[new_index:])
         POGGER.debug(">>consume_rest_of_line>>$<<", consume_rest_of_line)
         POGGER.debug(">>old_inline_blocks_count>>$<<", old_inline_blocks_count)
 
+        return InlineProcessor.__handle_link_label_end_calc(
+            delta_line,
+            new_token,
+            inline_blocks,
+            new_index,
+            next_index,
+            remaining_line_size,
+            para_owner,
+            old_inline_blocks_count,
+            old_inline_blocks_last_token,
+            is_active,
+            consume_rest_of_line,
+            special_sequence,
+        )
+
+    # pylint: enable=too-many-arguments, too-many-locals
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_link_label_end_calc(
+        delta_line: int,
+        new_token: Optional[MarkdownToken],
+        inline_blocks: List[MarkdownToken],
+        new_index: int,
+        next_index: int,
+        remaining_line_size: int,
+        para_owner: Optional[ParagraphMarkdownToken],
+        old_inline_blocks_count: int,
+        old_inline_blocks_last_token: Optional[MarkdownToken],
+        is_active: bool,
+        consume_rest_of_line: bool,
+        special_sequence: str,
+    ) -> Tuple[str, int, int, Any, bool, List[MarkdownToken], bool, int]:
+        repeat_count = 1
         new_inline_blocks_count = len(inline_blocks)
         POGGER.debug(">>new_inline_blocks_count>>$<<", new_inline_blocks_count)
-
         if (
             new_token
             or old_inline_blocks_count != new_inline_blocks_count
             or (inline_blocks and old_inline_blocks_last_token != inline_blocks[-1])
         ):
             (
                 delta_line,
@@ -665,36 +760,37 @@
                 new_index,
                 next_index,
                 remaining_line_size,
                 para_owner,
                 delta_line,
             )
         return (
+            special_sequence,
+            repeat_count,
             new_index,
+            (None, None),
             is_active,
-            new_token,
+            [new_token] if new_token else [],
             consume_rest_of_line,
-            repeat_count,
             delta_line,
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __calculate_repeat_count_and_delta_line(
         inline_blocks: List[MarkdownToken],
         new_token: Optional[MarkdownToken],
         new_index: int,
         next_index: int,
         remaining_line_size: int,
         para_owner: Optional[ParagraphMarkdownToken],
         delta_line: int,
     ) -> Tuple[int, int]:
-
         if inline_blocks[-1].is_inline_image:
             repeat_count = (new_index - next_index) + remaining_line_size
             (
                 delta_line,
                 repeat_count,
             ) = InlineProcessor.__calculate_link_and_image_deltas(
                 para_owner, inline_blocks[-1], delta_line, repeat_count
@@ -918,15 +1014,14 @@
         delta_line: int,
         repeat_count: int,
         para_owner: Optional[ParagraphMarkdownToken],
         split_paragraph_lines: Optional[List[str]],
         link_part_lengths: List[int],
         last_spaces: str,
     ) -> Tuple[int, int]:
-
         POGGER.debug(">>link_part_index>>$<<", link_part_index)
         POGGER.debug(">>total_newlines>>$<<", total_newlines)
         POGGER.debug(">>delta_line>>$<<", delta_line)
 
         if para_owner:
             POGGER.debug(
                 ">>para_owner.rehydrate_index>>$<<", para_owner.rehydrate_index
@@ -951,15 +1046,14 @@
             POGGER.debug(">>repeat_count>>$<<", delta_line)
         return delta_line, repeat_count
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
     def __calculate_inline_label(current_token: MarkdownToken) -> Tuple[int, int]:
-
         reference_token = cast(ReferenceMarkdownToken, current_token)
         total_newlines = ParserHelper.count_newlines_in_text(
             reference_token.text_from_blocks
         )
         link_part_index = -1 if total_newlines else -2
         return link_part_index, total_newlines
 
@@ -1061,15 +1155,15 @@
                 ) = InlineProcessor.__calculate_shortcut_collapsed_deltas(
                     reference_token, delta_line, repeat_count
                 )
 
         POGGER.debug(">>delta_line>>$<<repeat_count>>$<<", delta_line, repeat_count)
         return delta_line, repeat_count
 
-    # pylint: disable=too-many-locals, too-many-arguments
+    # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod  # noqa: C901
     def __process_inline_text_block(  # noqa: C901
         source_text: str,
         coalesced_stack: List[MarkdownToken],
         starting_whitespace: str = "",
         whitespace_to_recombine: Optional[str] = None,
         is_setext: bool = False,
@@ -1094,24 +1188,22 @@
             current_string_unresolved,
         ) = (line_number, column_number, "", "")
         start_index: Optional[int] = 0
         inline_blocks: List[MarkdownToken] = []
         end_string: Optional[str] = ""
         fold_space: Optional[List[str]] = None
 
-        # POGGER.debug(
-        #    "__process_inline_text_block>>source_text>>$>",
-        #    source_text,
-        # )
+        # POGGER.debug("source_text>:$:<", source_text)
+        # POGGER.debug("tabified_text>:$:<", tabified_text)
         # POGGER.debug(
         #    "__process_inline_text_block>>starting_whitespace>>$>",
         #    starting_whitespace,
         # )
         # POGGER.debug(
-        #     "__process_inline_text_block>>whitespace_to_recombine>>$>",
+        #     "__process_inline_text_block>>whitespace_to_recombine>:$:<",
         #     whitespace_to_recombine,
         # )
         # POGGER.debug(
         #     "__process_inline_text_block>>line_number>>$>",
         #     line_number,
         # )
         # POGGER.debug(
@@ -1143,22 +1235,23 @@
         # POGGER.debug("look>$<", source_text[start_index:])
         assert start_index is not None
         next_index = ParserHelper.index_any_of(
             source_text,
             InlineProcessor.__valid_inline_text_block_sequence_starts,
             start_index,
         )
+        newlines_encountered = 0
+        # POGGER.debug("newlines_encountered>$<", newlines_encountered)
         # POGGER.debug("__process_inline_text_block>>is_setext>>$", is_setext)
         # POGGER.debug(
         #     "__process_inline_text_block>>$>>$",
         #     source_text,
         #     start_index,
         # )
         while next_index != -1:
-
             # POGGER.debug(
             #     "\n\n>>Token_start>>$,$<<",
             #     last_line_number,
             #     last_column_number,
             # )
             # POGGER.debug("line_number>>$>",line_number)
             # POGGER.debug("column_number>>$>", column_number)
@@ -1169,14 +1262,16 @@
             # POGGER.debug(">>end_string>>$<<", end_string)
             # POGGER.debug(
             #     ">>source_text[]>>$<<$<<",
             #     source_text[next_index],
             #     source_text[next_index:],
             # )
 
+            old_next_index = next_index
+            assert start_index is not None
             (
                 line_number,
                 column_number,
                 end_string,
                 current_string,
                 current_string_unresolved,
                 starting_whitespace,
@@ -1200,40 +1295,116 @@
                 is_setext,
                 whitespace_to_recombine,
                 starting_whitespace,
                 last_line_number,
                 last_column_number,
                 fold_space,
                 tabified_text,
+                newlines_encountered,
             )
+            # POGGER.debug("old_next_index>$<", old_next_index)
+            # POGGER.debug("source_text>:$:<", source_text)
+            # POGGER.debug("source_text[]>:$:<", source_text[old_next_index])
+            # POGGER.debug("newlines_encountered>$<", newlines_encountered)
+            if source_text[old_next_index] == "\n":
+                newlines_encountered += 1
+            # POGGER.debug("newlines_encountered>$<", newlines_encountered)
 
         # POGGER.debug("<<__complete_inline_block_processing<<")
         # POGGER.debug(
         #     "<<__complete_inline_block_processing<<end_string<<$<<",
         #     end_string,
         # )
+
         return InlineProcessor.__complete_inline_block_processing(
             inline_blocks,
             source_text,
             start_index,
             current_string,
             end_string,
             starting_whitespace,
             is_setext,
-            line_number=last_line_number,
-            column_number=last_column_number,
+            last_line_number,
+            last_column_number,
+            tabified_text,
+            newlines_encountered,
         )
 
-    # pylint: enable=too-many-locals, too-many-arguments
+    # pylint: enable=too-many-arguments, too-many-locals
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_next_inline_character_setup(
+        source_text: str,
+        start_index: int,
+        next_index: int,
+        inline_blocks: List[MarkdownToken],
+        tabified_text: Optional[str],
+        newlines_encountered: int,
+        current_string_unresolved: str,
+        line_number: int,
+        column_number: int,
+        para_owner: Optional[ParagraphMarkdownToken],
+    ) -> Tuple[bool, str, int, Optional[MarkdownToken], Optional[str], InlineRequest]:
+        (
+            remaining_line,
+            old_inline_blocks_count,
+            old_inline_blocks_last_token,
+        ) = (
+            source_text[start_index:next_index],
+            len(inline_blocks),
+            inline_blocks[-1] if inline_blocks else None,
+        )
+        # POGGER.debug("__process_inline_text_block>>$,$", start_index, next_index)
+        # POGGER.debug("__process_inline_text_block>:$:<", remaining_line)
+        # POGGER.debug("so far>:$:<", source_text[start_index:])
+        # POGGER.debug("newlines_encountered>:$:<", newlines_encountered)
+        tabified_remaining_line: Optional[str] = None
+        # POGGER.debug("tabified_text>:$:<", tabified_text)
+        if tabified_text:
+            # POGGER.debug("char>:$:<", source_text[next_index])
+            tabified_remaining_line = (
+                InlineProcessor.__handle_next_inline_character_tabified(
+                    source_text,
+                    tabified_text,
+                    newlines_encountered,
+                    start_index,
+                    next_index,
+                )
+            )
+            # POGGER.debug("tabified_remaining_line>:$:<", tabified_remaining_line)
+
+        inline_request = InlineRequest(
+            source_text,
+            next_index,
+            inline_blocks,
+            remaining_line,
+            tabified_remaining_line,
+            current_string_unresolved,
+            line_number,
+            column_number,
+            para_owner,
+            tabified_text,
+        )
+        return (
+            False,
+            remaining_line,
+            old_inline_blocks_count,
+            old_inline_blocks_last_token,
+            tabified_remaining_line,
+            inline_request,
+        )
+
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __handle_next_inline_character(
         source_text: str,
-        start_index: Optional[int],
+        start_index: int,
         next_index: int,
         inline_blocks: List[MarkdownToken],
         current_string: str,
         current_string_unresolved: str,
         line_number: int,
         column_number: int,
         para_owner: Optional[ParagraphMarkdownToken],
@@ -1242,66 +1413,64 @@
         is_setext: bool,
         whitespace_to_recombine: Optional[str],
         starting_whitespace: str,
         last_line_number: int,
         last_column_number: int,
         fold_space: Optional[List[str]],
         tabified_text: Optional[str],
+        newlines_encountered: int,
     ) -> Tuple[
         int,
         int,
         Optional[str],
         str,
         str,
         str,
         Optional[List[str]],
         int,
         int,
         Optional[int],
         int,
     ]:
-
         (
             reset_current_string,
             remaining_line,
             old_inline_blocks_count,
             old_inline_blocks_last_token,
-        ) = (
-            False,
-            source_text[start_index:next_index],
-            len(inline_blocks),
-            inline_blocks[-1] if inline_blocks else None,
-        )
-
-        # POGGER.debug("__process_inline_text_block>>$>>$", start_index, next_index)
-        # POGGER.debug(
-        #     "__process_inline_text_block>>$<<", source_text[start_index:next_index]
-        # )
-        inline_request = InlineRequest(
+            tabified_remaining_line,
+            inline_request,
+        ) = InlineProcessor.__handle_next_inline_character_setup(
             source_text,
+            start_index,
             next_index,
             inline_blocks,
-            remaining_line,
+            tabified_text,
+            newlines_encountered,
             current_string_unresolved,
             line_number,
             column_number,
             para_owner,
-            tabified_text,
         )
+
+        # POGGER.debug("current_string>:$:<", current_string)
+        # POGGER.debug("remaining_line>:$:<", remaining_line)
+        # POGGER.debug("tabified_remaining_line>:$:<", tabified_remaining_line)
+
         (
             inline_response,
             line_number,
             column_number,
             was_column_number_reset,
             did_line_number_change,
             whitespace_to_add,
             remaining_line,
             end_string,
             current_string,
             was_new_line,
+            tabified_remaining_line,
         ) = InlineProcessor.__handle_next_special_character(
             source_text,
             next_index,
             inline_request,
             line_number,
             column_number,
             coalesced_stack,
@@ -1310,31 +1479,41 @@
             end_string,
             current_string,
             inline_blocks,
             is_setext,
             whitespace_to_recombine,
             para_owner,
             tabified_text,
+            tabified_remaining_line,
         )
 
+        # POGGER.debug("current_string>:$:<", current_string)
+        # POGGER.debug("remaining_line>:$:<", remaining_line)
+        # POGGER.debug("tabified_remaining_line>:$:<", tabified_remaining_line)
+
         (
             reset_current_string,
             remaining_line,
             end_string,
             current_string,
             current_string_unresolved,
         ) = InlineProcessor.__cleanup_after_handling(
             inline_response,
             current_string,
             current_string_unresolved,
             remaining_line,
+            tabified_remaining_line,
             reset_current_string,
             end_string,
         )
 
+        # POGGER.debug("current_string>:$:<", current_string)
+        # POGGER.debug("remaining_line>:$:<", remaining_line)
+        # POGGER.debug("tabified_remaining_line>:$:<", tabified_remaining_line)
+
         (
             reset_current_string,
             starting_whitespace,
             end_string,
         ) = InlineProcessor.__create_new_text_token(
             inline_response,
             current_string,
@@ -1346,25 +1525,112 @@
             reset_current_string,
         )
 
         (
             line_number,
             column_number,
             fold_space,
+            current_string,
+            current_string_unresolved,
+            last_line_number,
+            last_column_number,
+            new_start_index,
+            next_index,
+            end_string,
+        ) = InlineProcessor.__handle_next_inline_character_finish_handling(
+            line_number,
+            column_number,
+            fold_space,
+            was_new_line,
+            coalesced_stack,
+            remaining_line,
+            did_line_number_change,
+            was_column_number_reset,
+            reset_current_string,
+            inline_blocks,
+            old_inline_blocks_count,
+            old_inline_blocks_last_token,
+            source_text,
+            whitespace_to_add,
+            inline_response,
+            current_string,
+            current_string_unresolved,
+            last_line_number,
+            last_column_number,
+            end_string,
+        )
+
+        # POGGER.debug("current_string>:$:<", current_string)
+        return (
+            line_number,
+            column_number,
+            end_string,
+            current_string,
+            current_string_unresolved,
+            starting_whitespace,
+            fold_space,
+            last_line_number,
+            last_column_number,
+            new_start_index,
+            next_index,
+        )
+
+    # pylint: enable=too-many-arguments, too-many-locals
+
+    # pylint: disable=too-many-arguments, too-many-locals
+    @staticmethod
+    def __handle_next_inline_character_finish_handling(
+        line_number: int,
+        column_number: int,
+        fold_space: Optional[List[str]],
+        was_new_line: bool,
+        coalesced_stack: List[MarkdownToken],
+        remaining_line: str,
+        did_line_number_change: bool,
+        was_column_number_reset: bool,
+        reset_current_string: bool,
+        inline_blocks: List[MarkdownToken],
+        old_inline_blocks_count: int,
+        old_inline_blocks_last_token: Optional[MarkdownToken],
+        source_text: str,
+        whitespace_to_add: Optional[str],
+        inline_response: InlineResponse,
+        current_string: str,
+        current_string_unresolved: str,
+        last_line_number: int,
+        last_column_number: int,
+        end_string: Optional[str],
+    ) -> Tuple[
+        int,
+        int,
+        Optional[List[str]],
+        str,
+        str,
+        int,
+        int,
+        Optional[int],
+        int,
+        Optional[str],
+    ]:
+        (
+            line_number,
+            column_number,
+            fold_space,
         ) = InlineProcessor.__adjust_line_and_column_number(
             was_new_line,
             coalesced_stack,
             line_number,
             column_number,
             fold_space,
             remaining_line,
             did_line_number_change,
             was_column_number_reset,
         )
 
+        # POGGER.debug("current_string>:$:<", current_string)
         (
             current_string,
             current_string_unresolved,
             last_line_number,
             last_column_number,
         ) = InlineProcessor.__fix_variables_before_next_loop(
             reset_current_string,
@@ -1375,14 +1641,15 @@
             old_inline_blocks_last_token,
             last_line_number,
             last_column_number,
             line_number,
             column_number,
         )
 
+        # POGGER.debug("current_string>:$:<", current_string)
         (
             new_start_index,
             next_index,
             end_string,
             current_string,
             current_string_unresolved,
         ) = InlineProcessor.__complete_inline_loop(
@@ -1395,27 +1662,270 @@
             inline_response.new_string_unresolved,
             inline_response.new_string,
             inline_response.original_string,
         )
         return (
             line_number,
             column_number,
-            end_string,
+            fold_space,
             current_string,
             current_string_unresolved,
-            starting_whitespace,
-            fold_space,
             last_line_number,
             last_column_number,
             new_start_index,
             next_index,
+            end_string,
         )
 
     # pylint: enable=too-many-arguments, too-many-locals
 
+    @staticmethod
+    def __xdg(tabified_text: str, newlines_encountered: int) -> Tuple[str, int]:
+        line_start_index = 0
+        for _ in range(newlines_encountered):
+            line_end_index = tabified_text.find("\n", line_start_index)
+            line_start_index = line_end_index + 1
+        POGGER.debug("line_start_index>:$:<", line_start_index)
+        line_end_index = tabified_text.find("\n", line_start_index)
+        return (
+            tabified_text[line_start_index:line_end_index]
+            if line_end_index != -1
+            else tabified_text[line_start_index:],
+            line_start_index,
+        )
+
+    @staticmethod
+    def __handle_next_inline_character_tabified(
+        source_text: str,
+        tabified_text: str,
+        newlines_encountered: int,
+        start_index: int,
+        next_index: int,
+    ) -> Optional[str]:
+        adj_tabified_text, _ = InlineProcessor.__xdg(
+            tabified_text, newlines_encountered
+        )
+        POGGER.debug("adj_tabified_text>:$:<", adj_tabified_text)
+
+        _, line_start_index = InlineProcessor.__xdg(source_text, newlines_encountered)
+        # POGGER.debug("adj_source_text>:$:<", adj_source_text)
+
+        current_line_source_text = source_text[start_index:next_index]
+        POGGER.debug("source_text>:$:<", source_text)
+        POGGER.debug("current_line_source_text>:$:<", current_line_source_text)
+
+        stop_character = source_text[next_index]
+        if stop_character == "\n":
+            ex_original_line, _ = TabHelper.find_detabify_string_ex(
+                adj_tabified_text, current_line_source_text
+            )
+            assert ex_original_line is not None
+            return ex_original_line
+
+        POGGER.debug("stop_character>:$:<", stop_character)
+
+        stop_character_in_tabified_index = (
+            InlineProcessor.__handle_next_inline_character_tabified_find_stop(
+                adj_tabified_text,
+                stop_character,
+                source_text,
+                line_start_index,
+                next_index,
+            )
+        )
+
+        (
+            current_line_leading_space_index,
+            current_line_leading_space,
+        ) = ParserHelper.extract_spaces(current_line_source_text, 0)
+        POGGER.debug(
+            "current_line_leading_space_index>:$:<, current_line_leading_space>:$:<",
+            current_line_leading_space_index,
+            current_line_leading_space,
+        )
+        assert current_line_leading_space_index is not None
+
+        return InlineProcessor.__handle_next_inline_character_tabified_cleanup(
+            current_line_source_text,
+            current_line_leading_space_index,
+            stop_character,
+            adj_tabified_text,
+            stop_character_in_tabified_index,
+            current_line_leading_space,
+        )
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_next_inline_character_tabified_cleanup(
+        current_line_source_text: str,
+        current_line_leading_space_index: int,
+        stop_character: str,
+        adj_tabified_text: str,
+        stop_character_in_tabified_index: int,
+        current_line_leading_space: Optional[str],
+    ) -> str:
+        (
+            current_line_first_word_index,
+            current_line_first_word,
+        ) = ParserHelper.collect_until_one_of_characters(
+            current_line_source_text,
+            current_line_leading_space_index,
+            " \t" + stop_character,
+        )
+        POGGER.debug(
+            "current_line_first_word_index>:$:<, current_line_first_word>:$:<",
+            current_line_first_word_index,
+            current_line_first_word,
+        )
+
+        if current_line_leading_space_index == current_line_first_word_index:
+            tabified_start_index, _ = ParserHelper.extract_spaces_from_end(
+                adj_tabified_text, stop_character_in_tabified_index
+            )
+        else:
+            assert current_line_first_word is not None
+            tabified_start_index = InlineProcessor.__pdff(
+                current_line_source_text,
+                current_line_first_word,
+                current_line_leading_space_index,
+                adj_tabified_text,
+                stop_character_in_tabified_index,
+                current_line_leading_space,
+            )
+        return adj_tabified_text[tabified_start_index:stop_character_in_tabified_index]
+
+    # pylint: enable=too-many-arguments
+
+    @staticmethod
+    def __handle_next_inline_character_tabified_find_stop(
+        adj_tabified_text: str,
+        stop_character: str,
+        source_text: str,
+        line_start_index: int,
+        next_index: int,
+    ) -> int:
+        found_in_source_text_count = 0
+        found_in_source_text_index = source_text.find(stop_character, line_start_index)
+        POGGER.debug(
+            "source_text[$]>:$:<",
+            found_in_source_text_index,
+            source_text[found_in_source_text_index:],
+        )
+        while found_in_source_text_index != next_index:
+            found_in_source_text_count += 1
+            found_in_source_text_index = source_text.find(
+                stop_character, found_in_source_text_index + 1
+            )
+            POGGER.debug(
+                "source_text[$]>:$:<",
+                found_in_source_text_index,
+                source_text[found_in_source_text_index:],
+            )
+        POGGER.debug("found_in_source_text_count>:$:<", found_in_source_text_count)
+        POGGER.debug(
+            "source_text[$]>:$:<",
+            found_in_source_text_index,
+            source_text[found_in_source_text_index:],
+        )
+
+        found_in_tabified_text_count = 0
+        stop_character_in_tabified_index = adj_tabified_text.find(stop_character)
+        POGGER.debug(
+            "adj_tabified_text[$]>:$:<",
+            stop_character_in_tabified_index,
+            adj_tabified_text[stop_character_in_tabified_index:],
+        )
+        while found_in_tabified_text_count != found_in_source_text_count:
+            found_in_tabified_text_count += 1
+            stop_character_in_tabified_index = adj_tabified_text.find(
+                stop_character, stop_character_in_tabified_index + 1
+            )
+            POGGER.debug(
+                "adj_tabified_text[$]>:$:<",
+                stop_character_in_tabified_index,
+                adj_tabified_text[stop_character_in_tabified_index:],
+            )
+            assert stop_character_in_tabified_index != -1
+        POGGER.debug("found_in_tabified_text_count>:$:<", found_in_tabified_text_count)
+        POGGER.debug(
+            "adj_tabified_text[$]>:$:<",
+            stop_character_in_tabified_index,
+            adj_tabified_text[stop_character_in_tabified_index:],
+        )
+        assert adj_tabified_text[stop_character_in_tabified_index] == stop_character
+        return stop_character_in_tabified_index
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __pdff(
+        current_line_source_text: str,
+        current_line_first_word: str,
+        current_line_leading_space_index: Optional[int],
+        adj_tabified_text: str,
+        stop_character_in_tabified_index: int,
+        current_line_leading_space: Optional[str],
+    ) -> int:
+        first_word_index = current_line_source_text.rfind(current_line_first_word)
+        POGGER.debug("first_word_index>:$:<", first_word_index)
+        first_word_count = 0
+        while (
+            first_word_index != current_line_leading_space_index
+            and first_word_index > 0
+        ):
+            first_word_index = current_line_source_text.rfind(
+                current_line_first_word, 0, first_word_index - 1
+            )
+            POGGER.debug("first_word_index>:$:<", first_word_index)
+            first_word_count += 1
+        POGGER.debug("first_word_count>:$:<", first_word_count)
+        assert first_word_index == current_line_leading_space_index
+
+        tabified_start_index = adj_tabified_text.rfind(
+            current_line_first_word, 0, stop_character_in_tabified_index
+        )
+        POGGER.debug(
+            "tabified_start_index=$,stop=$..>:$:<",
+            tabified_start_index,
+            stop_character_in_tabified_index,
+            adj_tabified_text[tabified_start_index:stop_character_in_tabified_index],
+        )
+        for _ in range(first_word_count):
+            tabified_start_index = adj_tabified_text.rfind(
+                current_line_first_word, 0, tabified_start_index - 1
+            )
+            POGGER.debug(
+                "tabified_start_index=$,stop=$..>:$:<",
+                tabified_start_index,
+                stop_character_in_tabified_index,
+                adj_tabified_text[
+                    tabified_start_index:stop_character_in_tabified_index
+                ],
+            )
+            assert tabified_start_index <= stop_character_in_tabified_index
+
+        if current_line_leading_space:
+            POGGER.debug(
+                "adj_tabified_text[$:]>:$:<",
+                tabified_start_index,
+                adj_tabified_text[tabified_start_index:],
+            )
+            tabified_start_index, _ = ParserHelper.extract_spaces_from_end(
+                adj_tabified_text, tabified_start_index
+            )
+            POGGER.debug(
+                "adj_tabified_text[$:]>:$:<",
+                tabified_start_index,
+                adj_tabified_text[tabified_start_index:],
+            )
+
+        assert tabified_start_index is not None
+        return tabified_start_index
+
+    # pylint: enable=too-many-arguments
+
     # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __handle_next_special_character(
         source_text: str,
         next_index: int,
         inline_request: InlineRequest,
         line_number: int,
@@ -1426,27 +1936,28 @@
         end_string: Optional[str],
         current_string: str,
         inline_blocks: List[MarkdownToken],
         is_setext: bool,
         whitespace_to_recombine: Optional[str],
         para_owner: Optional[ParagraphMarkdownToken],
         tabified_text: Optional[str],
+        tabified_remaining_line: Optional[str],
     ) -> Tuple[
         InlineResponse,
         int,
         int,
         bool,
         bool,
         Optional[str],
         str,
         Optional[str],
         str,
         bool,
+        Optional[str],
     ]:
-
         if source_text[next_index] in InlineProcessor.__inline_character_handlers:
             whitespace_to_add, was_new_line = None, False
             (
                 inline_response,
                 line_number,
                 column_number,
                 was_column_number_reset,
@@ -1463,14 +1974,15 @@
             was_column_number_reset, did_line_number_change = False, False
             (
                 whitespace_to_add,
                 remaining_line,
                 end_string,
                 current_string,
                 was_new_line,
+                tabified_remaining_line,
             ) = InlineProcessor.__process_inline_new_line(
                 source_text,
                 next_index,
                 inline_response,
                 remaining_line,
                 end_string,
                 current_string,
@@ -1478,37 +1990,41 @@
                 is_setext,
                 line_number,
                 column_number,
                 coalesced_stack,
                 whitespace_to_recombine,
                 para_owner,
                 tabified_text,
+                inline_request,
+                tabified_remaining_line,
             )
         return (
             inline_response,
             line_number,
             column_number,
             was_column_number_reset,
             did_line_number_change,
             whitespace_to_add,
             remaining_line,
             end_string,
             current_string,
             was_new_line,
+            tabified_remaining_line,
         )
 
     # pylint: enable=too-many-arguments, too-many-locals
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __cleanup_after_handling(
         inline_response: InlineResponse,
         current_string: str,
         current_string_unresolved: str,
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         reset_current_string: bool,
         end_string: Optional[str],
     ) -> Tuple[bool, str, Optional[str], str, str]:
         # POGGER.debug(
         #     "new_string-->$<--",
         #     inline_response.new_string,
         # )
@@ -1545,20 +2061,23 @@
             # )
         else:
             # POGGER.debug("append_rest_of_line>>rem>>$<", remaining_line)
             # POGGER.debug("append_rest_of_line>>cur>>$<", current_string)
             # POGGER.debug(
             #     "append_rest_of_line>>cur_un>>$<", current_string_unresolved
             # )
+            proper_remaining_line = tabified_remaining_line or remaining_line
             current_string, current_string_unresolved = (
                 InlineHelper.append_text(
                     current_string,
-                    remaining_line,
+                    proper_remaining_line,
+                ),
+                InlineHelper.append_text(
+                    current_string_unresolved, proper_remaining_line
                 ),
-                InlineHelper.append_text(current_string_unresolved, remaining_line),
             )
         return (
             reset_current_string,
             remaining_line,
             end_string,
             current_string,
             current_string_unresolved,
@@ -1643,16 +2162,16 @@
             column_number = 1
             if coalesced_stack and coalesced_stack[-1].is_block_quote_start:
                 block_quote_token = cast(BlockQuoteMarkdownToken, coalesced_stack[-1])
                 POGGER.debug(
                     "coalesced_list[-1]..leading_text_index=$",
                     block_quote_token.leading_text_index,
                 )
-                assert block_quote_token.leading_spaces is not None
-                split_leading_spaces = block_quote_token.leading_spaces.split(
+                assert block_quote_token.bleading_spaces is not None
+                split_leading_spaces = block_quote_token.bleading_spaces.split(
                     ParserHelper.newline_character
                 )
                 selected_split_length = len(
                     split_leading_spaces[block_quote_token.leading_text_index]
                 )
                 # POGGER.debug("l/c(before)>>newline-->$", selected_split_length)
                 column_number += selected_split_length
@@ -1669,16 +2188,16 @@
             assert did_line_number_change
             if coalesced_stack and coalesced_stack[-1].is_block_quote_start:
                 block_quote_token = cast(BlockQuoteMarkdownToken, coalesced_stack[-1])
                 POGGER.debug(
                     "coalesced_list[-1].leading_text_index=$",
                     block_quote_token.leading_text_index,
                 )
-                assert block_quote_token.leading_spaces is not None
-                split_leading_spaces = block_quote_token.leading_spaces.split(
+                assert block_quote_token.bleading_spaces is not None
+                split_leading_spaces = block_quote_token.bleading_spaces.split(
                     ParserHelper.newline_character
                 )
                 selected_split_length = len(
                     split_leading_spaces[block_quote_token.leading_text_index]
                 )
                 # POGGER.debug("l/c(before)>>newline-->$", selected_split_length)
                 column_number += selected_split_length
@@ -1835,15 +2354,15 @@
             column_number,
             was_column_number_reset,
             did_line_number_change,
         )
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments
+    # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __process_inline_new_line(
         source_text: str,
         next_index: int,
         inline_response: InlineResponse,
         remaining_line: str,
         end_string: Optional[str],
@@ -1852,41 +2371,49 @@
         is_setext: bool,
         line_number: int,
         column_number: int,
         coalesced_stack: List[MarkdownToken],
         whitespace_to_recombine: Optional[str],
         para_owner: Optional[ParagraphMarkdownToken],
         tabified_text: Optional[str],
-    ) -> Tuple[Optional[str], str, Optional[str], str, bool]:
-
+        inline_request: InlineRequest,
+        tabified_remaining_line: Optional[str],
+    ) -> Tuple[Optional[str], str, Optional[str], str, bool, Optional[str]]:
         assert source_text[next_index] == ParserHelper.newline_character
+        # POGGER.debug("end_string>:$:<", end_string)
+        # POGGER.debug("remaining_line>:$:<", remaining_line)
+        # POGGER.debug("tabified_remaining_line>:$:<", tabified_remaining_line)
+        # POGGER.debug("tabified_text>:$:<", tabified_text)
         # POGGER.debug(
-        #     "end_string(before)>>$<<",
-        #     end_string,
+        #     "inline_request.tabified_remaining_line>:$:<",
+        #     inline_request.tabified_remaining_line,
         # )
         (
             inline_response.new_string,
             whitespace_to_add,
             inline_response.new_tokens,
             remaining_line,
             end_string,
             current_string,
         ) = InlineHelper.handle_line_end(
             remaining_line,
+            tabified_remaining_line,
             end_string,
             current_string,
             inline_blocks,
             is_setext,
             line_number,
             column_number,
             coalesced_stack,
             tabified_text,
+            inline_request,
         )
         inline_response.new_index = next_index + 1
-        # POGGER.debug("2<<end_string<<$<<", end_string)
+        # POGGER.debug("end_string>:$:<", end_string)
+        # POGGER.debug("remaining_line>:$:<", remaining_line)
         # POGGER.debug(
         #     "handle_line_end>>new_tokens>>$<<",
         #     inline_response.new_tokens,
         # )
 
         if not inline_response.new_tokens:
             # POGGER.debug("ws")
@@ -1911,33 +2438,75 @@
         # )
         # POGGER.debug(">>line_number>>$<<", line_number)
         # POGGER.debug(">>column_number>>$<<", column_number)
         if para_owner:
             # POGGER.debug(">>para_owner.rehydrate_index>>$<<", para_owner.rehydrate_index)
             para_owner.rehydrate_index += 1
             # POGGER.debug(">>para_owner.rehydrate_index>>$<<", para_owner.rehydrate_index)
+
+        if tabified_remaining_line and end_string and len(end_string) > 1:
+            assert end_string is not None
+            tabified_remaining_line = InlineProcessor.__clean_up_new_line(
+                end_string, is_setext, tabified_remaining_line
+            )
+
         return (
             whitespace_to_add,
             remaining_line,
             end_string,
             current_string,
             True,
+            tabified_remaining_line,
         )
 
-    # pylint: enable=too-many-arguments
+    # pylint: enable=too-many-arguments, too-many-locals
+
+    @staticmethod
+    def __clean_up_new_line(
+        end_string: str, is_setext: bool, tabified_remaining_line: str
+    ) -> str:
+        POGGER.debug("end_string>$<", end_string)
+        POGGER.debug("tabified_remaining_line>$<", tabified_remaining_line)
+        assert end_string[-1] in ["\n", ParserHelper.whitespace_split_character]
+        if end_string[-1] == ParserHelper.whitespace_split_character:
+            newline_index = end_string.rfind("\n")
+            assert newline_index != -1
+            end_suffix = end_string[:newline_index]
+        else:
+            end_suffix = end_string[:-1]
+        POGGER.debug("end_suffix>$<", end_suffix)
+        newline_index = end_suffix.rfind("\n")
+        if is_setext:
+            special_index = end_suffix.rfind(ParserHelper.whitespace_split_character)
+            if special_index != -1 and newline_index != 1:
+                max_index = max(special_index, special_index)
+                end_suffix = end_suffix[max_index + 1 :]
+            else:
+                assert special_index == -1
+                assert newline_index != 1
+                end_suffix = end_suffix[newline_index + 1 :]
+        elif newline_index != -1:
+            end_suffix = end_suffix[newline_index + 1 :]
+
+        POGGER.debug("tabified_remaining_line>$<", tabified_remaining_line)
+        POGGER.debug("end_suffix>$<", end_suffix)
+        assert tabified_remaining_line.endswith(end_suffix)
+        if end_suffix:
+            tabified_remaining_line = tabified_remaining_line[: -(len(end_suffix))]
+        POGGER.debug("tabified_remaining_line>$<", tabified_remaining_line)
+        return tabified_remaining_line
 
     @staticmethod
     def __add_recombined_whitespace(
         did_recombine: bool,
         source_text: str,
         inline_response: InlineResponse,
         end_string: Optional[str],
         is_setext: bool,
     ) -> Optional[str]:
-
         POGGER.debug("__arw>>did_recombine>>$>>", did_recombine)
         POGGER.debug(
             "__arw>>end_string>>$>>",
             end_string,
         )
         if did_recombine:
             POGGER.debug(
@@ -2097,14 +2666,16 @@
         start_index: Optional[int],
         current_string: str,
         end_string: Optional[str],
         starting_whitespace: str,
         is_setext: bool,
         line_number: int,
         column_number: int,
+        tabified_text: Optional[str],
+        newlines_encountered: int,
     ) -> List[MarkdownToken]:
         POGGER.debug("__cibp>inline_blocks>$<", inline_blocks)
         POGGER.debug("__cibp>source_text>$<", source_text)
         POGGER.debug("__cibp>start_index>$<", start_index)
         POGGER.debug("__cibp>current_string>$<", current_string)
         POGGER.debug("__cibp>end_string>$<", end_string)
         POGGER.debug(
@@ -2113,25 +2684,35 @@
         )
         POGGER.debug("__cibp>is_setext>$<", is_setext)
         POGGER.debug("__cibp>line_number>$<", line_number)
         POGGER.debug("__cibp>column_number>$<", column_number)
 
         assert start_index is not None
         if start_index < len(source_text):
-            current_string = InlineHelper.append_text(
-                current_string, source_text[start_index:]
-            )
-            POGGER.debug("__cibp>current_string>$<", current_string)
+            text_to_append = source_text[start_index:]
+            POGGER.debug("text_to_append>:$:<", text_to_append)
+
+            POGGER.debug("tabified_text=>:$:<", tabified_text)
+            if tabified_text:
+                assert tabified_text is not None
+                text_to_append = (
+                    InlineProcessor.__complete_inline_block_processing_tabified(
+                        source_text, start_index, tabified_text, newlines_encountered
+                    )
+                )
+                POGGER.debug("text_to_append>:$:<", text_to_append)
+
+            POGGER.debug("current_string>:$:<", current_string)
+            POGGER.debug("text_to_append>:$:<", text_to_append)
+            current_string = InlineHelper.append_text(current_string, text_to_append)
+            POGGER.debug("current_string>:$:<", current_string)
 
         have_processed_once = len(inline_blocks) != 0 or start_index != 0
         if current_string or not have_processed_once:
-            (
-                current_string,
-                end_string,
-            ) = InlineProcessor.__complete_inline_block_processing_build_token(
+            InlineProcessor.__complete_inline_block_processing_build_token(
                 current_string,
                 end_string,
                 starting_whitespace,
                 is_setext,
                 inline_blocks,
                 line_number,
                 column_number,
@@ -2139,25 +2720,172 @@
         POGGER.debug(">>$<<", inline_blocks)
 
         EmphasisHelper.resolve_inline_emphasis(inline_blocks, None)
         return inline_blocks
 
     # pylint: enable=too-many-arguments
 
+    @staticmethod
+    def __complete_inline_block_processing_tabified(
+        source_text: str,
+        start_index: int,
+        tabified_text: str,
+        newlines_encountered: int,
+    ) -> str:
+        source_text_spaces_index, source_text_spaces = ParserHelper.extract_spaces(
+            source_text, start_index
+        )
+        POGGER.debug(
+            "source_text_spaces_index=>:$:<, source_text_spaces=>:$:<",
+            source_text_spaces_index,
+            source_text_spaces,
+        )
+        assert source_text_spaces_index is not None
+        (
+            source_text_word_index,
+            source_text_word,
+        ) = ParserHelper.collect_until_one_of_characters(
+            source_text, source_text_spaces_index, " \t"
+        )
+        POGGER.debug(
+            "source_text_word_index=>:$:<, source_text_word=>:$:<",
+            source_text_word_index,
+            source_text_word,
+        )
+        assert source_text_word is not None
+
+        current_line_source_text, current_line_start_index = InlineProcessor.__xdf(
+            source_text, newlines_encountered
+        )
+        POGGER.debug("current_line_source_text>:$:<", current_line_source_text)
+        POGGER.debug("current_line_start_index>:$:<", current_line_start_index)
+
+        find_word_count = 0
+        word_index = current_line_source_text.find(source_text_word, 0)
+        adj_word_index = word_index + current_line_start_index
+        POGGER.debug(
+            "[$]-->current_line_source_text[$:]>:$:<",
+            find_word_count,
+            word_index,
+            current_line_source_text[word_index:],
+        )
+        POGGER.debug(
+            "adj_word_index=$ != source_text_spaces_index=$",
+            adj_word_index,
+            source_text_spaces_index,
+        )
+        while adj_word_index != source_text_spaces_index:
+            find_word_count += 1
+            word_index = current_line_source_text.find(source_text_word, word_index + 1)
+            adj_word_index = word_index + current_line_start_index
+            POGGER.debug(
+                "[$]-->current_line_source_text[$:]>:$:<",
+                find_word_count,
+                word_index,
+                current_line_source_text[word_index:],
+            )
+            POGGER.debug(
+                "adj_word_index=$ != source_text_spaces_index=$",
+                adj_word_index,
+                source_text_spaces_index,
+            )
+        POGGER.debug(
+            "[$]-->current_line_source_text[$:]>:$:<",
+            find_word_count,
+            word_index,
+            current_line_source_text[word_index:],
+        )
+
+        current_line_tabified_text, _ = InlineProcessor.__xdf(
+            tabified_text, newlines_encountered
+        )
+        POGGER.debug("current_line_tabified_text>:$:<", current_line_tabified_text)
+
+        found_word_index = InlineProcessor.__calculate_word_index(
+            current_line_tabified_text,
+            source_text_word,
+            find_word_count,
+            source_text_spaces,
+        )
+        return current_line_tabified_text[found_word_index:]
+
+    @staticmethod
+    def __calculate_word_index(
+        current_line_tabified_text: str,
+        source_text_word: str,
+        find_word_count: int,
+        source_text_spaces: Optional[str],
+    ) -> int:
+        POGGER.debug("source_text_word>:$:<", source_text_word)
+        found_word_index = current_line_tabified_text.find(source_text_word)
+        POGGER.debug(
+            "[$]-->current_line_source_text[$:]>:$:<",
+            0,
+            found_word_index,
+            current_line_tabified_text[found_word_index:],
+        )
+        for found_word_count in range(find_word_count):
+            found_word_index = current_line_tabified_text.find(
+                source_text_word, found_word_index + 1
+            )
+            POGGER.debug(
+                "[$]-->current_line_source_text[$:]>:$:<",
+                found_word_count,
+                found_word_index,
+                current_line_tabified_text[found_word_index:],
+            )
+            assert found_word_index != -1
+
+        if source_text_spaces:
+            POGGER.debug(
+                "current_line_source_text[$:]>:$:<",
+                found_word_index,
+                current_line_tabified_text[found_word_index:],
+            )
+            found_word_index, _ = ParserHelper.extract_spaces_from_end(
+                current_line_tabified_text, found_word_index
+            )
+            POGGER.debug(
+                "current_line_source_text[$:]>:$:<",
+                found_word_index,
+                current_line_tabified_text[found_word_index:],
+            )
+        return found_word_index
+
+    @staticmethod
+    def __xdf(tabified_text: str, newlines_encountered: int) -> Tuple[str, int]:
+        # POGGER.debug("newlines_encountered=>:$:<", newlines_encountered)
+        # POGGER.debug("tabified_text>:$:<", tabified_text)
+        start_index = 0
+        for _ in range(newlines_encountered):
+            next_index = tabified_text.find("\n", start_index)
+            assert next_index != -1
+            start_index = next_index + 1
+        # POGGER.debug("start_index>:$:<", start_index)
+        # POGGER.debug("tabified_text[start_index:]>:$:<", tabified_text[start_index:])
+
+        next_index = tabified_text.find("\n", start_index)
+        # POGGER.debug("next_index>:$:<", next_index)
+        assert next_index == -1
+        # if next_index != -1:
+        #     start_index = next_index + 1
+
+        return tabified_text[start_index:], start_index
+
     # pylint: disable=too-many-arguments
     @staticmethod
     def __complete_inline_block_processing_build_token(
         current_string: str,
         end_string: Optional[str],
         starting_whitespace: str,
         is_setext: bool,
         inline_blocks: List[MarkdownToken],
         line_number: int,
         column_number: int,
-    ) -> Tuple[str, Optional[str]]:
+    ) -> None:
         POGGER.debug("__cibp>current_string>$<", current_string)
         POGGER.debug("__cibp>starting_whitespace>$<", starting_whitespace)
         if (
             is_setext
             and end_string is None
             and (inline_blocks and inline_blocks[-1].is_inline_hard_break)
         ):
@@ -2173,10 +2901,9 @@
                 current_string,
                 starting_whitespace,
                 end_whitespace=end_string,
                 line_number=line_number,
                 column_number=column_number,
             )
         )
-        return current_string, end_string
 
     # pylint: enable=too-many-arguments
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/inline_request.py` & `pymarkdownlnt-0.9.9/pymarkdown/inline_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Class to hold the request information to pass on to the handle_* functions.
     """
 
     source_text: str
     next_index: int
     inline_blocks: List[MarkdownToken] = field(default_factory=list)
     remaining_line: Optional[str] = None
+    tabified_remaining_line: Optional[str] = None
     current_string_unresolved: Optional[str] = None
     line_number: Optional[int] = None
     column_number: Optional[int] = None
     para_owner: Optional[ParagraphMarkdownToken] = None
     tabified_text: Optional[str] = None
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/inline_response.py` & `pymarkdownlnt-0.9.9/pymarkdown/inline_response.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/leaf_block_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/link_reference_definition_helper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1114 +1,1310 @@
 """
-Module to provide processing for the leaf blocks.
+Link reference definition helper
 """
 import logging
+from dataclasses import dataclass
 from typing import List, Optional, Tuple, cast
 
-from pymarkdown.block_quote_data import BlockQuoteData
-from pymarkdown.constants import Constants
-from pymarkdown.html_helper import HtmlHelper
+from pymarkdown.container_markdown_token import BlockQuoteMarkdownToken
 from pymarkdown.inline_helper import InlineHelper
-from pymarkdown.inline_markdown_token import TextMarkdownToken
-from pymarkdown.leaf_markdown_token import (
-    AtxHeadingMarkdownToken,
-    FencedCodeBlockMarkdownToken,
-    IndentedCodeBlockMarkdownToken,
-    ParagraphMarkdownToken,
-    SetextHeadingMarkdownToken,
-    ThematicBreakMarkdownToken,
-)
+from pymarkdown.leaf_markdown_token import LinkReferenceDefinitionMarkdownToken
+from pymarkdown.link_helper import LinkHelper
+from pymarkdown.link_reference_info import LinkReferenceInfo
+from pymarkdown.link_reference_titles import LinkReferenceTitles
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.parser_state import ParserState
 from pymarkdown.position_marker import PositionMarker
-from pymarkdown.stack_token import (
-    FencedCodeBlockStackToken,
-    IndentedCodeBlockStackToken,
-    ListStackToken,
-    ParagraphStackToken,
-    StackToken,
-)
+from pymarkdown.requeue_line_info import RequeueLineInfo
+from pymarkdown.stack_token import LinkDefinitionStackToken
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 # pylint: disable=too-many-lines
 
 
-class LeafBlockProcessor:
+@dataclass(frozen=True)
+class LinkReferenceDefinitionTuple:
     """
-    Class to provide processing for the leaf blocks.
+    Class to hold the tuple of information for creating a Link Reference Definition.
     """
 
-    __fenced_start_tilde = "~"
-    __fenced_start_backtick = "`"
-    __fenced_code_block_start_characters = (
-        f"{__fenced_start_tilde}{__fenced_start_backtick}"
-    )
-    __thematic_break_characters = "*_-"
-    __atx_character = "#"
-    __setext_characters = "-="
+    normalized_destination: Optional[str]
+    link_titles: LinkReferenceTitles
+    link_info: LinkReferenceInfo
 
-    @staticmethod
-    def is_fenced_code_block(
-        line_to_parse: str,
-        start_index: int,
-        extracted_whitespace: Optional[str],
-        skip_whitespace_check: bool = False,
-    ) -> Tuple[bool, Optional[int], Optional[int], Optional[str], Optional[int]]:
-        """
-        Determine if we have the start of a fenced code block.
-        """
 
-        assert extracted_whitespace is not None
-        after_fence_index: Optional[int] = None
-        if (
-            skip_whitespace_check
-            or ParserHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
-        ) and ParserHelper.is_character_at_index_one_of(
-            line_to_parse,
-            start_index,
-            LeafBlockProcessor.__fenced_code_block_start_characters,
-        ):
-            POGGER.debug("ifcb:collected_count>>$<<$<<", line_to_parse, start_index)
-            collected_count, new_index = ParserHelper.collect_while_character(
-                line_to_parse, start_index, line_to_parse[start_index]
-            )
-            POGGER.debug("ifcb:collected_count:$", collected_count)
-            assert collected_count is not None
-            assert new_index is not None
-            after_fence_index = new_index
-            (
-                non_whitespace_index,
-                extracted_whitespace_before_info_string,
-            ) = ParserHelper.extract_ascii_whitespace(line_to_parse, new_index)
-
-            if collected_count >= 3:
-                POGGER.debug("ifcb:True")
-                return (
-                    True,
-                    non_whitespace_index,
-                    after_fence_index,
-                    extracted_whitespace_before_info_string,
-                    collected_count,
-                )
-        return False, None, None, None, None
+class LinkReferenceDefinitionHelper:
+    """
+    Class to helper with the parsing of link reference definitions.
+    """
 
+    __lrd_start_character = "["
+
+    # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
-    def parse_fenced_code_block(
+    def process_link_reference_definition(
         parser_state: ParserState,
         position_marker: PositionMarker,
+        remaining_line_to_parse: str,
         extracted_whitespace: Optional[str],
+        unmodified_line_to_parse: str,
+        original_stack_depth: int,
+        original_document_depth: int,
         original_line: str,
-    ) -> Tuple[List[MarkdownToken], Optional[str]]:
+        process_mode: int,
+    ) -> Tuple[bool, bool, bool, Optional[RequeueLineInfo], List[MarkdownToken]]:
         """
-        Handle the parsing of a fenced code block
+        Process a link deference definition.  Note, this requires a lot of work to
+        handle properly because of partial definitions across lines.
         """
 
-        POGGER.debug(
-            "line>>$>>index>>$>>",
-            position_marker.text_to_parse,
-            position_marker.index_number,
+        line_to_parse = position_marker.text_to_parse
+        start_index: int = position_marker.index_number
+        lines_to_requeue: List[str] = []
+
+        POGGER.debug(">>remaining_line_to_parse>:$:<", remaining_line_to_parse)
+        POGGER.debug(">>line_to_parse>:$:<", line_to_parse)
+        POGGER.debug(">>start_index>:$:<", start_index)
+
+        (
+            line_to_parse,
+            unmodified_line_to_parse,
+            remaining_line_to_parse,
+            start_index,
+            is_blank_line,
+        ) = LinkReferenceDefinitionHelper.__handle_link_reference_definition_init(
+            remaining_line_to_parse,
+            line_to_parse,
+            start_index,
+            original_line,
+            unmodified_line_to_parse,
         )
-        new_tokens: List[MarkdownToken] = []
+
         (
-            is_fence_start,
-            non_whitespace_index,
-            after_fence_index,
-            extracted_whitespace_before_info_string,
-            collected_count,
-        ) = LeafBlockProcessor.is_fenced_code_block(
-            position_marker.text_to_parse,
-            position_marker.index_number,
+            was_started,
+            lrd_stack_token,
+            original_stack_depth,
+            original_document_depth,
+            line_to_parse,
+            extracted_whitespace,
+            start_index,
+        ) = LinkReferenceDefinitionHelper.__handle_link_reference_definition_started(
+            parser_state,
+            original_stack_depth,
+            original_document_depth,
+            line_to_parse,
             extracted_whitespace,
+            start_index,
         )
-        if is_fence_start and not parser_state.token_stack[-1].is_html_block:
-            POGGER.debug("parse_fenced_code_block:fenced")
-            assert collected_count is not None
-            assert non_whitespace_index is not None
-            assert after_fence_index is not None
-            if parser_state.token_stack[-1].is_fenced_code_block:
-                POGGER.debug("parse_fenced_code_block:check fence end")
-                LeafBlockProcessor.__check_for_fenced_end(
-                    parser_state,
-                    position_marker,
-                    collected_count,
-                    non_whitespace_index,
-                    extracted_whitespace,
-                    new_tokens,
-                    after_fence_index,
-                    original_line,
-                )
-            else:
-                POGGER.debug("parse_fenced_code_block:check fence start")
-                new_tokens = LeafBlockProcessor.__process_fenced_start(
-                    parser_state,
-                    position_marker,
-                    non_whitespace_index,
-                    collected_count,
-                    extracted_whitespace,
-                    extracted_whitespace_before_info_string,
-                )
-        elif parser_state.token_stack[-1].is_fenced_code_block:
-            extracted_whitespace = (
-                LeafBlockProcessor.__parse_fenced_code_block_already_in(
-                    parser_state, extracted_whitespace
-                )
-            )
-        return new_tokens, extracted_whitespace
 
-    @staticmethod
-    def __parse_fenced_code_block_already_in(
-        parser_state: ParserState, extracted_whitespace: Optional[str]
-    ) -> Optional[str]:
-        fenced_token = cast(FencedCodeBlockStackToken, parser_state.token_stack[-1])
-        if fenced_token.whitespace_start_count and extracted_whitespace:
-            current_whitespace_length = ParserHelper.calculate_length(
-                extracted_whitespace
-            )
-            whitespace_left = max(
-                0,
-                current_whitespace_length - fenced_token.whitespace_start_count,
-            )
-            POGGER.debug("previous_ws>>$", current_whitespace_length)
-            POGGER.debug("whitespace_left>>$", whitespace_left)
-            removed_whitespace = ParserHelper.create_replace_with_nothing_marker(
-                ParserHelper.repeat_string(
-                    ParserHelper.space_character,
-                    current_whitespace_length - whitespace_left,
-                )
-            )
-            whitespace_padding = ParserHelper.repeat_string(
-                ParserHelper.space_character, whitespace_left
-            )
-            extracted_whitespace = f"{removed_whitespace}{whitespace_padding}"
-        return extracted_whitespace
+        POGGER.debug(">>line_to_parse>:$:<", line_to_parse)
+        line_to_parse_size = len(line_to_parse)
+        assert start_index is not None
 
-    # pylint: disable=too-many-arguments, too-many-locals
-    @staticmethod
-    def __add_fenced_tokens(
-        parser_state: ParserState,
-        position_marker: PositionMarker,
-        non_whitespace_index: int,
-        collected_count: int,
-        extracted_whitespace: Optional[str],
-        extracted_whitespace_before_info_string: Optional[str],
-    ) -> Tuple[StackToken, List[MarkdownToken]]:
-        (_, proper_end_index,) = ParserHelper.collect_backwards_while_one_of_characters(
-            position_marker.text_to_parse, -1, Constants.ascii_whitespace
+        (
+            did_complete_lrd,
+            end_lrd_index,
+            parsed_lrd_tuple,
+            is_blank_line,
+            line_to_parse,
+        ) = LinkReferenceDefinitionHelper.__handle_link_reference_definition_processing(
+            parser_state,
+            line_to_parse,
+            start_index,
+            extracted_whitespace,
+            is_blank_line,
+            was_started,
+            line_to_parse_size,
+            remaining_line_to_parse,
+            lines_to_requeue,
+            unmodified_line_to_parse,
         )
-        adjusted_string = position_marker.text_to_parse[:proper_end_index]
-        non_whitespace_index = min(non_whitespace_index, len(adjusted_string))
         (
-            after_extracted_text_index,
-            extracted_text,
-        ) = ParserHelper.extract_until_spaces(adjusted_string, non_whitespace_index)
-        assert extracted_text is not None
-        text_after_extracted_text = position_marker.text_to_parse[
-            after_extracted_text_index:
-        ]
-
-        old_top_of_stack = parser_state.token_stack[-1]
-        new_tokens, _ = parser_state.close_open_blocks_fn(
+            did_pause_lrd,
+            force_ignore_first_as_lrd,
+            new_tokens,
+        ) = LinkReferenceDefinitionHelper.__determine_continue_or_stop(
             parser_state,
-            only_these_blocks=[ParagraphStackToken],
+            position_marker,
+            was_started,
+            remaining_line_to_parse,
+            extracted_whitespace,
+            unmodified_line_to_parse,
+            original_stack_depth,
+            original_document_depth,
+            end_lrd_index,
+            line_to_parse_size,
+            is_blank_line,
+            did_complete_lrd,
+            parsed_lrd_tuple,
+            lines_to_requeue,
+            process_mode,
         )
+        if lines_to_requeue:
+            LinkReferenceDefinitionHelper.__prepare_for_requeue(
+                parser_state,
+                lrd_stack_token,
+                did_complete_lrd,
+                original_stack_depth,
+                original_document_depth,
+                lines_to_requeue,
+            )
+            requeue_line_info = RequeueLineInfo(
+                lines_to_requeue, force_ignore_first_as_lrd
+            )
+        else:
+            requeue_line_info = None
 
-        pre_extracted_text, pre_text_after_extracted_text = (
-            extracted_text,
-            text_after_extracted_text,
+        return (
+            did_complete_lrd or end_lrd_index != -1,
+            did_complete_lrd,
+            did_pause_lrd,
+            requeue_line_info,
+            new_tokens,
         )
 
-        assert extracted_text is not None
-        extracted_text = InlineHelper.handle_backslashes(extracted_text)
-        text_after_extracted_text = InlineHelper.handle_backslashes(
-            text_after_extracted_text
-        )
+    # pylint: enable=too-many-arguments, too-many-locals
 
-        if pre_extracted_text == extracted_text:
-            pre_extracted_text = ""
-        if pre_text_after_extracted_text == text_after_extracted_text:
-            pre_text_after_extracted_text = ""
+    @staticmethod
+    def __handle_link_reference_definition_init(
+        remaining_line_to_parse: str,
+        line_to_parse: str,
+        start_index: int,
+        original_line: str,
+        unmodified_line_to_parse: str,
+    ) -> Tuple[str, str, str, int, Optional[bool]]:
+        is_blank_line: Optional[bool] = not line_to_parse and not start_index
+
+        POGGER.debug(">>original_line>:$:<", original_line)
+        if ParserHelper.tab_character in original_line and not is_blank_line:
+            POGGER.debug(">>tabified>:$:<", original_line)
+
+            first_character_to_parse = line_to_parse[start_index]
+            POGGER.debug(">>xx>:$:<", first_character_to_parse)
+            first_character_to_parse_index = original_line.find(
+                first_character_to_parse
+            )
+            assert first_character_to_parse_index != -1
+
+            line_to_parse = original_line[first_character_to_parse_index:]
+            unmodified_line_to_parse = original_line
+            remaining_line_to_parse = line_to_parse
+            start_index = 0
 
-        assert extracted_whitespace is not None
-        assert extracted_whitespace_before_info_string is not None
-        new_token = FencedCodeBlockMarkdownToken(
-            position_marker.text_to_parse[position_marker.index_number],
-            collected_count,
-            extracted_text,
-            pre_extracted_text,
-            text_after_extracted_text,
-            pre_text_after_extracted_text,
-            extracted_whitespace,
-            extracted_whitespace_before_info_string,
-            position_marker,
-        )
-        new_tokens.append(new_token)
-        assert extracted_whitespace is not None
-        parser_state.token_stack.append(
-            FencedCodeBlockStackToken(
-                code_fence_character=position_marker.text_to_parse[
-                    position_marker.index_number
-                ],
-                fence_character_count=collected_count,
-                whitespace_start_count=ParserHelper.calculate_length(
-                    extracted_whitespace
-                ),
-                matching_markdown_token=new_token,
-            )
+        POGGER.debug(">>line_to_parse>:$:<", line_to_parse)
+        return (
+            line_to_parse,
+            unmodified_line_to_parse,
+            remaining_line_to_parse,
+            start_index,
+            is_blank_line,
         )
-        return old_top_of_stack, new_tokens
-
-    # pylint: enable=too-many-arguments, too-many-locals
 
     # pylint: disable=too-many-arguments
     @staticmethod
-    def __process_fenced_start(
+    def __handle_link_reference_definition_started(
         parser_state: ParserState,
-        position_marker: PositionMarker,
-        non_whitespace_index: int,
-        collected_count: int,
+        original_stack_depth: int,
+        original_document_depth: int,
+        line_to_parse: str,
         extracted_whitespace: Optional[str],
-        extracted_whitespace_before_info_string: Optional[str],
-    ) -> List[MarkdownToken]:
-
-        POGGER.debug("pfcb->check")
-        new_tokens: List[MarkdownToken] = []
-        if (
-            position_marker.text_to_parse[position_marker.index_number]
-            == LeafBlockProcessor.__fenced_start_tilde
-            or LeafBlockProcessor.__fenced_start_backtick
-            not in position_marker.text_to_parse[non_whitespace_index:]
-        ):
-            POGGER.debug("pfcb->start")
-
-            old_top_of_stack, new_tokens = LeafBlockProcessor.__add_fenced_tokens(
-                parser_state,
-                position_marker,
-                non_whitespace_index,
-                collected_count,
-                extracted_whitespace,
-                extracted_whitespace_before_info_string,
+        start_index: int,
+    ) -> Tuple[
+        bool, Optional[LinkDefinitionStackToken], int, int, str, Optional[str], int
+    ]:
+        lrd_stack_token: Optional[LinkDefinitionStackToken] = None
+
+        if was_started := parser_state.token_stack[-1].was_link_definition_started:
+            lrd_stack_token = cast(
+                LinkDefinitionStackToken, parser_state.token_stack[-1]
+            )
+            assert lrd_stack_token is not None
+            assert lrd_stack_token.original_stack_depth is not None
+            assert lrd_stack_token.original_document_depth is not None
+            original_stack_depth, original_document_depth = (
+                lrd_stack_token.original_stack_depth,
+                lrd_stack_token.original_document_depth,
             )
-
-            POGGER.debug("StackToken-->$<<", parser_state.token_stack[-1])
             POGGER.debug(
-                "StackToken>start_markdown_token-->$<<",
-                parser_state.token_stack[-1].matching_markdown_token,
+                ">>continuation_lines>>$<<",
+                lrd_stack_token.continuation_lines,
             )
-
-            LeafBlockProcessor.correct_for_leaf_block_start_in_list(
-                parser_state,
-                position_marker.index_indent,
-                old_top_of_stack,
-                new_tokens,
+            line_to_parse = lrd_stack_token.add_joined_lines_before_suffix(
+                line_to_parse
             )
-        return new_tokens
+            (
+                new_start_index,
+                extracted_whitespace,
+            ) = ParserHelper.extract_ascii_whitespace(line_to_parse, 0)
+            assert new_start_index is not None
+            start_index = new_start_index
+
+            POGGER.debug(">>line_to_parse>>$<<", line_to_parse)
+        return (
+            was_started,
+            lrd_stack_token,
+            original_stack_depth,
+            original_document_depth,
+            line_to_parse,
+            extracted_whitespace,
+            start_index,
+        )
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
+    # pylint: disable=too-many-locals
     @staticmethod
-    def __check_for_fenced_end(
+    def __determine_continue_or_stop(
         parser_state: ParserState,
         position_marker: PositionMarker,
-        collected_count: int,
-        non_whitespace_index: int,
+        was_started: bool,
+        remaining_line_to_parse: str,
         extracted_whitespace: Optional[str],
-        new_tokens: List[MarkdownToken],
-        after_fence_index: int,
-        original_line: str,
-    ) -> None:
-        POGGER.debug("pfcb->end")
-        POGGER.debug("extracted_whitespace:$:", extracted_whitespace)
-        POGGER.debug("non_whitespace_index:$:", non_whitespace_index)
-        POGGER.debug("position_marker.text_to_parse:$:", position_marker.text_to_parse)
-        POGGER.debug(
-            "len(position_marker.text_to_parse):$:", len(position_marker.text_to_parse)
-        )
-        POGGER.debug("after_fence_index:$:", after_fence_index)
-
-        POGGER.debug("original_line:$:", original_line)
-        only_spaces_after_fence = True
-        if "\t" in original_line:
-            fence_string = position_marker.text_to_parse[:after_fence_index]
-            POGGER.debug("fence_string:$:", fence_string)
-            fence_index_in_original = original_line.find(fence_string)
-            POGGER.debug("xy:$:", fence_index_in_original)
-            assert fence_index_in_original != -1
-            after_fence_in_original = original_line[
-                fence_index_in_original + collected_count :
-            ]
-            POGGER.debug("xz:$:", after_fence_in_original)
-            _, after_space_in_original_index = ParserHelper.collect_while_character(
-                after_fence_in_original, 0, " "
-            )
-            only_spaces_after_fence = after_space_in_original_index == len(
-                after_fence_in_original
+        unmodified_line_to_parse: str,
+        original_stack_depth: int,
+        original_document_depth: int,
+        end_lrd_index: Optional[int],
+        line_to_parse_size: int,
+        is_blank_line: Optional[bool],
+        did_complete_lrd: bool,
+        parsed_lrd_tuple: Optional[LinkReferenceDefinitionTuple],
+        lines_to_requeue: List[str],
+        process_mode: int,
+    ) -> Tuple[bool, bool, List[MarkdownToken]]:
+        assert is_blank_line is not None
+        assert end_lrd_index is not None
+        did_pause_lrd: bool = (
+            end_lrd_index >= 0
+            and end_lrd_index == line_to_parse_size
+            and not is_blank_line
+        )
+        if did_pause_lrd:
+            POGGER.debug(">>parse_link_reference_definition>>continuation")
+            LinkReferenceDefinitionHelper.__add_line_for_lrd_continuation(
+                parser_state,
+                position_marker,
+                was_started,
+                remaining_line_to_parse,
+                extracted_whitespace,
+                unmodified_line_to_parse,
+                original_stack_depth,
+                original_document_depth,
             )
-            POGGER.debug("only_spaces_after_fence:$:", only_spaces_after_fence)
-
-        after_fence_and_spaces_index, extracted_spaces = ParserHelper.extract_spaces(
-            position_marker.text_to_parse, after_fence_index
-        )
-        assert after_fence_and_spaces_index is not None
-        POGGER.debug("after_fence_and_spaces_index:$:", after_fence_and_spaces_index)
-
-        fenced_token = cast(FencedCodeBlockStackToken, parser_state.token_stack[-1])
-        if (
-            fenced_token.code_fence_character
-            == position_marker.text_to_parse[position_marker.index_number]
-            and collected_count >= fenced_token.fence_character_count
-            and after_fence_and_spaces_index >= len(position_marker.text_to_parse)
-            and only_spaces_after_fence
-        ):
-            assert extracted_whitespace is not None
-            assert extracted_spaces is not None
-            new_end_token = parser_state.token_stack[
-                -1
-            ].generate_close_markdown_token_from_stack_token(
+        if not did_pause_lrd and was_started or did_complete_lrd:
+            return LinkReferenceDefinitionHelper.__stop_lrd_continuation(
+                parser_state,
+                did_complete_lrd,
+                parsed_lrd_tuple,
+                end_lrd_index,
+                remaining_line_to_parse,
+                is_blank_line,
+                lines_to_requeue,
                 extracted_whitespace,
-                extra_end_data=f"{extracted_spaces}:{collected_count}",
+                process_mode,
+                did_pause_lrd,
             )
 
-            new_tokens.append(new_end_token)
-            del parser_state.token_stack[-1]
-
-    # pylint: enable=too-many-arguments, too-many-locals
-
-    @staticmethod
-    def __recalculate_whitespace(
-        whitespace_to_parse: Optional[str], offset_index: int
-    ) -> Tuple[int, str, str]:
-        """
-        Recalculate the whitespace characteristics.
-        """
-        assert whitespace_to_parse is not None
-        POGGER.debug(
-            "whitespace_to_parse>>$>>",
-            whitespace_to_parse,
-        )
-        actual_whitespace_index = 4 + offset_index
-        adj_ws = whitespace_to_parse[:actual_whitespace_index]
-        left_ws = whitespace_to_parse[actual_whitespace_index:]
-        POGGER.debug("actual_whitespace_index>>$", actual_whitespace_index)
-        POGGER.debug("adj_ws>>$<<", adj_ws)
-        POGGER.debug("left_ws>>$<<", left_ws)
+        POGGER.debug(">>parse_link_reference_definition>>other")
+        return did_pause_lrd, False, []
 
-        return actual_whitespace_index, adj_ws, left_ws
+    # pylint: enable=too-many-arguments
+    # pylint: enable=too-many-locals
 
+    # pylint: disable=too-many-arguments
     @staticmethod
-    def parse_indented_code_block(
+    def __handle_link_reference_definition_processing(
         parser_state: ParserState,
-        position_marker: PositionMarker,
+        line_to_parse: str,
+        start_index: int,
         extracted_whitespace: Optional[str],
-        removed_chars_at_start: Optional[int],
-        last_block_quote_index: int,
-    ) -> List[MarkdownToken]:
-
-        """
-        Handle the parsing of an indented code block
-        """
-
-        new_tokens: List[MarkdownToken] = []
-
-        assert extracted_whitespace is not None
-        assert removed_chars_at_start is not None
-        if (
-            ParserHelper.is_length_greater_than_or_equal_to(
-                extracted_whitespace, 4, start_index=removed_chars_at_start
+        is_blank_line: Optional[bool],
+        was_started: bool,
+        line_to_parse_size: int,
+        remaining_line_to_parse: str,
+        lines_to_requeue: List[str],
+        unmodified_line_to_parse: str,
+    ) -> Tuple[
+        bool, Optional[int], Optional[LinkReferenceDefinitionTuple], Optional[bool], str
+    ]:
+        if was_started:
+            POGGER.debug(">>parse_link_reference_definition>>was_started")
+            did_complete_lrd: Optional[bool] = False
+            (
+                did_complete_lrd,
+                end_lrd_index,
+                parsed_lrd_tuple,
+            ) = LinkReferenceDefinitionHelper.__parse_link_reference_definition(
+                parser_state,
+                line_to_parse,
+                start_index,
+                extracted_whitespace,
+                is_blank_line,
             )
-            and not parser_state.token_stack[-1].is_paragraph
-        ):
             POGGER.debug(
-                "parse_indented_code_block>>start",
+                ">>parse_link_reference_definition>>was_started>>did_complete_lrd>>$"
+                + ">>end_lrd_index>>$>>len(line_to_parse)>>$",
+                did_complete_lrd,
+                end_lrd_index,
+                line_to_parse_size,
             )
-            if not parser_state.token_stack[-1].is_indented_code_block:
+
+            if not (
+                did_complete_lrd
+                or (
+                    not is_blank_line
+                    and not did_complete_lrd
+                    and (end_lrd_index == line_to_parse_size)
+                )
+            ):
+                POGGER.debug(
+                    ">>parse_link_reference_definition>>was_started>>GOT HARD FAILURE"
+                )
                 (
-                    last_block_quote_index,
-                    extracted_whitespace,
-                ) = LeafBlockProcessor.__create_indented_block(
+                    is_blank_line,
+                    line_to_parsex,
+                    did_complete_lrd,
+                    end_lrd_index,
+                    parsed_lrd_tuple,
+                ) = LinkReferenceDefinitionHelper.__process_lrd_hard_failure(
                     parser_state,
-                    last_block_quote_index,
-                    position_marker,
-                    extracted_whitespace,
-                    new_tokens,
-                )
-
-            assert extracted_whitespace is not None
-            new_tokens.append(
-                TextMarkdownToken(
-                    position_marker.text_to_parse[position_marker.index_number :],
-                    extracted_whitespace,
-                    position_marker=position_marker,
+                    remaining_line_to_parse,
+                    lines_to_requeue,
+                    unmodified_line_to_parse,
                 )
-            )
+                assert line_to_parsex is not None
+                line_to_parse = line_to_parsex
         else:
+            (
+                did_complete_lrd,
+                end_lrd_index,
+                parsed_lrd_tuple,
+            ) = LinkReferenceDefinitionHelper.__parse_link_reference_definition(
+                parser_state,
+                line_to_parse,
+                start_index,
+                extracted_whitespace,
+                is_blank_line,
+            )
             POGGER.debug(
-                "parse_indented_code_block>>not eligible",
+                ">>parse_link_reference_definition>>did_complete_lrd>>$>>end_lrd_index>>$>>len(line_to_parse)>>$",
+                did_complete_lrd,
+                end_lrd_index,
+                line_to_parse_size,
             )
-        return new_tokens
+        assert did_complete_lrd is not None
+        return (
+            did_complete_lrd,
+            end_lrd_index,
+            parsed_lrd_tuple,
+            is_blank_line,
+            line_to_parse,
+        )
 
-    @staticmethod
-    def __create_indented_block(
-        parser_state: ParserState,
-        last_block_quote_index: int,
-        position_marker: PositionMarker,
-        extracted_whitespace: Optional[str],
-        new_tokens: List[MarkdownToken],
-    ) -> Tuple[int, Optional[str]]:
+    # pylint: enable=too-many-arguments
 
-        assert extracted_whitespace is not None
-        line_number, column_number = position_marker.line_number, (
-            position_marker.index_number
-            + position_marker.index_indent
-            - len(extracted_whitespace)
-            + 1
+    @staticmethod
+    def __prepare_for_requeue_reset_markdown_token(
+        parser_state: ParserState, lrd_stack_token: LinkDefinitionStackToken
+    ) -> None:
+        assert lrd_stack_token.last_block_quote_markdown_token_index is not None
+        POGGER.debug(
+            ">>XXXXXX>>last_block_quote_markdown_token_index:$:",
+            lrd_stack_token.last_block_quote_markdown_token_index,
         )
-        (
-            last_block_quote_index,
-            actual_whitespace_index,
-            adj_ws,
-            extracted_whitespace,
-        ) = LeafBlockProcessor.__prepare_for_indented_block(
-            parser_state,
-            last_block_quote_index,
-            extracted_whitespace,
+        POGGER.debug(
+            ">>XXXXXX>>st-now:$:",
+            parser_state.token_document[
+                lrd_stack_token.last_block_quote_markdown_token_index
+            ],
         )
 
-        column_number += actual_whitespace_index
-        POGGER.debug("column_number>>$", column_number)
-
-        new_token = IndentedCodeBlockMarkdownToken(adj_ws, line_number, column_number)
-        parser_state.token_stack.append(IndentedCodeBlockStackToken(new_token))
-        new_tokens.append(new_token)
-        POGGER.debug("left_ws>>$<<", extracted_whitespace)
-
-        return last_block_quote_index, extracted_whitespace
+        del parser_state.token_document[
+            lrd_stack_token.last_block_quote_markdown_token_index
+        ]
+        assert lrd_stack_token.copy_of_last_block_quote_markdown_token is not None
+        parser_state.token_document.insert(
+            lrd_stack_token.last_block_quote_markdown_token_index,
+            lrd_stack_token.copy_of_last_block_quote_markdown_token,
+        )
+        assert lrd_stack_token.last_block_quote_stack_token is not None
+        POGGER.debug(
+            "last_block_quote_stack_token>:$:<",
+            lrd_stack_token.last_block_quote_stack_token,
+        )
+        lrd_stack_token.last_block_quote_stack_token.reset_matching_markdown_token(
+            lrd_stack_token.copy_of_last_block_quote_markdown_token
+        )
+        POGGER.debug(
+            "last_block_quote_stack_token>:$:<",
+            lrd_stack_token.last_block_quote_stack_token,
+        )
 
     @staticmethod
-    def __prepare_for_indented_block(
+    def __prepare_for_requeue_reset_document_and_stack(
         parser_state: ParserState,
-        last_block_quote_index: int,
-        extracted_whitespace: Optional[str],
-    ) -> Tuple[int, int, str, str]:
-        POGGER.debug(">>>>$", parser_state.token_stack[-1])
-        if parser_state.token_stack[-1].is_list:
-            list_token = cast(ListStackToken, parser_state.token_stack[-1])
-            POGGER.debug(
-                ">>indent>>$",
-                list_token.indent_level,
-            )
-            last_block_quote_index = 0
+        lrd_stack_token: LinkDefinitionStackToken,
+        original_stack_depth: int,
+        original_document_depth: int,
+    ) -> None:
+        POGGER.debug(">>XXXXXX>>original_stack_depth:$:", original_stack_depth)
+        POGGER.debug(">>XXXXXX>>token_stack_depth:$:", len(parser_state.token_stack))
+        POGGER.debug(">>XXXXXX>>token_stack(before):$:", parser_state.token_stack)
+        POGGER.debug(
+            ">>XXXXXX>>copy_of_token_stack:$:", parser_state.copy_of_token_stack
+        )
+        POGGER.debug(
+            ">>lrd_stack_token>>copy_of_token_stack:$:",
+            lrd_stack_token.copy_of_token_stack,
+        )
+        if len(parser_state.token_stack) >= original_stack_depth:
+            while len(parser_state.token_stack) > original_stack_depth:
+                del parser_state.token_stack[-1]
+        else:
+            while len(parser_state.token_stack):
+                del parser_state.token_stack[-1]
+            assert lrd_stack_token.copy_of_token_stack is not None
+            parser_state.token_stack.extend(lrd_stack_token.copy_of_token_stack)
+        POGGER.debug(">>XXXXXX>>token_stack(after):$:", parser_state.token_stack)
 
+        POGGER.debug(">>XXXXXX>>original_document_depth:$:", original_document_depth)
         POGGER.debug(
-            "__recalculate_whitespace>>$>>$",
-            extracted_whitespace,
-            0,
+            ">>XXXXXX>>token_document_depth:$:",
+            len(parser_state.token_document),
         )
-        (
-            actual_whitespace_index,
-            adj_ws,
-            left_ws,
-        ) = LeafBlockProcessor.__recalculate_whitespace(extracted_whitespace, 0)
-        return (
-            last_block_quote_index,
-            actual_whitespace_index,
-            adj_ws,
-            left_ws,
+        POGGER.debug(">>XXXXXX>>token_document(before):$:", parser_state.token_document)
+        while len(parser_state.token_document) > original_document_depth:
+            del parser_state.token_document[-1]
+        POGGER.debug(">>XXXXXX>>token_document(after):$:", parser_state.token_document)
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __prepare_for_requeue(
+        parser_state: ParserState,
+        lrd_stack_token: Optional[LinkDefinitionStackToken],
+        did_complete_lrd: bool,
+        original_stack_depth: int,
+        original_document_depth: int,
+        lines_to_requeue: List[str],
+    ) -> None:
+        # This works because in most cases, we add things.  However, in cases like
+        # an indented code block, we process the "is it indented enough" and close
+        # that block before hitting this.  As such, we have a special case to take
+        # care of that.  In the future, will possibly want to do something instead of
+        # original_document_depth and stack, such as passing in a copy of the both
+        # elements so they can be reset on the rewind.
+        # i.e. icode would go back on stack, end-icode would not be in document.
+        assert lrd_stack_token is not None
+        POGGER.debug("lines_to_requeue:$:", lines_to_requeue)
+        POGGER.debug(
+            ">>XXXXXX>>copy_of_last_block_quote_markdown_token:$:",
+            lrd_stack_token.copy_of_last_block_quote_markdown_token,
         )
+        if not did_complete_lrd:
+            if lrd_stack_token.copy_of_last_block_quote_markdown_token:
+                LinkReferenceDefinitionHelper.__prepare_for_requeue_reset_markdown_token(
+                    parser_state, lrd_stack_token
+                )
+            LinkReferenceDefinitionHelper.__prepare_for_requeue_reset_document_and_stack(
+                parser_state,
+                lrd_stack_token,
+                original_stack_depth,
+                original_document_depth,
+            )
+
+    # pylint: enable=too-many-arguments
 
     @staticmethod
-    def is_thematic_break(
+    def __is_link_reference_definition(
+        parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: Optional[str],
-        skip_whitespace_check: bool = False,
-        whitespace_allowed_between_characters: bool = True,
-    ) -> Tuple[Optional[str], Optional[int]]:
+    ) -> bool:
         """
-        Determine whether or not we have a thematic break.
+        Determine whether or not we have the start of a link reference definition.
         """
 
+        if parser_state.token_stack[-1].is_paragraph:
+            return False
+
         assert extracted_whitespace is not None
-        thematic_break_character, end_of_break_index = None, None
-        is_thematic_character = ParserHelper.is_character_at_index_one_of(
-            line_to_parse, start_index, LeafBlockProcessor.__thematic_break_characters
+        POGGER.debug(
+            "__is_link_reference_definition - extracted_whitespace:>:$:<",
+            extracted_whitespace,
+        )
+        POGGER.debug(
+            "__is_link_reference_definition - line_to_parse:>:$:<", line_to_parse
         )
-        POGGER.debug("skip_whitespace_check>>$", skip_whitespace_check)
-        POGGER.debug("is_thematic_character>>$", is_thematic_character)
         if (
-            ParserHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
-            or skip_whitespace_check
-        ) and is_thematic_character:
-            start_char, index, char_count, line_to_parse_size = (
-                line_to_parse[start_index],
-                start_index,
-                0,
-                len(line_to_parse),
-            )
-
-            while index < line_to_parse_size:
-                if (
-                    whitespace_allowed_between_characters
-                    and ParserHelper.is_character_at_index_whitespace(
-                        line_to_parse, index
+            TabHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
+        ) and ParserHelper.is_character_at_index_one_of(
+            line_to_parse,
+            start_index,
+            LinkReferenceDefinitionHelper.__lrd_start_character,
+        ):
+            POGGER.debug("__is_link_reference_definition - potential")
+            remaining_line, continue_with_lrd = line_to_parse[start_index + 1 :], True
+            if (
+                remaining_line
+                and remaining_line[-1] == InlineHelper.backslash_character
+            ):
+                remaining_line_size, start_index, found_index = (
+                    len(remaining_line),
+                    0,
+                    remaining_line.find(InlineHelper.backslash_character, start_index),
+                )
+                POGGER.debug(">>$<<$", remaining_line, remaining_line_size)
+                POGGER.debug(">>$<<$", remaining_line, start_index)
+                POGGER.debug(">>$<<", found_index)
+                while found_index != -1 and found_index < (remaining_line_size - 1):
+                    start_index = found_index + 2
+                    POGGER.debug(">>$<<$", remaining_line, start_index)
+                    found_index = remaining_line.find(
+                        InlineHelper.backslash_character, start_index
                     )
-                ):
-                    index += 1
-                elif line_to_parse[index] == start_char:
-                    index += 1
-                    char_count += 1
-                else:
-                    break  # pragma: no cover
-
-            POGGER.debug("char_count>>$", char_count)
-            POGGER.debug("index>>$", index)
-            POGGER.debug("line_to_parse_size>>$", line_to_parse_size)
-            if char_count >= 3 and index == line_to_parse_size:
-                thematic_break_character, end_of_break_index = start_char, index
+                    POGGER.debug(">>$<<", found_index)
+                POGGER.debug(">>>>>>>$<<", found_index)
+                continue_with_lrd = found_index != remaining_line_size - 1
+            return continue_with_lrd
+        return False
 
-        return thematic_break_character, end_of_break_index
+    @staticmethod
+    def __verify_link_definition_end(
+        line_to_parse: str, new_index: Optional[int]
+    ) -> Tuple[bool, Optional[int], Optional[str]]:
+        """
+        Verify that the link reference definition's ends properly.
+        """
 
+        assert new_index is not None
+        POGGER.debug("look for EOL-ws>>$<<", line_to_parse[new_index:])
+        new_index, ex_ws = ParserHelper.extract_ascii_whitespace(
+            line_to_parse, new_index
+        )
+        assert new_index is not None
+        POGGER.debug("look for EOL>>$<<", line_to_parse[new_index:])
+        if new_index < len(line_to_parse):
+            POGGER.debug(">> characters left at EOL, bailing")
+            return False, -1, None
+        return True, new_index, ex_ws
+
+    # pylint: disable=too-many-locals
     @staticmethod
-    def parse_thematic_break(
+    def __parse_link_reference_definition(
         parser_state: ParserState,
-        position_marker: PositionMarker,
+        line_to_parse: str,
+        start_index: int,
         extracted_whitespace: Optional[str],
-        block_quote_data: BlockQuoteData,
-    ) -> List[MarkdownToken]:
+        is_blank_line: Optional[bool],
+    ) -> Tuple[bool, Optional[int], Optional[LinkReferenceDefinitionTuple]]:
         """
-        Handle the parsing of a thematic break.
+        Handle the parsing of what appears to be a link reference definition.
         """
-
-        new_tokens: List[MarkdownToken] = []
-
-        start_char, index = LeafBlockProcessor.is_thematic_break(
-            position_marker.text_to_parse,
-            position_marker.index_number,
-            extracted_whitespace,
-        )
-        if start_char:
-            POGGER.debug(
-                "parse_thematic_break>>start",
+        # POGGER.debug("parse_link_reference_definition:$:", line_to_parse)
+        # POGGER.debug("start_index:$:", start_index)
+        # POGGER.debug("extracted_whitespace:$:", extracted_whitespace)
+        did_start = LinkReferenceDefinitionHelper.__is_link_reference_definition(
+            parser_state, line_to_parse, start_index, extracted_whitespace
+        )
+        if not did_start:
+            POGGER.debug("BAIL")
+            return False, -1, None
+
+        # POGGER.debug("parse_link_reference_definition")
+        new_index: Optional[int] = None
+        keep_going, new_index, collected_destination = LinkHelper.extract_link_label(
+            line_to_parse, start_index + 1
+        )
+        # POGGER.debug("parse_link_reference_definition: keep_going:>:$:<", keep_going)
+        # POGGER.debug("parse_link_reference_definition: new_index:>:$:<", new_index)
+        # POGGER.debug(
+        #     "parse_link_reference_definition: collected_destination:>:$:<",
+        #     collected_destination,
+        # )
+        assert is_blank_line is not None
+        if keep_going:
+            (
+                keep_going,
+                new_index,
+                inline_link,
+                _,
+                line_destination_whitespace,
+                inline_raw_link,
+            ) = LinkHelper.extract_link_destination(
+                line_to_parse, new_index, is_blank_line
             )
-            if parser_state.token_stack[-1].is_paragraph:
-                force_paragraph_close_if_present = (
-                    block_quote_data.current_count == 0
-                    and block_quote_data.stack_count > 0
-                )
-                new_tokens, _ = parser_state.close_open_blocks_fn(
-                    parser_state,
-                    only_these_blocks=[ParagraphStackToken],
-                    was_forced=force_paragraph_close_if_present,
-                )
-
-            assert (
-                block_quote_data.current_count != 0 or block_quote_data.stack_count <= 0
+            # POGGER.debug(
+            #     "parse_link_reference_definition: keep_going:>:$:<", keep_going
+            # )
+            # POGGER.debug("parse_link_reference_definition: new_index:>:$:<", new_index)
+            # POGGER.debug(
+            #     "parse_link_reference_definition: inline_link:>:$:<", inline_link
+            # )
+            # POGGER.debug(
+            #     "parse_link_reference_definition: line_destination_whitespace:>:$:<",
+            #     line_destination_whitespace,
+            # )
+            # POGGER.debug(
+            #     "parse_link_reference_definition: inline_raw_link:>:$:<",
+            #     inline_raw_link,
+            # )
+        else:
+            inline_link = None
+        if keep_going:
+            (
+                keep_going,
+                new_index,
+                inline_title,
+                _,
+                line_title_whitespace,
+                inline_raw_title,
+            ) = LinkHelper.extract_link_title(line_to_parse, new_index, is_blank_line)
+            # POGGER.debug(
+            #     "parse_link_reference_definition: keep_going:>:$:<", keep_going
+            # )
+            # POGGER.debug("parse_link_reference_definition: new_index:>:$:<", new_index)
+            # POGGER.debug(
+            #     "parse_link_reference_definition: inline_title:>:$:<", inline_title
+            # )
+            # POGGER.debug(
+            #     "parse_link_reference_definition: line_title_whitespace:>:$:<",
+            #     line_title_whitespace,
+            # )
+            # POGGER.debug(
+            #     "parse_link_reference_definition: inline_raw_title:>:$:<",
+            #     inline_raw_title,
+            # )
+        else:
+            inline_title = ""
+        if keep_going:
+            (
+                keep_going,
+                new_index,
+                end_whitespace,
+            ) = LinkReferenceDefinitionHelper.__verify_link_definition_end(
+                line_to_parse, new_index
             )
-            # new_tokens, _ = parser_state.close_open_blocks_fn(
-            #     parser_state,
-            #     only_these_blocks=[BlockQuoteStackToken],
-            #     include_block_quotes=True,
-            #     was_forced=True,
+        if keep_going:
+            assert collected_destination is not None
+            # POGGER.debug(
+            #     ">>collected_destination(not normalized)>>$", collected_destination
             # )
-            new_tokens.append(
-                ThematicBreakMarkdownToken(
-                    start_char,
-                    extracted_whitespace,
-                    position_marker.text_to_parse[position_marker.index_number : index],
-                    position_marker=position_marker,
-                )
+            normalized_destination = LinkHelper.normalize_link_label(
+                collected_destination
             )
+            if not normalized_destination:
+                keep_going, new_index = False, -1
         else:
-            POGGER.debug(
-                "parse_thematic_break>>not eligible",
+            normalized_destination = None
+        return (
+            LinkReferenceDefinitionHelper.__create_lrd_token(
+                new_index,
+                collected_destination,
+                normalized_destination,
+                line_destination_whitespace,
+                inline_link,
+                inline_raw_link,
+                inline_title,
+                inline_raw_title,
+                line_title_whitespace,
+                end_whitespace,
             )
-        return new_tokens
+            if keep_going
+            else (keep_going, new_index, None)
+        )
 
+    # pylint: enable=too-many-locals
+
+    # pylint: disable=too-many-arguments
     @staticmethod
-    def is_atx_heading(
-        line_to_parse: str,
-        start_index: int,
-        extracted_whitespace: Optional[str],
-        skip_whitespace_check: bool = False,
-    ) -> Tuple[bool, Optional[int], Optional[int], Optional[str]]:
-        """
-        Determine whether or not an ATX Heading is about to start.
-        """
+    def __create_lrd_token(
+        new_index: Optional[int],
+        collected_destination: Optional[str],
+        normalized_destination: Optional[str],
+        line_destination_whitespace: Optional[str],
+        inline_link: Optional[str],
+        inline_raw_link: Optional[str],
+        inline_title: Optional[str],
+        inline_raw_title: Optional[str],
+        line_title_whitespace: Optional[str],
+        end_whitespace: Optional[str],
+    ) -> Tuple[bool, Optional[int], Optional[LinkReferenceDefinitionTuple]]:
+        assert new_index != -1
+
+        POGGER.debug(
+            ">>collected_destination(normalized)>>$",
+            normalized_destination,
+        )
 
-        assert extracted_whitespace is not None
         if (
-            ParserHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
-            or skip_whitespace_check
-        ) and ParserHelper.is_character_at_index(
-            line_to_parse,
-            start_index,
-            LeafBlockProcessor.__atx_character,
+            not inline_title
+            and line_title_whitespace
+            and line_title_whitespace[-1] == ParserHelper.newline_character
         ):
-            hash_count, new_index = ParserHelper.collect_while_character(
-                line_to_parse,
-                start_index,
-                LeafBlockProcessor.__atx_character,
-            )
+            line_title_whitespace = line_title_whitespace[:-1]
 
-            assert new_index is not None
-            non_whitespace_index, _ = ParserHelper.collect_while_spaces(
-                line_to_parse, new_index
-            )
-            extracted_whitespace_at_start = line_to_parse[
-                new_index:non_whitespace_index
-            ]
+        POGGER.debug(">>inline_link>>$<<", inline_link)
+        POGGER.debug(">>inline_title>>$<<", inline_title)
+        parsed_lrd_tuple = LinkReferenceDefinitionTuple(
+            normalized_destination,
+            LinkReferenceTitles(inline_link, inline_title),
+            LinkReferenceInfo(
+                collected_destination,
+                line_destination_whitespace,
+                inline_raw_link,
+                line_title_whitespace,
+                inline_raw_title,
+                end_whitespace,
+            ),
+        )
+        return True, new_index, parsed_lrd_tuple
 
-            assert hash_count is not None
-            if hash_count <= 6 and (
-                extracted_whitespace_at_start
-                or non_whitespace_index == len(line_to_parse)
-            ):
-                return (
-                    True,
-                    non_whitespace_index,
-                    hash_count,
-                    extracted_whitespace_at_start,
-                )
-        return False, None, None, None
+    # pylint: enable=too-many-arguments
 
+    # pylint: disable=too-many-arguments
     @staticmethod
-    def parse_atx_headings(
+    def __add_line_for_lrd_continuation(
         parser_state: ParserState,
         position_marker: PositionMarker,
+        was_started: bool,
+        remaining_line_to_parse: str,
         extracted_whitespace: Optional[str],
-    ) -> List[MarkdownToken]:
+        unmodified_line_to_parse: str,
+        original_stack_depth: int,
+        original_document_depth: int,
+    ) -> None:
         """
-        Handle the parsing of an atx heading.
+        As part of processing a link reference definition, add a line to the continuation.
         """
 
-        (
-            heading_found,
-            non_whitespace_index,
-            hash_count,
-            extracted_whitespace_at_start,
-        ) = LeafBlockProcessor.is_atx_heading(
-            position_marker.text_to_parse,
-            position_marker.index_number,
-            extracted_whitespace,
-        )
-        if heading_found:
-            assert extracted_whitespace_at_start is not None
-            POGGER.debug(
-                "parse_atx_headings>>start",
-            )
+        line_to_store = remaining_line_to_parse
+        if not was_started:
+            POGGER.debug(">>parse_link_reference_definition>>marking start")
+            new_token = LinkDefinitionStackToken(extracted_whitespace, position_marker)
+            parser_state.token_stack.append(new_token)
+            new_token.original_stack_depth = original_stack_depth
+            new_token.original_document_depth = original_document_depth
 
-            assert non_whitespace_index is not None
-            (
-                old_top_of_stack,
-                remaining_line,
-                remove_trailing_count,
-                extracted_whitespace_before_end,
-                extracted_whitespace_at_end,
-                new_tokens,
-            ) = LeafBlockProcessor.__prepare_for_create_atx_heading(
-                parser_state, position_marker, [], non_whitespace_index
+            new_token.last_block_quote_stack_token = (
+                parser_state.last_block_quote_stack_token
             )
-            assert hash_count is not None
-            assert extracted_whitespace is not None
-            start_token = AtxHeadingMarkdownToken(
-                hash_count,
-                remove_trailing_count,
-                extracted_whitespace,
-                position_marker,
-            )
-            new_tokens.append(start_token)
-
-            LeafBlockProcessor.correct_for_leaf_block_start_in_list(
-                parser_state,
-                position_marker.index_indent,
-                old_top_of_stack,
-                new_tokens,
-                was_token_already_added_to_stack=False,
-            )
-
-            new_tokens.append(
-                TextMarkdownToken(
-                    remaining_line,
-                    extracted_whitespace_at_start,
-                    position_marker=position_marker,
-                )
+            new_token.last_block_quote_markdown_token_index = (
+                parser_state.last_block_quote_markdown_token_index
             )
-            end_token = start_token.generate_close_markdown_token_from_markdown_token(
-                extracted_whitespace_at_end, extracted_whitespace_before_end
+            new_token.copy_of_last_block_quote_markdown_token = (
+                parser_state.copy_of_last_block_quote_markdown_token
             )
-            new_tokens.append(end_token)
+            new_token.copy_of_token_stack = parser_state.copy_of_token_stack
         else:
-            POGGER.debug(
-                "parse_atx_headings>>not eligible",
-            )
-            new_tokens = []
-        return new_tokens
+            new_token = cast(LinkDefinitionStackToken, parser_state.token_stack[-1])
 
-    @staticmethod
-    def __prepare_for_create_atx_heading(
-        parser_state: ParserState,
-        position_marker: PositionMarker,
-        new_tokens: List[MarkdownToken],
-        non_whitespace_index: int,
-    ) -> Tuple[StackToken, str, int, str, str, List[MarkdownToken]]:
-        (
-            old_top_of_stack,
-            remaining_line,
-            remove_trailing_count,
-            extracted_whitespace_before_end,
-        ) = (
-            parser_state.token_stack[-1],
-            position_marker.text_to_parse[non_whitespace_index:],
-            0,
-            "",
-        )
+        POGGER.debug(">>line_to_store>>add>:$<<", line_to_store)
+        POGGER.debug(">>unmodified_line_to_parse>>add>:$<<", unmodified_line_to_parse)
+        assert unmodified_line_to_parse.endswith(line_to_store)
+        new_token.add_continuation_line(line_to_store)
+        new_token.add_unmodified_line(unmodified_line_to_parse)
 
-        new_tokens, _ = parser_state.close_open_blocks_fn(parser_state)
-        (
-            end_index,
-            extracted_whitespace_at_end,
-        ) = ParserHelper.extract_spaces_from_end(remaining_line)
-        while (
-            end_index > 0
-            and remaining_line[end_index - 1] == LeafBlockProcessor.__atx_character
-        ):
-            end_index -= 1
-            remove_trailing_count += 1
-        if remove_trailing_count:
-            if end_index > 0:
-                if ParserHelper.is_character_at_index_whitespace(
-                    remaining_line, end_index - 1
-                ):
-                    remaining_line = remaining_line[:end_index]
-                    (
-                        _,
-                        new_non_whitespace_index,
-                    ) = ParserHelper.collect_backwards_while_spaces(
-                        remaining_line, len(remaining_line) - 1
-                    )
-                    assert new_non_whitespace_index is not None
-                    end_index = new_non_whitespace_index
-                    extracted_whitespace_before_end = remaining_line[end_index:]
-                    remaining_line = remaining_line[:end_index]
-                else:
-                    extracted_whitespace_at_end, remove_trailing_count = "", 0
-            else:
-                remaining_line = ""
-        else:
-            extracted_whitespace_at_end = remaining_line[end_index:]
-            remaining_line = remaining_line[:end_index]
-
-        return (
-            old_top_of_stack,
-            remaining_line,
-            remove_trailing_count,
-            extracted_whitespace_before_end,
-            extracted_whitespace_at_end,
-            new_tokens,
-        )
+    # pylint: enable=too-many-arguments
 
+    # pylint: disable=too-many-arguments
     @staticmethod
-    def parse_setext_headings(
+    def __stop_lrd_continuation(
         parser_state: ParserState,
-        position_marker: PositionMarker,
+        did_complete_lrd: bool,
+        parsed_lrd_tuple: Optional[LinkReferenceDefinitionTuple],
+        end_lrd_index: int,
+        remaining_line_to_parse: str,
+        is_blank_line: bool,
+        lines_to_requeue: List[str],
         extracted_whitespace: Optional[str],
-        block_quote_data: BlockQuoteData,
-    ) -> List[MarkdownToken]:
-
-        """
-        Handle the parsing of an setext heading.
-        """
+        process_mode: int,
+        did_pause_lrd: bool,
+    ) -> Tuple[bool, bool, List[MarkdownToken]]:
+        """
+        As part of processing a link reference definition, stop a continuation.
+        """
+
+        POGGER.debug(">>parse_link_reference_definition>>no longer need start")
+        if did_complete_lrd:
+            assert parsed_lrd_tuple
+            assert parsed_lrd_tuple.normalized_destination is not None
+            did_add_definition = LinkHelper.add_link_definition(
+                parsed_lrd_tuple.normalized_destination, parsed_lrd_tuple.link_titles
+            )
+            assert not (end_lrd_index < -1 and remaining_line_to_parse)
+            link_def_token = cast(
+                LinkDefinitionStackToken, parser_state.token_stack[-1]
+            )
+            assert link_def_token.extracted_whitespace is not None
+            extracted_whitespace = link_def_token.extracted_whitespace
 
-        new_tokens: List[MarkdownToken] = []
-        assert extracted_whitespace is not None
-        if (
-            ParserHelper.is_length_less_than_or_equal_to(extracted_whitespace, 3)
-            and ParserHelper.is_character_at_index_one_of(
-                position_marker.text_to_parse,
-                position_marker.index_number,
-                LeafBlockProcessor.__setext_characters,
+            POGGER.debug(
+                "link_def_token.extracted_whitespace>:$:<",
+                link_def_token.extracted_whitespace,
             )
-            and parser_state.token_stack[-1].is_paragraph
-            and (block_quote_data.current_count == block_quote_data.stack_count)
-        ):
             POGGER.debug(
-                "parse_setext_headings>>start",
+                "link_def_token.continuation_lines>:$:<",
+                link_def_token.continuation_lines,
             )
-            is_paragraph_continuation = (
-                LeafBlockProcessor.__adjust_continuation_for_active_list(
-                    parser_state, position_marker
-                )
+            POGGER.debug(
+                "link_def_token.unmodified_lines>:$:<", link_def_token.unmodified_lines
             )
+            POGGER.debug("lines_to_requeue>:$:<", lines_to_requeue)
 
-            _, collected_to_index = ParserHelper.collect_while_character(
-                position_marker.text_to_parse,
-                position_marker.index_number,
-                position_marker.text_to_parse[position_marker.index_number],
-            )
-            assert collected_to_index is not None
-            (
-                after_whitespace_index,
-                extra_whitespace_after_setext,
-            ) = ParserHelper.extract_spaces(
-                position_marker.text_to_parse, collected_to_index
+            does_any_line_have_tabs = any(
+                ParserHelper.tab_character in ffg
+                for ffg in link_def_token.unmodified_lines
             )
+            POGGER.debug("does_any_line_have_tabs>:$:<", does_any_line_have_tabs)
 
-            if not is_paragraph_continuation and after_whitespace_index == len(
-                position_marker.text_to_parse
-            ):
-                LeafBlockProcessor.__create_setext_token(
+            last_container_index = parser_state.find_last_container_on_stack()
+            if does_any_line_have_tabs and last_container_index > 0:
+                (
+                    extracted_whitespace,
+                    parsed_lrd_tuple,
+                ) = LinkReferenceDefinitionHelper.__stop_lrd_continuation_with_tab(
                     parser_state,
-                    position_marker,
-                    collected_to_index,
-                    new_tokens,
+                    link_def_token,
+                    last_container_index,
+                    lines_to_requeue,
+                    process_mode,
                     extracted_whitespace,
-                    extra_whitespace_after_setext,
+                    parsed_lrd_tuple,
                 )
-        else:
+
+            assert extracted_whitespace is not None
+            assert parsed_lrd_tuple.normalized_destination is not None
+            new_tokens: List[MarkdownToken] = [
+                LinkReferenceDefinitionMarkdownToken(
+                    did_add_definition,
+                    extracted_whitespace,
+                    parsed_lrd_tuple.normalized_destination,
+                    parsed_lrd_tuple.link_titles,
+                    parsed_lrd_tuple.link_info,
+                    position_marker=link_def_token.start_position_marker,
+                )
+            ]
+            POGGER.debug(">>link_info>>$", parsed_lrd_tuple.link_info)
+            assert parsed_lrd_tuple.link_info.line_destination_whitespace is not None
             POGGER.debug(
-                "parse_setext_headings>>not eligible",
+                ">>line_destination_whitespace>>$",
+                ParserHelper.make_whitespace_visible(
+                    parsed_lrd_tuple.link_info.line_destination_whitespace
+                ),
             )
-        return new_tokens
+            POGGER.debug(">>new_tokens>>$", new_tokens)
+            del parser_state.token_stack[-1]
+            return did_pause_lrd, len(lines_to_requeue) > 1, new_tokens
+
+        assert is_blank_line
+        del parser_state.token_stack[-1]
+        return did_pause_lrd, True, []
+
+    # pylint: enable=too-many-arguments
 
     @staticmethod
-    def __adjust_continuation_for_active_list(
-        parser_state: ParserState, position_marker: PositionMarker
-    ) -> bool:
-        is_paragraph_continuation: bool = (
-            len(parser_state.token_stack) > 1 and parser_state.token_stack[-2].is_list
-        )
-        if is_paragraph_continuation:
-            list_token = cast(ListStackToken, parser_state.token_stack[-2])
-            POGGER.debug(
-                "parser_state.original_line_to_parse>:$:<",
-                parser_state.original_line_to_parse,
-            )
-            adj_text = position_marker.text_to_parse[position_marker.index_number :]
-            assert parser_state.original_line_to_parse is not None
-            assert parser_state.original_line_to_parse.endswith(adj_text)
-            removed_text_length = len(parser_state.original_line_to_parse) - len(
-                adj_text
-            )
-            POGGER.debug("removed_text_length>:$:<", removed_text_length)
-            POGGER.debug("adj_text>:$:<", adj_text)
-            POGGER.debug("indent_level>:$:<", list_token.indent_level)
-            is_paragraph_continuation = (
-                bool(adj_text) and removed_text_length < list_token.indent_level
-            )
-        return is_paragraph_continuation
+    def __find_line_ws(parsed_lines: str, original_lines: str) -> Tuple[str, bool, int]:
+        start_text_index = original_lines.find(parsed_lines)
+        assert start_text_index != -1
+        POGGER.debug("start_text_index>:$:<", start_text_index)
+        start_whitespace_index, _ = ParserHelper.extract_spaces_from_end(
+            original_lines, start_text_index
+        )
+        POGGER.debug("start_whitespace_index>:$:<", start_whitespace_index)
+        tabified_whitespace = original_lines[start_whitespace_index:start_text_index]
+        POGGER.debug("tabified_whitespace>:$:<", tabified_whitespace)
+        split_tab = bool(tabified_whitespace and tabified_whitespace[0] == "\t")
+        if not split_tab:
+            tabified_whitespace = tabified_whitespace[1:]
+            start_whitespace_index += 1
+        extracted_whitespace = tabified_whitespace
+        POGGER.debug("extracted_whitespace>:$:<", extracted_whitespace)
+        POGGER.debug("split_tab>:$:<", split_tab)
+        return extracted_whitespace, split_tab, start_whitespace_index
 
     # pylint: disable=too-many-arguments
     @staticmethod
-    def __create_setext_token(
+    def __stop_lrd_continuation_with_tab(
         parser_state: ParserState,
-        position_marker: PositionMarker,
-        collected_to_index: int,
-        new_tokens: List[MarkdownToken],
+        link_def_token: LinkDefinitionStackToken,
+        last_container_index: int,
+        lines_to_requeue: List[str],
+        process_mode: int,
         extracted_whitespace: Optional[str],
-        extra_whitespace_after_setext: Optional[str],
-    ) -> None:
-        token_index = len(parser_state.token_document) - 1
-        while not parser_state.token_document[token_index].is_paragraph:
-            token_index -= 1
-
-        paragraph_token = cast(
-            ParagraphMarkdownToken, parser_state.token_document[token_index]
-        )
-        assert paragraph_token.extra_data is not None
-        replacement_token = SetextHeadingMarkdownToken(
-            position_marker.text_to_parse[position_marker.index_number],
-            collected_to_index - position_marker.index_number,
-            paragraph_token.extra_data,
-            position_marker,
-            paragraph_token,
+        parsed_lrd_tuple: LinkReferenceDefinitionTuple,
+    ) -> Tuple[Optional[str], LinkReferenceDefinitionTuple]:
+        POGGER.debug(
+            "extracted_whitespace>:$:<",
+            link_def_token.extracted_whitespace,
         )
+        assert parser_state.token_stack[last_container_index].is_block_quote
+        # POGGER.debug("link_def_token>:$:<", link_def_token)
+        # POGGER.debug("link_def_token.last_block_quote_stack_token>:$:<", link_def_token.last_block_quote_stack_token)
+        last_block_quote_index = parser_state.find_last_block_quote_on_stack()
+        last_block_quote_token = parser_state.token_stack[last_block_quote_index]
+        # POGGER.debug("last_block_quote_token>:$:<", last_block_quote_token)
+        block_quote_token = cast(
+            BlockQuoteMarkdownToken, last_block_quote_token.matching_markdown_token
+        )
+        # POGGER.debug("block_quote_token.leading_spaces>:$:<", block_quote_token.leading_spaces)
 
-        # This is unusual.  Normally, close_open_blocks is used to close off
-        # blocks based on the stack token.  However, since the setext takes
-        # the last paragraph of text (see case 61) and translates it
-        # into a heading, this has to be done separately, as there is no
-        # stack token to close.
-        assert extra_whitespace_after_setext is not None
-        assert extracted_whitespace is not None
-        new_tokens.append(
-            replacement_token.generate_close_markdown_token_from_markdown_token(
-                extracted_whitespace, extra_whitespace_after_setext
-            )
+        POGGER.debug(
+            "link_def_token.continuation_lines>:$:<", link_def_token.continuation_lines
+        )
+        POGGER.debug(
+            "link_def_token.unmodified_lines>:$:<", link_def_token.unmodified_lines
         )
 
-        parser_state.token_document[token_index] = replacement_token
-        del parser_state.token_stack[-1]
+        if len(link_def_token.continuation_lines) == 1:
+            extracted_whitespace = (
+                LinkReferenceDefinitionHelper.__stop_lrd_continuation_with_tab_single(
+                    parser_state,
+                    link_def_token,
+                    process_mode,
+                    block_quote_token,
+                    lines_to_requeue,
+                )
+            )
+        else:
+            (
+                extracted_whitespace,
+                parsed_lrd_tuple,
+            ) = LinkReferenceDefinitionHelper.__stop_lrd_continuation_with_tab_multiple(
+                parser_state, extracted_whitespace, link_def_token, block_quote_token
+            )
+
+        return extracted_whitespace, parsed_lrd_tuple
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
-    def correct_for_leaf_block_start_in_list(
+    def __stop_lrd_continuation_with_tab_single(
         parser_state: ParserState,
-        removed_chars_at_start: int,
-        old_top_of_stack_token: StackToken,
-        html_tokens: List[MarkdownToken],
-        was_token_already_added_to_stack: bool = True,
-    ) -> None:
-        """
-        Check to see that if a paragraph has been closed within a list and
-        there is a leaf block token immediately following, that the right
-        actions are taken.
-        """
+        link_def_token: LinkDefinitionStackToken,
+        process_mode: int,
+        block_quote_token: BlockQuoteMarkdownToken,
+        lines_to_requeue: List[str],
+    ) -> str:
+        parsed_lines = link_def_token.continuation_lines[0]
+        original_lines = link_def_token.unmodified_lines[0]
+        # POGGER.debug("parsed_lines>:$:<", parsed_lines)
+        # POGGER.debug("original_lines>:$:<", original_lines)
 
-        POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>removed_chars_at_start>$>>",
-            removed_chars_at_start,
-        )
-        if not old_top_of_stack_token.is_paragraph:
-            POGGER.debug("1")
-            return
-
-        statck_index, top_of_stack, end_of_list = (
-            -2 if was_token_already_added_to_stack else -1,
-            None,
-            html_tokens[-1],
-        )
-        if not parser_state.token_stack[statck_index].is_list:
-            POGGER.debug("2")
-            return
+        (
+            extracted_whitespace,
+            split_tab,
+            _,
+        ) = LinkReferenceDefinitionHelper.__find_line_ws(parsed_lines, original_lines)
 
+        POGGER.debug("process_mode>:$:<", process_mode)
         POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>stack>>$>>",
-            parser_state.token_stack,
-        )
-        POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>tokens>>$>>",
-            parser_state.token_document,
+            "block_quote_token.leading_spaces>:$:<", block_quote_token.bleading_spaces
         )
+        if process_mode == 1:
+            block_quote_token.remove_last_bleading_space()
+            # POGGER.debug("block_quote_token.leading_spaces>:$:<", block_quote_token.leading_spaces)
+        else:
+            # POGGER.debug("lines_to_requeue>:$:<", lines_to_requeue)
+            for _ in lines_to_requeue:
+                # POGGER.debug("block_quote_token.leading_spaces>:$:<", block_quote_token.leading_spaces)
+                block_quote_token.remove_last_bleading_space()
+                # POGGER.debug("block_quote_token.leading_spaces>:$:<", block_quote_token.leading_spaces)
+
+        # POGGER.debug("block_quote_token.leading_spaces>:$:<", block_quote_token.leading_spaces)
+        if split_tab:
+            TabHelper.adjust_block_quote_indent_for_tab(parser_state)
         POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>tokens_to_add>>$>>", html_tokens
+            "block_quote_token.leading_spaces>:$:<", block_quote_token.bleading_spaces
         )
+        return extracted_whitespace
 
-        if was_token_already_added_to_stack:
-            top_of_stack = parser_state.token_stack[-1]
-            del parser_state.token_stack[-1]
-        del html_tokens[-1]
+    @staticmethod
+    def __stop_lrd_continuation_with_tab_multiple(
+        parser_state: ParserState,
+        extracted_whitespace: Optional[str],
+        link_def_token: LinkDefinitionStackToken,
+        block_quote_token: BlockQuoteMarkdownToken,
+    ) -> Tuple[Optional[str], LinkReferenceDefinitionTuple]:
+        split_tabs_list: List[bool] = []
+        completed_lrd_text: str = ""
+        alt_ws: Optional[str] = None
+        for this_line_index, this_line in enumerate(link_def_token.continuation_lines):
+            (
+                completed_lrd_text,
+                extracted_whitespace,
+                alt_ws,
+            ) = LinkReferenceDefinitionHelper.__stop_lrd_continuation_with_tab_multiple_loop(
+                link_def_token,
+                this_line_index,
+                this_line,
+                completed_lrd_text,
+                extracted_whitespace,
+                alt_ws,
+                split_tabs_list,
+            )
 
-        LeafBlockProcessor.__handle_leaf_start(
-            parser_state, removed_chars_at_start, html_tokens
+        POGGER.debug("completed_lrd_text>:$:<", completed_lrd_text)
+        (
+            did_succeed,
+            next_index,
+            new_parsed_lrd_tuple,
+        ) = LinkReferenceDefinitionHelper.__parse_link_reference_definition(
+            parser_state, completed_lrd_text, 0, alt_ws, True
+        )
+        assert did_succeed
+        assert len(completed_lrd_text) == next_index
+        # POGGER.debug("new_parsed_lrd_tuple>:$:<", new_parsed_lrd_tuple)
+        assert new_parsed_lrd_tuple is not None
+        parsed_lrd_tuple = new_parsed_lrd_tuple
+
+        LinkReferenceDefinitionHelper.__xx_multiple_fix_leading_spaces(
+            block_quote_token, split_tabs_list, link_def_token
         )
+        return extracted_whitespace, parsed_lrd_tuple
 
-        if was_token_already_added_to_stack:
-            assert top_of_stack is not None
-            parser_state.token_stack.append(top_of_stack)
-            POGGER.debug(
-                ">>correct_for_leaf_block_start_in_list>>stack>>$>>",
-                parser_state.token_stack,
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __stop_lrd_continuation_with_tab_multiple_loop(
+        link_def_token: LinkDefinitionStackToken,
+        this_line_index: int,
+        this_line: str,
+        completed_lrd_text: str,
+        extracted_whitespace: Optional[str],
+        alt_ws: Optional[str],
+        split_tabs_list: List[bool],
+    ) -> Tuple[str, Optional[str], Optional[str]]:
+        original_this_line = link_def_token.unmodified_lines[this_line_index]
+        POGGER.debug("this_line_index>:$:<", this_line_index)
+        POGGER.debug("this_line>:$:<", this_line)
+        POGGER.debug("original_this_line>:$:<", original_this_line)
+
+        (
+            extracted_ws,
+            split_tab,
+            start_whitespace_index,
+        ) = LinkReferenceDefinitionHelper.__find_line_ws(this_line, original_this_line)
+
+        if completed_lrd_text:
+            completed_lrd_text += "\n"
+        if this_line_index == 0:
+            extracted_whitespace = extracted_ws
+            alt_ws = TabHelper.detabify_string(
+                extracted_whitespace, start_whitespace_index
             )
-        html_tokens.append(end_of_list)
-        POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>tokens_to_add>>$>>", html_tokens
-        )
+        else:
+            completed_lrd_text += extracted_ws
+        completed_lrd_text += this_line
+        split_tabs_list.append(split_tab)
+        return completed_lrd_text, extracted_whitespace, alt_ws
+
+    # pylint: enable=too-many-arguments
 
     @staticmethod
-    def __handle_leaf_start(
-        parser_state: ParserState,
-        removed_chars_at_start: int,
-        html_tokens: List[MarkdownToken],
+    def __xx_multiple_fix_leading_spaces(
+        block_quote_token: BlockQuoteMarkdownToken,
+        split_tabs_list: List[bool],
+        link_def_token: LinkDefinitionStackToken,
     ) -> None:
+        POGGER.debug("split_tabs_list>:$:<", split_tabs_list)
         POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>stack>>$>>",
-            parser_state.token_stack,
+            "block_quote_token.leading_spaces>:$:<", block_quote_token.bleading_spaces
         )
+        assert block_quote_token.bleading_spaces is not None
+        leading_spaces: List[str] = []
+        for _ in link_def_token.continuation_lines:
+            last_leading_space = block_quote_token.remove_last_bleading_space()
+            POGGER.debug("last_leading_space>:$:<", last_leading_space)
+            if last_leading_space[0] == "\n":
+                last_leading_space = last_leading_space[1:]
+            leading_spaces.append(last_leading_space)
+        assert len(split_tabs_list) == len(leading_spaces)
+        POGGER.debug("leading_spaces>:$:<", leading_spaces)
         POGGER.debug(
-            ">>correct_for_leaf_block_start_in_list>>tokens_to_add>>$>>", html_tokens
+            "block_quote_token.leading_spaces>:$:<", block_quote_token.bleading_spaces
         )
+        is_first = len(block_quote_token.bleading_spaces) == 0
+        for prefix_to_add in leading_spaces:
+            if split_tabs_list[0]:
+                prefix_to_add = prefix_to_add[:-1]
+            del split_tabs_list[0]
+            block_quote_token.add_bleading_spaces(prefix_to_add, is_first)
+            is_first = False
 
-        is_remaining_list_token = True
-        while is_remaining_list_token:
-            assert parser_state.token_stack[-1].is_list
-            list_stack_token = cast(ListStackToken, parser_state.token_stack[-1])
-
-            POGGER.debug(">>removed_chars_at_start>>$>>", removed_chars_at_start)
-            POGGER.debug(">>stack indent>>$>>", list_stack_token.indent_level)
-            if removed_chars_at_start >= list_stack_token.indent_level:
-                break  # pragma: no cover
+    @staticmethod
+    def __process_lrd_hard_failure(
+        parser_state: ParserState,
+        remaining_line_to_parse: str,
+        lines_to_requeue: List[str],
+        unmodified_line_to_parse: str,
+    ) -> Tuple[
+        Optional[bool],
+        Optional[str],
+        Optional[bool],
+        Optional[int],
+        Optional[LinkReferenceDefinitionTuple],
+    ]:
+        """
+        In cases of a hard failure, we have had continuations to the original line
+        that make it a bit more difficult to figure out if we have an actual good
+        LRD in the mix somehow.  So take lines off the end while we have lines.
+        """
+        (
+            is_blank_line,
+            line_to_parse,
+            did_complete_lrd,
+            end_lrd_index,
+            parsed_lrd_tuple,
+        ) = (None, None, None, None, None)
+        link_ref_stack_token = cast(
+            LinkDefinitionStackToken, parser_state.token_stack[-1]
+        )
 
-            tokens_from_close, _ = parser_state.close_open_blocks_fn(
-                parser_state,
-                until_this_index=(len(parser_state.token_stack) - 1),
-                include_lists=True,
+        POGGER.debug(">>remaining_line_to_parse>>add>:$<<", remaining_line_to_parse)
+        POGGER.debug(">>unmodified_line_to_parse>>add>:$<<", unmodified_line_to_parse)
+        assert unmodified_line_to_parse.endswith(remaining_line_to_parse)
+        link_ref_stack_token.add_continuation_line(remaining_line_to_parse)
+        link_ref_stack_token.add_unmodified_line(unmodified_line_to_parse)
+        while link_ref_stack_token.continuation_lines:
+            POGGER.debug(
+                "continuation_lines>>$<<",
+                ParserHelper.make_whitespace_visible(
+                    str(link_ref_stack_token.continuation_lines)
+                ),
             )
             POGGER.debug(
-                ">>correct_for_leaf_block_start_in_list>>tokens_from_close>>$>>",
-                tokens_from_close,
+                "unmodified_lines>>$<<",
+                ParserHelper.make_whitespace_visible(
+                    str(link_ref_stack_token.unmodified_lines)
+                ),
             )
-            html_tokens.extend(tokens_from_close)
 
-            is_remaining_list_token = parser_state.token_stack[-1].is_list
-        if is_remaining_list_token:
-            assert parser_state.token_stack[-1].is_list
-            list_stack_token = cast(ListStackToken, parser_state.token_stack[-1])
-            delta_indent = removed_chars_at_start - list_stack_token.indent_level
+            lines_to_requeue.append(link_ref_stack_token.unmodified_lines[-1])
             POGGER.debug(
-                ">>correct_for_leaf_block_start_in_list>>delta_indent>>$>>",
-                delta_indent,
+                ">>continuation_line>>$",
+                link_ref_stack_token.continuation_lines[-1],
             )
-            assert not delta_indent
-
-    @staticmethod
-    def is_paragraph_ending_leaf_block_start(
-        parser_state: ParserState,
-        line_to_parse: str,
-        start_index: int,
-        extracted_whitespace: Optional[str],
-        exclude_thematic_break: bool = False,
-    ) -> bool:
-        """
-        Determine whether we have a valid leaf block start.
-        """
-
-        is_leaf_block_start = not exclude_thematic_break
-        assert not exclude_thematic_break
-
-        is_thematic_break_start, _ = LeafBlockProcessor.is_thematic_break(
-            line_to_parse,
-            start_index,
-            extracted_whitespace,
-            skip_whitespace_check=True,
-        )
-        is_leaf_block_start = bool(is_thematic_break_start)
-        POGGER.debug(
-            "is_paragraph_ending_leaf_block_start>>is_theme_break>>$",
-            is_leaf_block_start,
-        )
-        if not is_leaf_block_start:
-            is_html_block_start, _ = HtmlHelper.is_html_block(
-                line_to_parse,
-                start_index,
-                extracted_whitespace,
-                parser_state.token_stack,
+            POGGER.debug(
+                ">>unmodified_line>>$",
+                link_ref_stack_token.unmodified_lines[-1],
             )
-            is_leaf_block_start = bool(is_html_block_start)
+            del link_ref_stack_token.continuation_lines[-1]
+            del link_ref_stack_token.unmodified_lines[-1]
             POGGER.debug(
-                "is_paragraph_ending_leaf_block_start>>is_html_block>>$",
-                is_leaf_block_start,
+                ">>lines_to_requeue>>$>>",
+                lines_to_requeue,
             )
-        if not is_leaf_block_start:
-            is_leaf_block_start, _, _, _, _ = LeafBlockProcessor.is_fenced_code_block(
-                line_to_parse, start_index, extracted_whitespace
+            POGGER.debug(
+                ">>continuation_lines>>$<<",
+                link_ref_stack_token.continuation_lines,
             )
             POGGER.debug(
-                "is_paragraph_ending_leaf_block_start>>is_fenced_code_block>>$",
-                is_leaf_block_start,
+                ">>unmodified_lines>>$<<",
+                link_ref_stack_token.unmodified_lines,
             )
-        if not is_leaf_block_start:
-            is_leaf_block_start, _, _, _ = LeafBlockProcessor.is_atx_heading(
-                line_to_parse, start_index, extracted_whitespace
+            (
+                is_blank_line,
+                line_to_parse,
+            ) = True, link_ref_stack_token.add_joined_lines_before_suffix("")
+            line_to_parse = line_to_parse[:-1]
+            start_index, extracted_whitespace = ParserHelper.extract_spaces(
+                line_to_parse, 0
+            )
+            assert start_index is not None
+            POGGER.debug(">>line_to_parse>>$<<", line_to_parse)
+            (
+                did_complete_lrd,
+                end_lrd_index,
+                parsed_lrd_tuple,
+            ) = LinkReferenceDefinitionHelper.__parse_link_reference_definition(
+                parser_state,
+                line_to_parse,
+                start_index,
+                extracted_whitespace,
+                is_blank_line,
             )
             POGGER.debug(
-                "is_paragraph_ending_leaf_block_start>>is_atx_heading>>$",
-                is_leaf_block_start,
+                ">>parse_link_reference_definition>>was_started>>did_complete_lrd>>$"
+                + ">>end_lrd_index>>$>>len(line_to_parse)>>$",
+                did_complete_lrd,
+                end_lrd_index,
+                len(line_to_parse),
             )
+            if did_complete_lrd:
+                break
+        return (
+            is_blank_line,
+            line_to_parse,
+            did_complete_lrd,
+            end_lrd_index,
+            parsed_lrd_tuple,
+        )
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def handle_link_reference_definition_leaf_block(
+        parser_state: ParserState,
+        outer_processed: bool,
+        position_marker: PositionMarker,
+        leaf_token_whitespace: Optional[str],
+        remaining_line_to_parse: str,
+        ignore_link_definition_start: bool,
+        pre_tokens: List[MarkdownToken],
+        original_line: str,
+    ) -> Tuple[bool, Optional[RequeueLineInfo]]:
+        """
+        Take care of the processing for link reference definitions.
+        """
         POGGER.debug(
-            "is_paragraph_ending_leaf_block_start<<$",
-            is_leaf_block_start,
+            "handle_link_reference_definition>>pre_tokens>>$<<",
+            pre_tokens,
         )
-        return is_leaf_block_start
+
+        if not outer_processed and not ignore_link_definition_start:
+            POGGER.debug(
+                "plflb-process_link_reference_definition>>outer_processed>>$",
+                position_marker.text_to_parse[position_marker.index_number :],
+            )
+            assert parser_state.original_line_to_parse is not None
+            (
+                outer_processed,
+                _,  # did_complete_lrd,
+                _,  # did_pause_lrd,
+                requeue_line_info,
+                new_tokens,
+            ) = LinkReferenceDefinitionHelper.process_link_reference_definition(
+                parser_state,
+                position_marker,
+                remaining_line_to_parse,
+                leaf_token_whitespace,
+                parser_state.original_line_to_parse,
+                parser_state.original_stack_depth,
+                parser_state.original_document_depth,
+                original_line,
+                0,
+            )
+            if requeue_line_info:
+                outer_processed = True
+                POGGER.debug(
+                    "plflb-process_link_reference_definition>>outer_processed>>$<lines_to_requeue<$<$",
+                    outer_processed,
+                    requeue_line_info.lines_to_requeue,
+                    len(requeue_line_info.lines_to_requeue),
+                )
+            else:
+                POGGER.debug(
+                    "plflb-process_link_reference_definition>>outer_processed>>$<lines_to_requeue<(None)",
+                    outer_processed,
+                )
+        else:
+            requeue_line_info, new_tokens = None, []
+
+        POGGER.debug("handle_link_reference_definition>>pre_tokens>>$<<", pre_tokens)
+        pre_tokens.extend(new_tokens)
+        POGGER.debug("handle_link_reference_definition>>pre_tokens>>$<<", pre_tokens)
+        return outer_processed, requeue_line_info
+
+    # pylint: enable=too-many-arguments
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/leaf_markdown_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/leaf_markdown_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
     def __init__(
         self,
         extracted_whitespace: str,
         position_marker: Optional[PositionMarker],
         column_delta: int = 0,
     ) -> None:
-
         if position_marker:
             line_number, column_number = position_marker.line_number, (
                 position_marker.index_number
                 + position_marker.index_indent
                 + 1
                 - column_delta
             )
@@ -268,42 +267,46 @@
                 self.__link_destination_whitespace,
                 self.__link_destination_raw,
                 self.__link_title_whitespace,
                 self.__link_title_raw,
                 self.__end_whitespace,
             ) = ("", "", "", "", "", "")
 
+        extra_data = self.__validate_proper_fields_are_valid(extracted_whitespace)
+        LeafMarkdownToken.__init__(
+            self,
+            MarkdownToken._token_link_reference_definition,
+            extra_data,
+            position_marker=position_marker,
+            extracted_whitespace=extracted_whitespace,
+        )
+
+    def __validate_proper_fields_are_valid(self, extracted_whitespace: str) -> str:
         assert self.__end_whitespace is not None
         assert self.__link_title_raw is not None
         assert self.__link_title is not None
         assert self.__link_title_whitespace is not None
         assert self.__link_destination_raw is not None
         assert self.__link_destination is not None
         assert self.__link_destination_whitespace is not None
         assert self.__link_name_debug is not None
-        LeafMarkdownToken.__init__(
-            self,
-            MarkdownToken._token_link_reference_definition,
-            MarkdownToken.extra_data_separator.join(
-                [
-                    str(self.did_add_definition),
-                    extracted_whitespace,
-                    self.__link_name,
-                    self.__link_name_debug,
-                    self.__link_destination_whitespace,
-                    self.__link_destination,
-                    self.__link_destination_raw,
-                    self.__link_title_whitespace,
-                    self.__link_title,
-                    self.__link_title_raw,
-                    self.__end_whitespace,
-                ]
-            ),
-            position_marker=position_marker,
-            extracted_whitespace=extracted_whitespace,
+        return MarkdownToken.extra_data_separator.join(
+            [
+                str(self.did_add_definition),
+                extracted_whitespace,
+                self.__link_name,
+                self.__link_name_debug,
+                self.__link_destination_whitespace,
+                self.__link_destination,
+                self.__link_destination_raw,
+                self.__link_title_whitespace,
+                self.__link_title,
+                self.__link_title_raw,
+                self.__end_whitespace,
+            ]
         )
 
     # pylint: enable=too-many-arguments
     @property
     def did_add_definition(self) -> bool:
         """
         Returns an indication of whether the definition was actually added.
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/link_helper.py` & `pymarkdownlnt-0.9.9/pymarkdown/link_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     LinkStartMarkdownToken,
     RawHtmlMarkdownToken,
     ReferenceMarkdownToken,
     SpecialTextMarkdownToken,
     TextMarkdownToken,
 )
 from pymarkdown.inline_request import InlineRequest
+from pymarkdown.link_helper_properties import LinkHelperProperties
 from pymarkdown.link_reference_titles import LinkReferenceTitles
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.parser_logger import ParserLogger
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
@@ -198,43 +199,49 @@
             pre_inline_title,
             ex_ws,
             line_to_parse[start_index:new_index],
         )
 
     @staticmethod
     def extract_link_destination(
-        line_to_parse: str, new_indexx: int, is_blank_line: bool
+        line_to_parse: str, start_index: int, is_blank_line: bool
     ) -> Tuple[
         bool, Optional[int], Optional[str], Optional[str], Optional[str], Optional[str]
     ]:
         """
         Extract the link reference definition's link destination.
         """
-        # TODO if new_index recomputed, why being passed?
-        new_index: Optional[int] = None
-        new_index, prefix_whitespace = ParserHelper.collect_while_one_of_characters(
-            line_to_parse, new_indexx, Constants.ascii_whitespace
+        after_whitespace_index: Optional[int] = None
+        (
+            after_whitespace_index,
+            prefix_whitespace,
+        ) = ParserHelper.collect_while_one_of_characters(
+            line_to_parse, start_index, Constants.ascii_whitespace
         )
-        assert new_index is not None
-        if new_index == len(line_to_parse) and not is_blank_line:
-            return False, new_index, None, None, None, None
+        assert after_whitespace_index is not None
+        if after_whitespace_index == len(line_to_parse) and not is_blank_line:
+            return False, after_whitespace_index, None, None, None, None
 
-        POGGER.debug("LD>>$<<", line_to_parse[new_index:])
+        assert prefix_whitespace is not None
+        POGGER.debug(
+            "Pre-LD>>$<<", ParserHelper.make_whitespace_visible(prefix_whitespace)
+        )
+        POGGER.debug("LD>>$<<", line_to_parse[after_whitespace_index:])
         (
             inline_link,
             pre_inline_link,
-            new_index,
+            after_whitespace_index,
             inline_raw_link,
             _,
-        ) = LinkHelper.__parse_link_destination(line_to_parse, new_index)
-        if new_index == -1:
+        ) = LinkHelper.__parse_link_destination(line_to_parse, after_whitespace_index)
+        if after_whitespace_index == -1:
             return False, -1, None, None, None, None
         return (
             True,
-            new_index,
+            after_whitespace_index,
             inline_link,
             pre_inline_link,
             prefix_whitespace,
             inline_raw_link,
         )
 
     @staticmethod
@@ -259,43 +266,47 @@
     # pylint: disable=too-many-arguments
     @staticmethod
     def look_for_link_or_image(
         inline_blocks: List[MarkdownToken],
         source_text: str,
         next_index: int,
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: str,
         xx_fn: Callable[[str], str],
+        tabified_text: Optional[str],
     ) -> Tuple[int, bool, Optional[MarkdownToken], bool]:
         """
         Given that a link close character has been found, process it to see if
         there is actually enough other text to properly construct the link.
         """
 
         POGGER.debug(
             ">>look_for_link_or_image>>$<<",
             inline_blocks,
         )
         POGGER.debug(">>source_text>>$<<", source_text)
+        POGGER.debug(">>tabified_text>>$<<", tabified_text)
         POGGER.debug(">>next_index>>$<<", next_index)
         POGGER.debug(">>remaining_line>>$<<", remaining_line)
+        POGGER.debug(">>tabified_remaining_line>>$<<", tabified_remaining_line)
         POGGER.debug(
             ">>current_string_unresolved>>$<<",
             current_string_unresolved,
         )
-        is_valid, consume_rest_of_line, new_index, updated_index = (
+        is_valid, consume_rest_of_line, next_index, updated_index = (
             False,
             False,
             next_index + 1,
             -1,
         )
         token_to_append: Optional[MarkdownToken] = None
 
         POGGER.debug("LOOKING FOR START")
-        LinkHelper.__display_specials_in_tokens(inline_blocks)
+        LinkHelper.__debug_log_specials_in_tokens(inline_blocks)
 
         valid_special_start_text, search_index = None, len(inline_blocks) - 1
         while search_index >= 0:
             if inline_blocks[search_index].is_special_text:
                 (
                     is_done,
                     is_valid,
@@ -303,19 +314,21 @@
                     token_to_append,
                     consume_rest_of_line,
                     valid_special_start_text,
                 ) = LinkHelper.__find_link(
                     inline_blocks,
                     search_index,
                     source_text,
-                    new_index,
+                    next_index,
                     remaining_line,
+                    tabified_remaining_line,
                     current_string_unresolved,
                     xx_fn,
                     updated_index,
+                    tabified_text,
                 )
                 if is_done:
                     break
                 POGGER.debug("  not link")
             search_index -= 1
 
         POGGER.debug(
@@ -326,15 +339,15 @@
         )
         if is_valid:
             assert valid_special_start_text is not None
             LinkHelper.__deactivate_used_tokens(
                 inline_blocks, search_index, valid_special_start_text
             )
             return updated_index, True, token_to_append, consume_rest_of_line
-        return new_index, False, token_to_append, consume_rest_of_line
+        return next_index, False, token_to_append, consume_rest_of_line
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
     def __deactivate_used_tokens(
         inline_blocks: List[MarkdownToken],
         search_index: int,
@@ -360,74 +373,77 @@
         POGGER.debug(
             "resolve_inline_emphasis>>$\n",
             inline_blocks,
         )
 
         if valid_special_start_text == LinkHelper.__link_start_sequence:
             POGGER.debug("DEACTIVATING")
-            LinkHelper.__display_specials_in_tokens(inline_blocks)
+            LinkHelper.__debug_log_specials_in_tokens(inline_blocks)
             for deactivate_token in inline_blocks:
                 if deactivate_token.is_special_text:
                     special_token = cast(SpecialTextMarkdownToken, deactivate_token)
                     POGGER.debug("inline_blocks>>>>>>>>>>>>>>>>>>$", special_token)
                     if special_token.token_text == LinkHelper.__link_start_sequence:
                         special_token.deactivate()
             POGGER.debug("DEACTIVATED")
-            LinkHelper.__display_specials_in_tokens(inline_blocks)
+            LinkHelper.__debug_log_specials_in_tokens(inline_blocks)
 
-    # pylint: disable=too-many-arguments
+    # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __find_link(
         inline_blocks: List[MarkdownToken],
         search_index: int,
         source_text: str,
         new_index: int,
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: str,
         xx_fn: Callable[[str], str],
         updated_index: int,
+        tabified_text: Optional[str],
     ) -> Tuple[bool, bool, int, Optional[MarkdownToken], bool, Optional[str]]:
         special_text_token = cast(SpecialTextMarkdownToken, inline_blocks[search_index])
-        if POGGER.is_debug_enabled:
-            POGGER.debug(
-                "search_index>>$>>$",
-                search_index,
-                special_text_token.show_process_emphasis(),
-            )
+        # POGGER.debug(
+        #     "search_index>>$>>$",
+        #     search_index,
+        #     special_text_token.show_process_emphasis(),
+        # )
 
         (
             is_done,
             consume_rest_of_line,
             is_valid,
         ) = (False, False, False)
         token_to_append: Optional[MarkdownToken] = None
         if special_text_token.token_text in LinkHelper.__valid_link_starts:
             valid_special_start_text: Optional[str] = special_text_token.token_text
             if special_text_token.is_active:
-                POGGER.debug(">>>>>>$", inline_blocks)
+                # POGGER.debug(">>>>>>$", inline_blocks)
                 assert valid_special_start_text is not None
                 (
                     updated_index,
                     token_to_append,
                     consume_rest_of_line,
                 ) = LinkHelper.__handle_link_types(
                     inline_blocks,
                     search_index,
                     source_text,
                     new_index,
                     valid_special_start_text,
                     remaining_line,
+                    tabified_remaining_line,
                     current_string_unresolved,
                     xx_fn,
+                    tabified_text,
                 )
                 if updated_index != -1:
                     is_valid, is_done = True, True
 
             if not is_done:
-                POGGER.debug("  not active:$", search_index)
+                # POGGER.debug("  not active:$", search_index)
                 LinkHelper.__revert_token_to_normal_text_token(
                     inline_blocks, search_index
                 )
                 is_done = True
         else:
             valid_special_start_text = None
         return (
@@ -435,38 +451,38 @@
             is_valid,
             updated_index,
             token_to_append,
             consume_rest_of_line,
             valid_special_start_text,
         )
 
-    # pylint: enable=too-many-arguments
+    # pylint: enable=too-many-arguments, too-many-locals
 
     @staticmethod
     def __revert_token_to_normal_text_token(
         inline_blocks: List[MarkdownToken], search_index: int
     ) -> None:
         """
         Revert this token from a special text token back to a normal text token.
         """
 
         POGGER.debug("REVERTING")
-        LinkHelper.__display_specials_in_tokens(inline_blocks)
+        LinkHelper.__debug_log_specials_in_tokens(inline_blocks)
 
         text_token_to_replace = cast(
             SpecialTextMarkdownToken, inline_blocks[search_index]
         )
         inline_blocks.insert(search_index, text_token_to_replace.create_copy())
         del inline_blocks[search_index + 1]
 
         POGGER.debug("REVERTED")
-        LinkHelper.__display_specials_in_tokens(inline_blocks)
+        LinkHelper.__debug_log_specials_in_tokens(inline_blocks)
 
     @staticmethod
-    def __display_specials_in_tokens(inline_blocks: List[MarkdownToken]) -> None:
+    def __debug_log_specials_in_tokens(inline_blocks: List[MarkdownToken]) -> None:
         display_parts = []
         for deactivate_token in inline_blocks:
             if deactivate_token.is_special_text:
                 special_token = cast(SpecialTextMarkdownToken, deactivate_token)
                 display_parts.extend(
                     [
                         f",>>Spec:{special_token.is_active}:{deactivate_token}<<",
@@ -491,19 +507,17 @@
 
         inline_blocks_size, ind_plus_one = len(inline_blocks), ind + 1
 
         POGGER.debug("inline_blocks_size>>$<<", inline_blocks_size)
         POGGER.debug("ind>>$<<", ind)
         POGGER.debug(">>$<<", inline_blocks[ind_plus_one:])
         if inline_blocks_size > (ind_plus_one):
-
             alt_text_parts: List[str] = []
 
             while inline_blocks_size > ind_plus_one:
-
                 LinkHelper.__handle_next_alt_text(
                     inline_blocks, ind_plus_one, alt_text_parts
                 )
 
                 del inline_blocks[ind_plus_one]
                 inline_blocks_size -= 1
 
@@ -520,142 +534,227 @@
             POGGER.debug(">>composed>>$>>", image_alt_text)
 
         POGGER.debug(">>image_alt_text>>$>>", image_alt_text)
         POGGER.debug(">>text_from_blocks_raw>>$>>", text_from_blocks_raw)
         return image_alt_text, text_from_blocks_raw
 
     @staticmethod
+    def __handle_next_alt_text_special_text(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        text_token = cast(TextMarkdownToken, (next_token))
+        if text_token.token_text == "]":
+            alt_text_parts.append(text_token.token_text)
+
+    @staticmethod
+    def __handle_next_alt_text_normal_text(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        text_token = cast(TextMarkdownToken, next_token)
+        alt_text_parts.append(ParserHelper.resolve_all_from_text(text_token.token_text))
+
+    @staticmethod
+    def __handle_next_alt_text_raw_html(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        rawhtml_token = cast(RawHtmlMarkdownToken, next_token)
+        alt_text_parts.extend(["<", rawhtml_token.raw_tag, ">"])
+
+    @staticmethod
+    def __handle_next_alt_text_code_span(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        codespan_token = cast(InlineCodeSpanMarkdownToken, next_token)
+        alt_text_parts.append(
+            ParserHelper.resolve_all_from_text(codespan_token.span_text)
+        )
+
+    @staticmethod
+    def __handle_next_alt_text_auto_link(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        autolink_token = cast(EmailAutolinkMarkdownToken, next_token)
+        alt_text_parts.append(
+            ParserHelper.resolve_all_from_text(autolink_token.autolink_text)
+        )
+
+    @staticmethod
+    def __handle_next_alt_text_hard_break(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        _ = next_token
+        alt_text_parts.append(ParserHelper.newline_character)
+
+    @staticmethod
+    def __handle_next_alt_text_else(
+        next_token: MarkdownToken, alt_text_parts: List[str]
+    ) -> None:
+        assert (
+            next_token.is_inline_image
+        ), f"Not handled: {ParserHelper.make_value_visible(next_token)}"
+        image_token = cast(ImageStartMarkdownToken, next_token)
+        alt_text_parts.append(image_token.image_alt_text)
+
+    @staticmethod
     def __handle_next_alt_text(
         inline_blocks: List[MarkdownToken], ind_plus_one: int, alt_text_parts: List[str]
     ) -> None:
         if inline_blocks[ind_plus_one].is_special_text:
-            text_token = cast(TextMarkdownToken, inline_blocks[ind_plus_one])
-            if text_token.token_text == "]":
-                alt_text_parts.append(text_token.token_text)
+            LinkHelper.__handle_next_alt_text_special_text(
+                inline_blocks[ind_plus_one], alt_text_parts
+            )
         elif inline_blocks[ind_plus_one].is_text:
-            text_token = cast(TextMarkdownToken, inline_blocks[ind_plus_one])
-            alt_text_parts.append(
-                ParserHelper.resolve_all_from_text(text_token.token_text)
+            LinkHelper.__handle_next_alt_text_normal_text(
+                inline_blocks[ind_plus_one], alt_text_parts
             )
         elif inline_blocks[ind_plus_one].is_inline_raw_html:
-            rawhtml_token = cast(RawHtmlMarkdownToken, inline_blocks[ind_plus_one])
-            alt_text_parts.extend(["<", rawhtml_token.raw_tag, ">"])
-        elif inline_blocks[ind_plus_one].is_inline_code_span:
-            codespan_token = cast(
-                InlineCodeSpanMarkdownToken, inline_blocks[ind_plus_one]
+            LinkHelper.__handle_next_alt_text_raw_html(
+                inline_blocks[ind_plus_one], alt_text_parts
             )
-            alt_text_parts.append(
-                ParserHelper.resolve_all_from_text(codespan_token.span_text)
+        elif inline_blocks[ind_plus_one].is_inline_code_span:
+            LinkHelper.__handle_next_alt_text_code_span(
+                inline_blocks[ind_plus_one], alt_text_parts
             )
         elif inline_blocks[ind_plus_one].is_inline_autolink:
-            autolink_token = cast(
-                EmailAutolinkMarkdownToken, inline_blocks[ind_plus_one]
-            )
-            alt_text_parts.append(
-                ParserHelper.resolve_all_from_text(autolink_token.autolink_text)
+            LinkHelper.__handle_next_alt_text_auto_link(
+                inline_blocks[ind_plus_one], alt_text_parts
             )
         elif (
             inline_blocks[ind_plus_one].is_inline_link
             or inline_blocks[ind_plus_one].is_inline_link_end
             or inline_blocks[ind_plus_one].is_inline_emphasis
             or inline_blocks[ind_plus_one].is_inline_emphasis_end
         ):
             pass
         elif inline_blocks[ind_plus_one].is_inline_hard_break:
-            alt_text_parts.append(ParserHelper.newline_character)
+            LinkHelper.__handle_next_alt_text_hard_break(
+                inline_blocks[ind_plus_one], alt_text_parts
+            )
         else:
-            assert inline_blocks[
-                ind_plus_one
-            ].is_inline_image, f"Not handled: {ParserHelper.make_value_visible(inline_blocks[ind_plus_one])}"
-            image_token = cast(ImageStartMarkdownToken, inline_blocks[ind_plus_one])
-            alt_text_parts.append(image_token.image_alt_text)
+            LinkHelper.__handle_next_alt_text_else(
+                inline_blocks[ind_plus_one], alt_text_parts
+            )
 
     @staticmethod
     def __collect_text_from_blocks(
         inline_blocks: List[MarkdownToken], ind: int, suffix_text: str
     ) -> Tuple[str, str]:
         """
         Aggregate the text component of text blocks.
         """
 
         # POGGER.debug(
         #     ">>collect_text_from_blocks>>$",
         #     inline_blocks,
         # )
-        # POGGER.debug(
-        #     ">>collect_text_from_blocks>>suffix_text>>$",
-        #     suffix_text,
-        # )
+        POGGER.debug(
+            ">>collect_text_from_blocks>>suffix_text>>$",
+            suffix_text,
+        )
 
         (
             collect_index,
             is_inside_of_link,
             inline_blocks_size,
         ) = (ind + 1, False, len(inline_blocks))
         text_parts: List[str] = []
         text_raw_parts: List[str] = []
+        POGGER.debug(
+            ">>collect_index:$: < inline_blocks_size:$:",
+            collect_index,
+            inline_blocks_size,
+        )
         while collect_index < inline_blocks_size:
-
-            POGGER.debug(">>collect_text>>$<<", inline_blocks[collect_index])
-
-            if inline_blocks[collect_index].is_inline_link_end:
-                is_inside_of_link = LinkHelper.__collect_text_from_inline_link_end()
-            elif inline_blocks[collect_index].is_inline_link:
-                is_inside_of_link = LinkHelper.__collect_text_from_inline_link_start(
-                    inline_blocks, collect_index, text_raw_parts
-                )
-            elif inline_blocks[collect_index].is_inline_image:
-                LinkHelper.__collect_text_from_inline_image(
-                    inline_blocks, collect_index, text_raw_parts, text_parts
-                )
-            elif inline_blocks[collect_index].is_inline_code_span:
-                LinkHelper.__collect_text_from_inline_code_span(
-                    inline_blocks,
-                    collect_index,
-                    text_raw_parts,
-                    text_parts,
-                    is_inside_of_link,
-                )
-            elif inline_blocks[collect_index].is_inline_raw_html:
-                LinkHelper.__collect_text_from_inline_raw_html(
-                    inline_blocks,
-                    collect_index,
-                    text_raw_parts,
-                    text_parts,
-                    is_inside_of_link,
-                )
-            elif inline_blocks[collect_index].is_inline_autolink:
-                LinkHelper.__collect_text_from_inline_autolink(
-                    inline_blocks,
-                    collect_index,
-                    text_raw_parts,
-                    text_parts,
-                    is_inside_of_link,
-                )
-            elif inline_blocks[collect_index].is_inline_hard_break:
-                LinkHelper.__collect_text_from_inline_hard_break(
-                    inline_blocks, collect_index, text_raw_parts, text_parts
-                )
-            elif not is_inside_of_link:
-                LinkHelper.__collect_text_from_text(
-                    inline_blocks, collect_index, text_raw_parts, text_parts
-                )
-            POGGER.debug(
-                ">>collect_text>>$<<$<<", text_parts, inline_blocks[collect_index]
+            (
+                is_inside_of_link,
+                collect_index,
+            ) = LinkHelper.__collect_text_from_next_block(
+                inline_blocks,
+                inline_blocks_size,
+                collect_index,
+                text_raw_parts,
+                text_parts,
+                is_inside_of_link,
             )
-            POGGER.debug(">>collected_text_raw>>$<<", text_raw_parts)
-            collect_index += 1
 
         text_parts.append(suffix_text)
         text_raw_parts.append(suffix_text)
 
         text_from_blocks = "".join(text_parts)
+        POGGER.debug(">>text_from_blocks>:$:<", text_from_blocks)
         text_from_blocks = ParserHelper.resolve_backspaces_from_text(text_from_blocks)
+        POGGER.debug(">>text_from_blocks>:$:<", text_from_blocks)
+        POGGER.debug(">>text_raw_parts>:$:<", text_raw_parts)
         return text_from_blocks, "".join(text_raw_parts)
 
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __collect_text_from_next_block(
+        inline_blocks: List[MarkdownToken],
+        inline_blocks_size: int,
+        collect_index: int,
+        text_raw_parts: List[str],
+        text_parts: List[str],
+        is_inside_of_link: bool,
+    ) -> Tuple[bool, int]:
+        POGGER.debug(">>collect_text>>$<<", inline_blocks[collect_index])
+        if inline_blocks[collect_index].is_inline_link_end:
+            is_inside_of_link = LinkHelper.__collect_text_from_inline_link_end()
+        elif inline_blocks[collect_index].is_inline_link:
+            is_inside_of_link = LinkHelper.__collect_text_from_inline_link_start(
+                inline_blocks, collect_index, text_raw_parts
+            )
+        elif inline_blocks[collect_index].is_inline_image:
+            LinkHelper.__collect_text_from_inline_image(
+                inline_blocks, collect_index, text_raw_parts, text_parts
+            )
+        elif inline_blocks[collect_index].is_inline_code_span:
+            LinkHelper.__collect_text_from_inline_code_span(
+                inline_blocks,
+                collect_index,
+                text_raw_parts,
+                text_parts,
+                is_inside_of_link,
+            )
+        elif inline_blocks[collect_index].is_inline_raw_html:
+            LinkHelper.__collect_text_from_inline_raw_html(
+                inline_blocks,
+                collect_index,
+                text_raw_parts,
+                text_parts,
+                is_inside_of_link,
+            )
+        elif inline_blocks[collect_index].is_inline_autolink:
+            LinkHelper.__collect_text_from_inline_autolink(
+                inline_blocks,
+                collect_index,
+                text_raw_parts,
+                text_parts,
+                is_inside_of_link,
+            )
+        elif inline_blocks[collect_index].is_inline_hard_break:
+            LinkHelper.__collect_text_from_inline_hard_break(
+                inline_blocks, collect_index, text_raw_parts, text_parts
+            )
+        elif not is_inside_of_link:
+            LinkHelper.__collect_text_from_text(
+                inline_blocks, collect_index, text_raw_parts, text_parts
+            )
+        POGGER.debug(">>collect_text>>$<<$<<", text_parts, inline_blocks[collect_index])
+        POGGER.debug(">>collected_text_raw>>$<<", text_raw_parts)
+        collect_index += 1
+        POGGER.debug(
+            ">>collect_index:$: < inline_blocks_size:$:",
+            collect_index,
+            inline_blocks_size,
+        )
+        return is_inside_of_link, collect_index
+
+    # pylint: enable=too-many-arguments
+
     @staticmethod
     def __collect_text_from_inline_link_end() -> bool:
         return False
 
     @staticmethod
     def __collect_text_from_inline_link_start(
         inline_blocks: List[MarkdownToken],
@@ -743,16 +842,15 @@
         break_token = cast(HardBreakMarkdownToken, inline_blocks[collect_index])
         POGGER.debug("is_inline_hard_break>>collected_text_raw>>$<<", text_raw_parts)
         converted_text = break_token.line_end
         text_parts.append(converted_text)
         if converted_text == "\\":
             text_parts.append(converted_text)
         text_parts.append(ParserHelper.newline_character)
-        text_raw_parts.append(converted_text)
-        text_raw_parts.append(ParserHelper.newline_character)
+        text_raw_parts.extend((converted_text, ParserHelper.newline_character))
         POGGER.debug("is_inline_hard_break>>collected_text_raw>>$<<", text_raw_parts)
 
     @staticmethod
     def __collect_text_from_text(
         inline_blocks: List[MarkdownToken],
         collect_index: int,
         text_raw_parts: List[str],
@@ -990,175 +1088,230 @@
         POGGER.debug("parse_link_title>>after>>$>>", ex_title)
 
         assert newer_index is not None
         return ex_title, pre_ex_title, newer_index, bounding_character
 
     @staticmethod
     def __process_inline_link_body(
-        source_text: str, new_index: int
-    ) -> Tuple[
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        int,
-        bool,
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-    ]:
+        source_text: str,
+        new_index: int,
+        tabified_text: Optional[str],
+        lhp: LinkHelperProperties,
+    ) -> int:
         """
         Given that an inline link has been identified, process it's body.
         """
 
-        POGGER.debug("process_inline_link_body>>$<<", source_text[new_index:])
+        POGGER.debug("process_inline_link_body>:$:<", source_text[new_index:])
+        POGGER.debug("source_text>:$:<", source_text)
+        POGGER.debug("tabified_text>:$:<", tabified_text)
+
+        text_to_scan = source_text
+        if tabified_text:
+            text_to_scan = tabified_text
+            tabified_new_index = LinkHelper.__translate_between_strings(
+                source_text, tabified_text, new_index
+            )
+            POGGER.debug("tabified_new_index>:$:<", tabified_new_index)
+            new_index = tabified_new_index
 
-        newer_index: Optional[int] = new_index
-        newer_index, before_link_whitespace = ParserHelper.extract_ascii_whitespace(
-            source_text, new_index
+        new_index += 1
+
+        newer_index, lhp.before_link_whitespace = ParserHelper.extract_ascii_whitespace(
+            text_to_scan, new_index
         )
 
         POGGER.debug(
-            "newer_index>>$>>source_text[]>>$>", newer_index, source_text[newer_index:]
+            "newer_index>>$>>text_to_scan[]>>$>",
+            newer_index,
+            text_to_scan[newer_index:],
         )
         assert newer_index is not None
         if not ParserHelper.is_character_at_index(
-            source_text, newer_index, LinkHelper.__link_format_inline_end
+            text_to_scan, newer_index, LinkHelper.__link_format_inline_end
         ):
-            (
-                inline_link,
-                pre_inline_link,
-                newer_index,
-                did_use_angle_start,
-                before_title_whitespace,
-                inline_title,
-                pre_inline_title,
-                bounding_character,
-                after_title_whitespace,
-            ) = LinkHelper.__parse_inline_link_properties(source_text, newer_index)
+            newer_index = LinkHelper.__parse_inline_link_properties(
+                text_to_scan, newer_index, lhp
+            )
         else:
             (
-                inline_link,
-                pre_inline_link,
-                inline_title,
-                pre_inline_title,
-                did_use_angle_start,
-                bounding_character,
-                before_title_whitespace,
-                after_title_whitespace,
+                lhp.inline_link,
+                lhp.pre_inline_link,
+                lhp.inline_title,
+                lhp.pre_inline_title,
+                lhp.did_use_angle_start,
+                lhp.bounding_character,
+                lhp.before_title_whitespace,
+                lhp.after_title_whitespace,
             ) = ("", "", "", "", False, "", "", "")
         POGGER.debug(
             "inline_link>>$>>inline_title>>$>newer_index>$>",
-            inline_link,
-            inline_title,
+            lhp.inline_link,
+            lhp.inline_title,
             newer_index,
         )
         assert newer_index is not None
+        (
+            newer_index,
+            lhp.did_use_angle_start,
+        ) = LinkHelper.__process_inline_link_body_final(
+            newer_index, source_text, tabified_text, lhp.did_use_angle_start
+        )
+        POGGER.debug(
+            "process_inline_link_body>>inline_link>>$>>inline_title>>$>new_index>$>",
+            lhp.inline_link,
+            lhp.inline_title,
+            newer_index,
+        )
+        return newer_index
+
+    @staticmethod
+    def __process_inline_link_body_final(
+        newer_index: int,
+        source_text: str,
+        tabified_text: Optional[str],
+        did_use_angle_start: Optional[bool],
+    ) -> Tuple[int, bool]:
         if newer_index != -1:
+            if tabified_text:
+                untabified_newer_index = LinkHelper.__translate_between_strings(
+                    tabified_text, source_text, newer_index
+                )
+                POGGER.debug("untabified_newer_index>:$:<", untabified_newer_index)
+                newer_index = untabified_newer_index
+
             assert did_use_angle_start is not None
             if ParserHelper.is_character_at_index(
                 source_text, newer_index, LinkHelper.__link_format_inline_end
             ):
                 newer_index += 1
             else:
                 newer_index = -1
         else:
             did_use_angle_start = False
+        return newer_index, did_use_angle_start
+
+    @staticmethod
+    def __translate_between_strings(
+        source_text: str, destination_text: str, next_index: int
+    ) -> int:
+        stop_character = source_text[next_index]
+
+        POGGER.debug("source_text>:$:<", source_text)
+        POGGER.debug("index>:$:< == >:$:<", next_index, stop_character)
+        POGGER.debug("destination_text>:$:<", destination_text)
+
+        found_in_source_text_count = 0
+        found_in_source_text_index = source_text.find(stop_character)
         POGGER.debug(
-            "process_inline_link_body>>inline_link>>$>>inline_title>>$>new_index>$>",
-            inline_link,
-            inline_title,
-            newer_index,
+            "source_text[$]>:$:<",
+            found_in_source_text_index,
+            source_text[found_in_source_text_index:],
         )
-        return (
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
-            newer_index,
-            did_use_angle_start,
-            bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
+        while found_in_source_text_index != next_index:
+            found_in_source_text_count += 1
+            found_in_source_text_index = source_text.find(
+                stop_character, found_in_source_text_index + 1
+            )
+            POGGER.debug(
+                "source_text[$]>:$:<",
+                found_in_source_text_index,
+                source_text[found_in_source_text_index:],
+            )
+        POGGER.debug("found_in_source_text_count>:$:<", found_in_source_text_count)
+        POGGER.debug(
+            "source_text[$]>:$:<",
+            found_in_source_text_index,
+            source_text[found_in_source_text_index:],
+        )
+
+        found_in_destination_text_count = 0
+        stop_character_in_destination_index = destination_text.find(stop_character)
+        POGGER.debug(
+            "stop_character_in_destination_index[$]>:$:<",
+            stop_character_in_destination_index,
+            destination_text[stop_character_in_destination_index:],
+        )
+        while found_in_destination_text_count != found_in_source_text_count:
+            found_in_destination_text_count += 1
+            stop_character_in_destination_index = destination_text.find(
+                stop_character, stop_character_in_destination_index + 1
+            )
+            POGGER.debug(
+                "adj_tabified_text[$]>:$:<",
+                stop_character_in_destination_index,
+                destination_text[stop_character_in_destination_index:],
+            )
+            assert stop_character_in_destination_index != -1
+        POGGER.debug(
+            "found_in_destination_text_count>:$:<", found_in_destination_text_count
+        )
+        POGGER.debug(
+            "adj_tabified_text[$]>:$:<",
+            stop_character_in_destination_index,
+            destination_text[stop_character_in_destination_index:],
         )
+        assert destination_text[stop_character_in_destination_index] == stop_character
+        return stop_character_in_destination_index
 
     @staticmethod
     def __parse_inline_link_properties(
-        source_text: str, new_index: int
-    ) -> Tuple[
-        Optional[str],
-        Optional[str],
-        Optional[int],
-        Optional[bool],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-    ]:
-        inline_title: Optional[str] = ""
-        pre_inline_title: Optional[str] = ""
-        bounding_character: Optional[str] = ""
-        before_title_whitespace: Optional[str] = ""
-        after_title_whitespace: Optional[str] = ""
+        source_text: str, new_index: int, lhp: LinkHelperProperties
+    ) -> int:
+        lhp.inline_title = ""
+        lhp.pre_inline_title = ""
+        lhp.bounding_character = ""
+        lhp.before_title_whitespace = ""
+        lhp.after_title_whitespace = ""
         newer_index: Optional[int] = None
+        temp_bool = None
         POGGER.debug(">>search for link destination")
         (
-            inline_link,
-            pre_inline_link,
+            lhp.inline_link,
+            lhp.pre_inline_link,
             newer_index,
             _,
-            did_use_angle_start,
+            temp_bool,
         ) = LinkHelper.__parse_link_destination(source_text, new_index)
+        lhp.did_use_angle_start = temp_bool
         POGGER.debug(
             ">>link destination>>$>>$>>",
             source_text,
             newer_index,
         )
         if newer_index != -1:
             POGGER.debug(
                 "before ws>>$<",
                 source_text[newer_index:],
             )
             (
                 newer_index,
-                before_title_whitespace,
+                lhp.before_title_whitespace,
             ) = ParserHelper.extract_ascii_whitespace(source_text, newer_index)
             POGGER.debug(
                 "after ws>>$>",
                 source_text[newer_index:],
             )
             assert newer_index is not None
             if ParserHelper.is_character_at_index_not(
                 source_text, newer_index, LinkHelper.__link_format_inline_end
             ):
                 (
-                    inline_title,
-                    pre_inline_title,
+                    lhp.inline_title,
+                    lhp.pre_inline_title,
                     newer_index,
-                    bounding_character,
+                    lhp.bounding_character,
                 ) = LinkHelper.__parse_link_title(source_text, newer_index)
         if newer_index != -1:
             (
                 newer_index,
-                after_title_whitespace,
+                lhp.after_title_whitespace,
             ) = ParserHelper.extract_ascii_whitespace(source_text, newer_index)
-        return (
-            inline_link,
-            pre_inline_link,
-            newer_index,
-            did_use_angle_start,
-            before_title_whitespace,
-            inline_title,
-            pre_inline_title,
-            bounding_character,
-            after_title_whitespace,
-        )
+        assert newer_index is not None
+        return newer_index
 
     @staticmethod
     def __look_up_link(
         link_to_lookup: str, new_index: int, link_type: str
     ) -> Tuple[int, str, str]:
         """
         Look up a link to see if it is present.
@@ -1184,201 +1337,151 @@
             update_index, inline_link, inline_title = (
                 new_index,
                 link_titles.inline_link,
                 link_titles.inline_title,
             )
         return update_index, inline_link, inline_title
 
-    # pylint: disable=too-many-arguments,too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __excavate_link(
         inline_blocks: List[MarkdownToken],
         ind: int,
         source_text: str,
         new_index: int,
         current_string_unresolved: str,
         remaining_line: str,
-    ) -> Tuple[
-        int,
-        str,
-        str,
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        bool,
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-    ]:
+        tabified_remaining_line: Optional[str],
+        tabified_text: Optional[str],
+    ) -> Tuple[int, str, str, LinkHelperProperties,]:
         POGGER.debug(
             "handle_link_types>>$<<$<<",
             inline_blocks,
             ind,
         )
         POGGER.debug(
             "handle_link_types>source_text>>$<<",
             source_text,
         )
         POGGER.debug("handle_link_types>>$<<", source_text[new_index:])
         POGGER.debug(
-            "handle_link_types>>current_string_unresolved>>$<<remaining_line<<$>>",
+            "handle_link_types>>current_string_unresolved>:$:<remaining_line>:$:<tabified_remaining_line>:$:<",
             current_string_unresolved,
             remaining_line,
+            tabified_remaining_line,
         )
+        text_to_scan = remaining_line
+        if tabified_remaining_line is not None:
+            text_to_scan = tabified_remaining_line
         text_from_blocks, text_from_blocks_raw = LinkHelper.__collect_text_from_blocks(
-            inline_blocks, ind, f"{current_string_unresolved}{remaining_line}"
+            inline_blocks, ind, f"{current_string_unresolved}{text_to_scan}"
         )
         POGGER.debug(
             "handle_link_types>>text_from_blocks_raw>>$<<",
             text_from_blocks_raw,
         )
         POGGER.debug(
             "handle_link_types>>text_from_blocks>>$<<",
             text_from_blocks,
         )
 
         POGGER.debug("__look_for_link_formats>>$>>", new_index)
         (
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
             update_index,
             tried_full_reference_form,
-            ex_label,
-            label_type,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
-        ) = LinkHelper.__look_for_link_formats(source_text, new_index, text_from_blocks)
+            lhp,
+        ) = LinkHelper.__look_for_link_formats(
+            source_text, new_index, text_from_blocks, tabified_text
+        )
 
         # u != -1 - inline valid
         # tried_full_reference_form - collapsed or full valid
         if update_index == -1 and not tried_full_reference_form:
             (
-                ex_label,
+                lhp.ex_label,
                 update_index,
-                inline_link,
-                inline_title,
-                label_type,
-                pre_inline_link,
+                lhp.inline_link,
+                lhp.inline_title,
+                lhp.label_type,
+                lhp.pre_inline_link,
             ) = LinkHelper.__look_for_shortcut_link(
                 inline_blocks, text_from_blocks, new_index
             )
         return (
             update_index,
             text_from_blocks,
             text_from_blocks_raw,
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
-            ex_label,
-            label_type,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
+            lhp,
         )
 
-    # pylint: enable=too-many-arguments,too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_link_types(
         inline_blocks: List[MarkdownToken],
         ind: int,
         source_text: str,
         new_index: int,
         start_text: str,
         remaining_line: str,
+        tabified_remaining_line: Optional[str],
         current_string_unresolved: str,
         xx_fn: Callable[[str], str],
+        tabified_text: Optional[str],
     ) -> Tuple[int, Optional[MarkdownToken], bool]:
         """
         After finding a link specifier, figure out what type of link it is.
         """
 
         (
             update_index,
             text_from_blocks,
             text_from_blocks_raw,
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
-            ex_label,
-            label_type,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
+            lhp,
         ) = LinkHelper.__excavate_link(
             inline_blocks,
             ind,
             source_text,
             new_index,
             current_string_unresolved,
             remaining_line,
+            tabified_remaining_line,
+            tabified_text,
         )
 
         POGGER.debug("<<<<<<<new_index<<<<<<<$<<", new_index)
         POGGER.debug("<<<<<<<update_index<<<<<<<$<<", update_index)
         POGGER.debug("<<<<<<<text_from_blocks_raw<<<<<<<$<<", text_from_blocks_raw)
         if update_index != -1:
-            assert ex_label is not None
-            assert before_link_whitespace is not None
-            assert inline_link is not None
-            assert pre_inline_link is not None
-            assert inline_title is not None
-            assert pre_inline_title is not None
-            assert inline_title_bounding_character is not None
-            assert before_title_whitespace is not None
-            assert after_title_whitespace is not None
-            assert label_type is not None
-            consume_rest_of_line, token_to_append = LinkHelper.__create_link_token(
+            assert lhp.ex_label is not None
+            assert lhp.inline_link is not None
+            assert lhp.pre_inline_link is not None
+            assert lhp.inline_title is not None
+            assert lhp.pre_inline_title is not None
+            assert lhp.bounding_character is not None
+            assert lhp.before_title_whitespace is not None
+            assert lhp.after_title_whitespace is not None
+            assert lhp.before_link_whitespace is not None
+            assert lhp.label_type is not None
+            return LinkHelper.__create_link_token(
                 start_text,
-                inline_link,
-                pre_inline_link,
-                inline_title,
-                pre_inline_title,
                 text_from_blocks,
                 text_from_blocks_raw,
                 inline_blocks,
                 ind,
-                did_use_angle_start,
-                inline_title_bounding_character,
-                before_link_whitespace,
-                before_title_whitespace,
-                after_title_whitespace,
-                ex_label,
-                label_type,
                 remaining_line,
                 current_string_unresolved,
                 xx_fn,
+                lhp,
+                update_index,
             )
-        else:
-            consume_rest_of_line, token_to_append = False, None
-
-        POGGER.debug(
-            "handle_link_types<update_index<$<<$<<",
-            update_index,
-            token_to_append,
-        )
-        return update_index, token_to_append, consume_rest_of_line
+        return update_index, None, False
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
     @staticmethod
     def __look_for_shortcut_link(
         inline_blocks: List[MarkdownToken], text_from_blocks: str, new_index: int
     ) -> Tuple[str, int, str, str, str, str]:
         POGGER.debug("shortcut?")
         POGGER.debug(
@@ -1398,358 +1501,315 @@
             update_index,
             inline_link,
             inline_title,
             Constants.link_type__shortcut,
             "",
         )
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __create_link_token(
         start_text: str,
-        inline_link: str,
-        pre_inline_link: str,
-        inline_title: str,
-        pre_inline_title: str,
         text_from_blocks: str,
         text_from_blocks_raw: str,
         inline_blocks: List[MarkdownToken],
         ind: int,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: str,
-        before_link_whitespace: str,
-        before_title_whitespace: str,
-        after_title_whitespace: str,
-        ex_label: str,
-        label_type: str,
         remaining_line: str,
         current_string_unresolved: str,
         xx_fn: Callable[[str], str],
-    ) -> Tuple[bool, Optional[MarkdownToken]]:
+        lhp: LinkHelperProperties,
+        update_index: int,
+    ) -> Tuple[int, Optional[MarkdownToken], bool]:
         """
         Create the right type of link token.
         """
-        (text_from_blocks_raw, line_number, column_number,) = (
+        (
+            text_from_blocks_raw,
+            line_number,
+            column_number,
+        ) = (
             ParserHelper.resolve_backspaces_from_text(text_from_blocks_raw),
             inline_blocks[ind].line_number,
             inline_blocks[ind].column_number,
         )
 
-        POGGER.debug("<<<<<<<start_text<<<<<<<$<<", start_text)
-        POGGER.debug(">>inline_link>>$>>", inline_link)
-        POGGER.debug(">>pre_inline_link>>$>>", pre_inline_link)
-        POGGER.debug(">>inline_title>>$>>", inline_title)
-        POGGER.debug(">>pre_inline_title>>$>>", pre_inline_title)
-        POGGER.debug(
-            ">>text_from_blocks>>$>>",
-            text_from_blocks,
-        )
-        if pre_inline_link == inline_link:
-            pre_inline_link = ""
-        if pre_inline_title == inline_title:
-            pre_inline_title = ""
-        POGGER.debug(">>pre_inline_link>>$>>", pre_inline_link)
+        # POGGER.debug("<<<<<<<start_text<<<<<<<$<<", start_text)
+        # POGGER.debug(">>inline_link>>$>>", inline_link)
+        # POGGER.debug(">>pre_inline_link>>$>>", pre_inline_link)
+        # POGGER.debug(">>inline_title>>$>>", inline_title)
+        # POGGER.debug(">>pre_inline_title>>$>>", pre_inline_title)
+        # POGGER.debug(
+        #     ">>text_from_blocks>>$>>",
+        #     text_from_blocks,
+        # )
+        _ = text_from_blocks
+        if lhp.pre_inline_link == lhp.inline_link:
+            lhp.pre_inline_link = ""
+        if lhp.pre_inline_title == lhp.inline_title:
+            lhp.pre_inline_title = ""
+        # POGGER.debug(">>pre_inline_link>>$>>", pre_inline_link)
 
-        POGGER.debug(">>text_from_blocks_raw>>$>>", text_from_blocks_raw)
-        POGGER.debug(">>inline_blocks[ind]>>$>>", inline_blocks[ind])
+        # POGGER.debug(">>text_from_blocks_raw>>$>>", text_from_blocks_raw)
+        # POGGER.debug(">>inline_blocks[ind]>>$>>", inline_blocks[ind])
 
         if start_text == LinkHelper.__link_start_sequence:
             consume_rest_of_line = False
             token_to_append = LinkHelper.__add_link_start_token(
                 inline_blocks,
                 ind,
-                inline_link,
-                pre_inline_link,
-                inline_title,
-                pre_inline_title,
-                ex_label,
-                label_type,
                 text_from_blocks_raw,
-                did_use_angle_start,
-                inline_title_bounding_character,
-                before_link_whitespace,
-                before_title_whitespace,
-                after_title_whitespace,
                 line_number,
                 column_number,
+                lhp,
             )
         else:
             token_to_append = None
             consume_rest_of_line, text_from_blocks_raw = LinkHelper.__add_image_token(
                 start_text,
                 inline_blocks,
                 ind,
                 remaining_line,
                 text_from_blocks_raw,
                 xx_fn,
-                inline_link,
-                pre_inline_link,
-                inline_title,
-                pre_inline_title,
-                ex_label,
-                label_type,
-                did_use_angle_start,
-                inline_title_bounding_character,
-                before_link_whitespace,
-                before_title_whitespace,
-                after_title_whitespace,
                 line_number,
                 column_number,
                 current_string_unresolved,
+                lhp,
             )
-        return consume_rest_of_line, token_to_append
+        return update_index, token_to_append, consume_rest_of_line
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __add_link_start_token(
         inline_blocks: List[MarkdownToken],
         ind: int,
-        inline_link: str,
-        pre_inline_link: str,
-        inline_title: str,
-        pre_inline_title: str,
-        ex_label: str,
-        label_type: str,
         text_from_blocks_raw: str,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: str,
-        before_link_whitespace: str,
-        before_title_whitespace: str,
-        after_title_whitespace: str,
         line_number: int,
         column_number: int,
+        lhp: LinkHelperProperties,
     ) -> MarkdownToken:
         inline_blocks[ind] = LinkStartMarkdownToken(
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
-            ex_label,
-            label_type,
-            text_from_blocks_raw,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
-            line_number,
-            column_number,
+            text_from_blocks_raw, line_number, column_number, lhp
         )
         return inline_blocks[ind].generate_close_markdown_token_from_markdown_token(
             "", ""
         )
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __add_image_token(
         start_text: str,
         inline_blocks: List[MarkdownToken],
         ind: int,
         remaining_line: str,
         text_from_blocks_raw: str,
         xx_fn: Callable[[str], str],
-        inline_link: str,
-        pre_inline_link: str,
-        inline_title: str,
-        pre_inline_title: str,
-        ex_label: str,
-        label_type: str,
-        did_use_angle_start: bool,
-        inline_title_bounding_character: str,
-        before_link_whitespace: str,
-        before_title_whitespace: str,
-        after_title_whitespace: str,
         line_number: int,
         column_number: int,
         current_string_unresolved: str,
+        lhp: LinkHelperProperties,
     ) -> Tuple[bool, str]:
         assert start_text == LinkHelper.image_start_sequence
         POGGER.debug("\n>>__consume_text_for_image_alt_text>>$>>", inline_blocks)
         POGGER.debug("\n>>__consume_text_for_image_alt_text>>$>>", ind)
         POGGER.debug("\n>>__consume_text_for_image_alt_text>>$>>", remaining_line)
         (
             image_alt_text,
             text_from_blocks_raw,
         ) = LinkHelper.__consume_text_for_image_alt_text(
             inline_blocks, ind, remaining_line, text_from_blocks_raw, xx_fn
         )
         POGGER.debug("\n>>__consume_text_for_image_alt_text>>$>>", image_alt_text)
 
         inline_blocks[ind] = ImageStartMarkdownToken(
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
             image_alt_text,
-            ex_label,
-            label_type,
             text_from_blocks_raw,
-            did_use_angle_start,
-            inline_title_bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
             line_number,
             column_number,
+            lhp,
         )
         POGGER.debug("\n>>Image>>$", inline_blocks)
         POGGER.debug(">>start_text>>$<<", start_text)
         POGGER.debug(">>remaining_line>>$<<", remaining_line)
         POGGER.debug(">>current_string_unresolved>>$<<", current_string_unresolved)
         return True, text_from_blocks_raw
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-locals
     @staticmethod
     def __look_for_link_formats(
-        source_text: str, new_index: int, text_from_blocks: str
-    ) -> Tuple[
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        int,
-        bool,
-        Optional[str],
-        Optional[str],
-        bool,
-        Optional[str],
-        Optional[str],
-        Optional[str],
-        Optional[str],
-    ]:
+        source_text: str,
+        new_index: int,
+        text_from_blocks: str,
+        tabified_text: Optional[str],
+    ) -> Tuple[int, bool, LinkHelperProperties,]:
         """
         Look for links in the various formats.
         """
         (
             update_index,
             tried_full_reference_form,
         ) = (-1, False)
-        did_use_angle_start: bool = False
-        bounding_character: Optional[str] = ""
-        label_type: Optional[str] = ""
-        inline_link: Optional[str] = ""
-        pre_inline_link: Optional[str] = ""
-        inline_title: Optional[str] = ""
-        pre_inline_title: Optional[str] = ""
-        ex_label: Optional[str] = ""
-        before_link_whitespace: Optional[str] = ""
-        before_title_whitespace: Optional[str] = ""
-        after_title_whitespace: Optional[str] = ""
+        lhp: LinkHelperProperties = LinkHelperProperties()
+        lhp.did_use_angle_start = False
+        lhp.bounding_character = ""
+        lhp.label_type = ""
+        lhp.inline_link = ""
+        lhp.pre_inline_link = ""
+        lhp.inline_title = ""
+        lhp.pre_inline_title = ""
+        lhp.ex_label = ""
+        lhp.before_link_whitespace = ""
+        lhp.before_title_whitespace = ""
+        lhp.after_title_whitespace = ""
         if ParserHelper.is_character_at_index(
             source_text, new_index, LinkHelper.__link_format_inline_start
         ):
             POGGER.debug("inline reference? >>$>>", new_index)
-            (
-                inline_link,
-                pre_inline_link,
-                inline_title,
-                pre_inline_title,
-                update_index,
-                did_use_angle_start,
-                bounding_character,
-                before_link_whitespace,
-                before_title_whitespace,
-                after_title_whitespace,
-            ) = LinkHelper.__process_inline_link_body(source_text, new_index + 1)
-            label_type = Constants.link_type__inline
+            update_index = LinkHelper.__process_inline_link_body(
+                source_text, new_index, tabified_text, lhp
+            )
+            lhp.label_type = Constants.link_type__inline
         elif ParserHelper.is_character_at_index(
             source_text, new_index, LinkHelper.__link_format_reference_start
         ):
             (
-                label_type,
+                lhp.label_type,
                 tried_full_reference_form,
                 update_index,
-                inline_link,
-                inline_title,
-                ex_label,
+                lhp.inline_link,
+                lhp.inline_title,
+                lhp.ex_label,
             ) = LinkHelper.__try_to_find_link_match(
-                new_index, source_text, text_from_blocks
+                new_index, source_text, text_from_blocks, tabified_text
             )
         POGGER.debug("__look_for_link_formats>>update_index>>$>>", update_index)
         return (
-            inline_link,
-            pre_inline_link,
-            inline_title,
-            pre_inline_title,
             update_index,
             tried_full_reference_form,
-            ex_label,
-            label_type,
-            did_use_angle_start,
-            bounding_character,
-            before_link_whitespace,
-            before_title_whitespace,
-            after_title_whitespace,
+            lhp,
         )
 
-    # pylint: enable=too-many-locals
-
     @staticmethod
     def __try_to_find_link_match(
-        new_index: int, source_text: str, text_from_blocks: str
+        new_index: int,
+        source_text: str,
+        text_from_blocks: str,
+        tabified_text: Optional[str],
     ) -> Tuple[str, bool, int, str, str, Optional[str]]:
         POGGER.debug("collapsed reference?")
 
         # TODO label type as Enum?
 
+        text_to_scan = source_text
+        if tabified_text:
+            assert tabified_text is not None
+            text_to_scan = tabified_text
+            tabified_new_index = LinkHelper.__translate_between_strings(
+                source_text, tabified_text, new_index
+            )
+            POGGER.debug("tabified_new_index>:$:<", tabified_new_index)
+            new_index = tabified_new_index
+
         after_open_index = new_index + 1
         tried_full_reference_form = ParserHelper.is_character_at_index(
-            source_text, after_open_index, LinkHelper.__link_format_reference_end
+            text_to_scan, after_open_index, LinkHelper.__link_format_reference_end
         )
         if tried_full_reference_form:
             ex_label: Optional[str] = ""
 
             POGGER.debug("collapsed reference")
             POGGER.debug(">>$>>", text_from_blocks)
             update_index, inline_link, inline_title = LinkHelper.__look_up_link(
                 text_from_blocks,
                 after_open_index + 1,
                 "collapsed reference",
             )
             POGGER.debug("collapsed reference>update_index>$", update_index)
             label_type = Constants.link_type__collapsed
         else:
-            POGGER.debug("full reference?")
-            POGGER.debug(">>did_extract>>$>", source_text[after_open_index:])
-            (did_extract, after_label_index, ex_label,) = LinkHelper.extract_link_label(
-                source_text, after_open_index, include_reference_colon=False
-            )
-            POGGER.debug(
-                ">>did_extract>>$>after_label_index>$>ex_label>$>",
-                did_extract,
-                after_label_index,
+            (
                 ex_label,
+                label_type,
+                inline_link,
+                inline_title,
+                update_index,
+                tried_full_reference_form,
+            ) = LinkHelper.__try_to_find_link_match_try_full(
+                text_to_scan, after_open_index
             )
-            tried_full_reference_form = did_extract
-            if did_extract:
-                assert ex_label is not None
-                label_type = Constants.link_type__full
-                update_index, inline_link, inline_title = LinkHelper.__look_up_link(
-                    ex_label, after_label_index, "full reference"
-                )
-            else:
-                label_type, inline_link, inline_title, update_index = "", "", "", -1
+
+        if tabified_text and update_index != -1:
+            assert tabified_text is not None
+
+            # Both of the above functions consume the last character of the link.
+            # Instead of guessing, we "rewind" the index by one character so that
+            # we can have something to sync on that is not an end of line or whitespace.
+            assert (
+                tabified_text[update_index - 1]
+                == LinkHelper.__link_format_reference_end
+            )
+            untabified_update_index = LinkHelper.__translate_between_strings(
+                tabified_text, source_text, update_index - 1
+            )
+            POGGER.debug("untabified_update_index>:$:<", untabified_update_index)
+            update_index = untabified_update_index + 1
+
         return (
             label_type,
             tried_full_reference_form,
             update_index,
             inline_link,
             inline_title,
             ex_label,
         )
 
     @staticmethod
-    def __encode_link_destination(link_to_encode: str) -> str:
+    def __try_to_find_link_match_try_full(
+        text_to_scan: str, after_open_index: int
+    ) -> Tuple[Optional[str], str, str, str, int, bool]:
+        POGGER.debug("full reference?")
+        POGGER.debug(">>did_extract>>$>", text_to_scan[after_open_index:])
+        (
+            did_extract,
+            after_label_index,
+            ex_label,
+        ) = LinkHelper.extract_link_label(
+            text_to_scan, after_open_index, include_reference_colon=False
+        )
+        POGGER.debug(
+            ">>did_extract>>$>after_label_index>$>ex_label>$>",
+            did_extract,
+            after_label_index,
+            ex_label,
+        )
+        tried_full_reference_form = did_extract
+        if tried_full_reference_form:
+            assert ex_label is not None
+            label_type = Constants.link_type__full
+            update_index, inline_link, inline_title = LinkHelper.__look_up_link(
+                ex_label, after_label_index, "full reference"
+            )
+        else:
+            label_type, inline_link, inline_title, update_index = "", "", "", -1
+        return (
+            ex_label,
+            label_type,
+            inline_link,
+            inline_title,
+            update_index,
+            tried_full_reference_form,
+        )
 
+    @staticmethod
+    def __encode_link_destination(link_to_encode: str) -> str:
         percent_index, before_data = ParserHelper.collect_until_one_of_characters(
             link_to_encode, 0, LinkHelper.__special_link_destination_characters
         )
         assert percent_index is not None
         assert before_data is not None
         el_parts, link_to_encode_size = [
             urllib.parse.quote(before_data, safe=LinkHelper.__link_safe_characters)
@@ -1791,14 +1851,54 @@
     ) -> str:
         """
         Given an image token, rehydrate it's original text from the token.
         """
         return f"!{LinkHelper.rehydrate_inline_link_text_from_token(image_token)}"
 
     @staticmethod
+    def __rehydrate_inline_link_text_from_token_type_inline(
+        link_token: ReferenceMarkdownToken, link_parts: List[str]
+    ) -> None:
+        assert link_token.before_title_whitespace is not None
+        assert link_token.before_link_whitespace is not None
+        link_parts.extend(
+            [
+                "[",
+                ParserHelper.remove_all_from_text(link_token.text_from_blocks),
+                "](",
+                link_token.before_link_whitespace,
+                f"<{link_token.active_link_uri}>"
+                if link_token.did_use_angle_start
+                else link_token.active_link_uri,
+                link_token.before_title_whitespace,
+            ]
+        )
+        if link_token.active_link_title:
+            if link_token.inline_title_bounding_character == "'":
+                title_prefix = "'"
+                title_suffix = "'"
+            elif link_token.inline_title_bounding_character == "(":
+                title_prefix = "("
+                title_suffix = ")"
+            else:
+                title_prefix = '"'
+                title_suffix = '"'
+
+            assert link_token.after_title_whitespace is not None
+            link_parts.extend(
+                [
+                    title_prefix,
+                    link_token.active_link_title,
+                    title_suffix,
+                    link_token.after_title_whitespace,
+                ]
+            )
+        link_parts.append(")")
+
+    @staticmethod
     def rehydrate_inline_link_text_from_token(
         link_token: ReferenceMarkdownToken,
     ) -> str:
         """
         Given a link token, rehydrate it's original text from the token.
         """
 
@@ -1816,44 +1916,12 @@
             link_parts.extend(
                 ["[", link_token.text_from_blocks, "][", link_token.ex_label, "]"]
             )
         elif link_token.label_type == Constants.link_type__collapsed:
             link_parts.extend(["[", link_token.text_from_blocks, "][]"])
         else:
             assert link_token.label_type == Constants.link_type__inline
-
-            assert link_token.before_title_whitespace is not None
-            assert link_token.before_link_whitespace is not None
-            link_parts.extend(
-                [
-                    "[",
-                    ParserHelper.remove_all_from_text(link_token.text_from_blocks),
-                    "](",
-                    link_token.before_link_whitespace,
-                    f"<{link_token.active_link_uri}>"
-                    if link_token.did_use_angle_start
-                    else link_token.active_link_uri,
-                    link_token.before_title_whitespace,
-                ]
+            LinkHelper.__rehydrate_inline_link_text_from_token_type_inline(
+                link_token, link_parts
             )
-            if link_token.active_link_title:
-                if link_token.inline_title_bounding_character == "'":
-                    title_prefix = "'"
-                    title_suffix = "'"
-                elif link_token.inline_title_bounding_character == "(":
-                    title_prefix = "("
-                    title_suffix = ")"
-                else:
-                    title_prefix = '"'
-                    title_suffix = '"'
 
-                assert link_token.after_title_whitespace is not None
-                link_parts.extend(
-                    [
-                        title_prefix,
-                        link_token.active_link_title,
-                        title_suffix,
-                        link_token.after_title_whitespace,
-                    ]
-                )
-            link_parts.append(")")
         return "".join(link_parts)
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/list_block_processor.py` & `pymarkdownlnt-0.9.9/pymarkdown/list_block_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from pymarkdown.stack_token import (
     BlockQuoteStackToken,
     ListStackToken,
     OrderedListStackToken,
     StackToken,
     UnorderedListStackToken,
 )
+from pymarkdown.tab_helper import TabHelper
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 
 # pylint: disable=too-many-lines
 class ListBlockProcessor:
     """
@@ -70,19 +71,23 @@
 
         assert adj_ws is not None
         POGGER.debug("skip_whitespace_check>>$", skip_whitespace_check)
         POGGER.debug("len(adj_ws)>>$", len(adj_ws))
         POGGER.debug("parent_indent>>$", parent_indent)
 
         if (
-            ParserHelper.is_length_less_than_or_equal_to(adj_ws, 3 + parent_indent)
+            TabHelper.is_length_less_than_or_equal_to(adj_ws, 3 + parent_indent)
             or skip_whitespace_check
         ):
+            assert extracted_whitespace is not None
+            adj_extracted_whitespace = extracted_whitespace
+            if parent_indent:
+                adj_extracted_whitespace = extracted_whitespace[parent_indent:]
             is_start = ListBlockProcessor.__is_start_ulist(
-                line_to_parse, start_index, extracted_whitespace
+                line_to_parse, start_index, adj_extracted_whitespace
             )
         else:
             is_start = False
         if is_start:
             (
                 is_start,
                 after_all_whitespace_index,
@@ -134,15 +139,15 @@
 
         assert adj_ws is not None
 
         POGGER.debug("skip_whitespace_check>>$", skip_whitespace_check)
         POGGER.debug("len(adj_ws)>>$", len(adj_ws))
 
         if (
-            ParserHelper.is_length_less_than_or_equal_to(adj_ws, 3 + parent_indent)
+            TabHelper.is_length_less_than_or_equal_to(adj_ws, 3 + parent_indent)
             or skip_whitespace_check
         ):
             (
                 is_start,
                 index,
                 number_of_digits,
                 is_not_one,
@@ -248,15 +253,14 @@
     @staticmethod
     def __adjust_whitespace_for_nested_lists(
         parser_state: ParserState,
         adj_ws: Optional[str],
         line_to_parse: str,
         start_index: int,
     ) -> Tuple[Optional[str], int]:
-
         assert adj_ws is not None
         (
             child_list_token,
             parent_list_token,
         ) = ListBlockProcessor.__determine_child_and_parent_tokens(parser_state)
         POGGER.debug("len(adj_ws)>>$", len(adj_ws))
 
@@ -293,15 +297,14 @@
     @staticmethod
     def __is_start_phase_one(
         parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         is_not_one: bool,
     ) -> Tuple[bool, int]:
-
         start_index += 1
         line_to_parse_size = len(line_to_parse)
         after_all_whitespace_index, _ = ParserHelper.extract_spaces(
             line_to_parse, start_index
         )
         assert after_all_whitespace_index is not None
         POGGER.debug(
@@ -412,15 +415,15 @@
         is_ulist: bool,
     ) -> Tuple[
         Callable[
             [ParserState, str, int, Optional[str], bool, Optional[str]],
             Tuple[bool, int, Optional[int], Optional[int]],
         ],
         Callable[
-            [PositionMarker, int, Optional[str], int, int, int],
+            [PositionMarker, int, int, Optional[str], Optional[str], int, int, int],
             Tuple[ListStartMarkdownToken, ListStackToken],
         ],
     ]:
         if is_ulist:
             POGGER.debug("hlb>>searching for ulist")
             is_start_fn = ListBlockProcessor.is_ulist_start
             create_token_fn = ListBlockProcessor.__handle_list_block_unordered
@@ -478,15 +481,14 @@
         parser_state: ParserState,
         container_depth: int,
         removed_chars_at_start: int,
         extracted_whitespace: Optional[str],
         indent_already_processed: bool,
         adj_ws: Optional[str],
     ) -> Tuple[int, Optional[str], Optional[str], Optional[str], bool]:
-
         indent_already_used, forced_container_whitespace = 0, None
         is_in_root_list = (
             not container_depth
             and parser_state.token_stack
             and len(parser_state.token_stack) >= 2
             and parser_state.token_stack[1].is_list
         )
@@ -498,15 +500,14 @@
         if (
             not removed_chars_at_start
             and is_in_root_list
             and adj_ws == extracted_whitespace
             and len(extracted_whitespace) >= 4
             and not indent_already_processed
         ):
-
             # POGGER.debug("extracted_whitespace>$<", extracted_whitespace)
             # POGGER.debug("parser_state.token_stack>$<", parser_state.token_stack)
             stack_index = 1
             acceptable_indent_stack_index = 0
             while (
                 stack_index < len(parser_state.token_stack)
                 and parser_state.token_stack[stack_index].is_list
@@ -541,30 +542,26 @@
             extracted_whitespace,
             adj_ws,
             indent_already_processed,
         )
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-locals, too-many-arguments
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_list_block_init(
         parser_state: ParserState,
         position_marker: PositionMarker,
         extracted_whitespace: Optional[str],
         adj_ws: Optional[str],
         is_ulist: bool,
         container_depth: int,
         removed_chars_at_start: int,
         indent_already_processed: bool,
     ) -> Tuple[
-        Callable[
-            [PositionMarker, int, Optional[str], int, int, int],
-            Tuple[ListStartMarkdownToken, ListStackToken],
-        ],
         bool,
         int,
         Optional[int],
         Optional[int],
         int,
         Optional[str],
         Optional[str],
@@ -594,42 +591,41 @@
             container_depth,
             removed_chars_at_start,
             extracted_whitespace,
             indent_already_processed,
             adj_ws,
         )
 
-        is_start_fn, create_token_fn = ListBlockProcessor.__get_list_functions(is_ulist)
+        is_start_fn, _ = ListBlockProcessor.__get_list_functions(is_ulist)
         (
             started_ulist,
             end_of_ulist_start_index,
             index,
             number_of_digits,
         ) = is_start_fn(
             parser_state,
             position_marker.text_to_parse,
             position_marker.index_number,
             extracted_whitespace,
             False,
             adj_ws,
         )
         return (
-            create_token_fn,
             started_ulist,
             end_of_ulist_start_index,
             index,
             number_of_digits,
             indent_already_used,
             forced_container_whitespace,
             extracted_whitespace,
             adj_ws,
             indent_already_processed,
         )
 
-    # pylint: enable=too-many-locals, too-many-arguments
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __create_new_list_if_indented(
         parser_state: ParserState,
         position_marker: PositionMarker,
         indent_level: int,
@@ -640,22 +636,18 @@
         adj_ws: Optional[str],
         adjusted_text_to_parse: Optional[str],
         index: int,
         container_level_tokens: List[MarkdownToken],
         remaining_whitespace: int,
         after_marker_ws_index: int,
         current_container_blocks: List[StackToken],
-        create_token_fn: Callable[
-            [PositionMarker, int, Optional[str], int, int, int],
-            Tuple[ListStartMarkdownToken, ListStackToken],
-        ],
         container_depth: int,
+        original_line: str,
+        is_ulist: bool,
     ) -> Tuple[bool, Optional[str], Optional[RequeueLineInfo]]:
-        requeue_line_info = None
-        did_process = False
         POGGER.debug(
             "total=$;ws-before=$;ws_after=$;start_index=$",
             indent_level,
             ws_before_marker,
             ws_after_marker,
             position_marker.index_number,
         )
@@ -663,63 +655,98 @@
         if indent_level >= 0:
             POGGER.debug("indent_level=$=", indent_level)
             POGGER.debug("ws_before_marker=$=", ws_before_marker)
             POGGER.debug("forced_container_whitespace=$=", forced_container_whitespace)
             create_adj_ws = ListBlockProcessor.__calculate_create_adj_ws(
                 adj_ws, position_marker, parser_state
             )
-            (
-                adjusted_text_to_parse,
-                requeue_line_info,
-            ) = ListBlockProcessor.__create_new_list(
+            return ListBlockProcessor.__create_new_list(
                 parser_state,
                 position_marker,
                 indent_level,
                 extracted_whitespace,
                 ws_before_marker,
                 ws_after_marker,
                 index,
                 container_level_tokens,
                 remaining_whitespace,
                 after_marker_ws_index,
                 current_container_blocks,
-                create_token_fn,
                 container_depth,
+                original_line,
+                is_ulist,
                 adj_ws=create_adj_ws,
                 alt_adj_ws=adj_ws,
                 forced_container_whitespace=forced_container_whitespace,
             )
-            did_process = True
         return (
-            did_process,
+            False,
             adjusted_text_to_parse,
-            requeue_line_info,
+            None,
         )
 
     # pylint: enable=too-many-arguments, too-many-locals
 
+    @staticmethod
+    def __handle_list_block_pull_from_grab_bag(
+        grab_bag: ContainerGrabBag,
+    ) -> Tuple[
+        Optional[str],
+        Optional[str],
+        BlockQuoteData,
+        int,
+        List[StackToken],
+        int,
+        bool,
+        str,
+    ]:
+        extracted_whitespace: Optional[str] = grab_bag.extracted_whitespace
+        adj_ws: Optional[str] = grab_bag.adj_ws
+        block_quote_data: BlockQuoteData = grab_bag.block_quote_data
+        assert grab_bag.removed_chars_at_start_of_line is not None
+        removed_chars_at_start: int = grab_bag.removed_chars_at_start_of_line
+
+        current_container_blocks: List[StackToken] = grab_bag.current_container_blocks
+        container_depth: int = grab_bag.container_depth
+
+        indent_already_processed: bool = grab_bag.was_indent_already_processed
+        original_line = grab_bag.original_line
+
+        return (
+            extracted_whitespace,
+            adj_ws,
+            block_quote_data,
+            removed_chars_at_start,
+            current_container_blocks,
+            container_depth,
+            indent_already_processed,
+            original_line,
+        )
+
     # pylint: disable=too-many-locals
     @staticmethod
     def handle_list_block(
         is_ulist: bool,
         parser_state: ParserState,
         position_marker: PositionMarker,
         grab_bag: ContainerGrabBag,
     ) -> Tuple[bool, int, Optional[str], List[MarkdownToken]]:
         """
         Handle the processing of a ulist block.
         """
-        extracted_whitespace: Optional[str] = grab_bag.extracted_whitespace
-        adj_ws: Optional[str] = grab_bag.adj_ws
-        block_quote_data: BlockQuoteData = grab_bag.block_quote_data
-        assert grab_bag.removed_chars_at_start_of_line is not None
-        removed_chars_at_start: int = grab_bag.removed_chars_at_start_of_line
-        current_container_blocks: List[StackToken] = grab_bag.current_container_blocks
-        container_depth: int = grab_bag.container_depth
-        indent_already_processed: bool = grab_bag.was_indent_already_processed
+        (
+            extracted_whitespace,
+            adj_ws,
+            block_quote_data,
+            removed_chars_at_start,
+            current_container_blocks,
+            container_depth,
+            indent_already_processed,
+            original_line,
+        ) = ListBlockProcessor.__handle_list_block_pull_from_grab_bag(grab_bag)
 
         (
             did_process,
             requeue_line_info,
             old_extracted_whitespace,
             old_indent_already_processed,
         ) = (
@@ -728,15 +755,14 @@
             extracted_whitespace,
             indent_already_processed,
         )
         adjusted_text_to_parse: Optional[str] = position_marker.text_to_parse
         container_level_tokens: List[MarkdownToken] = []
 
         (
-            create_token_fn,
             started_ulist,
             end_of_ulist_start_index,
             index,
             number_of_digits,
             indent_already_used,
             forced_container_whitespace,
             extracted_whitespace,
@@ -750,18 +776,14 @@
             is_ulist,
             container_depth,
             removed_chars_at_start,
             indent_already_processed,
         )
         POGGER.debug("clt>>list-start=$", started_ulist)
         if started_ulist:
-
-            # if not j:
-            #     parser_state.token_stack[j].matching_markdown_token.add_leading_spaces(dfg)
-
             POGGER.debug("clt>>ulist-start")
             removed_chars_at_start = indent_already_used
             assert index is not None
             assert number_of_digits is not None
             (
                 indent_level,
                 remaining_whitespace,
@@ -797,34 +819,57 @@
                 adj_ws,
                 adjusted_text_to_parse,
                 index,
                 container_level_tokens,
                 remaining_whitespace,
                 after_marker_ws_index,
                 current_container_blocks,
-                create_token_fn,
                 container_depth,
+                original_line,
+                is_ulist,
             )
         else:
             extracted_whitespace = old_extracted_whitespace
             indent_already_processed = old_indent_already_processed
 
-        grab_bag.removed_chars_at_start_of_line = removed_chars_at_start
-        grab_bag.block_quote_data = block_quote_data
-        grab_bag.requeue_line_info = requeue_line_info
-        grab_bag.was_indent_already_processed = indent_already_processed
-        grab_bag.extracted_whitespace = extracted_whitespace
+        ListBlockProcessor.__handle_list_block_push_to_grab_bag(
+            grab_bag,
+            removed_chars_at_start,
+            block_quote_data,
+            requeue_line_info,
+            indent_already_processed,
+            extracted_whitespace,
+        )
 
         return (
             did_process,
             end_of_ulist_start_index,
             adjusted_text_to_parse,
             container_level_tokens,
         )
-        # pylint: enable=too-many-locals
+
+    # pylint: enable=too-many-locals
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __handle_list_block_push_to_grab_bag(
+        grab_bag: ContainerGrabBag,
+        removed_chars_at_start: int,
+        block_quote_data: BlockQuoteData,
+        requeue_line_info: Optional[RequeueLineInfo],
+        indent_already_processed: bool,
+        extracted_whitespace: Optional[str],
+    ) -> None:
+        grab_bag.removed_chars_at_start_of_line = removed_chars_at_start
+        grab_bag.block_quote_data = block_quote_data
+        grab_bag.requeue_line_info = requeue_line_info
+        grab_bag.was_indent_already_processed = indent_already_processed
+        grab_bag.extracted_whitespace = extracted_whitespace
+
+    # pylint: enable=too-many-arguments
 
     @staticmethod
     def __find_block_quote_before_list(
         parser_state: ParserState,
     ) -> Optional[BlockQuoteStackToken]:
         POGGER.debug_with_visible_whitespace(
             "parser_state.token_stack>$", parser_state.token_stack
@@ -842,69 +887,181 @@
                     break
                 token_stack_index -= 1
         POGGER.debug_with_visible_whitespace(
             "found_block_quote_before_list>$", found_block_quote_before_list
         )
         return found_block_quote_before_list
 
-    # pylint: disable=too-many-locals, too-many-arguments
+    @staticmethod
+    def __create_new_list_with_tab(
+        position_marker: PositionMarker,
+        original_line: str,
+        is_ulist: bool,
+        whitespace_to_add: Optional[str],
+        index: int,
+    ) -> Tuple[Optional[str], int]:
+        tabbed_whitespace_to_add = None
+        tabbed_adjust = -1
+        (
+            tabbed_extract_spaces_index,
+            tabbed_extract_spaces,
+        ) = ParserHelper.extract_spaces(original_line, 0)
+        POGGER.debug("tabbed_extract_spaces_index>:$:<", tabbed_extract_spaces_index)
+        assert tabbed_extract_spaces_index is not None
+        assert tabbed_extract_spaces is not None
+        POGGER.debug("tabbed_extract_spaces>:$:<", tabbed_extract_spaces)
+        POGGER.debug("text_to_parse>:$:<", position_marker.text_to_parse)
+        POGGER.debug("index_number>:$:<", position_marker.index_number)
+        detabbed_tabbed_extract_spaces = TabHelper.detabify_string(
+            tabbed_extract_spaces
+        )
+        POGGER.debug(
+            "detabbed_tabbed_extract_spaces>:$:<", detabbed_tabbed_extract_spaces
+        )
+        assert detabbed_tabbed_extract_spaces == whitespace_to_add
+        if "\t" in tabbed_extract_spaces:
+            tabbed_whitespace_to_add = tabbed_extract_spaces
+
+        POGGER.debug("is_ulist>:$:<", is_ulist)
+
+        # parse_index = position_marker.text_to_parse[position_marker.index_number]
+        # POGGER.debug("parse_index>:$:<", parse_index)
+        parse_index = 1 if is_ulist else index - position_marker.index_number + 1
+        POGGER.debug("parse_index>:$:<", parse_index)
+
+        new_index = position_marker.index_number + parse_index
+        untabbed_marker = position_marker.text_to_parse[
+            position_marker.index_number : new_index
+        ]
+        POGGER.debug("untabbed_marker>:$:<", untabbed_marker)
+        tabbed_marker = original_line[
+            tabbed_extract_spaces_index : tabbed_extract_spaces_index + parse_index
+        ]
+        POGGER.debug("tabbed_marker>:$:<", tabbed_marker)
+        assert untabbed_marker == tabbed_marker
+
+        tabbed_extract_spaces_index += len(tabbed_marker)
+        POGGER.debug(
+            "position_marker.text_to_parse[new_index:]>:$:<",
+            position_marker.text_to_parse[new_index:],
+        )
+        POGGER.debug(
+            "original_line[tabbed_extract_spaces_index:]>:$:<",
+            original_line[tabbed_extract_spaces_index:],
+        )
+        if original_line[tabbed_extract_spaces_index] == "\t":
+            POGGER.debug("new_index>:$:<", new_index)
+            POGGER.debug(
+                "tabbed_extract_spaces_index>:$:<", tabbed_extract_spaces_index
+            )
+            adj_string = TabHelper.detabify_string(
+                original_line[tabbed_extract_spaces_index],
+                additional_start_delta=new_index,
+            )
+            POGGER.debug("adj_string>:$:<", adj_string)
+            tabbed_adjust = len(adj_string) - 1
+            POGGER.debug("tabbed_adjust>:$:<", tabbed_adjust)
+
+        return tabbed_whitespace_to_add, tabbed_adjust
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __create_new_list_handle_whitespace(
+        forced_container_whitespace: Optional[str],
+        alt_adj_ws: Optional[str],
+        ws_before_marker: int,
+        indent_level: int,
+        extracted_whitespace: Optional[str],
+        adj_ws: Optional[str],
+    ) -> Tuple[Optional[str], Optional[str], int, int]:
+        if forced_container_whitespace:
+            whitespace_to_add: Optional[str] = forced_container_whitespace
+            assert whitespace_to_add is not None
+            if alt_adj_ws:
+                whitespace_to_add += alt_adj_ws
+            ws_before_marker += len(forced_container_whitespace)
+            indent_level += len(forced_container_whitespace)
+            assert alt_adj_ws is not None
+            alt_adj_ws += forced_container_whitespace
+        else:
+            whitespace_to_add = extracted_whitespace if adj_ws is None else adj_ws
+        return whitespace_to_add, alt_adj_ws, ws_before_marker, indent_level
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments, too-many-locals
     @staticmethod
     def __create_new_list(
         parser_state: ParserState,
         position_marker: PositionMarker,
         indent_level: int,
         extracted_whitespace: Optional[str],
         ws_before_marker: int,
         ws_after_marker: int,
         index: int,
         container_level_tokens: List[MarkdownToken],
         remaining_whitespace: int,
         after_marker_ws_index: int,
         current_container_blocks: List[StackToken],
-        create_token_fn: Callable[
-            [PositionMarker, int, Optional[str], int, int, int],
-            Tuple[ListStartMarkdownToken, ListStackToken],
-        ],
         container_depth: int,
+        original_line: str,
+        is_ulist: bool,
         adj_ws: Optional[str] = None,
         alt_adj_ws: Optional[str] = None,
         forced_container_whitespace: Optional[str] = None,
-    ) -> Tuple[Optional[str], Optional[RequeueLineInfo]]:
+    ) -> Tuple[bool, Optional[str], Optional[RequeueLineInfo]]:
         found_block_quote_before_list = (
             ListBlockProcessor.__find_block_quote_before_list(parser_state)
         )
         if found_block_quote_before_list and adj_ws is None and alt_adj_ws is not None:
             adj_ws = alt_adj_ws
 
-        POGGER.debug("ws_before_marker=$=", ws_before_marker)
-        POGGER.debug("forced_container_whitespace=$=", forced_container_whitespace)
-        if forced_container_whitespace:
-            whitespace_to_add: Optional[str] = forced_container_whitespace
-            assert whitespace_to_add is not None
-            if alt_adj_ws:
-                whitespace_to_add += alt_adj_ws
-            ws_before_marker += len(forced_container_whitespace)
-            indent_level += len(forced_container_whitespace)
-            assert alt_adj_ws is not None
-            alt_adj_ws += forced_container_whitespace
-        else:
-            whitespace_to_add = extracted_whitespace if adj_ws is None else adj_ws
-        POGGER.debug("ws_before_marker=$=", ws_before_marker)
-        POGGER.debug_with_visible_whitespace("whitespace_to_add>$:", whitespace_to_add)
-        POGGER.debug_with_visible_whitespace("adj_ws>$<", adj_ws)
-        POGGER.debug_with_visible_whitespace("alt_adj_ws>$<", alt_adj_ws)
-        new_token, new_stack = create_token_fn(
+        # POGGER.debug("ws_before_marker=$=", ws_before_marker)
+        # POGGER.debug("forced_container_whitespace=$=", forced_container_whitespace)
+        (
+            whitespace_to_add,
+            alt_adj_ws,
+            ws_before_marker,
+            indent_level,
+        ) = ListBlockProcessor.__create_new_list_handle_whitespace(
+            forced_container_whitespace,
+            alt_adj_ws,
+            ws_before_marker,
+            indent_level,
+            extracted_whitespace,
+            adj_ws,
+        )
+        # POGGER.debug("ws_before_marker=$=", ws_before_marker)
+        # POGGER.debug_with_visible_whitespace("whitespace_to_add>$:", whitespace_to_add)
+        # POGGER.debug_with_visible_whitespace("adj_ws>$<", adj_ws)
+        # POGGER.debug_with_visible_whitespace("alt_adj_ws>$<", alt_adj_ws)
+        # POGGER.debug("original_line>:$:<", original_line)
+        # POGGER.debug("ws_after_marker=$=", ws_after_marker)
+        tabbed_whitespace_to_add = None
+        tabbed_adjust = -1
+        if "\t" in original_line:
+            (
+                tabbed_whitespace_to_add,
+                tabbed_adjust,
+            ) = ListBlockProcessor.__create_new_list_with_tab(
+                position_marker, original_line, is_ulist, whitespace_to_add, index
+            )
+
+        _, other_create_token_fn = ListBlockProcessor.__get_list_functions(is_ulist)
+        new_token, new_stack = other_create_token_fn(
             position_marker,
             indent_level,
+            tabbed_adjust,
             whitespace_to_add,
+            tabbed_whitespace_to_add,
             ws_before_marker,
             ws_after_marker,
             index,
         )
-        POGGER.debug_with_visible_whitespace("__create_new_list>$", new_token)
+        # POGGER.debug_with_visible_whitespace("__create_new_list>$", new_token)
 
         (
             new_container_level_tokens,
             adjusted_text_to_parse,
             requeue_line_info,
         ) = ListBlockProcessor.__post_list(
             parser_state,
@@ -918,37 +1075,41 @@
             position_marker,
             adj_ws,
             alt_adj_ws,
             container_depth,
         )
         assert new_container_level_tokens is not None
         container_level_tokens.extend(new_container_level_tokens)
-        return adjusted_text_to_parse, requeue_line_info
+        return True, adjusted_text_to_parse, requeue_line_info
 
-    # pylint: enable=too-many-locals, too-many-arguments
+    # pylint: enable=too-many-arguments, too-many-locals
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_list_block_unordered(
         position_marker: PositionMarker,
         indent_level: int,
+        tabbed_adjust: int,
         extracted_whitespace: Optional[str],
+        tabbed_whitespace_to_add: Optional[str],
         ws_before_marker: int,
         ws_after_marker: int,
         index: int,
     ) -> Tuple[ListStartMarkdownToken, ListStackToken]:
         # This is done to allow for this function and __handle_list_block_ordered
         # to be called using the same pattern.
         _ = index
 
         assert extracted_whitespace is not None
         new_token = UnorderedListStartMarkdownToken(
             position_marker.text_to_parse[position_marker.index_number],
             indent_level,
+            tabbed_adjust,
             extracted_whitespace,
+            tabbed_whitespace_to_add,
             position_marker,
         )
 
         POGGER.debug("unordered-token-->$", new_token)
 
         return new_token, UnorderedListStackToken(
             indent_level,
@@ -962,25 +1123,29 @@
     # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __handle_list_block_ordered(
         position_marker: PositionMarker,
         indent_level: int,
+        tabbed_adjust: int,
         extracted_whitespace: Optional[str],
+        tabbed_whitespace_to_add: Optional[str],
         ws_before_marker: int,
         ws_after_marker: int,
         index: int,
     ) -> Tuple[ListStartMarkdownToken, ListStackToken]:
         assert extracted_whitespace is not None
         new_token = OrderedListStartMarkdownToken(
             position_marker.text_to_parse[index],
             position_marker.text_to_parse[position_marker.index_number : index],
             indent_level,
+            tabbed_adjust,
             extracted_whitespace,
+            tabbed_whitespace_to_add,
             position_marker,
         )
 
         POGGER.debug("ordered-token-->$", new_token)
 
         return new_token, OrderedListStackToken(
             indent_level,
@@ -998,79 +1163,90 @@
         parser_state: ParserState,
         ind: Optional[int],
         used_indent: Optional[str],
         was_paragraph_continuation: bool,
         start_index: int,
     ) -> None:
         assert ind is not None
-        POGGER.debug(">>used_indent>>$<<", used_indent)
-        POGGER.debug(">>was_paragraph_continuation>>$<<", was_paragraph_continuation)
-        if used_indent is not None:
-            block_token = cast(
-                BlockQuoteMarkdownToken,
-                parser_state.token_stack[ind].matching_markdown_token,
+
+        stack_index = parser_state.find_last_list_block_on_stack()
+        if stack_index > 0:
+            list_token = cast(
+                ListStartMarkdownToken,
+                parser_state.token_stack[stack_index].matching_markdown_token,
             )
             POGGER.debug(
                 "lip>>last_block_token>>$",
-                block_token,
+                list_token,
             )
-            block_token.add_leading_spaces(used_indent)
-            POGGER.debug(
-                "lip>>last_block_token>>$",
-                block_token,
+
+        POGGER.debug(">>used_indent>>$<<", used_indent)
+        POGGER.debug(">>was_paragraph_continuation>>$<<", was_paragraph_continuation)
+        if used_indent is not None:
+            list_token = cast(
+                ListStartMarkdownToken,
+                parser_state.token_stack[ind].matching_markdown_token,
             )
+            # POGGER.debug(
+            #     "lip>>list_token>>$",
+            #     list_token,
+            # )
+            list_token.add_leading_spaces(used_indent)
+            # POGGER.debug(
+            #     "lip>>list_token>>$",
+            #     list_token,
+            # )
         else:
-            need_to_add_leading_spaces = False
             stack_index = parser_state.find_last_list_block_on_stack()
+            need_to_add_leading_spaces = False
             if stack_index > 0:
-
                 assert parser_state.original_line_to_parse is not None
 
                 last_container_index = parser_state.find_last_container_on_stack()
-                POGGER.debug("ind=:$:", ind)
-                POGGER.debug("parser_state.token_stack=:$:", parser_state.token_stack)
-                POGGER.debug(
-                    "parser_state.token_stack[ind]=:$:", parser_state.token_stack[ind]
-                )
-                POGGER.debug(
-                    "parser_state.original_line_to_parse=:$:",
-                    parser_state.original_line_to_parse,
-                )
-                POGGER.debug("start_index=:$:", start_index)
-                POGGER.debug("stack_index=:$:", stack_index)
+                # POGGER.debug("ind=:$:", ind)
+                # POGGER.debug("parser_state.token_stack=:$:", parser_state.token_stack)
+                # POGGER.debug(
+                #     "parser_state.token_stack[ind]=:$:", parser_state.token_stack[ind]
+                # )
+                # POGGER.debug(
+                #     "parser_state.original_line_to_parse=:$:",
+                #     parser_state.original_line_to_parse,
+                # )
+                # POGGER.debug("start_index=:$:", start_index)
+                # POGGER.debug("stack_index=:$:", stack_index)
                 consumed_text = parser_state.original_line_to_parse[:start_index]
-                POGGER.debug("consumed_text=:$:", consumed_text)
+                # POGGER.debug("consumed_text=:$:", consumed_text)
                 back_index = stack_index
                 while back_index and parser_state.token_stack[back_index].is_list:
                     back_index -= 1
-                POGGER.debug("back_index=:$:", back_index)
-                need_to_add_leading_spaces = not (
-                    back_index > 0
-                    and consumed_text
-                    and ">" not in consumed_text
-                    and stack_index == last_container_index
-                )
-                POGGER.debug(
-                    "need_to_add_leading_spaces=:$:", need_to_add_leading_spaces
-                )
+                # POGGER.debug("back_index=:$:", back_index)
+                need_to_add_leading_spaces = (
+                    back_index <= 0
+                    or not consumed_text
+                    or ">" in consumed_text
+                    or stack_index != last_container_index
+                )
+                # POGGER.debug(
+                #     "need_to_add_leading_spaces=:$:", need_to_add_leading_spaces
+                # )
 
             if need_to_add_leading_spaces:
                 list_token = cast(
                     ListStartMarkdownToken,
                     parser_state.token_stack[stack_index].matching_markdown_token,
                 )
-                POGGER.debug(
-                    "lip>>last_block_token>>$",
-                    list_token,
-                )
+                # POGGER.debug(
+                #     "lip>>last_block_token>>$",
+                #     list_token,
+                # )
                 list_token.add_leading_spaces("")
-                POGGER.debug(
-                    "lip>>last_block_token>>$",
-                    list_token,
-                )
+                # POGGER.debug(
+                #     "lip>>last_block_token>>$",
+                #     list_token,
+                # )
 
     @staticmethod
     def list_in_process(
         parser_state: ParserState, ind: Optional[int], grab_bag: ContainerGrabBag
     ) -> List[MarkdownToken]:
         """
         Handle the processing of a line where there is a list in process.
@@ -1080,30 +1256,30 @@
         extracted_whitespace = grab_bag.extracted_whitespace
 
         assert extracted_whitespace is not None
         assert ind is not None
         assert parser_state.token_stack[ind].is_list
         list_stack_token = cast(ListStackToken, parser_state.token_stack[ind])
         before_ws_length = list_stack_token.ws_before_marker
-        leading_space_length = ParserHelper.calculate_length(extracted_whitespace)
+        leading_space_length = TabHelper.calculate_length(extracted_whitespace)
         if list_stack_token.last_new_list_token:
             requested_list_indent = list_stack_token.last_new_list_token.indent_level
         else:
             requested_list_indent = list_stack_token.indent_level
 
-        POGGER.debug("!!!!!FOUND>>$", list_stack_token)
-        POGGER.debug("!!!!!FOUND>>$", list_stack_token.extra_data)
-        POGGER.debug("!!!!!ALL>>$", parser_state.token_stack)
-        POGGER.debug("!!!!!ALL>>$", parser_state.token_document)
-
-        POGGER.debug(
-            "!!!!!requested_list_indent>>$,before_ws=$",
-            requested_list_indent,
-            before_ws_length,
-        )
+        # POGGER.debug("!!!!!FOUND>>$", list_stack_token)
+        # POGGER.debug("!!!!!FOUND>>$", list_stack_token.extra_data)
+        # POGGER.debug("!!!!!ALL>>$", parser_state.token_stack)
+        # POGGER.debug("!!!!!ALL>>$", parser_state.token_document)
+
+        # POGGER.debug(
+        #     "!!!!!requested_list_indent>>$,before_ws=$",
+        #     requested_list_indent,
+        #     before_ws_length,
+        # )
 
         allow_list_continue = ListBlockProcessor.__can_list_continue(
             parser_state,
             line_to_parse,
             start_index,
             extracted_whitespace,
             leading_space_length,
@@ -1117,33 +1293,35 @@
         )
 
         used_indent = None
         was_paragraph_continuation = (
             leading_space_length >= requested_list_indent and allow_list_continue
         )
         if was_paragraph_continuation:
-
+            POGGER.debug("list-in-progress: was_paragraph_continuation")
             container_level_tokens: List[MarkdownToken] = []
-            POGGER.debug("before>>$>>", line_to_parse)
+            # POGGER.debug("before>>$>>", line_to_parse)
             (
                 line_to_parse,
                 used_indent,
             ) = ListBlockProcessor.__adjust_line_for_list_in_process(
                 line_to_parse,
                 start_index,
                 extracted_whitespace,
                 leading_space_length,
                 requested_list_indent,
+                grab_bag.original_line,
             )
-            POGGER.debug(
-                "after>>$>>$>>",
-                line_to_parse,
-                used_indent,
-            )
+            # POGGER.debug(
+            #     "after>>$>>$>>",
+            #     line_to_parse,
+            #     used_indent,
+            # )
         else:
+            POGGER.debug("list-in-progress: not was_paragraph_continuation")
             (
                 container_level_tokens,
                 line_to_parse,
                 used_indent,
                 ind,
                 requeue_line_info,
                 was_paragraph_continuation,
@@ -1153,14 +1331,15 @@
                 leading_space_length,
                 before_ws_length,
                 line_to_parse,
                 start_index,
                 extracted_whitespace,
                 allow_list_continue,
                 ind,
+                grab_bag.original_line,
             )
             if requeue_line_info:
                 grab_bag.line_to_parse = line_to_parse
                 grab_bag.indent_used_by_list = None
                 grab_bag.requeue_line_info = requeue_line_info
                 grab_bag.was_paragraph_continuation = False
                 return []
@@ -1207,29 +1386,33 @@
     @staticmethod
     def __check_for_paragraph_break(
         parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: Optional[str],
     ) -> bool:
+        POGGER.debug("is_theme_break>>?")
         is_theme_break, _ = LeafBlockProcessor.is_thematic_break(
             line_to_parse,
             start_index,
             extracted_whitespace,
             skip_whitespace_check=True,
         )
         POGGER.debug("is_theme_break>>$", is_theme_break)
+        POGGER.debug("is_atx_heading>>?")
         is_atx_heading, _, _, _ = LeafBlockProcessor.is_atx_heading(
             line_to_parse, start_index, extracted_whitespace, skip_whitespace_check=True
         )
         POGGER.debug("is_atx_heading>>$", is_atx_heading)
+        POGGER.debug("is_fenced_start>>?")
         is_fenced_start, _, _, _, _ = LeafBlockProcessor.is_fenced_code_block(
             line_to_parse, start_index, extracted_whitespace, skip_whitespace_check=True
         )
         POGGER.debug("is_fenced_start>>$", is_fenced_start)
+        POGGER.debug("is_html_start>>?")
         is_html_start, _ = HtmlHelper.is_html_block(
             line_to_parse,
             start_index,
             extracted_whitespace,
             parser_state.token_stack,
         )
         POGGER.debug("is_html_start>>$", is_html_start)
@@ -1248,28 +1431,27 @@
         leading_space_length: int,
         before_ws_length: int,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: Optional[str],
         allow_list_continue: bool,
         ind: Optional[int],
+        original_line: str,
     ) -> Tuple[
         List[MarkdownToken],
         str,
         Optional[str],
         Optional[int],
         Optional[RequeueLineInfo],
         bool,
     ]:
-
         POGGER.debug(
             "requested_list_indent>>$<<",
             requested_list_indent,
         )
-        original_requested_list_indent = requested_list_indent
         requested_list_indent -= before_ws_length
 
         POGGER.debug(
             "leading_space_length>>$>>adj requested_list_indent>>$>>$<<",
             leading_space_length,
             requested_list_indent,
             parser_state.token_stack[-1].is_paragraph,
@@ -1295,15 +1477,16 @@
                 line_to_parse,
                 used_indent,
             ) = ListBlockProcessor.__adjust_line_for_list_in_process(
                 line_to_parse,
                 start_index,
                 extracted_whitespace,
                 leading_space_length,
-                original_requested_list_indent,
+                requested_list_indent + before_ws_length,
+                original_line,
             )
             was_paragraph_continuation = used_indent is None
             POGGER.debug(
                 ">>line_to_parse>>$>>",
                 line_to_parse,
             )
             POGGER.debug(">>used_indent>>$>>", used_indent)
@@ -1324,31 +1507,30 @@
                 leading_space_length,
             )
             POGGER.debug(
                 "2>>requeue_line_info>>$>>",
                 requeue_line_info,
             )
             if requeue_line_info:
-                used_indent = None
-                ind = None
-                return [], line_to_parse, used_indent, ind, requeue_line_info, False
+                return [], line_to_parse, None, None, requeue_line_info, False
 
             (
                 line_to_parse,
                 used_indent,
                 ind,
             ) = ListBlockProcessor.__adjust_for_nested_list(
                 parser_state,
                 container_level_tokens,
                 ind,
                 line_to_parse,
                 extracted_whitespace,
                 start_index,
                 before_ws_length,
                 leading_space_length,
+                original_line,
             )
 
         return (
             container_level_tokens,
             line_to_parse,
             used_indent,
             ind,
@@ -1365,16 +1547,16 @@
         container_level_tokens: List[MarkdownToken],
         ind: Optional[int],
         line_to_parse: str,
         extracted_whitespace: Optional[str],
         start_index: int,
         before_ws_length: int,
         leading_space_length: int,
+        original_line: str,
     ) -> Tuple[str, Optional[str], Optional[int]]:
-
         assert ind is not None
         POGGER.debug(
             "2>>__check_for_list_closures>>$>>",
             container_level_tokens,
         )
         POGGER.debug(
             "2>>parser_state.token_stack>>$>>",
@@ -1420,24 +1602,25 @@
                 used_indent,
             ) = ListBlockProcessor.__adjust_line_for_list_in_process(
                 line_to_parse,
                 start_index,
                 extracted_whitespace,
                 leading_space_length,
                 requested_list_indent,
+                original_line,
             )
             POGGER.debug(">>line_to_parse>>$", line_to_parse)
             POGGER.debug(">>used_indent>>$<<", used_indent)
         else:
             used_indent = None
         return line_to_parse, used_indent, ind
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __pre_list(
         parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: Optional[str],
         marker_width_minus_one: int,
@@ -1470,14 +1653,38 @@
             marker_width_minus_one,
             ws_after_marker,
             ws_before_marker,
             adj_ws,
             container_depth,
         )
 
+        return ListBlockProcessor.__check_for_list_nesting(
+            parser_state,
+            position_marker,
+            indent_level,
+            after_marker_ws_index,
+            block_quote_data,
+            remaining_whitespace,
+            ws_after_marker,
+            ws_before_marker,
+        )
+        # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __check_for_list_nesting(
+        parser_state: ParserState,
+        position_marker: PositionMarker,
+        indent_level: int,
+        after_marker_ws_index: int,
+        block_quote_data: BlockQuoteData,
+        remaining_whitespace: int,
+        ws_after_marker: int,
+        ws_before_marker: int,
+    ) -> Tuple[int, int, int, int, int, List[MarkdownToken], BlockQuoteData]:
         check_list_nesting = True
         if (
             parser_state.token_stack[-1].is_html_block
             or parser_state.token_stack[-1].is_fenced_code_block
         ):
             did_find, _ = LeafBlockProcessorParagraph.check_for_list_in_process(
                 parser_state
@@ -1509,42 +1716,42 @@
                 container_level_tokens,
                 block_quote_data,
             ) = ListBlockProcessor.__handle_list_nesting(
                 parser_state, block_quote_data, position_marker
             )
         else:
             container_level_tokens = []
-
         return (
             indent_level,
             remaining_whitespace,
             ws_after_marker,
             after_marker_ws_index,
             ws_before_marker,
             container_level_tokens,
             block_quote_data,
         )
-        # pylint: enable=too-many-arguments, too-many-locals
+
+    # pylint: enable=too-many-arguments
 
     @staticmethod
     def __calculate_whitespace_values(
         line_to_parse: str, start_index: int, extracted_whitespace: Optional[str]
     ) -> Tuple[int, int, int, int]:
         (
             after_marker_ws_index,
             after_marker_whitespace,
         ) = ParserHelper.extract_spaces(line_to_parse, start_index + 1)
         assert after_marker_ws_index is not None
         assert after_marker_whitespace is not None
         assert extracted_whitespace is not None
         ws_after_marker, ws_before_marker, line_to_parse_size = (
-            ParserHelper.calculate_length(
+            TabHelper.calculate_length(
                 after_marker_whitespace, start_index=start_index + 1
             ),
-            ParserHelper.calculate_length(extracted_whitespace),
+            TabHelper.calculate_length(extracted_whitespace),
             len(line_to_parse),
         )
         POGGER.debug(
             "after-marker>>$>>total=$", after_marker_whitespace, ws_after_marker
         )
         return (
             after_marker_ws_index,
@@ -1627,15 +1834,14 @@
             ">>block_quote_data.stack_count>>$>>block_quote_data.current_count>>$",
             block_quote_data.stack_count,
             block_quote_data.current_count,
         )
         container_level_tokens: List[MarkdownToken] = []
         adjusted_stack_count = block_quote_data.stack_count
         while block_quote_data.current_count < adjusted_stack_count:
-
             assert not container_level_tokens
             last_block_index = parser_state.find_last_block_quote_on_stack()
             previous_last_block_token = cast(
                 BlockQuoteMarkdownToken,
                 parser_state.token_stack[last_block_index].matching_markdown_token,
             )
             POGGER.debug(
@@ -1718,23 +1924,23 @@
         )
 
         POGGER.debug(
             "prev>>$<<, current>>$<<",
             previous_last_block_token,
             current_last_block_token,
         )
-        removed_leading_spaces = previous_last_block_token.remove_last_leading_space()
+        removed_leading_spaces = previous_last_block_token.remove_last_bleading_space()
         POGGER.debug("removed_leading_spaces>>$<<", removed_leading_spaces)
         assert removed_leading_spaces is not None
         POGGER.debug(
             "prev>>$<<, current>>$<<",
             previous_last_block_token,
             current_last_block_token,
         )
-        current_last_block_token.add_leading_spaces(
+        current_last_block_token.add_bleading_spaces(
             removed_leading_spaces, skip_adding_newline=True
         )
         POGGER.debug(
             "prev>>$<<, current>>$<<",
             previous_last_block_token,
             current_last_block_token,
         )
@@ -1755,16 +1961,16 @@
         alt_adj_ws: Optional[str],
         container_depth: int,
     ) -> Tuple[Optional[List[MarkdownToken]], Optional[str], Optional[RequeueLineInfo]]:
         """
         Handle the processing of the last part of the list.
         """
 
-        POGGER.debug("new_stack>>$", new_stack)
-        POGGER.debug("indent_level>>$", indent_level)
+        # POGGER.debug("new_stack>>$", new_stack)
+        # POGGER.debug("indent_level>>$", indent_level)
 
         (
             did_find,
             last_list_index,
         ) = LeafBlockProcessorParagraph.check_for_list_in_process(parser_state)
         if did_find:
             POGGER.debug(
@@ -1772,14 +1978,15 @@
                 parser_state.token_stack[last_list_index],
             )
             (
                 container_level_tokens,
                 emit_li,
                 requeue_line_info,
             ) = ListBlockProcessor.__close_required_lists_after_start(
+                position_marker,
                 parser_state,
                 last_list_index,
                 new_stack,
                 new_token,
                 current_container_blocks,
                 container_depth,
             )
@@ -1789,15 +1996,15 @@
             POGGER.debug(
                 "NOT list-in-process>>$",
                 parser_state.token_stack[last_list_index],
             )
             container_level_tokens, _ = parser_state.close_open_blocks_fn(
                 parser_state, was_forced=True
             )
-        POGGER.debug("container_level_tokens>>$", container_level_tokens)
+        # POGGER.debug("container_level_tokens>>$", container_level_tokens)
 
         assert container_level_tokens is not None
         POGGER.debug("__post_list>>before>>$", container_level_tokens)
         if not did_find or not emit_li:
             POGGER.debug("__post_list>>adding>>$", new_token)
             parser_state.token_stack.append(new_stack)
             container_level_tokens.append(new_token)
@@ -1809,20 +2016,20 @@
                 new_token,
                 container_level_tokens,
                 indent_level,
                 position_marker,
                 adj_ws,
                 alt_adj_ws,
             )
-        POGGER.debug(
-            "__post_list>>rem>>$>>after_in>>$",
-            remaining_whitespace,
-            after_marker_ws_index,
-        )
-        POGGER.debug("__post_list>>after>>$", container_level_tokens)
+        # POGGER.debug(
+        #     "__post_list>>rem>>$>>after_in>>$",
+        #     remaining_whitespace,
+        #     after_marker_ws_index,
+        # )
+        # POGGER.debug("__post_list>>after>>$", container_level_tokens)
 
         parser_state.set_no_para_start_if_empty()
         padded_spaces = ParserHelper.repeat_string(
             ParserHelper.space_character, remaining_whitespace
         )
         return (
             container_level_tokens,
@@ -1897,14 +2104,15 @@
         container_level_tokens.append(replacement_token)
 
     # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __close_required_lists_after_start(
+        position_marker: PositionMarker,
         parser_state: ParserState,
         last_list_index: int,
         new_stack: ListStackToken,
         new_token: ListStartMarkdownToken,
         current_container_blocks: List[StackToken],
         container_depth: int,
     ) -> Tuple[
@@ -1953,29 +2161,37 @@
         POGGER.debug("old-stack>>$<<", container_level_tokens)
         while repeat_check:
             (
                 repeat_check,
                 emit_li_token_instead_of_list_start_token,
                 last_list_index,
             ) = ListBlockProcessor.__close_next_level_of_lists(
+                position_marker,
                 parser_state,
                 new_stack,
                 new_token,
                 current_container_blocks,
                 container_level_tokens,
                 last_list_index,
                 container_depth,
             )
+        POGGER.debug("token_stack>>$", parser_state.token_stack)
+        POGGER.debug("container_level_tokens>>$", container_level_tokens)
+        POGGER.debug(
+            "emit_li_token_instead_of_list_start_token>>$",
+            emit_li_token_instead_of_list_start_token,
+        )
         return container_level_tokens, emit_li_token_instead_of_list_start_token, None
 
     # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __close_next_level_of_lists(
+        position_marker: PositionMarker,
         parser_state: ParserState,
         new_stack: ListStackToken,
         new_token: ListStartMarkdownToken,
         current_container_blocks: List[StackToken],
         container_level_tokens: List[MarkdownToken],
         last_list_index: int,
         container_depth: int,
@@ -1983,109 +2199,127 @@
         POGGER.debug("start")
 
         (
             do_not_emit,
             emit_li_token_instead_of_list_start_token,
             extra_tokens,
         ) = ListBlockProcessor.__are_list_starts_equal(
+            position_marker,
             parser_state,
             last_list_index,
             new_stack,
-            new_token,
             current_container_blocks,
             container_depth,
         )
         POGGER.debug("extra_tokens>>$", extra_tokens)
         POGGER.debug(
             "emit_li_token_instead_of_list_start_token>>$",
             emit_li_token_instead_of_list_start_token,
         )
         POGGER.debug("do_not_emit>>$", do_not_emit)
         container_level_tokens.extend(extra_tokens)
         repeat_check = False
         if do_not_emit:
             (
-                did_find,
                 last_list_index,
                 repeat_check,
             ) = ListBlockProcessor.__close_next_level_of_lists_do_not_emit(
                 parser_state,
                 new_stack,
                 new_token,
                 current_container_blocks,
                 emit_li_token_instead_of_list_start_token,
                 container_level_tokens,
                 container_depth,
             )
         else:
             POGGER.debug("post_list>>close open blocks and emit")
-            close_tokens, _ = parser_state.close_open_blocks_fn(
-                parser_state,
-                until_this_index=last_list_index,
-                include_lists=True,
-                include_block_quotes=True,
-            )
-            container_level_tokens.extend(close_tokens)
-
             (
-                did_find,
+                repeat_check,
                 last_list_index,
-            ) = LeafBlockProcessorParagraph.check_for_list_in_process(parser_state)
-            POGGER.debug(
-                "did_find>>$--last_list_index--$",
-                did_find,
+            ) = ListBlockProcessor.__close_next_level_of_lists_do_emit(
+                parser_state,
                 last_list_index,
+                container_level_tokens,
+                new_stack,
+                new_token,
             )
-            if did_find:
-                last_list_stack_token = cast(
-                    ListStackToken, parser_state.token_stack[last_list_index]
-                )
-                POGGER.debug(
-                    "ARE-EQUAL>>stack>>$>>new>>$",
-                    last_list_stack_token,
-                    new_stack,
-                )
-                POGGER.debug(
-                    "ARE-EQUAL>>stack>>$>>new>>$",
-                    last_list_stack_token.matching_markdown_token,
-                    new_token,
-                )
-                last_list_markdown_token = cast(
-                    ListStartMarkdownToken,
-                    last_list_stack_token.matching_markdown_token,
-                )
-                old_indent = 2
-                if last_list_markdown_token.is_ordered_list_start:
-                    old_indent += len(last_list_markdown_token.list_start_content)
-                POGGER.debug(
-                    "new_token.column_number($) <= old_indent($)",
-                    new_token.column_number,
-                    old_indent,
-                )
-                repeat_check = (
-                    new_token.column_number <= last_list_stack_token.indent_level
-                )
-                POGGER.debug(
-                    "repeat_check($) = new_token.column_number($) - last_list_stack_token.indent_level($)",
-                    repeat_check,
-                    new_token.column_number,
-                    last_list_stack_token.indent_level,
-                )
         return repeat_check, emit_li_token_instead_of_list_start_token, last_list_index
 
     @staticmethod
+    def __close_next_level_of_lists_do_emit(
+        parser_state: ParserState,
+        last_list_index: int,
+        container_level_tokens: List[MarkdownToken],
+        new_stack: ListStackToken,
+        new_token: ListStartMarkdownToken,
+    ) -> Tuple[bool, int]:
+        close_tokens, _ = parser_state.close_open_blocks_fn(
+            parser_state,
+            until_this_index=last_list_index,
+            include_lists=True,
+            include_block_quotes=True,
+        )
+        container_level_tokens.extend(close_tokens)
+
+        (
+            did_find,
+            last_list_index,
+        ) = LeafBlockProcessorParagraph.check_for_list_in_process(parser_state)
+        POGGER.debug(
+            "did_find>>$--last_list_index--$",
+            did_find,
+            last_list_index,
+        )
+        repeat_check = False
+        if did_find:
+            last_list_stack_token = cast(
+                ListStackToken, parser_state.token_stack[last_list_index]
+            )
+            POGGER.debug(
+                "ARE-EQUAL>>stack>>$>>new>>$",
+                last_list_stack_token,
+                new_stack,
+            )
+            POGGER.debug(
+                "ARE-EQUAL>>stack>>$>>new>>$",
+                last_list_stack_token.matching_markdown_token,
+                new_token,
+            )
+            last_list_markdown_token = cast(
+                ListStartMarkdownToken,
+                last_list_stack_token.matching_markdown_token,
+            )
+            old_indent = 2
+            if last_list_markdown_token.is_ordered_list_start:
+                old_indent += len(last_list_markdown_token.list_start_content)
+            POGGER.debug(
+                "new_token.column_number($) <= old_indent($)",
+                new_token.column_number,
+                old_indent,
+            )
+            repeat_check = new_token.column_number <= last_list_stack_token.indent_level
+            POGGER.debug(
+                "repeat_check($) = new_token.column_number($) - last_list_stack_token.indent_level($)",
+                repeat_check,
+                new_token.column_number,
+                last_list_stack_token.indent_level,
+            )
+        return repeat_check, last_list_index
+
+    @staticmethod
     def __close_next_level_of_lists_do_not_emit(
         parser_state: ParserState,
         new_stack: ListStackToken,
         new_token: ListStartMarkdownToken,
         current_container_blocks: List[StackToken],
         emit_li_token_instead_of_list_start_token: bool,
         container_level_tokens: List[MarkdownToken],
         container_depth: int,
-    ) -> Tuple[bool, int, bool]:
+    ) -> Tuple[int, bool]:
         POGGER.debug("post_list>>don't emit")
         (
             did_find,
             last_list_index,
         ) = LeafBlockProcessorParagraph.check_for_list_in_process(parser_state)
         assert last_list_index > 0
         last_list_index_token = cast(
@@ -2111,51 +2345,72 @@
         POGGER.debug(
             "emit_li_token_instead_of_list_start_token>:$:  repeat_check:$:",
             emit_li_token_instead_of_list_start_token,
             repeat_check,
         )
 
         if not repeat_check and not emit_li_token_instead_of_list_start_token:
-            parent_list_indent = last_list_index_token.indent_level
-            POGGER.debug("parent_list_indent>>$", parent_list_indent)
-            new_token_column_number = new_token.column_number
-            POGGER.debug("new_token_column_number>>$", new_token_column_number)
-            assert parser_state.original_line_to_parse is not None
-            intermediate_line_content = parser_state.original_line_to_parse[
-                parent_list_indent : new_token_column_number - 1
-            ]
-            POGGER.debug("intermediate_line_content:$:", intermediate_line_content)
-            if ">" not in intermediate_line_content:
-                close_tokens, _ = parser_state.close_open_blocks_fn(
-                    parser_state,
-                    until_this_index=last_list_index,
-                    include_block_quotes=True,
+            ListBlockProcessor.__close_next_level_of_lists_do_not_emit_cleanup(
+                parser_state,
+                last_list_index_token,
+                new_token,
+                last_list_index,
+                container_level_tokens,
+                container_depth,
+            )
+        return last_list_index, repeat_check
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __close_next_level_of_lists_do_not_emit_cleanup(
+        parser_state: ParserState,
+        last_list_index_token: ListStackToken,
+        new_token: ListStartMarkdownToken,
+        last_list_index: int,
+        container_level_tokens: List[MarkdownToken],
+        container_depth: int,
+    ) -> None:
+        parent_list_indent = last_list_index_token.indent_level
+        POGGER.debug("parent_list_indent>>$", parent_list_indent)
+        new_token_column_number = new_token.column_number
+        POGGER.debug("new_token_column_number>>$", new_token_column_number)
+        assert parser_state.original_line_to_parse is not None
+        intermediate_line_content = parser_state.original_line_to_parse[
+            parent_list_indent : new_token_column_number - 1
+        ]
+        POGGER.debug("intermediate_line_content:$:", intermediate_line_content)
+        if ">" not in intermediate_line_content:
+            close_tokens, _ = parser_state.close_open_blocks_fn(
+                parser_state,
+                until_this_index=last_list_index,
+                include_block_quotes=True,
+            )
+            if close_tokens:
+                container_level_tokens.extend(close_tokens)
+                assert not container_depth
+                list_token = cast(
+                    ListStartMarkdownToken,
+                    last_list_index_token.matching_markdown_token,
+                )
+                delta = new_token.column_number - list_token.column_number
+                new_token.set_extracted_whitespace(
+                    "".rjust(delta, ParserHelper.space_character)
                 )
-                if close_tokens:
-                    container_level_tokens.extend(close_tokens)
-                    assert not container_depth
-                    list_token = cast(
-                        ListStartMarkdownToken,
-                        last_list_index_token.matching_markdown_token,
-                    )
-                    delta = new_token.column_number - list_token.column_number
-                    new_token.set_extracted_whitespace(
-                        "".rjust(delta, ParserHelper.space_character)
-                    )
-        return did_find, last_list_index, repeat_check
 
-    # pylint: enable=too-many-arguments, too-many-locals
+    # pylint: enable=too-many-arguments
 
-    # pylint: disable=too-many-arguments, too-many-locals
+    # pylint: disable=too-many-arguments
     @staticmethod
     def __are_list_starts_equal(
+        position_marker: PositionMarker,
         parser_state: ParserState,
         last_list_index: int,
         new_stack: ListStackToken,
-        new_token: ListStartMarkdownToken,
         current_container_blocks: List[StackToken],
         container_depth: int,
     ) -> Tuple[bool, bool, List[MarkdownToken]]:
         """
         Check to see if the list starts are equal, and hence a continuation of
         the current list.
         """
@@ -2182,31 +2437,76 @@
         document_list_token = cast(
             ListStartMarkdownToken, parser_state.token_document[document_token_index]
         )
         last_list_stack_token = cast(
             ListStackToken, parser_state.token_stack[last_list_index]
         )
 
+        POGGER.debug("parser_state.token_document=$", parser_state.token_document)
+        POGGER.debug("parser_state.token_stack=$", parser_state.token_stack)
         POGGER.debug("ARE-EQUAL>>Last_List_token=$", document_list_token)
         old_start_index, old_last_marker_character, current_start_index = (
             document_list_token.indent_level,
             last_list_stack_token.list_character[-1],
             new_stack.ws_before_marker,
         )
         POGGER.debug(
             "old>>$>>$",
             last_list_stack_token.extra_data,
             old_last_marker_character,
         )
         POGGER.debug("new>>$>>$", new_stack.extra_data, new_stack.list_character[-1])
+        return ListBlockProcessor.__implement_based_on_equality(
+            parser_state,
+            position_marker,
+            last_list_stack_token,
+            old_last_marker_character,
+            new_stack,
+            current_start_index,
+            old_start_index,
+            current_container_blocks,
+            container_depth,
+        )
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def __implement_based_on_equality(
+        parser_state: ParserState,
+        position_marker: PositionMarker,
+        last_list_stack_token: ListStackToken,
+        old_last_marker_character: str,
+        new_stack: ListStackToken,
+        current_start_index: int,
+        old_start_index: int,
+        current_container_blocks: List[StackToken],
+        container_depth: int,
+    ) -> Tuple[bool, bool, List[MarkdownToken]]:
+        ## Determine if the new start is within the range of the old stack.  If so
+        ## AND some combination of the IF statement, then switch.
+        ## i.e. a + at col 1 followed by a - at column 1 is a new list
+        ## i.e. a + at col 1 followed by a - at column 3 is a new sublist
+        last_list_indent = last_list_stack_token.indent_level
+        if last_list_stack_token.last_new_list_token:
+            last_list_indent = last_list_stack_token.last_new_list_token.indent_level
+
+        POGGER.debug(
+            "position_marker.index_number>>$ >= xx>>$",
+            position_marker,
+            last_list_indent,
+        )
+        is_indented_enough = position_marker.index_number >= last_list_indent
+        POGGER.debug("is_indented_enough>>$", is_indented_enough)
         if (
-            last_list_stack_token.type_name == new_stack.type_name
-            and old_last_marker_character == new_stack.list_character[-1]
+            is_indented_enough
+            or old_last_marker_character == new_stack.list_character[-1]
+            and last_list_stack_token.type_name == new_stack.type_name
         ):
-            balancing_tokens = []
+            balancing_tokens: List[MarkdownToken] = []
             POGGER.debug("new_stack>$<", new_stack)
             POGGER.debug("new_stack>$<", new_stack.matching_markdown_token)
             POGGER.debug("old_stack>$<", last_list_stack_token)
             POGGER.debug(
                 "old_stack>$<",
                 last_list_stack_token.matching_markdown_token,
             )
@@ -2214,91 +2514,67 @@
                 ListBlockProcessor.__process_eligible_list_start(
                     parser_state,
                     balancing_tokens,
                     current_start_index,
                     old_start_index,
                     current_container_blocks,
                     new_stack,
+                    last_list_stack_token,
                 )
             )
             return True, emit_li_token_instead_of_list_start_token, balancing_tokens
 
         POGGER.debug("SUBLIST WITH DIFFERENT")
         POGGER.debug("container_depth:$:", container_depth)
         POGGER.debug("are_list_starts_equal>>ELIGIBLE!!!")
         POGGER.debug(
             "are_list_starts_equal>>current_start_index>>$>>old_start_index>>$",
             current_start_index,
             old_start_index,
         )
-        (
-            are_equal,
-            balancing_tokens,
-        ) = ListBlockProcessor.__are_list_starts_equal_cleanup(
-            parser_state,
-            current_start_index,
-            old_start_index,
-            new_token,
-            container_depth,
-        )
+        empty_balancing_tokens: List[MarkdownToken] = []
+        return current_start_index >= old_start_index, False, empty_balancing_tokens
 
-        return are_equal, False, balancing_tokens
-
-    # pylint: enable=too-many-arguments, too-many-locals
-
-    @staticmethod
-    def __are_list_starts_equal_cleanup(
-        parser_state: ParserState,
-        current_start_index: int,
-        old_start_index: int,
-        new_token: ListStartMarkdownToken,
-        container_depth: int,
-    ) -> Tuple[bool, List[MarkdownToken]]:
-        balancing_tokens: List[MarkdownToken] = []
-        are_equal = current_start_index >= old_start_index
-        POGGER.debug("are_list_starts_equal>>$", are_equal)
-
-        if (
-            are_equal
-            and not container_depth
-            and not parser_state.token_stack[-1].is_list
-        ):
-            POGGER.debug("parser_state.token_stack>>$", parser_state.token_stack)
-            stack_index = len(parser_state.token_stack) - 1
-            while stack_index and not parser_state.token_stack[stack_index].is_list:
-                stack_index -= 1
-            assert stack_index
-            balancing_tokens, _ = parser_state.close_open_blocks_fn(
-                parser_state,
-                until_this_index=stack_index + 1,
-                include_block_quotes=True,
-            )
-            POGGER.debug("parser_state.token_stack>>$", parser_state.token_stack)
-            new_token.set_extracted_whitespace(
-                "".rjust(new_token.column_number - 1, ParserHelper.space_character)
-            )
-        return are_equal, balancing_tokens
+    # pylint: enable=too-many-arguments
 
     # pylint: disable=too-many-arguments
     @staticmethod
     def __process_eligible_list_start(
         parser_state: ParserState,
         balancing_tokens: List[MarkdownToken],
         current_start_index: int,
         old_start_index: int,
         current_container_blocks: List[StackToken],
         new_stack: StackToken,
+        last_list_stack_token: ListStackToken,
     ) -> bool:
         POGGER.debug("are_list_starts_equal>>ELIGIBLE!!!")
+        POGGER.debug("current_container_blocks>>$", current_container_blocks)
         POGGER.debug(
             "are_list_starts_equal>>current_start_index>>$>>old_start_index>>$",
             current_start_index,
             old_start_index,
         )
-        if current_start_index >= old_start_index:
+        POGGER.debug("last_list_stack_token>>$", last_list_stack_token)
+        assert last_list_stack_token is not None
+        last_list_markdown_token = cast(
+            ListStartMarkdownToken, last_list_stack_token.matching_markdown_token
+        )
+        POGGER.debug("last_list_markdown_token>>$", last_list_markdown_token)
+
+        last_list_indent = last_list_markdown_token.indent_level
+        if last_list_stack_token.last_new_list_token:
+            last_list_indent = last_list_stack_token.last_new_list_token.indent_level
+
+        POGGER.debug(
+            "current_start_index>>$ >= last_list_indent>>$",
+            last_list_stack_token,
+            last_list_indent,
+        )
+        if current_start_index >= last_list_indent:
             return False
 
         POGGER.debug("current_container_blocks>>$", current_container_blocks)
         if len(current_container_blocks) > 1:
             POGGER.debug("current_container_blocks-->$", parser_state.token_stack)
             allow_list_removal = ListBlockProcessor.__calculate_can_remove_list(
                 parser_state, current_start_index
@@ -2377,15 +2653,14 @@
         return (
             adjusted_index > stack_index_token.indent_level
             or not with_previous_list_bounds
         )
 
     @staticmethod
     def __close_required_lists_calc(parser_state: ParserState) -> Tuple[int, int]:
-
         token_stack_index = len(parser_state.token_stack) - 1
         found_list_tokens = []
         while token_stack_index:
             if parser_state.token_stack[token_stack_index].is_list:
                 found_list_tokens.append(parser_state.token_stack[token_stack_index])
             token_stack_index -= 1
 
@@ -2457,25 +2732,63 @@
                 matching_column_number,
                 parent_indent_level,
                 allow_list_removal,
                 list_count,
             )
 
     @staticmethod
+    def __adjust_line_for_list_in_process_with_tab(
+        original_line: str, remaining_indent: int, removed_whitespace: str
+    ) -> str:
+        _, ex_ws = ParserHelper.extract_spaces(original_line, 0)
+        POGGER.debug("ex_ws($)", ex_ws)
+        assert ex_ws is not None
+        if "\t" in ex_ws:
+            detabified_ws = TabHelper.detabify_string(ex_ws, 0)
+            POGGER.debug("detabified_ws($)", detabified_ws)
+            assert len(detabified_ws) >= remaining_indent
+
+            sub_ws = None
+            i = -1
+            do_loop = True
+            # for i in range(len(ex_ws)):
+            while do_loop:
+                i += 1
+                assert i < len(ex_ws)
+                sub_ws = ex_ws[: i + 1]
+                POGGER.debug("sub_ws($)", sub_ws)
+                detabified_ws = TabHelper.detabify_string(sub_ws, 0)
+                POGGER.debug("detabified_ws($)", detabified_ws)
+                POGGER.debug(
+                    "detabified_ws($),removed_whitespace($)",
+                    len(detabified_ws),
+                    len(removed_whitespace),
+                )
+                if len(detabified_ws) >= len(removed_whitespace):
+                    do_loop = False
+            if len(detabified_ws) <= len(removed_whitespace):
+                assert sub_ws is not None
+                removed_whitespace = sub_ws
+        return removed_whitespace
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
     def __adjust_line_for_list_in_process(
         line_to_parse: str,
         start_index: int,
         leading_space: Optional[str],
         leading_space_length: int,
         requested_list_indent: int,
+        original_line: str,
     ) -> Tuple[str, Optional[str]]:
         """
         Alter the current line to better represent the current level of lists.
         """
         remaining_indent = leading_space_length - requested_list_indent
+        POGGER.debug("original_line($)", original_line)
         POGGER.debug(
             "enough ws to continue; line($),start_index($),leading_space($)",
             line_to_parse,
             start_index,
             leading_space,
         )
         POGGER.debug(
@@ -2486,23 +2799,34 @@
         )
         if remaining_indent < 0:
             padded_spaces = ""
             start_index = 0
             removed_whitespace = None
         else:
             assert leading_space is not None
+            POGGER.debug("requested_list_indent($)", requested_list_indent)
+            POGGER.debug("leading_space($)", leading_space)
             removed_whitespace = leading_space[:requested_list_indent]
             padded_spaces = ParserHelper.repeat_string(
                 ParserHelper.space_character, remaining_indent
             )
+            if "\t" in original_line:
+                removed_whitespace = (
+                    ListBlockProcessor.__adjust_line_for_list_in_process_with_tab(
+                        original_line, remaining_indent, removed_whitespace
+                    )
+                )
+        POGGER.debug("removed_whitespace($)", removed_whitespace)
         return (
             f"{padded_spaces}{line_to_parse[start_index:]}",
             removed_whitespace,
         )
 
+    # pylint: enable=too-many-arguments
+
     # pylint: disable=too-many-arguments
     @staticmethod
     def __check_for_list_closures(
         parser_state: ParserState,
         line_to_parse: str,
         start_index: int,
         extracted_whitespace: Optional[str],
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/main.py` & `pymarkdownlnt-0.9.9/pymarkdown/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,74 @@
 """
 Module to provide for a simple implementation of a title case algorithm.
 """
 import argparse
-import glob
 import logging
 import os
 import runpy
 import sys
 import tempfile
 import traceback
-from typing import List, Optional, Set, Tuple, cast
+from typing import List, Optional, cast
 
 from application_properties import (
     ApplicationProperties,
     ApplicationPropertiesJsonLoader,
 )
 
+from pymarkdown.application_file_scanner import ApplicationFileScanner
+from pymarkdown.application_logging import ApplicationLogging
 from pymarkdown.bad_tokenization_error import BadTokenizationError
 from pymarkdown.extension_manager.extension_manager import ExtensionManager
 from pymarkdown.extensions.pragma_token import PragmaToken
-from pymarkdown.parser_helper import ParserHelper
+from pymarkdown.main_presentation import MainPresentation
 from pymarkdown.parser_logger import ParserLogger
 from pymarkdown.plugin_manager.bad_plugin_error import BadPluginError
 from pymarkdown.plugin_manager.plugin_manager import PluginManager
 from pymarkdown.source_providers import FileSourceProvider
 from pymarkdown.tokenized_markdown import TokenizedMarkdown
 
 POGGER = ParserLogger(logging.getLogger(__name__))
 
 LOGGER = logging.getLogger(__name__)
 
+# pylint: disable=too-few-public-methods
+
 
 class PyMarkdownLint:
     """
     Class to provide for a simple implementation of a title case algorithm.
     """
 
-    available_log_maps = {
-        "CRITICAL": logging.CRITICAL,
-        "ERROR": logging.ERROR,
-        "WARNING": logging.WARNING,
-        "INFO": logging.INFO,
-        "DEBUG": logging.DEBUG,
-    }
-
     __normal_scan_subcommand = "scan"
     __stdin_scan_subcommand = "scan-stdin"
 
-    def __init__(self) -> None:
-        (
-            self.__version_number,
-            self.__show_stack_trace,
-            self.default_log_level,
-        ) = (PyMarkdownLint.__get_semantic_version(), False, "CRITICAL")
-        self.__tokenizer: Optional[TokenizedMarkdown] = None
+    def __init__(self, presentation: Optional[MainPresentation] = None) -> None:
+        self.__version_number = PyMarkdownLint.__get_semantic_version()
 
+        self.__presentation = presentation or MainPresentation()
         self.__properties: ApplicationProperties = ApplicationProperties()
-        self.__plugins: PluginManager = PluginManager()
-        self.__extensions: ExtensionManager = ExtensionManager()
+        self.__logging = ApplicationLogging(
+            self.__properties, default_log_level="CRITICAL"
+        )
+        self.__tokenizer: Optional[TokenizedMarkdown] = None
+        self.__plugins: PluginManager = PluginManager(self.__presentation)
+        self.__extensions: ExtensionManager = ExtensionManager(self.__presentation)
 
     @staticmethod
     def __get_semantic_version() -> str:
         file_path = __file__
         assert os.path.isabs(file_path)
         file_path = file_path.replace(os.sep, "/")
         last_index = file_path.rindex("/")
         file_path = f"{file_path[: last_index + 1]}version.py"
         version_meta = runpy.run_path(file_path)
         return str(version_meta["__version__"])
 
-    @staticmethod
-    def log_level_type(argument: str) -> str:
-        """
-        Function to help argparse limit the valid log levels.
-        """
-        if argument in PyMarkdownLint.available_log_maps:
-            return argument
-        raise ValueError(f"Value '{argument}' is not a valid log level.")
-
-    @staticmethod
-    def alternate_extension_type(argument: str) -> str:
-        """
-        Function to help argparse limit the valid log levels.
-        """
-        split_argument = argument.split(",")
-        for next_split in split_argument:
-            if not next_split.startswith("."):
-                raise argparse.ArgumentTypeError(
-                    f"Extension '{next_split}' must start with a period."
-                )
-            clean_split = next_split[1:]
-            if not clean_split:
-                raise argparse.ArgumentTypeError(
-                    f"Extension '{next_split}' must have at least one character after the period."
-                )
-            for clean_split_char in clean_split:
-                if not clean_split_char.isalnum():
-                    raise argparse.ArgumentTypeError(
-                        f"Extension '{next_split}' must only contain alphanumeric characters after the period."
-                    )
-        return argument.lower()
-
-    def __parse_arguments(self) -> argparse.Namespace:
+    def __parse_arguments(self, direct_args: Optional[List[str]]) -> argparse.Namespace:
         parser = argparse.ArgumentParser(description="Lint any found Markdown files.")
 
         parser.add_argument(
             "-e",
             "--enable-rules",
             dest="enable_rules",
             action="store",
@@ -170,119 +133,59 @@
         parser.add_argument(
             "--strict-config",
             dest="strict_configuration",
             action="store_true",
             default=False,
             help="throw an error if configuration is bad, instead of assuming default",
         )
-        parser.add_argument(
-            "--stack-trace",
-            dest="show_stack_trace",
-            action="store_true",
-            default=False,
-            help="if an error occurs, print out the stack trace for debug purposes",
-        )
-        parser.add_argument(
-            "--log-level",
-            dest="log_level",
-            action="store",
-            help="minimum level required to log messages",
-            type=PyMarkdownLint.log_level_type,
-            choices=list(PyMarkdownLint.available_log_maps.keys()),
-        )
-        parser.add_argument(
-            "--log-file",
-            dest="log_file",
-            action="store",
-            help="destination file for log messages",
-        )
+        ApplicationLogging.add_default_command_line_arguments(parser)
 
         subparsers = parser.add_subparsers(dest="primary_subparser")
 
         PluginManager.add_argparse_subparser(subparsers)
         ExtensionManager.add_argparse_subparser(subparsers)
 
         new_sub_parser = subparsers.add_parser(
             PyMarkdownLint.__normal_scan_subcommand,
             help="scan the Markdown files in the specified paths",
         )
-        subparsers.add_parser(
-            PyMarkdownLint.__stdin_scan_subcommand,
-            help="scan the standard input as a Markdown files",
+        ApplicationFileScanner.add_default_command_line_arguments(
+            new_sub_parser, ".md", "Markdown"
         )
 
-        new_sub_parser.add_argument(
-            "-l",
-            "--list-files",
-            dest="list_files",
-            action="store_true",
-            default=False,
-            help="list the markdown files found and exit",
-        )
-        new_sub_parser.add_argument(
-            "-r",
-            "--recurse",
-            dest="recurse_directories",
-            action="store_true",
-            default=False,
-            help="recursively scan directories",
-        )
-        new_sub_parser.add_argument(
-            "-ae",
-            "--alternate-extensions",
-            dest="alternate_extensions",
-            action="store",
-            default=".md",
-            type=PyMarkdownLint.alternate_extension_type,
-            help="provider an alternate set of file extensions to scan",
-        )
-        new_sub_parser.add_argument(
-            "paths",
-            metavar="path",
-            type=str,
-            nargs="+",
-            default=None,
-            help="one or more paths to scan for eligible Markdown files",
+        subparsers.add_parser(
+            PyMarkdownLint.__stdin_scan_subcommand,
+            help="scan the standard input as a Markdown file",
         )
 
         subparsers.add_parser("version", help="version of the application")
 
-        parse_arguments = parser.parse_args()
+        parse_arguments = parser.parse_args(args=direct_args)
 
         if not parse_arguments.primary_subparser:
             parser.print_help()
             sys.exit(2)
         elif parse_arguments.primary_subparser == "version":
             print(f"{self.__version_number}")
             sys.exit(0)
         return parse_arguments
 
-    @classmethod
-    def __is_file_eligible_to_scan(
-        cls, path_to_test: str, eligible_extensions: List[str]
-    ) -> bool:
-        """
-        Determine if the presented path is one that we want to scan.
-        """
-        return os.path.isfile(path_to_test) and any(
-            path_to_test.endswith(next_extension)
-            for next_extension in eligible_extensions
-        )
-
     def __scan_file(
         self, args: argparse.Namespace, next_file: str, next_file_name: str
     ) -> None:
         """
         Scan a given file and call the plugin manager for any significant events.
         """
 
         POGGER.info("Scanning file '$'.", next_file_name)
         context = self.__plugins.starting_new_file(next_file_name)
 
         try:
+            POGGER.info("Starting file '$'.", next_file_name)
+
             POGGER.info("Scanning file '$' token-by-token.", next_file_name)
             source_provider = (
                 None if args.x_test_scan_fault else FileSourceProvider(next_file)
             )
             assert self.__tokenizer
             actual_tokens = self.__tokenizer.transform_from_provider(source_provider)
 
@@ -307,153 +210,34 @@
                 line_number += 1
                 next_line = source_provider.get_next_line()
 
             POGGER.info("Completed scanning file '$'.", next_file_name)
             self.__plugins.completed_file(context, line_number)
 
             context.report_on_triggered_rules()
+            POGGER.info("Ending file '$'.", next_file_name)
         except Exception:
             context.report_on_triggered_rules()
+            POGGER.info("Ending file '$' with exception.", next_file_name)
             raise
 
-    def __process_next_path(
-        self,
-        next_path: str,
-        files_to_parse: Set[str],
-        recurse_directories: bool,
-        eligible_extensions: List[str],
-    ) -> bool:
-
-        did_find_any = False
-        POGGER.info("Determining files to scan for path '$'.", next_path)
-        if not os.path.exists(next_path):
-            print(
-                f"Provided path '{next_path}' does not exist.",
-                file=sys.stderr,
-            )
-            POGGER.debug("Provided path '$' does not exist.", next_path)
-        elif os.path.isdir(next_path):
-            self.__process_next_path_directory(
-                next_path, files_to_parse, recurse_directories, eligible_extensions
-            )
-            did_find_any = True
-        elif self.__is_file_eligible_to_scan(next_path, eligible_extensions):
-            POGGER.debug(
-                "Provided path '$' is a valid file. Adding.",
-                next_path,
-            )
-            normalized_path = (
-                next_path.replace(os.altsep, os.sep) if os.altsep else next_path
-            )
-            files_to_parse.add(normalized_path)
-            did_find_any = True
-        else:
-            POGGER.debug(
-                "Provided path '$' is not a valid file. Skipping.",
-                next_path,
-            )
-            print(
-                f"Provided file path '{next_path}' is not a valid file. Skipping.",
-                file=sys.stderr,
-            )
-        return did_find_any
-
-    def __process_next_path_directory(
-        self,
-        next_path: str,
-        files_to_parse: Set[str],
-        recurse_directories: bool,
-        eligible_extensions: List[str],
-    ) -> None:
-        POGGER.debug("Provided path '$' is a directory. Walking directory.", next_path)
-        normalized_next_path = (
-            next_path.replace(os.altsep, os.sep) if os.altsep else next_path
-        )
-        for root, _, files in os.walk(normalized_next_path):
-            normalized_root = root.replace(os.altsep, os.sep) if os.altsep else root
-            if not recurse_directories and normalized_root != normalized_next_path:
-                continue
-            normalized_root = (
-                normalized_root[:-1]
-                if normalized_root.endswith(os.sep)
-                else normalized_root
-            )
-            for file in files:
-                rooted_file_path = f"{normalized_root}{os.sep}{file}"
-                if self.__is_file_eligible_to_scan(
-                    rooted_file_path, eligible_extensions
-                ):
-                    files_to_parse.add(rooted_file_path)
-
-    def __determine_files_to_scan(
-        self,
-        eligible_paths: List[str],
-        recurse_directories: bool,
-        eligible_extensions: str,
-    ) -> Tuple[List[str], bool]:
-
-        split_eligible_extensions: List[str] = eligible_extensions.split(",")
-
-        did_error_scanning_files = False
-        files_to_parse: Set[str] = set()
-        for next_path in eligible_paths:
-            if "*" in next_path or "?" in next_path:
-                globbed_paths = glob.glob(next_path)
-                if not globbed_paths:
-                    print(
-                        f"Provided glob path '{next_path}' did not match any files.",
-                        file=sys.stderr,
-                    )
-                    did_error_scanning_files = True
-                    break
-                for next_globbed_path in globbed_paths:
-                    self.__process_next_path(
-                        next_globbed_path,
-                        files_to_parse,
-                        recurse_directories,
-                        split_eligible_extensions,
-                    )
-            elif not self.__process_next_path(
-                next_path,
-                files_to_parse,
-                recurse_directories,
-                split_eligible_extensions,
-            ):
-                did_error_scanning_files = True
-                break
-
-        sorted_files_to_parse = sorted(files_to_parse)
-        POGGER.info("Number of files found: $", len(sorted_files_to_parse))
-        return sorted_files_to_parse, did_error_scanning_files
-
-    @classmethod
-    def __handle_list_files(cls, files_to_scan: List[str]) -> int:
-
-        if files_to_scan:
-            print(ParserHelper.newline_character.join(files_to_scan))
-            return 0
-        print("No matching files found.", file=sys.stderr)
-        return 1
-
-    # pylint: disable=broad-except
+    # pylint: disable=broad-exception-caught
     def __apply_configuration_to_plugins(self) -> None:
-
         try:
             self.__plugins.apply_configuration(self.__properties)
         except Exception as this_exception:
             formatted_error = (
                 f"{type(this_exception).__name__} encountered while configuring plugins:\n"
                 + f"{this_exception}"
             )
             self.__handle_error(formatted_error, this_exception)
 
-    # pylint: enable=broad-except
+    # pylint: enable=broad-exception-caught
 
     def __initialize_parser(self, args: argparse.Namespace) -> None:
-
         resource_path = "fredo" if args.x_test_init_fault else None
         try:
             self.__tokenizer = TokenizedMarkdown(resource_path)
             self.__tokenizer.apply_configuration(self.__properties, self.__extensions)
         except BadTokenizationError as this_exception:
             formatted_error = (
                 f"{type(this_exception).__name__} encountered while initializing tokenizer:\n"
@@ -471,112 +255,70 @@
         try:
             self.__plugins.initialize(
                 plugin_dir,
                 args.add_plugin,
                 args.enable_rules,
                 args.disable_rules,
                 self.__properties,
-                self.__show_stack_trace,
+                self.__logging.show_stack_trace,
             )
         except BadPluginError as this_exception:
             formatted_error = (
                 f"BadPluginError encountered while loading plugins:\n{this_exception}"
             )
             self.__handle_error(formatted_error, this_exception)
 
     def __handle_error(self, formatted_error: str, thrown_error: Exception) -> None:
-
-        show_error = self.__show_stack_trace or not isinstance(thrown_error, ValueError)
+        show_error = self.__logging.show_stack_trace or not isinstance(
+            thrown_error, ValueError
+        )
         LOGGER.warning(formatted_error, exc_info=show_error)
 
-        print(f"\n\n{formatted_error}", file=sys.stderr)
-        if self.__show_stack_trace:
-            traceback.print_exc(file=sys.stderr)
+        stack_trace = (
+            "\n" + traceback.format_exc() if self.__logging.show_stack_trace else ""
+        )
+        self.__presentation.print_system_error(f"\n\n{formatted_error}{stack_trace}")
         sys.exit(1)
 
     def __handle_scan_error(self, next_file: str, this_exception: Exception) -> None:
-
-        formatted_error = f"{type(this_exception).__name__} encountered while scanning '{next_file}':\n{this_exception}"
-        self.__handle_error(formatted_error, this_exception)
+        if formatted_error := self.__presentation.format_scan_error(
+            next_file, this_exception
+        ):
+            self.__handle_error(formatted_error, this_exception)
+        sys.exit(1)
 
     def __set_initial_state(self, args: argparse.Namespace) -> None:
-
-        self.__show_stack_trace = args.show_stack_trace
-        base_logger = logging.getLogger()
-        base_logger.setLevel(
-            logging.DEBUG if self.__show_stack_trace else logging.WARNING
-        )
-
+        self.__logging.pre_initialize_with_args(args)
         if args.configuration_file:
             LOGGER.debug("Loading configuration file: %s", args.configuration_file)
             ApplicationPropertiesJsonLoader.load_and_set(
                 self.__properties, args.configuration_file, self.__handle_error
             )
         if args.set_configuration:
             self.__properties.set_manual_property(args.set_configuration)
 
-    def __initialize_strict_mode(self, args: argparse.Namespace) -> None:
         if args.strict_configuration or self.__properties.get_boolean_property(
             "mode.strict-config", strict_mode=True
         ):
             self.__properties.enable_strict_mode()
 
-    def __initialize_logging(
-        self, args: argparse.Namespace
-    ) -> Optional[logging.FileHandler]:
-
-        self.__show_stack_trace = args.show_stack_trace
-        if not self.__show_stack_trace:
-            self.__show_stack_trace = self.__properties.get_boolean_property(
-                "log.stack-trace"
-            )
-
-        effective_log_file = (
-            self.__properties.get_string_property("log.file")
-            if args.log_file is None
-            else args.log_file
-        )
-        new_handler = None
-        if effective_log_file:
-            new_handler = logging.FileHandler(effective_log_file)
-            logging.getLogger().addHandler(new_handler)
-        else:
-            temp_log_level = (
-                logging.DEBUG if self.__show_stack_trace else logging.CRITICAL
-            )
-            logging.basicConfig(stream=sys.stdout, level=temp_log_level)
-
-        effective_log_level = args.log_level or None
-        if effective_log_level is None:
-            effective_log_level = self.__properties.get_string_property(
-                "log.level", valid_value_fn=PyMarkdownLint.log_level_type
-            )
-        if effective_log_level is None:
-            effective_log_level = self.default_log_level
-
-        log_level_to_enact = PyMarkdownLint.available_log_maps[effective_log_level]
-
-        logging.getLogger().setLevel(log_level_to_enact)
-        ParserLogger.sync_on_next_call()
-        return new_handler
-
     def __initialize_plugins(self, args: argparse.Namespace) -> None:
         try:
             plugin_dir = os.path.dirname(os.path.realpath(__file__))
             plugin_dir = os.path.join(plugin_dir, "plugins")
             self.__initialize_plugin_manager(args, plugin_dir)
             self.__apply_configuration_to_plugins()
         except ValueError as this_exception:
             formatted_error = (
                 f"{type(this_exception).__name__} encountered while initializing plugins:\n"
                 + f"{this_exception}"
             )
             self.__handle_error(formatted_error, this_exception)
 
-    # pylint: disable=broad-except
+    # pylint: disable=broad-exception-caught
     def __initialize_extensions(self, args: argparse.Namespace) -> None:
         try:
             self.__extensions.initialize(
                 args,
                 self.__properties,
             )
             self.__extensions.apply_configuration()
@@ -590,32 +332,25 @@
         except Exception as this_exception:
             formatted_error = (
                 f"Error {type(this_exception).__name__} encountered while initializing extensions:\n"
                 + f"{this_exception}"
             )
             self.__handle_error(formatted_error, this_exception)
 
-    # pylint: enable=broad-except
+    # pylint: enable=broad-exception-caught
 
     def __handle_plugins_and_extensions(self, args: argparse.Namespace) -> None:
         self.__initialize_plugins(args)
         self.__initialize_extensions(args)
 
         if args.primary_subparser == PluginManager.argparse_subparser_name():
             sys.exit(self.__plugins.handle_argparse_subparser(args))
         if args.primary_subparser == ExtensionManager.argparse_subparser_name():
             sys.exit(self.__extensions.handle_argparse_subparser(args))
 
-    def __handle_main_list_files(
-        self, args: argparse.Namespace, files_to_scan: List[str]
-    ) -> None:
-        if args.list_files:
-            POGGER.info("Sending list of files that would have been scanned to stdout.")
-            sys.exit(self.__handle_list_files(files_to_scan))
-
     def __scan_specific_file(
         self, args: argparse.Namespace, next_file: str, next_file_name: str
     ) -> None:
         try:
             self.__scan_file(args, next_file, next_file_name)
         except BadPluginError as this_exception:
             self.__handle_scan_error(next_file, this_exception)
@@ -623,14 +358,16 @@
             self.__handle_scan_error(next_file, this_exception)
 
     def __process_files_to_scan(
         self, args: argparse.Namespace, use_standard_in: bool, files_to_scan: List[str]
     ) -> None:
         # sourcery skip: raise-specific-error
         if use_standard_in:
+            POGGER.debug("Scanning from: (stdin)")
+
             temporary_file = None
             scan_exception = None
             try:
                 if args.x_test_stdin_fault:
                     raise IOError("made up")
 
                 with tempfile.NamedTemporaryFile("wt", delete=False) as outfile:
@@ -651,58 +388,71 @@
                 try:
                     raise IOError(
                         f"Temporary file to capture stdin was not written ({scan_exception})."
                     ) from scan_exception
                 except IOError as this_exception:
                     self.__handle_scan_error("stdin", this_exception)
         else:
-            self.__handle_main_list_files(args, files_to_scan)
+            POGGER.debug("Scanning from: $", files_to_scan)
             for next_file in files_to_scan:
                 self.__scan_specific_file(args, next_file, next_file)
 
-    def main(self) -> None:
+    def __initialize_subsystems(
+        self, direct_args: Optional[List[str]]
+    ) -> argparse.Namespace:
+        args = self.__parse_arguments(direct_args=direct_args)
+        self.__set_initial_state(args)
+
+        self.__logging.initialize(args)
+        ParserLogger.sync_on_next_call()
+
+        if direct_args is None:
+            LOGGER.debug("Using supplied command line arguments.")
+        else:
+            LOGGER.debug("Using direct arguments: %s", str(direct_args))
+
+        self.__handle_plugins_and_extensions(args)
+        return args
+
+    def main(self, direct_args: Optional[List[str]] = None) -> None:
         """
         Main entrance point.
         """
-        args = self.__parse_arguments()
-        self.__set_initial_state(args)
-
-        new_handler, total_error_count = None, 0
+        total_error_count = 0
         try:
-            self.__initialize_strict_mode(args)
-            new_handler = self.__initialize_logging(args)
+            args = self.__initialize_subsystems(direct_args)
 
-            self.__handle_plugins_and_extensions(args)
+            files_to_scan: List[str] = []
+            did_error_scanning_files = False
 
             use_standard_in = (
                 args.primary_subparser == PyMarkdownLint.__stdin_scan_subcommand
             )
-            files_to_scan: List[str] = []
-            did_error_scanning_files = False
-
             if not use_standard_in:
                 POGGER.info("Determining files to scan.")
                 (
                     files_to_scan,
                     did_error_scanning_files,
-                ) = self.__determine_files_to_scan(
-                    args.paths, args.recurse_directories, args.alternate_extensions
-                )
+                ) = ApplicationFileScanner.determine_files_to_scan_with_args(args)
             if did_error_scanning_files:
                 total_error_count = 1
             else:
+                POGGER.info("Initializing parser.")
                 self.__initialize_parser(args)
 
+                POGGER.info("Processing files with parser.")
                 self.__process_files_to_scan(args, use_standard_in, files_to_scan)
+                POGGER.info("Files have been processed.")
         except ValueError as this_exception:
             formatted_error = f"Configuration Error: {this_exception}"
             self.__handle_error(formatted_error, this_exception)
         finally:
-            if new_handler:
-                new_handler.close()
+            self.__logging.terminate()
 
         if self.__plugins.number_of_scan_failures or total_error_count:
             sys.exit(1)
 
 
+# pylint: enable=too-few-public-methods
+
 if __name__ == "__main__":
     PyMarkdownLint().main()
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/markdown_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/markdown_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -668,14 +668,21 @@
     @property
     def extra_end_data(self) -> Optional[str]:
         """
         Returns any extra data specifically tied to the end element.
         """
         return self.__extra_end_data
 
+    def set_extra_end_data(self, new_end_data: Optional[str]) -> None:
+        """
+        Sets the extra data specifically tied to the end element. Use sparingly.
+        """
+        self.__extra_end_data = new_end_data
+        self.__compose_data_field()
+
     @property
     def start_markdown_token(self) -> MarkdownToken:
         """
         Returns the start markdown token that this end token is the end for.
         """
         return self.__start_markdown_token
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/parse_block_pass_properties.py` & `pymarkdownlnt-0.9.9/pymarkdown/parse_block_pass_properties.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/parser_helper.py` & `pymarkdownlnt-0.9.9/pymarkdown/parser_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Module to provide helper functions for parsing.
 """
 
+import logging
 from typing import Any, List, Optional, Tuple
 
 from pymarkdown.constants import Constants
 
+LOGGER = logging.getLogger(__name__)
+
 
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-public-methods
 class ParserHelper:
     """
     Class to provide helper functions for parsing.
     """
@@ -379,90 +382,14 @@
             index < source_string_size and source_string[index] not in match_characters
         ):
             index += 1
 
         return index, source_string[start_index:index]
 
     @staticmethod
-    def calculate_length(source_string: str, start_index: int = 0) -> int:
-        """
-        Calculate an adjusted length for the string.
-        """
-
-        string_length = start_index
-        for source_character in source_string:
-            string_length = (
-                (int((string_length + 4) / 4) * 4)
-                if source_character == ParserHelper.tab_character
-                else (string_length + 1)
-            )
-        return string_length - start_index
-
-    @staticmethod
-    def detabify_string(source_string: str, additional_start_delta: int = 0) -> str:
-        """
-        Given a string that may have one or more tabstops in it, resolve the
-        tabstops into more easily handled space characters.
-        """
-        if ParserHelper.tab_character not in source_string:
-            return source_string
-
-        rebuilt_string = ""
-        current_start_index = 0
-        next_tab_index = source_string.find(ParserHelper.tab_character)
-        while next_tab_index != -1:
-            _, start_index = ParserHelper.collect_backwards_while_spaces(
-                source_string, next_tab_index
-            )
-            assert start_index is not None
-            end_index, _ = ParserHelper.collect_while_spaces(
-                source_string, next_tab_index
-            )
-            whitespace_section = source_string[start_index:end_index]
-            if start_index:
-                rebuilt_string += source_string[:start_index]
-            realized_start_index = (
-                current_start_index + start_index + additional_start_delta
-            )
-            whitespace_actual_length = ParserHelper.calculate_length(
-                whitespace_section, realized_start_index
-            )
-            rebuilt_string += ParserHelper.repeat_string(
-                ParserHelper.space_character, whitespace_actual_length
-            )
-            current_start_index += start_index + whitespace_actual_length
-
-            source_string = source_string[end_index:]
-            next_tab_index = source_string.find(ParserHelper.tab_character)
-        if source_string:
-            rebuilt_string += source_string
-        return rebuilt_string
-
-    @staticmethod
-    def is_length_less_than_or_equal_to(source_string: str, length_limit: int) -> bool:
-        """
-        Determine if the adjusted length of the string is less than or equal to the
-        specified limit.
-        """
-        return ParserHelper.calculate_length(source_string) <= length_limit
-
-    @staticmethod
-    def is_length_greater_than_or_equal_to(
-        source_string: str, length_limit: int, start_index: int = 0
-    ) -> bool:
-        """
-        Determine if the adjusted length of the string is greater than or equal to the
-        specified limit.
-        """
-        return (
-            ParserHelper.calculate_length(source_string, start_index=start_index)
-            >= length_limit
-        )
-
-    @staticmethod
     def index_any_of(source_text: str, find_any: str, start_index: int = 0) -> int:
         """
         Determine if any of the specified characters are in the source string.
         """
 
         first_index = -1
         for next_character in find_any:
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/parser_logger.py` & `pymarkdownlnt-0.9.9/pymarkdown/parser_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 """
 import logging
 from typing import Any, List, cast
 
 from pymarkdown.parser_helper import ParserHelper
 
 
+class ParserLoggerException(Exception):
+    """
+    Custom exception for the ParserLogger class.
+    """
+
+    def __init__(self, message: str) -> None:
+        self.message = message
+        super().__init__(self.message)
+
+
 class ParserLogger:
     """
     Class to provide for a simple logger wrapper that provides extra
     functionality for logging parsing information.
 
     To keep things performant, the calls to the underlying logging libraries
     are only done when needed.
@@ -88,15 +98,15 @@
 
     @classmethod
     def __munge(cls, show_whitespace: bool, log_format: str, args: List[Any]) -> str:
         split_log_format = log_format.split("$")
         split_log_format_length = len(split_log_format)
         args_length = len(args)
         if split_log_format_length != args_length + 1:
-            raise Exception(
+            raise ParserLoggerException(
                 "The number of $ substitution characters does not equal the number of arguments in the list."
             )
 
         recipient_array: List[str] = [""] * (split_log_format_length + args_length)
         for next_array_index, _ in enumerate(recipient_array):
             if next_array_index % 2 == 0:
                 recipient_array[next_array_index] = split_log_format[
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/parser_state.py` & `pymarkdownlnt-0.9.9/pymarkdown/parser_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def __call__(
         self,
         parser_state: ParserState,
         input_line: str,
         from_main_transform: bool,
         position_marker: Optional[PositionMarker] = None,
-    ) -> Tuple[List[MarkdownToken], Optional[RequeueLineInfo]]:
+    ) -> Tuple[Optional[List[MarkdownToken]], Optional[RequeueLineInfo]]:
         ...  # pragma: no cover
 
 
 # pylint: enable=too-few-public-methods
 
 
 # pylint: disable=too-many-instance-attributes
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/bad_plugin_error.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/bad_plugin_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         formatted_message: Optional[str] = None,
         line_number: int = 0,
         column_number: int = 0,
         actual_line: Optional[str] = None,
         actual_token: Optional[MarkdownToken] = None,
         cause: Optional[Exception] = None,
     ) -> None:
-
         if not formatted_message:
             if file_name:
                 formatted_message = BadPluginError.__create_file_name_message(
                     file_name, class_name, is_constructor
                 )
             elif class_name:
                 formatted_message = BadPluginError.__create_class_name_message(
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/found_plugin.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/found_plugin.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_details.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_details.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_manager.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import sys
 from typing import Any, Dict, List, Optional, Pattern, Set, Tuple
 
 from application_properties import ApplicationProperties, ApplicationPropertiesFacade
 from columnar import columnar
 
 from pymarkdown.extensions.pragma_token import PragmaExtension
+from pymarkdown.main_presentation import MainPresentation
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.plugin_manager.bad_plugin_error import BadPluginError
 from pymarkdown.plugin_manager.found_plugin import FoundPlugin
 from pymarkdown.plugin_manager.plugin_scan_context import PluginScanContext
 from pymarkdown.plugin_manager.plugin_scan_failure import PluginScanFailure
 from pymarkdown.plugin_manager.rule_plugin import RulePlugin
@@ -31,27 +32,32 @@
     """
     Manager object to take care of load and accessing plugin modules.
     """
 
     __plugin_prefix = "plugins"
     __root_subparser_name = "pm_subcommand"
     __argparse_subparser: Optional[argparse.ArgumentParser] = None
-    __id_regex = re.compile("^[a-z]{2,3}[0-9]{3,3}$")
+    __id_regex = re.compile("^[a-z]{2,3}\\d{3}$")
     __name_regex = re.compile("^[a-zA-Z0-9][a-zA-Z0-9-]*[a-zA-Z0-9]$")
     __filter_regex = re.compile("^[a-zA-Z0-9-]+$")
     __version_regex = re.compile("^(0|[1-9]\\d*)\\.(0|[1-9]\\d*)\\.(0|[1-9]\\d*)$")
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        presentation: MainPresentation,
+    ) -> None:
         (
             self.number_of_scan_failures,
             self.number_of_pragma_failures,
             self.__show_stack_trace,
         ) = (0, 0, False)
         self.__loaded_classes: List[Tuple[RulePlugin, str]] = []
 
+        self.__presentation = presentation
+
         self.__document_pragmas: Dict[int, Set[str]] = {}
 
         self.__registered_plugins: List[FoundPlugin] = []
         self.__enabled_plugins: List[FoundPlugin] = []
         self.__enabled_plugins_for_starting_new_file: List[FoundPlugin] = []
         self.__enabled_plugins_for_next_token: List[FoundPlugin] = []
         self.__enabled_plugins_for_next_line: List[FoundPlugin] = []
@@ -190,15 +196,15 @@
             if next_plugin.plugin_id == next_plugin_id:
                 next_plugin_list.append(next_plugin)
         assert len(next_plugin_list) == 1
         next_plugin = next_plugin_list[0]
         if next_plugin.plugin_version != "0.0.0" or args.show_all:
             self.__show_row_if_matches(list_re, next_plugin_id, next_plugin, show_rows)
 
-    def __handle_argparse_subparser_list(self, args: argparse.Namespace) -> None:
+    def __handle_argparse_subparser_list(self, args: argparse.Namespace) -> int:
         list_re = None
         if args.list_filter:
             list_re = re.compile(
                 "^" + args.list_filter.replace("*", ".*").replace("?", ".") + "$"
             )
 
         show_rows: List[List[str]] = []
@@ -211,18 +217,19 @@
                 "id",
                 "names",
                 "enabled\n(default)",
                 "enabled\n(current)",
                 "version",
             ]
             self.__print_columnar_data(headers, show_rows)
-        else:
-            print(
-                f"No plugin rule identifiers matches the pattern '{args.list_filter}'."
-            )
+            return 0
+        self.__presentation.print_system_error(
+            f"No plugin rule identifiers matches the pattern '{args.list_filter}'."
+        )
+        return 1
 
     def __show_row_if_matches(
         self,
         list_re: Optional[Pattern[str]],
         next_plugin_id: str,
         next_plugin: FoundPlugin,
         show_rows: List[List[str]],
@@ -242,32 +249,33 @@
                 ", ".join(next_plugin.plugin_names),
                 str(next_plugin.plugin_enabled_by_default),
                 str(is_enabled_now),
                 next_plugin.plugin_version,
             ]
             show_rows.append(display_row)
 
-    @classmethod
     def __print_columnar_data(
-        cls, headers: List[str], show_rows: List[List[str]]
+        self, headers: List[str], show_rows: List[List[str]]
     ) -> None:
         table = columnar(show_rows, headers, no_borders=True)
         split_rows = table.split(ParserHelper.newline_character)
         new_rows = [next_row.rstrip() for next_row in split_rows]
-        print(ParserHelper.newline_character.join(new_rows))
+        self.__presentation.print_system_output(
+            ParserHelper.newline_character.join(new_rows)
+        )
 
     def __handle_argparse_subparser_info(self, args: argparse.Namespace) -> int:
         matching_plugins: List[FoundPlugin] = list(
             filter(
                 lambda x: args.info_filter in x.plugin_identifiers,
                 self.__registered_plugins,
             )
         )
         if not matching_plugins:
-            print(
+            self.__presentation.print_system_error(
                 f"Unable to find a plugin with an id or name of '{args.info_filter}'."
             )
             return 1
 
         found_plugin = matching_plugins[0]
         show_rows = [
             ["Id", found_plugin.plugin_id],
@@ -289,15 +297,15 @@
         """
         Handle the parsing for this subparser.
         """
         return_code, subparser_value = 0, getattr(
             args, PluginManager.__root_subparser_name
         )
         if subparser_value == "list":
-            self.__handle_argparse_subparser_list(args)
+            return_code = self.__handle_argparse_subparser_list(args)
         elif subparser_value == "info":
             return_code = self.__handle_argparse_subparser_info(args)
         else:
             assert PluginManager.__argparse_subparser
             PluginManager.__argparse_subparser.print_help()
             sys.exit(2)
         return return_code
@@ -317,30 +325,35 @@
                 return
 
         extra_info = (
             f" [{scan_failure.extra_error_information}]"
             if scan_failure.extra_error_information
             else ""
         )
-
         rule_id = scan_failure.rule_id.upper()
-        print(
-            f"{scan_failure.scan_file}:{scan_failure.line_number}:{scan_failure.column_number}: "
-            + f"{rule_id}: {scan_failure.rule_description}{extra_info} ({scan_failure.rule_name})"
+
+        adjusted_failure = PluginScanFailure(
+            scan_failure.scan_file,
+            scan_failure.line_number,
+            scan_failure.column_number,
+            rule_id,
+            scan_failure.rule_name,
+            scan_failure.rule_description,
+            extra_info,
         )
+        self.__presentation.print_scan_failure(adjusted_failure)
         self.number_of_scan_failures += 1
 
     def log_pragma_failure(
         self, scan_file: str, line_number: int, pragma_error: str
     ) -> None:
         """
         Log the pragma failure in the appropriate format.
         """
-
-        print(f"{scan_file}:{line_number}:1: INLINE: {pragma_error}")
+        self.__presentation.print_pragma_failure(scan_file, line_number, pragma_error)
         self.number_of_pragma_failures += 1
 
     def compile_pragmas(self, scan_file: str, pragma_lines: Dict[int, str]) -> None:
         """
         Go through the list of extracted pragmas and compile them.
         """
 
@@ -366,15 +379,14 @@
             x
             for x in os.listdir(directory_to_search)
             if x.endswith(".py") and x[:-3] != "__init__"
         ]
 
     @classmethod
     def __snake_to_camel(cls, word: str) -> str:
-
         return "".join(x.capitalize() or "_" for x in word.split("_"))
 
     def __attempt_to_load_plugin(
         self, next_plugin_module: str, plugin_class_name: str, next_plugin_file: str
     ) -> None:
         """
         Attempt to cleanly load the specified plugin.
@@ -528,47 +540,32 @@
         """
 
         if not isinstance(field_value, int):
             raise BadPluginError(
                 class_name=type(plugin_instance).__name__, field_name=field_name
             )
 
-    # pylint: disable=too-many-locals
     def __get_plugin_details(
         self, plugin_instance: RulePlugin, instance_file_name: str
     ) -> FoundPlugin:
         """
         Query the plugin for details and verify that they are reasonable.
         """
 
-        try:
-            instance_details = plugin_instance.get_details()
-            (
-                plugin_id,
-                plugin_name,
-                plugin_description,
-                plugin_enabled_by_default,
-                plugin_version,
-                plugin_interface_version,
-                plugin_url,
-                plugin_configuration,
-            ) = (
-                instance_details.plugin_id,
-                instance_details.plugin_name,
-                instance_details.plugin_description,
-                instance_details.plugin_enabled_by_default,
-                instance_details.plugin_version,
-                instance_details.plugin_interface_version,
-                instance_details.plugin_url,
-                instance_details.plugin_configuration,
-            )
-        except Exception as this_exception:
-            raise BadPluginError(
-                class_name=type(plugin_instance).__name__,
-            ) from this_exception
+        (
+            plugin_id,
+            plugin_name,
+            plugin_description,
+            plugin_enabled_by_default,
+            plugin_version,
+            plugin_interface_version,
+            plugin_url,
+            plugin_configuration,
+            plugin_names,
+        ) = self.__unpack_plugin_details(plugin_instance)
 
         self.__verify_string_field(plugin_instance, "plugin_id", plugin_id)
         self.__verify_string_field(plugin_instance, "plugin_name", plugin_name)
         self.__verify_string_field(
             plugin_instance, "plugin_description", plugin_description
         )
         self.__verify_boolean_field(
@@ -581,46 +578,83 @@
         if plugin_url:
             self.__verify_string_field(plugin_instance, "plugin_url", plugin_url)
         if plugin_configuration:
             self.__verify_string_field(
                 plugin_instance, "plugin_configuration", plugin_configuration
             )
 
-        plugin_id = plugin_id.strip().lower()
-
-        plugin_names = []
-        for next_name in plugin_name.lower().split(","):
-            if next_name := next_name.strip():
-                plugin_names.append(next_name)
-
-        plugin_identifiers = [plugin_id, *plugin_names]
-
         plugin_object = FoundPlugin(
             plugin_id,
             plugin_names,
             plugin_description,
             plugin_instance,
             plugin_enabled_by_default,
             plugin_version,
             plugin_interface_version,
             instance_file_name,
             plugin_url,
             plugin_configuration,
-            plugin_identifiers,
+            [plugin_id, *plugin_names],
         )
 
         if plugin_object.plugin_interface_version != 1:
             raise BadPluginError(
                 formatted_message=f"Plugin '{instance_file_name}' with an interface version "
                 + f"('{plugin_object.plugin_interface_version}') that is not '1'."
             )
 
         return plugin_object
 
-    # pylint: enable=too-many-locals
+    def __unpack_plugin_details(
+        self, plugin_instance: RulePlugin
+    ) -> Tuple[str, str, str, bool, str, int, Optional[str], Optional[str], List[str]]:
+        try:
+            instance_details = plugin_instance.get_details()
+            (
+                plugin_id,
+                plugin_name,
+                plugin_description,
+                plugin_enabled_by_default,
+                plugin_version,
+                plugin_interface_version,
+                plugin_url,
+                plugin_configuration,
+            ) = (
+                instance_details.plugin_id,
+                instance_details.plugin_name,
+                instance_details.plugin_description,
+                instance_details.plugin_enabled_by_default,
+                instance_details.plugin_version,
+                instance_details.plugin_interface_version,
+                instance_details.plugin_url,
+                instance_details.plugin_configuration,
+            )
+        except Exception as this_exception:
+            raise BadPluginError(
+                class_name=type(plugin_instance).__name__,
+            ) from this_exception
+
+        plugin_id = plugin_id.strip().lower()
+
+        plugin_names = []
+        for next_name in plugin_name.lower().split(","):
+            if next_name := next_name.strip():
+                plugin_names.append(next_name)
+
+        return (
+            plugin_id,
+            plugin_name,
+            plugin_description,
+            plugin_enabled_by_default,
+            plugin_version,
+            plugin_interface_version,
+            plugin_url,
+            plugin_configuration,
+            plugin_names,
+        )
 
     def __register_plugin_id(
         self, plugin_object: FoundPlugin, instance_file_name: str, next_key: str
     ) -> None:
         if not PluginManager.__id_regex.match(next_key):
             raise ValueError(
                 f"Unable to register plugin '{instance_file_name}' with id '{next_key}' as "
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_scan_context.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_scan_context.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/plugin_scan_failure.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/plugin_scan_failure.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugin_manager/rule_plugin.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugin_manager/rule_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,31 +143,33 @@
             self.get_details().plugin_name,
             self.get_details().plugin_description,
             extra_error_information,
         )
 
     # pylint: enable=too-many-arguments
 
-    def initialize_from_config(self) -> None:
+    def initialize_from_config(self) -> None:  # noqa: B027
         """
         Event to allow the plugin to load configuration information.
         """
 
-    def starting_new_file(self) -> None:
+    def starting_new_file(self) -> None:  # noqa: B027
         """
         Event that the a new file to be scanned is starting.
         """
 
-    def completed_file(self, context: PluginScanContext) -> None:
+    def completed_file(self, context: PluginScanContext) -> None:  # noqa: B027
         """
         Event that the file being currently scanned is now completed.
         """
 
-    def next_line(self, context: PluginScanContext, line: str) -> None:
+    def next_line(self, context: PluginScanContext, line: str) -> None:  # noqa: B027
         """
         Event that a new line is being processed.
         """
 
-    def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
+    def next_token(  # noqa: B027
+        self, context: PluginScanContext, token: MarkdownToken
+    ) -> None:
         """
         Event that a new token is being processed.
         """
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/plugin_one.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/plugin_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 """
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.plugin_manager.plugin_details import PluginDetails
 from pymarkdown.plugin_manager.plugin_scan_context import PluginScanContext
 from pymarkdown.plugin_manager.rule_plugin import RulePlugin
 
 
+class PluginTestException(Exception):
+    """
+    Custom exception for the PluginOne class.
+    """
+
+    def __init__(self, message: str) -> None:
+        self.message = message
+        super().__init__(self.message)
+
+
 class PluginOne(RulePlugin):
     """
     Class to implement a sample plugin that just reports that it has been called.
     """
 
     __valid_values = [0, 1, 2]
 
@@ -51,15 +61,15 @@
             default_value=1,
             valid_value_fn=self.__validate_configuration_other_test_value,
         )
         print(
             f"{self.get_details().plugin_id}>>other_test_value>>{self.other_test_value}"
         )
         if self.test_value == 10:
-            raise Exception("because")
+            raise PluginTestException("because")
 
     def starting_new_file(self) -> None:
         """
         Event that the a new file to be scanned is starting.
         """
         print(f"{self.get_details().plugin_id}>>starting_new_file>>")
 
@@ -73,15 +83,15 @@
     def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
         """
         Event that a new token is being processed.
         """
         _ = context
         print(f"{self.get_details().plugin_id}>>token:{token}")
         if self.test_value == 20:
-            raise Exception("because")
+            raise PluginTestException("because")
 
     def completed_file(self, context: PluginScanContext) -> None:
         """
         Event that the file being currently scanned is now completed.
         """
         _ = context
         print(f"{self.get_details().plugin_id}>>completed_file")
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_001.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_001.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_002.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_002.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_003.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_003.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,34 +85,32 @@
         self.__actual_style_type = ""
         if self.__style_type != RuleMd003.__consistent_style:
             self.__actual_style_type = self.__style_type
 
     def __handle_simple_styles(
         self, heading_style_type: str, is_heading_level_1_or_2: bool
     ) -> Tuple[bool, str]:
-        is_heading_bad = bool(heading_style_type != self.__actual_style_type)
+        is_heading_bad = heading_style_type != self.__actual_style_type
 
         if (
             is_heading_bad
             and self.__allow_consistent_setext_update
             and self.__actual_style_type == RuleMd003.__setext_style
             and heading_style_type == RuleMd003.__atx_style
             and not is_heading_level_1_or_2
         ):
-
             is_heading_bad = False
             self.__actual_style_type = RuleMd003.__setext_with_atx_style
 
         expected_style_type = self.__actual_style_type
         return is_heading_bad, expected_style_type
 
     def __handle_complex_styles(
         self, heading_style_type: str, is_heading_level_1_or_2: bool
     ) -> Tuple[bool, str]:
-
         is_heading_bad, expected_style_type = False, ""
         if self.__actual_style_type == RuleMd003.__setext_with_atx_style:
             base_atx_style = RuleMd003.__atx_style
         else:
             assert self.__actual_style_type == RuleMd003.__setext_with_atx_closed_style
             base_atx_style = RuleMd003.__atx_closed_style
         if not (
@@ -172,12 +170,12 @@
         if token.is_atx_heading:
             atx_token = cast(AtxHeadingMarkdownToken, token)
             heading_style_type = (
                 RuleMd003.__atx_closed_style
                 if atx_token.remove_trailing_count
                 else RuleMd003.__atx_style
             )
-            is_heading_level_1_or_2 = bool(atx_token.hash_count < 3)
+            is_heading_level_1_or_2 = atx_token.hash_count < 3
         elif token.is_setext_heading:
             heading_style_type = RuleMd003.__setext_style
             is_heading_level_1_or_2 = True
         return heading_style_type, is_heading_level_1_or_2
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_004.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_004.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_005.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_005.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
             # if self.__debug:
             #     print("ri2")
             self.__report_issue(
                 context, token, self.__ordered_list_starts[list_level].column_number - 1
             )
 
     def __compute_ordered_list_alignment(self) -> None:
-
         list_level = len(self.__list_stack)
 
         last_length = 0
         last_token: Optional[NewListItemMarkdownToken] = None
 
         for next_token in self.__ordered_tokens[list_level]:
             list_token = cast(NewListItemMarkdownToken, next_token)
@@ -163,16 +162,15 @@
             self.__report_issue(
                 context, token, self.__unordered_list_indents[list_level] - 2
             )
 
     def __handle_ordered_list_start(self, token: OrderedListStartMarkdownToken) -> None:
         self.__list_stack.append(token)
         list_level = len(self.__list_stack)
-        self.__ordered_tokens[list_level] = []
-        self.__ordered_tokens[list_level].append(token)
+        self.__ordered_tokens[list_level] = [token]
         if list_level not in self.__ordered_list_starts:
             self.__ordered_list_starts[list_level] = token
             self.__ordered_list_alignment[list_level] = OrderedListAlignment.UNKNOWN
 
     def __handle_list_item(
         self, context: PluginScanContext, token: NewListItemMarkdownToken
     ) -> None:
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_006.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_006.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     def __calculate_expected_indent(self) -> int:
         expected_indent = 0
         if len(self.__token_stack) > 1:
             if self.__token_stack[-2].is_block_quote_start:
                 block_quote_token = cast(
                     BlockQuoteMarkdownToken, self.__token_stack[-2]
                 )
-                assert block_quote_token.leading_spaces is not None
-                split_spaces = block_quote_token.leading_spaces.split(
+                assert block_quote_token.bleading_spaces is not None
+                split_spaces = block_quote_token.bleading_spaces.split(
                     ParserHelper.newline_character
                 )
                 expected_indent = len(split_spaces[0]) + (
                     block_quote_token.column_number - 1
                 )
             else:
                 list_token = cast(ListStartMarkdownToken, self.__token_stack[-2])
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_007.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_007.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,14 +99,25 @@
         return bool(
             token.is_indented_code_block_end
             or token.is_html_block_end
             or token.is_setext_heading_end
             or token.is_fenced_code_block_end
         )
 
+    def __manage_leaf_tokens_text(self, token: MarkdownToken) -> int:
+        assert self.__last_leaf_token is not None
+        text_token = cast(TextMarkdownToken, token)
+        if self.__last_leaf_token.is_setext_heading:
+            assert text_token.end_whitespace is not None
+            return text_token.end_whitespace.count(ParserHelper.newline_character) + 1
+        assert (
+            self.__last_leaf_token.is_html_block or self.__last_leaf_token.is_code_block
+        )
+        return text_token.token_text.count(ParserHelper.newline_character) + 1
+
     def __manage_leaf_tokens(self, token: MarkdownToken) -> None:
         bq_delta = 0
         if self.__is_simple_delta(token):
             bq_delta = 1
         elif self.__is_remember_leaf_token(token):
             self.__last_leaf_token = token
         elif self.__is_clear_leaf_token(token):
@@ -120,28 +131,15 @@
             paragraph_token = cast(ParagraphMarkdownToken, token)
             bq_delta = paragraph_token.extracted_whitespace.count(
                 ParserHelper.newline_character
             )
         elif token.is_link_reference_definition:
             bq_delta = self.__manage_lrd_token(token)
         elif token.is_text and self.__last_leaf_token:
-            text_token = cast(TextMarkdownToken, token)
-            if self.__last_leaf_token.is_setext_heading:
-                assert text_token.end_whitespace is not None
-                bq_delta = (
-                    text_token.end_whitespace.count(ParserHelper.newline_character) + 1
-                )
-            else:
-                assert (
-                    self.__last_leaf_token.is_html_block
-                    or self.__last_leaf_token.is_code_block
-                )
-                bq_delta = (
-                    text_token.token_text.count(ParserHelper.newline_character) + 1
-                )
+            bq_delta = self.__manage_leaf_tokens_text(token)
         self.__bq_line_index[len(self.__container_token_stack)] += bq_delta
 
     @classmethod
     def __manage_lrd_token(cls, token: MarkdownToken) -> int:
         lrd_token = cast(LinkReferenceDefinitionMarkdownToken, token)
         assert lrd_token.link_title_raw is not None
         assert lrd_token.link_title_whitespace is not None
@@ -186,14 +184,48 @@
             token.is_new_list_item
             and self.__container_token_stack[-1].is_unordered_list_start
         ):
             self.__check(context, token)
 
         self.manage_container_tokens(token)
 
+    def __calculate_base_column_ordered_list(
+        self, stack_index: int, ignore_list_starts: bool, container_base_column: int
+    ) -> Tuple[bool, int]:
+        if not ignore_list_starts:
+            list_token = cast(
+                ListStartMarkdownToken,
+                self.__container_token_stack[stack_index],
+            )
+            container_base_column += list_token.indent_level
+        ignore_list_starts = True
+        return ignore_list_starts, container_base_column
+
+    def __calculate_base_column_block_quote(
+        self, stack_index: int, container_base_column: int, block_quote_base: int
+    ) -> Tuple[bool, int, int]:
+        block_quote_token = cast(
+            BlockQuoteMarkdownToken,
+            self.__container_token_stack[stack_index],
+        )
+        bq_index = self.__bq_line_index[stack_index + 1]
+        assert block_quote_token.bleading_spaces is not None
+        split_leading_spaces = block_quote_token.bleading_spaces.split(
+            ParserHelper.newline_character
+        )
+        # print(f"bq_index={bq_index},split_leading_spaces={split_leading_spaces}")
+        # print(f"split_leading_spaces[bq_index]={split_leading_spaces[bq_index]}=")
+        if not block_quote_base:
+            block_quote_base = container_base_column + len(
+                split_leading_spaces[bq_index]
+            )
+        container_base_column += len(split_leading_spaces[bq_index])
+        ignore_list_starts = False
+        return ignore_list_starts, container_base_column, block_quote_base
+
     def __calculate_base_column(self) -> Tuple[int, int, int]:
         container_base_column = 0
         block_quote_base = 0
         list_depth = 0
         if self.__container_token_stack:
             stack_index = len(self.__container_token_stack) - 1
             while (
@@ -204,39 +236,28 @@
                 stack_index -= 1
             # print(f"stack_index={stack_index}")
             ignore_list_starts = False
             while stack_index >= 0:
                 # print(f"stack_index>{stack_index}," + \
                 #   f"token={self.__container_token_stack[stack_index]}".replace(ParserHelper.newline_character, "\\n"))
                 if self.__container_token_stack[stack_index].is_ordered_list_start:
-                    if not ignore_list_starts:
-                        list_token = cast(
-                            ListStartMarkdownToken,
-                            self.__container_token_stack[stack_index],
-                        )
-                        container_base_column += list_token.indent_level
-                    ignore_list_starts = True
-                elif self.__container_token_stack[stack_index].is_block_quote_start:
-                    block_quote_token = cast(
-                        BlockQuoteMarkdownToken,
-                        self.__container_token_stack[stack_index],
+                    (
+                        ignore_list_starts,
+                        container_base_column,
+                    ) = self.__calculate_base_column_ordered_list(
+                        stack_index, ignore_list_starts, container_base_column
                     )
-                    bq_index = self.__bq_line_index[stack_index + 1]
-                    assert block_quote_token.leading_spaces is not None
-                    split_leading_spaces = block_quote_token.leading_spaces.split(
-                        ParserHelper.newline_character
+                elif self.__container_token_stack[stack_index].is_block_quote_start:
+                    (
+                        ignore_list_starts,
+                        container_base_column,
+                        block_quote_base,
+                    ) = self.__calculate_base_column_block_quote(
+                        stack_index, container_base_column, block_quote_base
                     )
-                    # print(f"bq_index={bq_index},split_leading_spaces={split_leading_spaces}")
-                    # print(f"split_leading_spaces[bq_index]={split_leading_spaces[bq_index]}=")
-                    if not block_quote_base:
-                        block_quote_base = container_base_column + len(
-                            split_leading_spaces[bq_index]
-                        )
-                    container_base_column += len(split_leading_spaces[bq_index])
-                    ignore_list_starts = False
                 # print(f"container_base_column>{container_base_column}")
                 stack_index -= 1
         return container_base_column, block_quote_base, list_depth
 
     def __check(self, context: PluginScanContext, token: MarkdownToken) -> None:
         # print(f"{token}".replace(ParserHelper.newline_character, "\\n"))
         # print(f"{self.__container_token_stack}".replace(ParserHelper.newline_character, "\\n"))
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_009.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_009.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,38 +121,41 @@
             self.__inline_token_index += 1
 
         if (
             not self.__leaf_tokens[self.__leaf_token_index].is_code_block
             and line
             and line[-1] == " "
         ):
+            self.__next_line_check_for_error(line, context)
+        self.__line_index += 1
 
-            (
-                first_non_whitespace_index,
-                extracted_whitespace,
-            ) = ParserHelper.extract_spaces_from_end(line)
-            extracted_whitespace_length = len(extracted_whitespace)
-
-            is_list_empty_line = False
-            leaf_token = self.__leaf_owner_tokens[self.__leaf_token_index]
-            if leaf_token is not None:
-                is_list_empty_line = (
-                    self.__list_item_empty_lines_mode
-                    and leaf_token.is_list_start
-                    and first_non_whitespace_index == 0
-                )
-
-            if extracted_whitespace_length != self.__break_spaces or (
-                self.__strict_mode and not is_list_empty_line
-            ):
-                self.__report_error(
-                    context, extracted_whitespace_length, first_non_whitespace_index
-                )
+    def __next_line_check_for_error(
+        self, line: str, context: PluginScanContext
+    ) -> None:
+        (
+            first_non_whitespace_index,
+            extracted_whitespace,
+        ) = ParserHelper.extract_spaces_from_end(line)
+        extracted_whitespace_length = len(extracted_whitespace)
+
+        is_list_empty_line = False
+        leaf_token = self.__leaf_owner_tokens[self.__leaf_token_index]
+        if leaf_token is not None:
+            is_list_empty_line = (
+                self.__list_item_empty_lines_mode
+                and leaf_token.is_list_start
+                and first_non_whitespace_index == 0
+            )
 
-        self.__line_index += 1
+        if extracted_whitespace_length != self.__break_spaces or (
+            self.__strict_mode and not is_list_empty_line
+        ):
+            self.__report_error(
+                context, extracted_whitespace_length, first_non_whitespace_index
+            )
 
     def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
         """
         Event that a new token is being processed.
         """
         _ = context
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_010.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_010.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_011.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_011.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_012.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_012.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_013.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_013.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,20 +139,18 @@
         ):
             self.__leaf_token_index += 1
 
         line_length = len(line)
         compare_length = self.__line_length
         is_actually_longer = False
         if line_length > self.__minimum_line_length:
-
             is_actually_longer, compare_length = self.__is_really_longer(
                 line_length, compare_length
             )
         if is_actually_longer:
-
             trigger_rule = False
             if self.__strict_mode:
                 trigger_rule = True
             else:
                 next_space_index, _ = ParserHelper.extract_until_spaces(
                     line, compare_length
                 )
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_014.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_014.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_018.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_018.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_019.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_019.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_020.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_020.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_021.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_021.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_022.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_022.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,35 @@
     def completed_file(self, context: PluginScanContext) -> None:
         """
         Event that the file being currently scanned is now completed.
         """
         if (self.__blank_line_count != -1) and self.__blank_line_count >= 0:
             self.perform_close_check(context, None)
 
+    def __next_token_heading_start(self, token: MarkdownToken) -> None:
+        # print(">>token.is_setext_heading or token.is_atx_heading>>")
+        self.__did_above_line_count_match = self.__blank_line_count in [
+            -1,
+            self.__lines_above,
+        ]
+
+        self.__start_heading_token = token
+        self.__start_heading_blank_line_count = self.__blank_line_count
+        self.__did_heading_end = False
+        # print("self.__did_above_line_count_match>>" + str(self.__did_above_line_count_match))
+
+    def __next_token_heading_end(self, token: MarkdownToken) -> None:
+        # print(">>token.is_end_token>>")
+        if not token.is_list_end and not token.is_block_quote_end:
+            self.__blank_line_count = (
+                0 if token.is_leaf_end_token or token.is_container_end_token else -1
+            )
+        if token.is_atx_heading_end or token.is_setext_heading_end:
+            self.__did_heading_end = True
+
     def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
         """
         Event that a new token is being processed.
         """
         # print("START>>" + str(token).replace(ParserHelper.newline_character, "\\n").replace("\t", "\\t"))
         # print(">>self.__blank_line_count>>" + str(self.__blank_line_count))
         if (self.__blank_line_count != -1) and self.__blank_line_count >= 0:
@@ -89,68 +110,57 @@
         if (
             token.is_blank_line
             and (self.__blank_line_count != -1)
             and self.__blank_line_count >= 0
         ):
             self.__blank_line_count += 1
         if token.is_setext_heading or token.is_atx_heading:
-            # print(">>token.is_setext_heading or token.is_atx_heading>>")
-            self.__did_above_line_count_match = bool(
-                self.__blank_line_count in [-1, self.__lines_above]
-            )
-
-            self.__start_heading_token = token
-            self.__start_heading_blank_line_count = self.__blank_line_count
-            self.__did_heading_end = False
-            # print("self.__did_above_line_count_match>>" + str(self.__did_above_line_count_match))
-        elif token.is_thematic_break:
+            self.__next_token_heading_start(token)
+        elif token.is_thematic_break or token.is_link_reference_definition:
             self.__blank_line_count = 0
         elif token.is_end_token:
-            # print(">>token.is_end_token>>")
-            if not token.is_list_end and not token.is_block_quote_end:
-                self.__blank_line_count = (
-                    0 if token.is_leaf_end_token or token.is_container_end_token else -1
-                )
-            if token.is_atx_heading_end or token.is_setext_heading_end:
-                self.__did_heading_end = True
+            self.__next_token_heading_end(token)
         # print(">>self.__blank_line_count>>" + str(self.__blank_line_count))
 
     def perform_close_check(
         self, context: PluginScanContext, token: Optional[MarkdownToken]
     ) -> None:
         """
         Perform any state checks necessary upon closing the heading context.  Also
         called at the end of a document to make sure the implicit close of the
         document is handled properly.
         """
 
-        if ((self.__start_heading_token and self.__did_heading_end)) and (
+        if (self.__start_heading_token and self.__did_heading_end) and (
             not token or (not token.is_blank_line and not token.is_block_quote_end)
         ):
-            did_end_match = bool(self.__blank_line_count == self.__lines_below)
+            did_end_match = self.__blank_line_count == self.__lines_below
+            # print(">>END: did_end_match>>" + str(did_end_match))
             self.report_any_match_failures(context, did_end_match)
             self.__start_heading_token = None
 
     def report_any_match_failures(
         self, context: PluginScanContext, did_end_match: bool
     ) -> None:
         """
         Take care of reporting any match failures.
         """
 
         assert self.__start_heading_token is not None
         if not self.__did_above_line_count_match:
             extra_info = f"Expected: {self.__lines_above}; Actual: {self.__start_heading_blank_line_count}; Above"
+            # print(">>above>>" + extra_info)
             self.report_next_token_error(
                 context,
                 self.__start_heading_token,
                 extra_error_information=extra_info,
                 use_original_position=self.__start_heading_token.is_setext_heading,
             )
         if not did_end_match:
             extra_info = f"Expected: {self.__lines_below}; Actual: {self.__blank_line_count}; Below"
+            # print(">>below>>" + extra_info)
             self.report_next_token_error(
                 context,
                 self.__start_heading_token,
                 extra_error_information=extra_info,
                 use_original_position=self.__start_heading_token.is_setext_heading,
             )
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_023.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_023.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_024.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_024.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_025.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_025.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_026.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_026.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_027.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_027.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,27 +176,27 @@
 
         num_container_tokens = len(
             [i for i in self.__container_tokens if i.is_block_quote_start]
         )
         # if self.__debug_on:
         #     print(f"leading_spaces>{ParserHelper.make_value_visible(self.__container_tokens[-1].leading_spaces)}")
         block_quote_token = cast(BlockQuoteMarkdownToken, self.__container_tokens[-1])
-        assert block_quote_token.leading_spaces is not None
-        newlines_in_container = block_quote_token.leading_spaces.count(
+        assert block_quote_token.bleading_spaces is not None
+        newlines_in_container = block_quote_token.bleading_spaces.count(
             ParserHelper.newline_character
         )
         if (
             not (
-                block_quote_token.leading_spaces
-                and block_quote_token.leading_spaces.endswith(
+                block_quote_token.bleading_spaces
+                and block_quote_token.bleading_spaces.endswith(
                     ParserHelper.newline_character
                 )
             )
             and self.__container_tokens
-            and block_quote_token.leading_spaces
+            and block_quote_token.bleading_spaces
         ):
             # if self.__debug_on:
             #     print(f"newlines_in_container>{newlines_in_container}")
             newlines_in_container += 1
 
         # if self.__debug_on:
         #     print(f"newlines_in_container>{newlines_in_container}")
@@ -266,16 +266,18 @@
                     block_quote_token = cast(
                         BlockQuoteMarkdownToken, end_token.start_markdown_token
                     )
                     # if self.__debug_on:
                     #     print(f"self.__last_token.start_markdown_token>:{ParserHelper.make_value_visible(\
                     #       self.__last_token.start_markdown_token)}:")
                     #     print("BOOM")
-                    assert block_quote_token.leading_spaces is not None
-                    split_line_length = block_quote_token.leading_spaces.split("\n")[-1]
+                    assert block_quote_token.bleading_spaces is not None
+                    split_line_length = block_quote_token.bleading_spaces.split("\n")[
+                        -1
+                    ]
                     # if self.__debug_on:
                     #     print(f"BOOM:{split_line_length}:")
                     whitespace_to_use = whitespace_to_use[len(split_line_length) :]
 
             if is_start_properly_scoped and whitespace_to_use:
                 column_number_delta = -(token.column_number - len(whitespace_to_use))
                 # if self.__debug_on:
@@ -360,26 +362,15 @@
             )
             self.report_next_token_error(
                 context, token, column_number_delta=column_number_delta
             )
         self.__bq_line_index[num_container_tokens] += 1
         self.__last_leaf_token = token
 
-    def __handle_thematic_break(
-        self,
-        context: PluginScanContext,
-        token: MarkdownToken,
-        num_container_tokens: int,
-        is_directly_within_block_quote: bool,
-    ) -> None:
-        self.__handle_common_element(
-            context, token, num_container_tokens, is_directly_within_block_quote
-        )
-
-    def __handle_atx_heading(
+    def __handle_atx_heading_or_thematic_break(
         self,
         context: PluginScanContext,
         token: MarkdownToken,
         num_container_tokens: int,
         is_directly_within_block_quote: bool,
     ) -> None:
         self.__handle_common_element(
@@ -454,16 +445,16 @@
         is_directly_within_block_quote: bool,
     ) -> None:
         fenced_token = cast(FencedCodeBlockMarkdownToken, token)
         if fenced_token.extracted_whitespace and is_directly_within_block_quote:
             scoped_block_quote_token = cast(
                 BlockQuoteMarkdownToken, self.__container_tokens[-1]
             )
-            assert scoped_block_quote_token.leading_spaces is not None
-            split_leading_spaces = scoped_block_quote_token.leading_spaces.split(
+            assert scoped_block_quote_token.bleading_spaces is not None
+            split_leading_spaces = scoped_block_quote_token.bleading_spaces.split(
                 ParserHelper.newline_character
             )
             specific_block_quote_prefix = split_leading_spaces[
                 self.__bq_line_index[num_container_tokens]
             ]
 
             assert self.__line_index_at_bq_start is not None
@@ -495,23 +486,23 @@
         lrd_token: LinkReferenceDefinitionMarkdownToken,
         num_container_tokens: int,
         context: PluginScanContext,
         token: MarkdownToken,
         scoped_block_quote_token: BlockQuoteMarkdownToken,
     ) -> None:
         assert lrd_token.link_name_debug is not None
-        assert scoped_block_quote_token.leading_spaces is not None
+        assert scoped_block_quote_token.bleading_spaces is not None
         line_number_delta = (
             lrd_token.link_name_debug.count(ParserHelper.newline_character) + 1
         )
 
         split_array_index = (
             self.__bq_line_index[num_container_tokens] + line_number_delta
         )
-        split_leading_spaces = scoped_block_quote_token.leading_spaces.split(
+        split_leading_spaces = scoped_block_quote_token.bleading_spaces.split(
             ParserHelper.newline_character
         )
         specific_block_quote_prefix = split_leading_spaces[split_array_index]
 
         column_number_delta = -(len(specific_block_quote_prefix) + 1)
 
         # if self.__debug_on:
@@ -527,24 +518,73 @@
             token,
             line_number_delta=line_number_delta,
             column_number_delta=column_number_delta,
         )
 
     # pylint: enable=too-many-arguments
 
+    # pylint: disable=too-many-arguments
+    def __handle_link_reference_definition_check_after(
+        self,
+        context: PluginScanContext,
+        token: MarkdownToken,
+        num_container_tokens: int,
+        lrd_token: LinkReferenceDefinitionMarkdownToken,
+        leading_spaces: str,
+    ) -> None:
+        assert lrd_token.link_name_debug is not None
+        assert lrd_token.link_title_whitespace is not None
+        line_number_delta = (
+            lrd_token.link_name_debug.count(ParserHelper.newline_character)
+            + lrd_token.link_title_whitespace.count(ParserHelper.newline_character)
+            + 1
+        )
+
+        split_array_index = (
+            self.__bq_line_index[num_container_tokens] + line_number_delta
+        )
+        split_leading_spaces = leading_spaces.split(ParserHelper.newline_character)
+        specific_block_quote_prefix = split_leading_spaces[split_array_index]
+
+        column_number_delta = -(len(specific_block_quote_prefix) + 1)
+        # if self.__debug_on:
+        #     print("line_number_delta>>" + str(line_number_delta))
+        #     print("split_array_index>>" + str(split_array_index))
+        #     print(f"end-container>>{ParserHelper.make_value_visible(self.__container_tokens[-1])}")
+        #     print(f"split_leading_spaces>>{ParserHelper.make_value_visible(split_leading_spaces)}")
+        #     print("specific_block_quote_prefix>>:" + \
+        #       f"{ParserHelper.make_value_visible(specific_block_quote_prefix)}:")
+        #     print("lrd-3-error")
+        self.report_next_token_error(
+            context,
+            token,
+            line_number_delta=line_number_delta,
+            column_number_delta=column_number_delta,
+        )
+
+    # pylint: enable=too-many-arguments
+
     def __handle_link_reference_definition(
         self,
         context: PluginScanContext,
         token: MarkdownToken,
         num_container_tokens: int,
     ) -> None:
         scoped_block_quote_token = cast(
             BlockQuoteMarkdownToken, self.__container_tokens[-1]
         )
-        assert scoped_block_quote_token.leading_spaces is not None
+        if scoped_block_quote_token.is_block_quote_start:
+            assert scoped_block_quote_token.bleading_spaces is not None
+            leading_spaces = scoped_block_quote_token.bleading_spaces
+        else:
+            scoped_list_token = cast(
+                ListStartMarkdownToken, self.__container_tokens[-1]
+            )
+            assert scoped_list_token.leading_spaces is not None
+            leading_spaces = scoped_list_token.leading_spaces
         lrd_token = cast(LinkReferenceDefinitionMarkdownToken, token)
         if lrd_token.extracted_whitespace:
             column_number_delta = -(
                 lrd_token.column_number - len(lrd_token.extracted_whitespace)
             )
             # if self.__debug_on:
             #     print("lrd-1-error")
@@ -570,56 +610,68 @@
         assert lrd_token.link_title_whitespace is not None
         found_index = lrd_token.link_title_whitespace.find(
             ParserHelper.newline_character
         )
         if found_index != -1 and ParserHelper.is_character_at_index_whitespace(
             lrd_token.link_title_whitespace, found_index + 1
         ):
-            assert lrd_token.link_name_debug is not None
-            line_number_delta = (
-                lrd_token.link_name_debug.count(ParserHelper.newline_character)
-                + lrd_token.link_title_whitespace.count(ParserHelper.newline_character)
-                + 1
+            self.__handle_link_reference_definition_check_after(
+                context, token, num_container_tokens, lrd_token, leading_spaces
             )
 
-            split_array_index = (
-                self.__bq_line_index[num_container_tokens] + line_number_delta
+        assert lrd_token.link_name_debug is not None
+        assert lrd_token.link_title_raw is not None
+        self.__bq_line_index[num_container_tokens] += (
+            1
+            + lrd_token.link_name_debug.count(ParserHelper.newline_character)
+            + lrd_token.link_destination_whitespace.count(
+                ParserHelper.newline_character
             )
-            split_leading_spaces = scoped_block_quote_token.leading_spaces.split(
+            + lrd_token.link_title_whitespace.count(ParserHelper.newline_character)
+            + lrd_token.link_title_raw.count(ParserHelper.newline_character)
+        )
+
+    # pylint: disable=too-many-arguments
+    def __scan_text(
+        self,
+        context: PluginScanContext,
+        token: MarkdownToken,
+        next_line: str,
+        scoped_block_quote_token: BlockQuoteMarkdownToken,
+        num_container_tokens: int,
+        line_number_delta: int,
+    ) -> None:
+        found_index = next_line.find(ParserHelper.whitespace_split_character)
+        if found_index != -1:
+            next_line = next_line[:found_index]
+        if next_line:
+            assert scoped_block_quote_token.bleading_spaces is not None
+            split_leading_spaces = scoped_block_quote_token.bleading_spaces.split(
                 ParserHelper.newline_character
             )
+            split_array_index = (
+                self.__bq_line_index[num_container_tokens] + line_number_delta + 1
+            )
             specific_block_quote_prefix = split_leading_spaces[split_array_index]
+            calculated_column_number = -(len(specific_block_quote_prefix) + 1)
 
-            column_number_delta = -(len(specific_block_quote_prefix) + 1)
             # if self.__debug_on:
-            #     print("line_number_delta>>" + str(line_number_delta))
-            #     print("split_array_index>>" + str(split_array_index))
-            #     print(f"end-container>>{ParserHelper.make_value_visible(self.__container_tokens[-1])}")
             #     print(f"split_leading_spaces>>{ParserHelper.make_value_visible(split_leading_spaces)}")
+            #     print(f"split_array_index>>{ParserHelper.make_value_visible(split_array_index)}")
             #     print("specific_block_quote_prefix>>:" + \
             #       f"{ParserHelper.make_value_visible(specific_block_quote_prefix)}:")
-            #     print("lrd-3-error")
+            #     print("setext-text-error")
             self.report_next_token_error(
                 context,
                 token,
                 line_number_delta=line_number_delta,
-                column_number_delta=column_number_delta,
+                column_number_delta=calculated_column_number,
             )
 
-        assert lrd_token.link_name_debug is not None
-        assert lrd_token.link_title_raw is not None
-        self.__bq_line_index[num_container_tokens] += (
-            1
-            + lrd_token.link_name_debug.count(ParserHelper.newline_character)
-            + lrd_token.link_destination_whitespace.count(
-                ParserHelper.newline_character
-            )
-            + lrd_token.link_title_whitespace.count(ParserHelper.newline_character)
-            + lrd_token.link_title_raw.count(ParserHelper.newline_character)
-        )
+    # pylint: enable=too-many-arguments
 
     def __handle_text(
         self,
         context: PluginScanContext,
         token: MarkdownToken,
         num_container_tokens: int,
         is_directly_within_block_quote: bool,
@@ -627,55 +679,28 @@
         assert self.__last_leaf_token is not None
         text_token = cast(TextMarkdownToken, token)
         if self.__last_leaf_token.is_setext_heading:
             if is_directly_within_block_quote:
                 scoped_block_quote_token = cast(
                     BlockQuoteMarkdownToken, self.__container_tokens[-1]
                 )
-                assert scoped_block_quote_token.leading_spaces is not None
+                assert scoped_block_quote_token.bleading_spaces is not None
                 assert text_token.end_whitespace is not None
 
                 for line_number_delta, next_line in enumerate(
                     text_token.end_whitespace.split(ParserHelper.newline_character)
                 ):
-                    found_index = next_line.find(
-                        ParserHelper.whitespace_split_character
+                    self.__scan_text(
+                        context,
+                        token,
+                        next_line,
+                        scoped_block_quote_token,
+                        num_container_tokens,
+                        line_number_delta,
                     )
-                    if found_index != -1:
-                        next_line = next_line[:found_index]
-                    if next_line:
-                        split_leading_spaces = (
-                            scoped_block_quote_token.leading_spaces.split(
-                                ParserHelper.newline_character
-                            )
-                        )
-                        split_array_index = (
-                            self.__bq_line_index[num_container_tokens]
-                            + line_number_delta
-                            + 1
-                        )
-                        specific_block_quote_prefix = split_leading_spaces[
-                            split_array_index
-                        ]
-                        calculated_column_number = -(
-                            len(specific_block_quote_prefix) + 1
-                        )
-
-                        # if self.__debug_on:
-                        #     print(f"split_leading_spaces>>{ParserHelper.make_value_visible(split_leading_spaces)}")
-                        #     print(f"split_array_index>>{ParserHelper.make_value_visible(split_array_index)}")
-                        #     print("specific_block_quote_prefix>>:" + \
-                        #       f"{ParserHelper.make_value_visible(specific_block_quote_prefix)}:")
-                        #     print("setext-text-error")
-                        self.report_next_token_error(
-                            context,
-                            token,
-                            line_number_delta=line_number_delta,
-                            column_number_delta=calculated_column_number,
-                        )
             assert text_token.end_whitespace is not None
             self.__bq_line_index[num_container_tokens] += (
                 text_token.end_whitespace.count(ParserHelper.newline_character) + 1
             )
         elif (
             self.__last_leaf_token.is_html_block or self.__last_leaf_token.is_code_block
         ):
@@ -700,21 +725,21 @@
             #     print(f"para>>>{scoped_block_quote_token}")
 
             for line_number_delta, next_line in enumerate(
                 paragraph_token.extracted_whitespace.split(
                     ParserHelper.newline_character
                 )
             ):
-                if next_line and scoped_block_quote_token.leading_spaces:
+                if next_line and scoped_block_quote_token.bleading_spaces:
                     # if self.__debug_on:
                     #     print(f"1>{self.__bq_line_index[num_container_tokens]}")
                     #     print(f"2>{line_number_delta}")
                     #     print(f"3>{ParserHelper.make_value_visible(scoped_block_quote_token)}")
                     split_leading_spaces = (
-                        scoped_block_quote_token.leading_spaces.split(
+                        scoped_block_quote_token.bleading_spaces.split(
                             ParserHelper.newline_character
                         )
                     )
                     line_index = (
                         self.__bq_line_index[num_container_tokens] + line_number_delta
                     )
                     calculated_column_number = len(split_leading_spaces[line_index]) + 1
@@ -766,30 +791,26 @@
             self.__is_paragraph_end_delayed = True
             # if self.__debug_on:
             #     print("[[Delaying paragraph end]]")
         elif token.is_blank_line:
             self.__delayed_blank_line = token
             # if self.__debug_on:
             #     print("[[Delaying blank line]]")
-        elif token.is_atx_heading:
-            self.__handle_atx_heading(
+        elif token.is_atx_heading or token.is_thematic_break:
+            self.__handle_atx_heading_or_thematic_break(
                 context, token, num_container_tokens, is_directly_within_block_quote
             )
         elif token.is_setext_heading:
             self.__handle_setext_heading(context, token, is_directly_within_block_quote)
         elif token.is_setext_heading_end:
             self.__handle_setext_heading_end(
                 context, token, num_container_tokens, is_directly_within_block_quote
             )
         elif token.is_atx_heading_end:
             self.__last_leaf_token = None
-        elif token.is_thematic_break:
-            self.__handle_thematic_break(
-                context, token, num_container_tokens, is_directly_within_block_quote
-            )
         elif token.is_link_reference_definition:
             self.__handle_link_reference_definition(
                 context, token, num_container_tokens
             )
         else:
             self.__handle_within_block_quotes_blocks(
                 token, context, num_container_tokens, is_directly_within_block_quote
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_028.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_028.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_029.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_029.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_030.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_030.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
         """
         self.__list_stack = []
         self.__list_tokens = []
         self.__current_list_parent = None
         self.__paragraph_count_map = {}
 
     def __handle_list_end(self, context: PluginScanContext) -> None:
-
         for list_token in self.__list_tokens[-1]:
             this_list_token_paragraph_count = 0
             if str(list_token) in self.__paragraph_count_map:
                 this_list_token_paragraph_count = self.__paragraph_count_map[
                     str(list_token)
                 ]
             if self.__list_tokens[-1][0].is_ordered_list_start:
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_031.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_031.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_032.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_032.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
             self.__end_list_end_token = None
 
         if token.is_block_quote_start:
             self.__container_token_stack.append(token)
         elif token.is_block_quote_end:
             del self.__container_token_stack[-1]
         elif token.is_list_start:
-
             if (
                 self.__last_non_end_token
                 and not (
                     self.__container_token_stack
                     and self.__container_token_stack[-1].is_list_start
                 )
                 and not self.__last_non_end_token.is_blank_line
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_033.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_033.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_034.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_034.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_035.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_035.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_036.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_041.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,107 @@
 """
-Module to implement a plugin that looks for single line emphasis text that looks
-like it is being used instead of a heading.
+Module to implement a plugin that ensures that the first line in a file is a top level heading.
 """
-from enum import Enum
 from typing import Optional, cast
 
+from pymarkdown.extensions.front_matter_markdown_token import FrontMatterMarkdownToken
 from pymarkdown.inline_markdown_token import TextMarkdownToken
+from pymarkdown.leaf_markdown_token import AtxHeadingMarkdownToken
 from pymarkdown.markdown_token import MarkdownToken
-from pymarkdown.parser_helper import ParserHelper
 from pymarkdown.plugin_manager.plugin_details import PluginDetails
 from pymarkdown.plugin_manager.plugin_scan_context import PluginScanContext
 from pymarkdown.plugin_manager.rule_plugin import RulePlugin
 
 
-class RuleMd036States(Enum):
+class RuleMd041(RulePlugin):
     """
-    Enumeration to provide guidance on what to look for as the tokens come in.
-    """
-
-    LOOK_FOR_PARAGRAPH = 0
-    LOOK_FOR_EMPHASIS_START = 1
-    LOOK_FOR_ELIGIBLE_TEXT = 2
-    LOOK_FOR_EMPHASIS_END = 3
-    LOOK_FOR_PARAGRAPH_END = 4
-
-
-class RuleMd036(RulePlugin):
-    """
-    Class to implement a plugin that looks for single line emphasis text that looks
-    like it is being used instead of a heading.
+    Class to implement a plugin that ensures that the first line in a file is a top level heading.
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.__punctuation: str = ""
-        self.__current_state: RuleMd036States = RuleMd036States.LOOK_FOR_PARAGRAPH
-        self.__start_token: Optional[MarkdownToken] = None
+        self.__start_level: int = -1
+        self.__front_matter_title: str = ""
+        self.__have_seen_first_token: bool = False
+        self.__seen_html_block_start: Optional[MarkdownToken] = None
 
     def get_details(self) -> PluginDetails:
         """
         Get the details for the plugin.
         """
         return PluginDetails(
-            plugin_name="no-emphasis-as-heading,no-emphasis-as-header",
-            plugin_id="MD036",
+            plugin_name="first-line-heading,first-line-h1",
+            plugin_id="MD041",
             plugin_enabled_by_default=True,
-            plugin_description="Emphasis possibly used instead of a heading element.",
+            plugin_description="First line in file should be a top level heading",
             plugin_version="0.5.0",
             plugin_interface_version=1,
-            plugin_url="https://github.com/jackdewinter/pymarkdown/blob/main/docs/rules/rule_md036.md",
-            plugin_configuration="punctuation",
+            plugin_url="https://github.com/jackdewinter/pymarkdown/blob/main/docs/rules/rule_md041.md",
+            plugin_configuration="level,front_matter_title",
         )
 
+    @classmethod
+    def __validate_configuration_level(cls, found_value: int) -> None:
+        if found_value < 1 or found_value > 6:
+            raise ValueError("Allowable values are between 1 and 6.")
+
+    @classmethod
+    def __validate_configuration_title(cls, found_value: str) -> None:
+        found_value = found_value.strip()
+        if ":" in found_value:
+            raise ValueError("Colons (:) are not allowed in the value.")
+
     def initialize_from_config(self) -> None:
         """
         Event to allow the plugin to load configuration information.
         """
-        self.__punctuation = self.plugin_configuration.get_string_property(
-            "punctuation", default_value=".,;:!?。，；：？"
+        self.__start_level = self.plugin_configuration.get_integer_property(
+            "level",
+            default_value=1,
+            valid_value_fn=self.__validate_configuration_level,
+        )
+        self.__front_matter_title = (
+            self.plugin_configuration.get_string_property(
+                "front_matter_title",
+                default_value="title",
+                valid_value_fn=self.__validate_configuration_title,
+            )
+            .lower()
+            .strip()
         )
 
     def starting_new_file(self) -> None:
         """
         Event that the a new file to be scanned is starting.
         """
-        self.__current_state = RuleMd036States.LOOK_FOR_PARAGRAPH
-        self.__start_token = None
+        self.__have_seen_first_token = False
+        self.__seen_html_block_start = None
 
     def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
         """
         Event that a new token is being processed.
         """
-        new_state = RuleMd036States.LOOK_FOR_PARAGRAPH
-
-        if self.__current_state == RuleMd036States.LOOK_FOR_PARAGRAPH:
-            if token.is_paragraph:
-                new_state = RuleMd036States.LOOK_FOR_EMPHASIS_START
-                self.__start_token = token
-        elif self.__current_state == RuleMd036States.LOOK_FOR_EMPHASIS_START:
-            if token.is_inline_emphasis:
-                new_state = RuleMd036States.LOOK_FOR_ELIGIBLE_TEXT
-        elif self.__current_state == RuleMd036States.LOOK_FOR_ELIGIBLE_TEXT:
-            if token.is_text:
-                text_token = cast(TextMarkdownToken, token)
-                if (
-                    ParserHelper.newline_character not in text_token.token_text
-                    and text_token.token_text[-1] not in self.__punctuation
-                ):
-                    new_state = RuleMd036States.LOOK_FOR_EMPHASIS_END
-        elif self.__current_state == RuleMd036States.LOOK_FOR_EMPHASIS_END:
-            if token.is_inline_emphasis_end:
-                new_state = RuleMd036States.LOOK_FOR_PARAGRAPH_END
-        else:
-            assert self.__current_state == RuleMd036States.LOOK_FOR_PARAGRAPH_END
-            if token.is_paragraph_end:
-                assert self.__start_token is not None
-                self.report_next_token_error(context, self.__start_token)
-
-        self.__current_state = new_state
+        if self.__have_seen_first_token:
+            return
+        if token.is_atx_heading or token.is_setext_heading:
+            atx_token = cast(AtxHeadingMarkdownToken, token)
+            self.__have_seen_first_token = True
+            if atx_token.hash_count != self.__start_level:
+                self.report_next_token_error(context, token)
+        elif token.is_front_matter and self.__front_matter_title:
+            front_token = cast(FrontMatterMarkdownToken, token)
+            if self.__front_matter_title in front_token.matter_map:
+                self.__have_seen_first_token = True
+        elif token.is_html_block:
+            self.__seen_html_block_start = token
+        elif self.__seen_html_block_start:
+            assert token.is_text
+            text_token = cast(TextMarkdownToken, token)
+            html_block_contents = text_token.token_text.strip()
+            if not html_block_contents.startswith(
+                "<h1 "
+            ) and not html_block_contents.startswith("<h1>"):
+                self.report_next_token_error(context, self.__seen_html_block_start)
+            self.__have_seen_first_token = True
+        elif not token.is_blank_line:
+            self.report_next_token_error(context, token)
+            self.__have_seen_first_token = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_037.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_037.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,45 +39,51 @@
         """
         Event that the a new file to be scanned is starting.
         """
         self.__block_stack = []
         self.__start_emphasis_token = None
         self.__emphasis_token_list = []
 
+    def __handle_emphasis_text(
+        self, context: PluginScanContext, token: MarkdownToken
+    ) -> None:
+        text_token = cast(TextMarkdownToken, token)
+        assert self.__start_emphasis_token is not None
+        if text_token.token_text == self.__start_emphasis_token.token_text:
+            assert self.__emphasis_token_list
+            did_first_start_with_space = self.__handle_emphasis_text_space_check(0)
+            did_last_end_with_space = self.__handle_emphasis_text_space_check(-1)
+            if did_first_start_with_space or did_last_end_with_space:
+                assert self.__start_emphasis_token is not None
+                self.report_next_token_error(context, self.__start_emphasis_token)
+
+            self.__start_emphasis_token = None
+            self.__emphasis_token_list = []
+        else:
+            self.__emphasis_token_list.append(token)
+
+    def __handle_emphasis_text_space_check(self, token_text_index: int) -> bool:
+        first_capture_token = self.__emphasis_token_list[token_text_index]
+        assert first_capture_token.is_text
+        other_text_token = cast(TextMarkdownToken, first_capture_token)
+        return other_text_token.token_text[token_text_index] == " "
+
     def __handle_start_emphasis(
         self, context: PluginScanContext, token: MarkdownToken
     ) -> None:
         if (
             token.is_paragraph_end
             or token.is_setext_heading_end
             or token.is_atx_heading_end
         ):
             del self.__block_stack[-1]
             self.__start_emphasis_token = None
             self.__emphasis_token_list = []
         elif token.is_text and self.__start_emphasis_token is not None:
-            text_token = cast(TextMarkdownToken, token)
-            if text_token.token_text == self.__start_emphasis_token.token_text:
-                assert self.__emphasis_token_list
-                first_capture_token = self.__emphasis_token_list[0]
-                assert first_capture_token.is_text
-                other_text_token = cast(TextMarkdownToken, first_capture_token)
-                did_first_start_with_space = other_text_token.token_text[0] == " "
-                last_capture_token = self.__emphasis_token_list[-1]
-                assert last_capture_token.is_text
-                another_text_token = cast(TextMarkdownToken, last_capture_token)
-                did_last_end_with_space = another_text_token.token_text[-1] == " "
-                if did_first_start_with_space or did_last_end_with_space:
-                    assert self.__start_emphasis_token is not None
-                    self.report_next_token_error(context, self.__start_emphasis_token)
-
-                self.__start_emphasis_token = None
-                self.__emphasis_token_list = []
-            else:
-                self.__emphasis_token_list.append(token)
+            self.__handle_emphasis_text(context, token)
         else:
             self.__emphasis_token_list.append(token)
 
     def next_token(self, context: PluginScanContext, token: MarkdownToken) -> None:
         """
         Event that a new token is being processed.
         """
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_038.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_038.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_039.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_039.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_040.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_040.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_042.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_042.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_043.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_043.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,50 +133,56 @@
             while heading_index >= 0 and self.__suffix_index == -1:
                 heading_contents = self.__compiled_headings[heading_index]
                 if heading_contents == "*":
                     self.__suffix_index = heading_index + 1
                 else:
                     heading_index -= 1
 
+    def __verify_single_heading_match_atx(
+        self, matching_all_token_index: int, hash_count: int, expected_text: str
+    ) -> Tuple[Optional[MarkdownToken], Optional[str]]:
+        failure_token, failure_reason = (None, None)
+
+        these_tokens = self.__all_tokens[matching_all_token_index]
+        atx_token = cast(AtxHeadingMarkdownToken, these_tokens[0])
+        if atx_token.hash_count != hash_count:
+            failure_reason = f"Bad heading level: Expected: {hash_count}, Actual: {atx_token.hash_count}"
+        elif len(these_tokens) != 2 or not these_tokens[1].is_text:
+            failure_reason = "Bad heading: Required headings must only be normal text."
+        else:
+            text_token = cast(TextMarkdownToken, these_tokens[1])
+            if text_token.token_text != expected_text:
+                failure_reason = f"Bad heading text: Expected: {expected_text}, Actual: {text_token.token_text}"
+        if failure_reason:
+            failure_token = these_tokens[0]
+        return failure_token, failure_reason
+
     def __verify_single_heading_match(
         self,
         this_compiled_heading: Union[str, Tuple[int, str]],
         matching_all_token_index: int,
     ) -> Tuple[Optional[MarkdownToken], Optional[str]]:
-
         failure_token, failure_reason = (None, None)
 
         assert len(this_compiled_heading) == 2
         this_heading = cast(Tuple[int, str], this_compiled_heading)
         hash_count: int = this_heading[0]
         expected_text: str = this_heading[1]
         if matching_all_token_index >= len(self.__all_tokens):
             failure_token = self.__all_tokens[-1][0]
             failure_reason = f"Missing heading: {ParserHelper.repeat_string('#', hash_count)} {expected_text}"
         else:
-            these_tokens = self.__all_tokens[matching_all_token_index]
-            atx_token = cast(AtxHeadingMarkdownToken, these_tokens[0])
-            if atx_token.hash_count != hash_count:
-                failure_reason = f"Bad heading level: Expected: {hash_count}, Actual: {atx_token.hash_count}"
-            elif len(these_tokens) != 2 or not these_tokens[1].is_text:
-                failure_reason = (
-                    "Bad heading: Required headings must only be normal text."
-                )
-            else:
-                text_token = cast(TextMarkdownToken, these_tokens[1])
-                if text_token.token_text != expected_text:
-                    failure_reason = f"Bad heading text: Expected: {expected_text}, Actual: {text_token.token_text}"
-            if failure_reason:
-                failure_token = these_tokens[0]
+            failure_token, failure_reason = self.__verify_single_heading_match_atx(
+                matching_all_token_index, hash_count, expected_text
+            )
         return failure_token, failure_reason
 
     def __verify_group_heading_match(
         self, heading_index: int, all_token_index: int, scan_limit: int = -1
     ) -> Tuple[int, int, Optional[MarkdownToken], Optional[str]]:
-
         if scan_limit < 0:
             scan_limit = len(self.__compiled_headings)
 
         failure_token, failure_reason = (None, None)
         # if self.__show_debug:
         #     print(
         #         "vghm:heading_index="
@@ -213,15 +219,14 @@
             #     )
             if not failure_token:
                 heading_index += 1
                 all_token_index += 1
         return heading_index, all_token_index, failure_token, failure_reason
 
     def __handle_no_wildcards_match(self, context: PluginScanContext) -> None:
-
         end_index, _, failure_token, failure_reason = self.__verify_group_heading_match(
             0, 0
         )
         if failure_token:
             self.report_next_token_error(
                 context, failure_token, extra_error_information=failure_reason
             )
@@ -230,15 +235,14 @@
             self.report_next_token_error(
                 context, anchor_token, extra_error_information="Extra heading"
             )
 
     def __handle_wildcard_prefix(
         self,
     ) -> Tuple[int, int, Optional[MarkdownToken], Optional[str]]:
-
         (
             top_heading_index,
             top_token_index,
             failure_token,
             failure_reason,
         ) = self.__verify_group_heading_match(0, 0, scan_limit=self.__prefix_index)
         # if self.__show_debug:
@@ -268,15 +272,20 @@
         #         + ",top_token_index="
         #         + str(top_token_index)
         #     )
         if start_all_token_index < top_token_index:
             failure_token: Optional[MarkdownToken] = self.__all_tokens[-1][0]
             failure_reason: Optional[str] = "Overlapped."
         else:
-            (_, _, failure_token, failure_reason,) = self.__verify_group_heading_match(
+            (
+                _,
+                _,
+                failure_token,
+                failure_reason,
+            ) = self.__verify_group_heading_match(
                 self.__suffix_index, start_all_token_index
             )
             # if self.__show_debug:
             #     print(
             #         "bottom_suffix_index="
             #         + str(bottom_suffix_index)
             #         + ",bottom_all_token_index="
@@ -291,23 +300,21 @@
     def starting_new_file(self) -> None:
         """
         Event that the a new file to be scanned is starting.
         """
         self.__collected_tokens = []
         self.__all_tokens = []
 
-    # pylint: disable=too-many-locals
     def __do_recursive(
         self,
         remaining_headings: List[Union[str, Tuple[int, str]]],
         top_heading_index: int,
         remaining_tokens: List[List[MarkdownToken]],
         top_token_index: int,
     ) -> bool:
-
         bottom_heading_index = top_heading_index + len(remaining_headings)
 
         # if self.__show_debug:
         #     print(
         #         "remaining_headings:"
         #         + str(remaining_headings)
         #         + ",top="
@@ -340,61 +347,104 @@
         search_index = 0
         heading_index = top_heading_index + 1
         scan_limit = top_heading_index + 1 + delta
         found_match = False
         while search_index < len(remaining_headings) and search_index < len(
             remaining_tokens
         ):
-            (
-                end_heading_index,
-                end_token_index,
-                failure_token,
-                _,
-            ) = self.__verify_group_heading_match(
-                heading_index, top_token_index + search_index, scan_limit=scan_limit
+            found_match, search_index = self.__do_recursive_loop(
+                heading_index,
+                top_token_index,
+                search_index,
+                scan_limit,
+                bottom_heading_index,
+                top_heading_index,
+                remaining_tokens,
+                remaining_headings,
             )
-            # if self.__show_debug:
-            #     print(str((end_heading_index, end_token_index, failure_token)))
-            if not failure_token and end_heading_index < len(self.__compiled_headings):
-                # if self.__show_debug:
-                #     print(
-                #         "FOUND:"
-                #         + str((end_heading_index, end_token_index, failure_token))
-                #     )
-                if end_heading_index == bottom_heading_index - 1:
-                    # if self.__show_debug:
-                    #     print("done")
-                    found_match = True
-                else:
-                    new_top_heading_index = end_heading_index
-                    new_remaining_headings = remaining_headings[
-                        (end_heading_index - top_heading_index) :
-                    ]
-
-                    new_remaining_tokens = remaining_tokens[
-                        (end_token_index - top_token_index) :
-                    ]
-                    new_top_token_index = end_token_index
-
-                    # if self.__show_debug:
-                    #     print("recurse")
-                    found_match = self.__do_recursive(
-                        new_remaining_headings,
-                        new_top_heading_index,
-                        new_remaining_tokens,
-                        new_top_token_index,
-                    )
-                    # if self.__show_debug:
-                    #     print("found_match=" + str(found_match))
             if found_match:
                 break
-            search_index += 1
         return found_match
 
-    # pylint: enable=too-many-locals
+    # pylint: disable=too-many-arguments
+    def __do_recursive_loop(
+        self,
+        heading_index: int,
+        top_token_index: int,
+        search_index: int,
+        scan_limit: int,
+        bottom_heading_index: int,
+        top_heading_index: int,
+        remaining_tokens: List[List[MarkdownToken]],
+        remaining_headings: List[Union[str, Tuple[int, str]]],
+    ) -> Tuple[bool, int]:
+        (
+            end_heading_index,
+            end_token_index,
+            failure_token,
+            _,
+        ) = self.__verify_group_heading_match(
+            heading_index, top_token_index + search_index, scan_limit=scan_limit
+        )
+        # if self.__show_debug:
+        #     print(str((end_heading_index, end_token_index, failure_token)))
+        found_match = False
+        if not failure_token and end_heading_index < len(self.__compiled_headings):
+            # if self.__show_debug:
+            #     print(
+            #         "FOUND:"
+            #         + str((end_heading_index, end_token_index, failure_token))
+            #     )
+            if end_heading_index == bottom_heading_index - 1:
+                # if self.__show_debug:
+                #     print("done")
+                found_match = True
+            else:
+                found_match = self.__prepare_and_do_recurse(
+                    end_heading_index,
+                    top_heading_index,
+                    end_token_index,
+                    top_token_index,
+                    remaining_headings,
+                    remaining_tokens,
+                )
+                # if self.__show_debug:
+                #     print("found_match=" + str(found_match))
+        if not found_match:
+            search_index += 1
+        return found_match, search_index
+
+    # pylint: enable=too-many-arguments
+
+    # pylint: disable=too-many-arguments
+    def __prepare_and_do_recurse(
+        self,
+        end_heading_index: int,
+        top_heading_index: int,
+        end_token_index: int,
+        top_token_index: int,
+        remaining_headings: List[Union[str, Tuple[int, str]]],
+        remaining_tokens: List[List[MarkdownToken]],
+    ) -> bool:
+        new_top_heading_index = end_heading_index
+        new_remaining_headings = remaining_headings[
+            (end_heading_index - top_heading_index) :
+        ]
+
+        new_remaining_tokens = remaining_tokens[(end_token_index - top_token_index) :]
+        new_top_token_index = end_token_index
+
+        return self.__do_recursive(
+            new_remaining_headings,
+            new_top_heading_index,
+            new_remaining_tokens,
+            new_top_token_index,
+        )
+
+    # pylint: enable=too-many-arguments
 
     def completed_file(self, context: PluginScanContext) -> None:
         """
         Event that the file being currently scanned is now completed.
         """
         if not self.__compiled_headings:
             return
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_044.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_044.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         found_index: int,
         required_capitalization: str,
         context: PluginScanContext,
         token: MarkdownToken,
         line_adjust: int,
         col_adjust: int,
     ) -> None:
-
         original_found_text = original_source[
             found_index : found_index + len(required_capitalization)
         ]
         after_found_index = found_index + len(required_capitalization)
 
         is_character_before_match = False
         if found_index > 0:
@@ -163,23 +162,21 @@
         string_to_check: str,
         context: PluginScanContext,
         token: MarkdownToken,
         same_line_offset: int = 0,
         start_x_offset: int = 0,
         start_y_offset: int = 0,
     ) -> None:
-
         string_to_check = ParserHelper.remove_all_from_text(string_to_check)
         string_to_check_lower = string_to_check.lower()
         for next_name in self.__proper_name_list:
             next_name_lower = next_name.lower()
             search_start = 0
             found_index = string_to_check_lower.find(next_name_lower, search_start)
             while found_index != -1:
-
                 self.__search_for_possible_matches(
                     string_to_check,
                     string_to_check_lower,
                     search_start,
                     found_index,
                     start_x_offset,
                     start_y_offset,
@@ -200,15 +197,14 @@
         context: PluginScanContext,
         token: MarkdownToken,
         link_body_text: str,
         full_link_text: str,
         string_to_check: str,
         same_line_offset: int,
     ) -> None:
-
         start_x_offset = 0
         start_y_offset = 0
         if ParserHelper.newline_character in link_body_text:
             start_x_offset, start_y_offset = ParserHelper.adjust_for_newlines(
                 full_link_text, 0, len(full_link_text)
             )
         self.__search_for_matches(
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_045.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_045.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_046.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_046.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_047.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_047.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/plugins/rule_md_048.py` & `pymarkdownlnt-0.9.9/pymarkdown/plugins/rule_md_048.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/resources/entities.json` & `pymarkdownlnt-0.9.9/pymarkdown/resources/entities.json`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/source_providers.py` & `pymarkdownlnt-0.9.9/pymarkdown/source_providers.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/stack_token.py` & `pymarkdownlnt-0.9.9/pymarkdown/stack_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,28 +474,32 @@
     """
     Class to provide for a stack token for a possible link definition.
     """
 
     def __init__(
         self, extracted_whitespace: Optional[str], position_marker: PositionMarker
     ) -> None:
-        (self.__extracted_whitespace, self.__start_position_marker,) = (
+        (
+            self.__extracted_whitespace,
+            self.__start_position_marker,
+        ) = (
             extracted_whitespace,
             position_marker,
         )
         self.original_stack_depth: Optional[int] = None
         self.original_document_depth: Optional[int] = None
         self.last_block_quote_stack_token: Optional[StackToken] = None
         self.last_block_quote_markdown_token_index: Optional[int] = None
         self.copy_of_last_block_quote_markdown_token: Optional[
             BlockQuoteMarkdownToken
         ] = None
         self.copy_of_token_stack: Optional[List[StackToken]] = None
         self.__continuation_lines: List[str] = []
         self.__unmodified_lines: List[str] = []
+        # self.__original_lines: List[str] = []
         StackToken.__init__(self, StackToken._stack_link_definition)
 
     @property
     def extracted_whitespace(self) -> Optional[str]:
         """
         Returns the extracted whitespace associated with this stack token.
         """
@@ -511,14 +515,21 @@
     @property
     def unmodified_lines(self) -> List[str]:
         """
         Returns the unmodified continuation lines associated with this stack token.
         """
         return self.__unmodified_lines
 
+    # @property
+    # def original_lines(self) -> List[str]:
+    #     """
+    #     Returns the original lines associated with this stack token.
+    #     """
+    #     return self.__original_lines
+
     @property
     def start_position_marker(self) -> PositionMarker:
         """
         Returns the start position associated with this stack token.
         """
         return self.__start_position_marker
 
@@ -532,15 +543,21 @@
         """
         Add the line to the collection of lines to keep as "umodified line".
         These are the same as the continuation_lines values, just with the exact
         text that was presented to the parser.
         """
         self.__unmodified_lines.append(new_line)
 
-    def get_joined_lines(self, join_suffix: str) -> str:
+    # def add_original_line(self, new_line: str) -> None:
+    #     """
+    #     ...
+    #     """
+    #     self.__original_lines.append(new_line)
+
+    def add_joined_lines_before_suffix(self, join_suffix: str) -> str:
         """
         Grab the continuation lines as a single line.
         """
 
         return (
             f"{ParserHelper.newline_character.join(self.continuation_lines) }"
             + f"{ParserHelper.newline_character}{join_suffix}"
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/tokenized_markdown.py` & `pymarkdownlnt-0.9.9/pymarkdown/tokenized_markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import os
 from typing import Any, List, Optional, Tuple, cast
 
 from application_properties import ApplicationProperties
 
 from pymarkdown.bad_tokenization_error import BadTokenizationError
 from pymarkdown.coalesce_processor import CoalesceProcessor
-from pymarkdown.container_block_leaf_processor import ContainerBlockLeafProcessor
 from pymarkdown.container_block_processor import ContainerBlockProcessor
 from pymarkdown.container_markdown_token import (
     BlockQuoteMarkdownToken,
     ListStartMarkdownToken,
 )
 from pymarkdown.extension_manager.extension_manager import ExtensionManager
 from pymarkdown.extensions.front_matter_extension import FrontMatterExtension
 from pymarkdown.extensions.pragma_token import PragmaToken
 from pymarkdown.html_helper import HtmlHelper
 from pymarkdown.inline_helper import InlineHelper
 from pymarkdown.inline_processor import InlineProcessor
+from pymarkdown.leaf_block_processor import LeafBlockProcessor
 from pymarkdown.leaf_block_processor_paragraph import LeafBlockProcessorParagraph
 from pymarkdown.leaf_markdown_token import BlankLineMarkdownToken
 from pymarkdown.link_helper import LinkHelper
 from pymarkdown.link_reference_definition_helper import LinkReferenceDefinitionHelper
 from pymarkdown.markdown_token import MarkdownToken
 from pymarkdown.parse_block_pass_properties import ParseBlockPassProperties
 from pymarkdown.parser_helper import ParserHelper
@@ -154,84 +154,126 @@
                 did_start_close,
                 did_started_close,
                 keep_on_going,
                 ignore_link_definition_start,
             ) = (first_line_in_document is None, False, True, False)
             next_line_in_document = first_line_in_document
             while keep_on_going:
-                POGGER.debug("next-line>>$", next_line_in_document)
-                POGGER.debug("stack>>$", self.__token_stack)
-                POGGER.debug("current_block>>$", self.__token_stack[-1])
-                POGGER.debug("line_number>>$", line_number)
-                POGGER.debug("---")
-
-                parser_state = ParserState(
-                    self.__token_stack,
-                    self.__tokenized_document,
-                    TokenizedMarkdown.__close_open_blocks,
-                    self.__handle_blank_line,
+                (
+                    keep_on_going,
+                    did_start_close,
+                    did_started_close,
+                    ignore_link_definition_start,
+                    requeue,
+                    line_number,
+                    next_line_in_document,
+                ) = self.__parse_blocks_pass_next_line(
+                    next_line_in_document,
+                    line_number,
+                    requeue,
+                    did_start_close,
+                    did_started_close,
+                    ignore_link_definition_start,
                 )
-                if did_start_close:
-                    (
-                        did_started_close,
-                        did_start_close,
-                        tokens_from_line,
-                        line_number,
-                        keep_on_going,
-                        requeue_line_info,
-                    ) = self.__main_pass_did_start_close(parser_state, line_number)
-                else:
-                    assert next_line_in_document is not None
-                    position_marker = PositionMarker(
-                        line_number, 0, next_line_in_document
-                    )
-                    (
-                        tokens_from_line,
-                        requeue_line_info,
-                    ) = self.__main_pass_did_not_start_close(
-                        parser_state,
-                        position_marker,
-                        next_line_in_document,
-                        ignore_link_definition_start,
-                    )
-
-                if keep_on_going:
-                    (
-                        line_number,
-                        ignore_link_definition_start,
-                        next_line_in_document,
-                        did_start_close,
-                        did_started_close,
-                    ) = self.__main_pass_keep_on_going(
-                        line_number,
-                        requeue_line_info,
-                        requeue,
-                        tokens_from_line,
-                        did_start_close,
-                        did_started_close,
-                    )
         except AssertionError as this_exception:
             error_message = f"A project assertion failed on line {line_number} of the current document."
             raise BadTokenizationError(error_message) from this_exception
 
         if self.__parse_properties.pragma_lines:
             self.__tokenized_document.append(
                 PragmaToken(self.__parse_properties.pragma_lines)
             )
         return self.__tokenized_document
 
+    # pylint: disable=too-many-arguments
+    def __parse_blocks_pass_next_line(
+        self,
+        next_line_in_document: Optional[str],
+        line_number: int,
+        requeue: List[str],
+        did_start_close: bool,
+        did_started_close: bool,
+        ignore_link_definition_start: bool,
+    ) -> Tuple[bool, bool, bool, bool, List[str], int, Optional[str]]:
+        POGGER.debug("next-line>>$", next_line_in_document)
+        POGGER.debug("stack>>$", self.__token_stack)
+        POGGER.debug("current_block>>$", self.__token_stack[-1])
+        POGGER.debug("line_number>>$", line_number)
+        POGGER.debug("---")
+
+        parser_state = ParserState(
+            self.__token_stack,
+            self.__tokenized_document,
+            TokenizedMarkdown.__close_open_blocks,
+            self.__handle_blank_line,
+        )
+        keep_on_going = True
+        if did_start_close:
+            (
+                did_started_close,
+                did_start_close,
+                tokens_from_line,
+                line_number,
+                keep_on_going,
+                requeue_line_info,
+            ) = self.__main_pass_did_start_close(parser_state, line_number)
+        else:
+            assert next_line_in_document is not None
+            position_marker = PositionMarker(line_number, 0, next_line_in_document)
+            (
+                tfl,
+                requeue_line_info,
+            ) = self.__main_pass_did_not_start_close(
+                parser_state,
+                position_marker,
+                next_line_in_document,
+                ignore_link_definition_start,
+            )
+            assert tfl is not None
+            tokens_from_line = tfl
+
+        if keep_on_going:
+            (
+                line_number,
+                ignore_link_definition_start,
+                next_line_in_document,
+                did_start_close,
+                did_started_close,
+            ) = self.__main_pass_keep_on_going(
+                line_number,
+                requeue_line_info,
+                requeue,
+                tokens_from_line,
+                did_start_close,
+                did_started_close,
+            )
+        return (
+            keep_on_going,
+            did_start_close,
+            did_started_close,
+            ignore_link_definition_start,
+            requeue,
+            line_number,
+            next_line_in_document,
+        )
+
+    # pylint: enable=too-many-arguments
+
     def __main_pass_did_start_close(
         self, parser_state: ParserState, line_number: int
     ) -> Tuple[bool, bool, List[MarkdownToken], int, bool, Optional[RequeueLineInfo]]:
         POGGER.debug("\n\ncleanup")
 
         was_link_definition_started_before_close = self.__token_stack[
             -1
         ].was_link_definition_started
-        (tokens_from_line, requeue_line_info,) = TokenizedMarkdown.__close_open_blocks(
+        (
+            tokens_from_line,
+            requeue_line_info,
+        ) = TokenizedMarkdown.__close_open_blocks(
             parser_state,
             self.__tokenized_document,
             include_block_quotes=True,
             include_lists=True,
             caller_can_handle_requeue=True,
             was_forced=True,
         )
@@ -260,20 +302,23 @@
 
     def __main_pass_did_not_start_close(
         self,
         parser_state: ParserState,
         position_marker: PositionMarker,
         next_line_in_document: str,
         ignore_link_definition_start: bool,
-    ) -> Tuple[List[MarkdownToken], Optional[RequeueLineInfo]]:
+    ) -> Tuple[Optional[List[MarkdownToken]], Optional[RequeueLineInfo]]:
         POGGER.debug(">>>>$", self.__tokenized_document)
 
         if not next_line_in_document or not next_line_in_document.strip():
             POGGER.debug("call __parse_blocks_pass>>handle_blank_line")
-            (tokens_from_line, requeue_line_info,) = self.__handle_blank_line(
+            (
+                tokens_from_line,
+                requeue_line_info,
+            ) = self.__handle_blank_line(
                 parser_state,
                 next_line_in_document,
                 from_main_transform=True,
                 position_marker=position_marker,
             )
         else:
             POGGER.debug("\n\nnormal lines")
@@ -303,15 +348,14 @@
         line_number: int,
         requeue_line_info: Optional[RequeueLineInfo],
         requeue: List[str],
         tokens_from_line: List[MarkdownToken],
         did_start_close: bool,
         did_started_close: bool,
     ) -> Tuple[int, bool, Optional[str], bool, bool]:
-
         (
             line_number,
             ignore_link_definition_start,
         ) = TokenizedMarkdown.__handle_parse_increment_line(
             line_number, requeue_line_info, requeue
         )
 
@@ -348,15 +392,14 @@
 
     @staticmethod
     def __handle_parse_increment_line(
         line_number: int,
         requeue_line_info: Optional[RequeueLineInfo],
         requeue: List[str],
     ) -> Tuple[int, bool]:
-
         if requeue_line_info:
             number_of_lines_to_requeue = len(requeue_line_info.lines_to_requeue)
             POGGER.debug("\n\n---lines_to_requeue>>$", number_of_lines_to_requeue)
             line_number -= number_of_lines_to_requeue - 1
 
             for i in requeue_line_info.lines_to_requeue:
                 requeue.insert(0, i)
@@ -441,15 +484,14 @@
             include_block_quotes,
             include_lists,
             until_this_index,
             caller_can_handle_requeue,
             was_forced,
         )
         while not parser_state.token_stack[-1].is_document:
-
             was_close_forced = was_forced
 
             (
                 can_continue,
                 adjusted_tokens,
                 requeue_line_info,
                 was_close_forced,
@@ -509,26 +551,27 @@
         was_close_forced: bool,
         caller_can_handle_requeue: bool,
         until_this_index: int,
         include_lists: bool,
         include_block_quotes: bool,
         only_these_blocks: Optional[List[type]],
     ) -> Tuple[bool, List[MarkdownToken], Optional[RequeueLineInfo], bool]:
-
         requeue_line_info = None
 
         POGGER.debug("cob>>$", parser_state.token_stack)
         can_continue, was_close_forced = TokenizedMarkdown.__can_close_continue(
             parser_state,
             only_these_blocks,
             include_block_quotes,
             include_lists,
             until_this_index,
             was_close_forced,
         )
+        POGGER.debug("can_continue>>$", can_continue)
+        POGGER.debug("was_close_forced>>$", was_close_forced)
         if can_continue:
             if parser_state.token_stack[-1].was_link_definition_started:
                 (
                     can_continue,
                     adjusted_tokens,
                     requeue_line_info,
                 ) = TokenizedMarkdown.__close_open_blocks_lrd(
@@ -575,14 +618,16 @@
                 token_stack_size,
             )
             if until_this_index >= token_stack_size:
                 can_continue = False
             else:
                 was_close_forced = True
 
+        POGGER.debug("cob>>can_continue=$", can_continue)
+        POGGER.debug("cob>>was_close_forced=$", was_close_forced)
         return can_continue, was_close_forced
 
     # pylint: enable=too-many-arguments
 
     @staticmethod
     def __close_open_blocks_normal(
         parser_state: ParserState, was_close_forced: bool
@@ -610,15 +655,15 @@
         (
             outer_processed,
             did_complete_lrd,
             did_pause_lrd,
             requeue_line_info,
             adjusted_tokens,
         ) = LinkReferenceDefinitionHelper.process_link_reference_definition(
-            parser_state, empty_position_marker, "", "", "", 0, 0
+            parser_state, empty_position_marker, "", "", "", 0, 0, "", 1
         )
 
         POGGER.debug("BOOOM: caller_can_handle_requeue=$", caller_can_handle_requeue)
         can_continue = not (
             caller_can_handle_requeue
             and requeue_line_info
             and requeue_line_info.lines_to_requeue
@@ -653,15 +698,15 @@
 
         POGGER.debug("cob->top_element->$", parser_state.token_stack[-1])
         POGGER.debug("cob->was_forced->$", was_forced)
         extra_elements = []
         extra_end_data = None
         if parser_state.token_stack[-1].is_indented_code_block:
             extra_elements.extend(
-                ContainerBlockLeafProcessor.extract_markdown_tokens_back_to_blank_line(
+                LeafBlockProcessor.extract_markdown_tokens_back_to_blank_line(
                     parser_state, was_forced
                 )
             )
         elif parser_state.token_stack[-1].is_fenced_code_block:
             extra_end_data = ":"
 
         new_tokens = [
@@ -695,22 +740,21 @@
         return (
             close_only_these_blocks,
             do_include_block_quotes,
             non_whitespace_index,
             extracted_whitespace,
         )
 
-    # pylint: disable=too-many-locals
     @staticmethod
     def __handle_blank_line(
         parser_state: ParserState,
         input_line: str,
         from_main_transform: bool,
         position_marker: Optional[PositionMarker] = None,
-    ) -> Tuple[List[MarkdownToken], Optional[RequeueLineInfo]]:
+    ) -> Tuple[Optional[List[MarkdownToken]], Optional[RequeueLineInfo]]:
         """
         Handle the processing of a blank line.
         """
 
         (
             close_only_these_blocks,
             do_include_block_quotes,
@@ -720,14 +764,17 @@
 
         (
             new_tokens,
             force_default_handling,
             requeue_line_info,
         ) = TokenizedMarkdown.__handle_blank_line_token_stack(parser_state)
 
+        if requeue_line_info:
+            return new_tokens, requeue_line_info
+
         if from_main_transform:
             POGGER.debug("hbl>>__handle_blank_line_in_block_quote")
             TokenizedMarkdown.__handle_blank_line_in_block_quote(
                 parser_state, new_tokens
             )
 
         if force_default_handling or new_tokens is None:
@@ -754,24 +801,20 @@
             )
             POGGER.debug("hbl>>last_block_token>>$", list_token)
             list_token.add_leading_spaces("")
             POGGER.debug("hbl>>last_block_token>>$", list_token)
 
         POGGER.debug("hbl>>new_tokens>>$", new_tokens)
         assert non_whitespace_index == len(input_line)
-        if not (requeue_line_info and requeue_line_info.force_ignore_first_as_lrd):
-            new_tokens.append(
-                BlankLineMarkdownToken(extracted_whitespace, position_marker)
-            )
+        assert not (requeue_line_info and requeue_line_info.force_ignore_first_as_lrd)
+        new_tokens.append(BlankLineMarkdownToken(extracted_whitespace, position_marker))
         POGGER.debug("hbl>>new_tokens>>$", new_tokens)
 
         return new_tokens, requeue_line_info
 
-    # pylint: enable=too-many-locals
-
     @staticmethod
     def __handle_blank_line_token_stack(
         parser_state: ParserState,
     ) -> Tuple[Optional[List[MarkdownToken]], bool, Optional[RequeueLineInfo]]:
         (
             is_processing_list,
             in_index,
@@ -796,15 +839,15 @@
             (
                 _,
                 _,
                 did_pause_lrd,
                 requeue_line_info,
                 new_tokens,
             ) = LinkReferenceDefinitionHelper.process_link_reference_definition(
-                parser_state, empty_position_marker, "", "", "", 0, 0
+                parser_state, empty_position_marker, "", "", "", 0, 0, "", 2
             )
             assert not did_pause_lrd
             POGGER.debug(
                 "hbl<<process_link_reference_definition>>stopping link definition"
             )
         elif parser_state.token_stack[-1].is_code_block:
             if parser_state.count_of_block_quotes_on_stack():
@@ -828,23 +871,23 @@
             POGGER.debug("hbl<<double blank in list")
         return new_tokens, force_default_handling, requeue_line_info
 
     @staticmethod
     def __handle_blank_line_in_block_quote(
         parser_state: ParserState, new_tokens: Optional[List[MarkdownToken]]
     ) -> None:
-
         stack_index = parser_state.find_last_container_on_stack()
         POGGER.debug_with_visible_whitespace("new_tokens>>$", new_tokens)
         POGGER.debug("stack_index>>$", stack_index)
         if new_tokens and stack_index > 0:
             POGGER.debug_with_visible_whitespace("new_tokens[-1]>>$", new_tokens[-1])
-            assert new_tokens[-1].is_html_block_end and stack_index == (
-                len(parser_state.token_stack) - 1
-            )
+            assert (
+                new_tokens[-1].is_html_block_end
+                or new_tokens[-1].is_link_reference_definition
+            ) and stack_index == (len(parser_state.token_stack) - 1)
             close_tokens, _ = parser_state.close_open_blocks_fn(
                 parser_state,
                 only_these_blocks=[BlockQuoteStackToken],
                 include_block_quotes=True,
             )
             POGGER.debug("close_tokens>>$", close_tokens)
             new_tokens.extend(close_tokens)
@@ -859,15 +902,15 @@
                 BlockQuoteMarkdownToken,
                 parser_state.token_stack[stack_index].matching_markdown_token,
             )
             POGGER.debug("hblibq>>last_block_token>>$", block_quote_token)
             POGGER.debug(
                 "hblibq>>leading_text_index>>$", block_quote_token.leading_text_index
             )
-            block_quote_token.add_leading_spaces("")
+            block_quote_token.add_bleading_spaces("")
             POGGER.debug("hblibq>>last_block_token>>$", block_quote_token)
             POGGER.debug(
                 "hblibq>>leading_text_index>>$", block_quote_token.leading_text_index
             )
 
     def __process_front_matter_header_if_present(
         self,
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/transform_state.py` & `pymarkdownlnt-0.9.9/pymarkdown/transform_state.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/transform_to_gfm.py` & `pymarkdownlnt-0.9.9/pymarkdown/transform_to_gfm.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,23 +183,32 @@
             token_type, MarkdownToken
         ), f"Token class '{token_type}' must be descended from the 'MarkdownToken' class."
 
         # This is being done to create a rough "default" instance of the type in
         # question.  Because it is a rough creation and we have no intentions of
         # using it, each parameter is an empty string.  Therefore, we expect that
         # mypy will have issues when we create the instance, hence ignoring them.
-        token_init_fn = token_type.__dict__["__init__"]
-        init_parameters = {
-            i: "" for i in inspect.getfullargspec(token_init_fn)[0] if i != "self"
-        }
-        handler_instance = token_type(**init_parameters)  # type: ignore
+        #
+        # That was the old way, and had problems.  The new way is to call a new
+        # static method directly.  Both are here until that is completed.
 
-        self.start_token_handlers[handler_instance.token_name] = start_token_handler
+        if "get_markdown_token_type" in token_type.__dict__:
+            token_name = token_type.__dict__["get_markdown_token_type"].__func__()
+        else:
+            token_init_fn = token_type.__dict__["__init__"]
+            init_parameters = {
+                i: "" for i in inspect.getfullargspec(token_init_fn)[0] if i != "self"
+            }
+            handler_instance = token_type(**init_parameters)  # type: ignore
+            token_name = handler_instance.token_name
+
+        assert token_name
+        self.start_token_handlers[token_name] = start_token_handler
         if end_token_handler:
-            self.end_token_handlers[handler_instance.token_name] = end_token_handler
+            self.end_token_handlers[token_name] = end_token_handler
 
     def transform(self, actual_tokens: List[MarkdownToken]) -> str:
         """
         Transform the tokens into html.
         """
         POGGER.debug("\n\n---\n")
         transform_state, output_html, actual_tokens_size = (
@@ -209,15 +218,14 @@
         )
 
         # This is the easiest way to finish covering the missing items.
         assert transform_state.next_token is None
         assert not transform_state.is_in_fenced_code_block
 
         for next_token in transform_state.actual_tokens:
-
             output_html = self.__apply_transformation(
                 transform_state,
                 actual_tokens,
                 actual_tokens_size,
                 next_token,
                 output_html,
             )
@@ -228,17 +236,19 @@
                 transform_state.add_trailing_text,
             )
             POGGER.debug("add_leading_text -->$<--", transform_state.add_leading_text)
             POGGER.debug("output_html    -->$<--", output_html)
 
             if transform_state.add_trailing_text:
                 output_html = self.__apply_trailing_text(output_html, transform_state)
+                POGGER.debug("output_html    -->$<--", output_html)
 
             if transform_state.add_leading_text:
                 output_html = self.__apply_leading_text(output_html, transform_state)
+                POGGER.debug("output_html    -->$<--", output_html)
 
             POGGER.debug("------")
             POGGER.debug("next_token     -->$<--", next_token)
             POGGER.debug("output_html    -->$<--", output_html)
             POGGER.debug("transform_stack-->$<--", transform_state.transform_stack)
 
             transform_state.last_token = next_token
@@ -263,25 +273,30 @@
 
         if (transform_state.actual_token_index + 1) < actual_tokens_size:
             transform_state.next_token = actual_tokens[
                 transform_state.actual_token_index + 1
             ]
         if next_token.token_name in self.start_token_handlers:
             start_handler_fn = self.start_token_handlers[next_token.token_name]
+            POGGER.debug("next_token>:$:<", next_token)
+            POGGER.debug("output_html>:$:<", output_html)
             output_html = start_handler_fn(output_html, next_token, transform_state)
+            POGGER.debug("output_html>:$:<", output_html)
 
         elif next_token.is_end_token:
             end_token = cast(EndMarkdownToken, next_token)
-            if end_token.type_name in self.end_token_handlers:
-                end_handler_fn = self.end_token_handlers[end_token.type_name]
-                output_html = end_handler_fn(output_html, end_token, transform_state)
-            else:
+            if end_token.type_name not in self.end_token_handlers:
                 raise AssertionError(
                     f"Markdown token end type {end_token.type_name} not supported."
                 )
+            end_handler_fn = self.end_token_handlers[end_token.type_name]
+            POGGER.debug("end_token>:$:<", end_token)
+            POGGER.debug("output_html>:$:<", output_html)
+            output_html = end_handler_fn(output_html, end_token, transform_state)
+            POGGER.debug("output_html>:$:<", output_html)
         else:
             raise AssertionError(
                 f"Markdown token type {type(next_token)} not supported."
             )
         return output_html
 
     # pylint: enable=too-many-arguments
@@ -343,24 +358,43 @@
         Handle the text token.
         """
         text_token = cast(TextMarkdownToken, next_token)
         adjusted_text_token = ParserHelper.resolve_all_from_text(text_token.token_text)
 
         token_parts: List[str] = []
         if transform_state.is_in_code_block:
+            POGGER.debug(
+                "text_token.extracted_whitespace>:$:<", text_token.extracted_whitespace
+            )
+            leading_space = ParserHelper.resolve_all_from_text(
+                text_token.extracted_whitespace
+            )
+
+            POGGER.debug("leading_space>:$:<", leading_space)
+            POGGER.debug("adjusted_text_token>:$:<", adjusted_text_token)
             token_parts.extend(
                 [
-                    ParserHelper.resolve_all_from_text(text_token.extracted_whitespace),
+                    leading_space,
                     adjusted_text_token,
                 ]
             )
         elif transform_state.is_in_html_block:
+            POGGER.debug(
+                "text_token.extracted_whitespace>:$:<", text_token.extracted_whitespace
+            )
+            leading_space = ParserHelper.resolve_all_from_text(
+                text_token.extracted_whitespace
+            )
+
+            POGGER.debug("leading_space>:$:<", leading_space)
+            POGGER.debug("adjusted_text_token>:$:<", adjusted_text_token)
+            POGGER.debug("newline_character>:$:<", ParserHelper.newline_character)
             token_parts.extend(
                 [
-                    text_token.extracted_whitespace,
+                    leading_space,
                     adjusted_text_token,
                     ParserHelper.newline_character,
                 ]
             )
         elif transform_state.is_in_setext_block:
             token_parts.append(adjusted_text_token)
         else:
@@ -375,15 +409,14 @@
         token_parts: List[str],
         text_token: TextMarkdownToken,
         adjusted_text_token: str,
     ) -> None:
         POGGER.debug("adjusted_text_token>:$:<", adjusted_text_token)
         POGGER.debug("text_token.end_whitespace>:$:<", text_token.end_whitespace)
         if text_token.end_whitespace is not None:
-
             newlines_in_adjusted = ParserHelper.count_newlines_in_text(
                 adjusted_text_token
             )
 
             resolved_whitespace = ParserHelper.resolve_all_from_text(
                 text_token.end_whitespace
             )
@@ -753,17 +786,17 @@
 
         atx_token = cast(AtxHeadingMarkdownToken, next_token)
         previous_token = transform_state.actual_tokens[
             transform_state.actual_token_index - 1
         ]
 
         token_parts = [output_html]
-        if output_html.endswith("</ol>") or output_html.endswith("</ul>"):
-            token_parts.append(ParserHelper.newline_character)
-        elif previous_token.is_paragraph_end and not transform_state.is_in_loose_list:
+        if (output_html.endswith("</ol>") or output_html.endswith("</ul>")) or (
+            previous_token.is_paragraph_end and not transform_state.is_in_loose_list
+        ):
             token_parts.append(ParserHelper.newline_character)
         token_parts.extend(["<h", str(atx_token.hash_count), ">"])
         return "".join(token_parts)
 
     @classmethod
     def __handle_end_atx_heading_token(
         cls,
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdown/transform_to_gfm_list_looseness.py` & `pymarkdownlnt-0.9.9/pymarkdown/transform_to_gfm_list_looseness.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
             (
                 stop_me,
                 is_loose,
                 stack_count,
             ) = TransformToGfmListLooseness.__handle_list_end(
                 stack_count,
                 is_loose,
-                stop_me,
                 actual_tokens,
                 current_token_index,
             )
             POGGER.debug("cll>>stop_me>>$", stop_me)
             POGGER.debug("cll>>is_loose>>$", is_loose)
         elif actual_tokens[current_token_index - 1].is_blank_line:
             POGGER.debug("cll>>__handle_blank_line>>")
@@ -139,15 +138,14 @@
         POGGER.debug(">>list--item>>$", stack_count)
         return stack_count == 0
 
     @staticmethod
     def __handle_list_end(
         stack_count: int,
         is_loose: bool,
-        stop_me: bool,
         actual_tokens: List[MarkdownToken],
         current_token_index: int,
     ) -> Tuple[bool, bool, int]:
         POGGER.debug(">>list--end>>$", stack_count)
         stop_me = not stack_count
         if not stop_me:
             stack_count -= 1
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/PKG-INFO` & `pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymarkdownlnt
-Version: 0.9.8
+Version: 0.9.9
 Summary: A GitHub Flavored Markdown compliant Markdown linter.
 Home-page: https://github.com/jackdewinter/pymarkdown
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/pymarkdown/blob/main/changelog.md
```

### Comparing `pymarkdownlnt-0.9.8/pymarkdownlnt.egg-info/SOURCES.txt` & `pymarkdownlnt-0.9.9/pymarkdownlnt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,49 +2,55 @@
 MANIFEST.in
 README.md
 install-requirements.txt
 setup.cfg
 setup.py
 pymarkdown/__init__.py
 pymarkdown/__main__.py
+pymarkdown/application_file_scanner.py
+pymarkdown/application_logging.py
 pymarkdown/bad_tokenization_error.py
 pymarkdown/block_quote_data.py
 pymarkdown/block_quote_processor.py
 pymarkdown/coalesce_processor.py
 pymarkdown/constants.py
 pymarkdown/container_block_leaf_processor.py
 pymarkdown/container_block_processor.py
 pymarkdown/container_grab_bag.py
+pymarkdown/container_helper.py
 pymarkdown/container_indices.py
 pymarkdown/container_markdown_token.py
 pymarkdown/emphasis_helper.py
 pymarkdown/html_helper.py
 pymarkdown/inline_helper.py
 pymarkdown/inline_markdown_token.py
 pymarkdown/inline_processor.py
 pymarkdown/inline_request.py
 pymarkdown/inline_response.py
 pymarkdown/leaf_block_processor.py
 pymarkdown/leaf_block_processor_paragraph.py
 pymarkdown/leaf_markdown_token.py
 pymarkdown/link_helper.py
+pymarkdown/link_helper_properties.py
 pymarkdown/link_reference_definition_helper.py
 pymarkdown/link_reference_info.py
 pymarkdown/link_reference_titles.py
 pymarkdown/list_block_processor.py
 pymarkdown/main.py
+pymarkdown/main_presentation.py
 pymarkdown/markdown_token.py
 pymarkdown/parse_block_pass_properties.py
 pymarkdown/parser_helper.py
 pymarkdown/parser_logger.py
 pymarkdown/parser_state.py
 pymarkdown/position_marker.py
 pymarkdown/requeue_line_info.py
 pymarkdown/source_providers.py
 pymarkdown/stack_token.py
+pymarkdown/tab_helper.py
 pymarkdown/tokenized_markdown.py
 pymarkdown/transform_state.py
 pymarkdown/transform_to_gfm.py
 pymarkdown/transform_to_gfm_list_looseness.py
 pymarkdown/version.py
 pymarkdown/extension_manager/__init__.py
 pymarkdown/extension_manager/extension_impl.py
@@ -118,13 +124,14 @@
 pymarkdown/resources/entities.json
 pymarkdownlnt.egg-info/PKG-INFO
 pymarkdownlnt.egg-info/SOURCES.txt
 pymarkdownlnt.egg-info/dependency_links.txt
 pymarkdownlnt.egg-info/entry_points.txt
 pymarkdownlnt.egg-info/requires.txt
 pymarkdownlnt.egg-info/top_level.txt
+test/test_application_file_scanner.py
 test/test_listfiles.py
 test/test_main.py
 test/test_markdown_extra.py
 test/test_markdown_transform_to_gfm.py
 test/test_perf.py
 test/test_transform_markdown.py
```

### Comparing `pymarkdownlnt-0.9.8/setup.py` & `pymarkdownlnt-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/test/test_listfiles.py` & `pymarkdownlnt-0.9.9/test/test_listfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     expected_output = """usage: main.py scan [-h] [-l] [-r] [-ae ALTERNATE_EXTENSIONS] path [path ...]
 
 positional arguments:
   path                  one or more paths to scan for eligible Markdown files
 
 optional arguments:
   -h, --help            show this help message and exit
-  -l, --list-files      list the markdown files found and exit
-  -r, --recurse         recursively scan directories
+  -l, --list-files      list the eligible Markdown files and exit
+  -r, --recurse         recursively scan directories for files
   -ae ALTERNATE_EXTENSIONS, --alternate-extensions ALTERNATE_EXTENSIONS
-                        provider an alternate set of file extensions to scan
+                        provide an alternate set of file extensions to scan
+                        for
 """
     expected_error = ""
 
     # Act
     execute_results = scanner.invoke_main(arguments=supplied_arguments)
 
     # Assert
@@ -70,15 +71,15 @@
     # Arrange
     scanner = MarkdownScanner()
     supplied_arguments = ["scan", "-l", "my-bad-path"]
 
     expected_return_code = 1
     expected_output = ""
     expected_error = """Provided path 'my-bad-path' does not exist.
-"""
+No matching files found."""
 
     # Act
     execute_results = scanner.invoke_main(
         arguments=supplied_arguments, cwd=scanner.resource_directory
     )
 
     # Assert
@@ -179,15 +180,15 @@
     scanner = MarkdownScanner()
     source_path = os.path.join("only-text", "simple_text_file.txt")
     supplied_arguments = ["scan", "-l", source_path]
 
     expected_return_code = 1
     expected_output = ""
     expected_error = """Provided file path '{source_path}' is not a valid file. Skipping.
-""".replace(
+No matching files found.""".replace(
         "{source_path}", source_path
     )
 
     # Act
     execute_results = scanner.invoke_main(
         arguments=supplied_arguments, cwd=scanner.resource_directory
     )
@@ -243,15 +244,15 @@
         nonexisting_source_path,
         existing_source_path,
     ]
 
     expected_return_code = 1
     expected_output = """"""
     expected_error = """Provided file path '{nonexisting_source_path}' is not a valid file. Skipping.
-""".replace(
+No matching files found.""".replace(
         "{nonexisting_source_path}", nonexisting_source_path
     )
 
     # Act
     execute_results = scanner.invoke_main(
         arguments=supplied_arguments, cwd=scanner.resource_directory
     )
@@ -306,15 +307,15 @@
     # Arrange
     scanner = MarkdownScanner()
     source_path = os.path.join("rules", "md001", "z*.md")
     supplied_arguments = ["scan", "-l", source_path]
 
     expected_return_code = 1
     expected_output = """"""
-    expected_error = f"Provided glob path '{source_path}' did not match any files."
+    expected_error = f"Provided glob path '{source_path}' did not match any files.\nNo matching files found."
 
     # Act
     execute_results = scanner.invoke_main(
         arguments=supplied_arguments, cwd=scanner.resource_directory
     )
 
     # Assert
```

### Comparing `pymarkdownlnt-0.9.8/test/test_main.py` & `pymarkdownlnt-0.9.9/test/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 Lint any found Markdown files.
 
 positional arguments:
   {plugins,extensions,scan,scan-stdin,version}
     plugins             plugin commands
     extensions          extension commands
     scan                scan the Markdown files in the specified paths
-    scan-stdin          scan the standard input as a Markdown files
+    scan-stdin          scan the standard input as a Markdown file
     version             version of the application
 
 optional arguments:
   -h, --help            show this help message and exit
   -e ENABLE_RULES, --enable-rules ENABLE_RULES
                         comma separated list of rules to enable
   -d DISABLE_RULES, --disable-rules DISABLE_RULES
@@ -97,15 +97,15 @@
 Lint any found Markdown files.
 
 positional arguments:
   {plugins,extensions,scan,scan-stdin,version}
     plugins             plugin commands
     extensions          extension commands
     scan                scan the Markdown files in the specified paths
-    scan-stdin          scan the standard input as a Markdown files
+    scan-stdin          scan the standard input as a Markdown file
     version             version of the application
 
 optional arguments:
   -h, --help            show this help message and exit
   -e ENABLE_RULES, --enable-rules ENABLE_RULES
                         comma separated list of rules to enable
   -d DISABLE_RULES, --disable-rules DISABLE_RULES
@@ -156,15 +156,15 @@
 Lint any found Markdown files.
 
 positional arguments:
   {plugins,extensions,scan,scan-stdin,version}
     plugins             plugin commands
     extensions          extension commands
     scan                scan the Markdown files in the specified paths
-    scan-stdin          scan the standard input as a Markdown files
+    scan-stdin          scan the standard input as a Markdown file
     version             version of the application
 
 optional arguments:
   -h, --help            show this help message and exit
   -e ENABLE_RULES, --enable-rules ENABLE_RULES
                         comma separated list of rules to enable
   -d DISABLE_RULES, --disable-rules DISABLE_RULES
@@ -214,15 +214,15 @@
 Lint any found Markdown files.
 
 positional arguments:
   {plugins,extensions,scan,scan-stdin,version}
     plugins             plugin commands
     extensions          extension commands
     scan                scan the Markdown files in the specified paths
-    scan-stdin          scan the standard input as a Markdown files
+    scan-stdin          scan the standard input as a Markdown file
     version             version of the application
 
 optional arguments:
   -h, --help            show this help message and exit
   -e ENABLE_RULES, --enable-rules ENABLE_RULES
                         comma separated list of rules to enable
   -d DISABLE_RULES, --disable-rules DISABLE_RULES
@@ -277,14 +277,66 @@
 
     # Assert
     execute_results.assert_results(
         expected_output, expected_error, expected_return_code
     )
 
 
+def test_markdown_with_direct_args(caplog):
+    """
+    Test to make sure we can specify the arguments directly.
+    """
+
+    # Arrange
+    scanner = MarkdownScanner(use_main=False)
+    supplied_arguments = ["--log-level", "DEBUG", "scan", "does-not-exist.md"]
+
+    expected_return_code = 1
+    expected_output = ""
+    expected_error = "Provided path 'does-not-exist.md' does not exist."
+
+    # Act
+    execute_results = scanner.invoke_main(
+        arguments=supplied_arguments, use_direct_arguments=True
+    )
+
+    # Assert
+    execute_results.assert_results(
+        expected_output, expected_error, expected_return_code
+    )
+
+    assert "Using direct arguments: [" in caplog.text
+
+
+def test_markdown_without_direct_args(caplog):
+    """
+    Test to make sure we can specify the arguments normally.
+    """
+
+    # Arrange
+    scanner = MarkdownScanner(use_main=False)
+    supplied_arguments = ["--log-level", "DEBUG", "scan", "does-not-exist.md"]
+
+    expected_return_code = 1
+    expected_output = ""
+    expected_error = "Provided path 'does-not-exist.md' does not exist."
+
+    # Act
+    execute_results = scanner.invoke_main(
+        arguments=supplied_arguments, use_direct_arguments=False
+    )
+
+    # Assert
+    execute_results.assert_results(
+        expected_output, expected_error, expected_return_code
+    )
+
+    assert "Using supplied command line arguments." in caplog.text
+
+
 def test_markdown_with_dash_e_single_by_name():
     """
     Test to make sure we get enable a rule if '-e' is supplied and the name of the
     rule is provided. The test data for MD047 is used as it is a simple file that
     passes normally, it is used as a comparison.
     """
 
@@ -731,15 +783,15 @@
     expected_output = ""
     expected_error = """usage: main.py [-h] [-e ENABLE_RULES] [-d DISABLE_RULES]
                [--add-plugin ADD_PLUGIN] [--config CONFIGURATION_FILE]
                [--set SET_CONFIGURATION] [--strict-config] [--stack-trace]
                [--log-level {CRITICAL,ERROR,WARNING,INFO,DEBUG}]
                [--log-file LOG_FILE]
                {plugins,extensions,scan,scan-stdin,version} ...
-main.py: error: argument --log-level: invalid log_level_type value: 'invalid'
+main.py: error: argument --log-level: invalid __log_level_type value: 'invalid'
 """
 
     # Act
     ParserLogger.sync_on_next_call()
     execute_results = scanner.invoke_main(arguments=supplied_arguments)
 
     # Assert
@@ -1565,39 +1617,39 @@
     source_path = os.path.join(
         "test",
         "resources",
         "rules",
         "md020",
         "single_paragraph_with_whitespace_at_end.md",
     )
+    expected_return_code = 1
     supplied_arguments = [
         "scan",
         source_path,
     ]
 
-    expected_return_code = 1
     expected_output = (
-        f"{source_path}:1:1: "
-        + "MD022: Headings should be surrounded by blank lines. "
+        f"{source_path}:1:1: MD022: Headings should be surrounded by blank lines. "
         + "[Expected: 1; Actual: 0; Below] (blanks-around-headings,blanks-around-headers)\n"
         + f"{source_path}:1:12: "
         + "MD010: Hard tabs "
         + "[Column: 12] (no-hard-tabs)\n"
-        + f"{source_path}:2:2: "
-        + "MD021: Multiple spaces are present inside hash characters on Atx Closed Heading. "
-        + "(no-multiple-space-closed-atx)\n"
+        # + f"{source_path}:2:2: "
+        # + "MD021: Multiple spaces are present inside hash characters on Atx Closed Heading. "
+        # + "(no-multiple-space-closed-atx)\n"
         + f"{source_path}:2:2: "
         + "MD022: Headings should be surrounded by blank lines. "
         + "[Expected: 1; Actual: 0; Above] (blanks-around-headings,blanks-around-headers)\n"
         + f"{source_path}:2:2: "
         + "MD023: Headings must start at the beginning of the line. (heading-start-left, header-start-left)\n"
         + f"{source_path}:2:14: "
         + "MD010: Hard tabs "
         + "[Column: 14] (no-hard-tabs)"
     )
+
     expected_error = ""
 
     # Act
     execute_results = scanner.invoke_main(arguments=supplied_arguments)
 
     # Assert
     execute_results.assert_results(
@@ -1871,15 +1923,15 @@
     supplied_standard_input = "test\nme\n"
     expected_return_code = 0
     expected_output = ""
     expected_error = ""
 
     # Act
     execute_results = scanner.invoke_main(
-        arguments=supplied_arguments, xyz=supplied_standard_input
+        arguments=supplied_arguments, standard_input_to_use=supplied_standard_input
     )
 
     # Assert
     execute_results.assert_results(
         expected_output, expected_error, expected_return_code
     )
 
@@ -1899,15 +1951,15 @@
     expected_return_code = 1
     expected_output = """stdin:1:1: MD022: Headings should be surrounded by blank lines. [Expected: 1; Actual: 0; Below] (blanks-around-headings,blanks-around-headers)
 stdin:1:6: MD047: Each file should end with a single newline character. (single-trailing-newline)"""
     expected_error = ""
 
     # Act
     execute_results = scanner.invoke_main(
-        arguments=supplied_arguments, xyz=supplied_standard_input
+        arguments=supplied_arguments, standard_input_to_use=supplied_standard_input
     )
 
     # Assert
     execute_results.assert_results(
         expected_output, expected_error, expected_return_code
     )
 
@@ -1928,14 +1980,14 @@
     expected_return_code = 1
     expected_output = ""
     expected_error = """OSError encountered while scanning 'stdin':
 Temporary file to capture stdin was not written (made up)."""
 
     # Act
     execute_results = scanner.invoke_main(
-        arguments=supplied_arguments, xyz=supplied_standard_input
+        arguments=supplied_arguments, standard_input_to_use=supplied_standard_input
     )
 
     # Assert
     execute_results.assert_results(
         expected_output, expected_error, expected_return_code
     )
```

### Comparing `pymarkdownlnt-0.9.8/test/test_markdown_extra.py` & `pymarkdownlnt-0.9.9/test/test_markdown_extra.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 </code></pre>
 <ol>
 <li>another list</li>
 </ol>
 </blockquote>"""
 
     # Act & Assert
-    act_and_assert(source_markdown, expected_gfm, expected_tokens, show_debug=True)
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
 
 
 @pytest.mark.gfm
 def test_extra_007a():
     """
     Text and a link reference definition within a block quote.
     """
@@ -3778,14 +3778,463 @@
 </ul>"""
 
     # Act & Assert
     act_and_assert(source_markdown, expected_gfm, expected_tokens)
 
 
 @pytest.mark.gfm
+def test_extra_029x():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- abc
+
+  + def"""
+    expected_tokens = [
+        "[ulist(1,1):-::2::]",
+        "[para(1,3):]",
+        "[text(1,3):abc:]",
+        "[end-para:::True]",
+        "[BLANK(2,1):]",
+        "[ulist(3,3):+::4:  ]",
+        "[para(3,5):]",
+        "[text(3,5):def:]",
+        "[end-para:::True]",
+        "[end-ulist:::True]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>
+<p>abc</p>
+<ul>
+<li>def</li>
+</ul>
+</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029a():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- l2:
+  + il2.1
+
+  ip1
+  + il2.2
+- l3
+"""
+    expected_tokens = [
+        "[ulist(1,1):-::2::  \n]",
+        "[para(1,3):]",
+        "[text(1,3):l2::]",
+        "[end-para:::True]",
+        "[ulist(2,3):+::4:  :]",
+        "[para(2,5):]",
+        "[text(2,5):il2.1:]",
+        "[end-para:::True]",
+        "[BLANK(3,1):]",
+        "[end-ulist:::True]",
+        "[para(4,3):]",
+        "[text(4,3):ip1:]",
+        "[end-para:::True]",
+        "[ulist(5,3):+::4:  ]",
+        "[para(5,5):]",
+        "[text(5,5):il2.2:]",
+        "[end-para:::True]",
+        "[end-ulist:::True]",
+        "[li(6,1):2::]",
+        "[para(6,3):]",
+        "[text(6,3):l3:]",
+        "[end-para:::True]",
+        "[BLANK(7,1):]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>
+<p>l2:</p>
+<ul>
+<li>il2.1</li>
+</ul>
+<p>ip1</p>
+<ul>
+<li>il2.2</li>
+</ul>
+</li>
+<li>
+<p>l3</p>
+</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029b():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- l2:
+  - il2.1
+
+  ip1
+  - il2.2
+- l3
+"""
+    expected_tokens = [
+        "[ulist(1,1):-::2::  \n]",
+        "[para(1,3):]",
+        "[text(1,3):l2::]",
+        "[end-para:::True]",
+        "[ulist(2,3):-::4:  :]",
+        "[para(2,5):]",
+        "[text(2,5):il2.1:]",
+        "[end-para:::True]",
+        "[BLANK(3,1):]",
+        "[end-ulist:::True]",
+        "[para(4,3):]",
+        "[text(4,3):ip1:]",
+        "[end-para:::True]",
+        "[ulist(5,3):-::4:  ]",
+        "[para(5,5):]",
+        "[text(5,5):il2.2:]",
+        "[end-para:::True]",
+        "[end-ulist:::True]",
+        "[li(6,1):2::]",
+        "[para(6,3):]",
+        "[text(6,3):l3:]",
+        "[end-para:::True]",
+        "[BLANK(7,1):]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>
+<p>l2:</p>
+<ul>
+<li>il2.1</li>
+</ul>
+<p>ip1</p>
+<ul>
+<li>il2.2</li>
+</ul>
+</li>
+<li>
+<p>l3</p>
+</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029c():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """# atx1
+
+p1
+
+- l1
+
+- l2:
+
+  + il2.1
+
+  ip1
+
+  + il2.2
+
+- l3
+
+p4
+"""
+    expected_tokens = [
+        "[atx(1,1):1:0:]",
+        "[text(1,3):atx1: ]",
+        "[end-atx::]",
+        "[BLANK(2,1):]",
+        "[para(3,1):]",
+        "[text(3,1):p1:]",
+        "[end-para:::True]",
+        "[BLANK(4,1):]",
+        "[ulist(5,1):-::2::\n\n  \n\n]",
+        "[para(5,3):]",
+        "[text(5,3):l1:]",
+        "[end-para:::True]",
+        "[BLANK(6,1):]",
+        "[li(7,1):2::]",
+        "[para(7,3):]",
+        "[text(7,3):l2::]",
+        "[end-para:::True]",
+        "[BLANK(8,1):]",
+        "[ulist(9,3):+::4:  :]",
+        "[para(9,5):]",
+        "[text(9,5):il2.1:]",
+        "[end-para:::True]",
+        "[BLANK(10,1):]",
+        "[end-ulist:::True]",
+        "[para(11,3):]",
+        "[text(11,3):ip1:]",
+        "[end-para:::True]",
+        "[BLANK(12,1):]",
+        "[ulist(13,3):+::4:  :]",
+        "[para(13,5):]",
+        "[text(13,5):il2.2:]",
+        "[end-para:::True]",
+        "[BLANK(14,1):]",
+        "[end-ulist:::True]",
+        "[li(15,1):2::]",
+        "[para(15,3):]",
+        "[text(15,3):l3:]",
+        "[end-para:::True]",
+        "[BLANK(16,1):]",
+        "[end-ulist:::True]",
+        "[para(17,1):]",
+        "[text(17,1):p4:]",
+        "[end-para:::True]",
+        "[BLANK(18,1):]",
+    ]
+    expected_gfm = """<h1>atx1</h1>
+<p>p1</p>
+<ul>
+<li>
+<p>l1</p>
+</li>
+<li>
+<p>l2:</p>
+<ul>
+<li>il2.1</li>
+</ul>
+<p>ip1</p>
+<ul>
+<li>il2.2</li>
+</ul>
+</li>
+<li>
+<p>l3</p>
+</li>
+</ul>
+<p>p4</p>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029d():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- l2:
+  1. il2.1
+
+  ip1
+  1. il2.2
+- l3
+"""
+    expected_tokens = [
+        "[ulist(1,1):-::2::  \n]",
+        "[para(1,3):]",
+        "[text(1,3):l2::]",
+        "[end-para:::True]",
+        "[olist(2,3):.:1:5:  :]",
+        "[para(2,6):]",
+        "[text(2,6):il2.1:]",
+        "[end-para:::True]",
+        "[BLANK(3,1):]",
+        "[end-olist:::True]",
+        "[para(4,3):]",
+        "[text(4,3):ip1:]",
+        "[end-para:::True]",
+        "[olist(5,3):.:1:5:  ]",
+        "[para(5,6):]",
+        "[text(5,6):il2.2:]",
+        "[end-para:::True]",
+        "[end-olist:::True]",
+        "[li(6,1):2::]",
+        "[para(6,3):]",
+        "[text(6,3):l3:]",
+        "[end-para:::True]",
+        "[BLANK(7,1):]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>
+<p>l2:</p>
+<ol>
+<li>il2.1</li>
+</ol>
+<p>ip1</p>
+<ol>
+<li>il2.2</li>
+</ol>
+</li>
+<li>
+<p>l3</p>
+</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029e():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- l1
++ l2
+ """
+    expected_tokens = [
+        "[ulist(1,1):-::2:]",
+        "[para(1,3):]",
+        "[text(1,3):l1:]",
+        "[end-para:::True]",
+        "[end-ulist:::True]",
+        "[ulist(2,1):+::2::]",
+        "[para(2,3):]",
+        "[text(2,3):l2:]",
+        "[end-para:::True]",
+        "[BLANK(3,1): ]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>l1</li>
+</ul>
+<ul>
+<li>l2</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029f():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """- l1
+1. l2
+ """
+    expected_tokens = [
+        "[ulist(1,1):-::2:]",
+        "[para(1,3):]",
+        "[text(1,3):l1:]",
+        "[end-para:::True]",
+        "[end-ulist:::True]",
+        "[olist(2,1):.:1:3::]",
+        "[para(2,4):]",
+        "[text(2,4):l2:]",
+        "[end-para:::True]",
+        "[BLANK(3,1): ]",
+        "[end-olist:::True]",
+    ]
+    expected_gfm = """<ul>
+<li>l1</li>
+</ul>
+<ol>
+<li>l2</li>
+</ol>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029g():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """1. l1
++ l2
+ """
+    expected_tokens = [
+        "[olist(1,1):.:1:3:]",
+        "[para(1,4):]",
+        "[text(1,4):l1:]",
+        "[end-para:::True]",
+        "[end-olist:::True]",
+        "[ulist(2,1):+::2::]",
+        "[para(2,3):]",
+        "[text(2,3):l2:]",
+        "[end-para:::True]",
+        "[BLANK(3,1): ]",
+        "[end-ulist:::True]",
+    ]
+    expected_gfm = """<ol>
+<li>l1</li>
+</ol>
+<ul>
+<li>l2</li>
+</ul>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
+def test_extra_029h():
+    """
+    TBD
+    """
+
+    # Arrange
+    source_markdown = """1. l1
+1) l2
+ """
+    expected_tokens = [
+        "[olist(1,1):.:1:3:]",
+        "[para(1,4):]",
+        "[text(1,4):l1:]",
+        "[end-para:::True]",
+        "[end-olist:::True]",
+        "[olist(2,1):):1:3::]",
+        "[para(2,4):]",
+        "[text(2,4):l2:]",
+        "[end-para:::True]",
+        "[BLANK(3,1): ]",
+        "[end-olist:::True]",
+    ]
+    expected_gfm = """<ol>
+<li>l1</li>
+</ol>
+<ol>
+<li>l2</li>
+</ol>"""
+
+    # Act & Assert
+    act_and_assert(source_markdown, expected_gfm, expected_tokens)
+
+
+@pytest.mark.gfm
 def test_extra_999():
     """
     Temporary test to keep coverage up while consistency checks disabled.
     """
 
     new_position = PositionMarker(1, 0, "text")
```

### Comparing `pymarkdownlnt-0.9.8/test/test_markdown_transform_to_gfm.py` & `pymarkdownlnt-0.9.9/test/test_markdown_transform_to_gfm.py`

 * *Files identical despite different names*

### Comparing `pymarkdownlnt-0.9.8/test/test_perf.py` & `pymarkdownlnt-0.9.9/test/test_perf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import pytest
 
 from pymarkdown.parser_helper import ParserHelper
 
 
 def xtest_block_quotes_extra_perf1():
-
     n = 500
     ex = (
         "\n"
         + "from pymarkdown.tokenized_markdown import TokenizedMarkdown\n"
         + "source_markdown = '> a``html\\n> maybe``\\n>\\n> end'\n"
         + "tokenizer = TokenizedMarkdown()\n"
         + "actual_tokens = tokenizer.transform(source_markdown, show_debug=False)\n"
@@ -64,15 +63,14 @@
     b = 1
     c = f"{a}{b}"
     assert c == "a1"
 
 
 @pytest.mark.timeout(120)
 def xtest_block_quotes_extra_perf3():
-
     assert fred() == barney()
     for _ in range(5):
         xx = timeit.timeit("barney()", globals=globals(), number=100)
     for _ in range(5):
         xx = timeit.timeit("fred()", globals=globals(), number=100)
 
     for y in range(5):
```

### Comparing `pymarkdownlnt-0.9.8/test/test_transform_markdown.py` & `pymarkdownlnt-0.9.9/test/test_transform_markdown.py`

 * *Files identical despite different names*

