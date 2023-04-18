# Comparing `tmp/ScenarioGUI-0.2.1.tar.gz` & `tmp/ScenarioGUI-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScenarioGUI-0.2.1.tar", last modified: Tue Apr 11 14:17:15 2023, max compression
+gzip compressed data, was "ScenarioGUI-0.2.2.tar", last modified: Tue Apr 18 15:09:58 2023, max compression
```

## Comparing `ScenarioGUI-0.2.1.tar` & `ScenarioGUI-0.2.2.tar`

### file list

```diff
@@ -1,94 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.616012 ScenarioGUI-0.2.1/
--rw-rw-rw-   0        0        0     1550 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    13181 2023-04-11 14:17:15.617015 ScenarioGUI-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    12496 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.457484 ScenarioGUI-0.2.1/ScenarioGUI/
--rw-rw-rw-   0        0        0      283 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/ScenarioGUI/__init__.py
--rw-rw-rw-   0        0        0     3629 2023-04-11 14:12:38.000000 ScenarioGUI-0.2.1/ScenarioGUI/global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.522491 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/
--rw-rw-rw-   0        0        0        0 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/__init__.py
--rw-rw-rw-   0        0        0    29594 2023-04-11 12:51:29.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_base_class.py
--rw-rw-rw-   0        0        0     2655 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_calculation_thread.py
--rw-rw-rw-   0        0        0    59525 2023-04-11 13:59:04.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_combine_window.py
--rw-rw-rw-   0        0        0     4824 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_data_storage.py
--rw-rw-rw-   0        0        0     8207 2023-04-11 12:59:59.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.547486 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/
--rw-rw-rw-   0        0        0     1002 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py
--rw-rw-rw-   0        0        0     6283 2023-04-11 12:58:07.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/aim.py
--rw-rw-rw-   0        0        0     9824 2023-04-11 11:44:38.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py
--rw-rw-rw-   0        0        0    10352 2023-04-11 13:00:40.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/category.py
--rw-rw-rw-   0        0        0     3535 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py
--rw-rw-rw-   0        0        0     7673 2023-04-11 12:50:25.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py
--rw-rw-rw-   0        0        0    15245 2023-04-11 13:49:17.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py
--rw-rw-rw-   0        0        0     9433 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py
--rw-rw-rw-   0        0        0     5770 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py
--rw-rw-rw-   0        0        0     5028 2023-04-11 11:30:06.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/functions.py
--rw-rw-rw-   0        0        0     4524 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/hint.py
--rw-rw-rw-   0        0        0     8909 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py
--rw-rw-rw-   0        0        0     7894 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
--rw-rw-rw-   0        0        0    10794 2023-04-11 14:10:30.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/option.py
--rw-rw-rw-   0        0        0    15083 2023-04-11 11:58:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/page.py
--rw-rw-rw-   0        0        0     3047 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
--rw-rw-rw-   0        0        0    10748 2023-04-11 13:50:58.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
--rw-rw-rw-   0        0        0     4670 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
--rw-rw-rw-   0        0        0     5841 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
--rw-rw-rw-   0        0        0     1569 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/status_bar_logger.py
--rw-rw-rw-   0        0        0     8448 2023-03-27 13:57:20.000000 ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/translation_class.py
--rw-rw-rw-   0        0        0     1513 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/ScenarioGUI/translation_csv_to_py.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.551003 ScenarioGUI-0.2.1/ScenarioGUI/utils/
--rw-rw-rw-   0        0        0      130 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-11 11:30:06.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/change_font_size.py
--rw-rw-rw-   0        0        0      838 2023-04-11 11:53:50.000000 ScenarioGUI-0.2.1/ScenarioGUI/utils/set_default_font.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.503482 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/
--rw-rw-rw-   0        0        0    13181 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3924 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-11 14:17:15.000000 ScenarioGUI-0.2.1/ScenarioGUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1732 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      985 2023-04-11 14:17:15.619014 ScenarioGUI-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      113 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.554014 ScenarioGUI-0.2.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-03 14:37:38.000000 ScenarioGUI-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0     7096 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/gui_structure_for_tests.py
--rw-rw-rw-   0        0        0     1618 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.1/tests/result_creating_class_for_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.574016 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/
--rw-rw-rw-   0        0        0        0 2023-03-20 10:23:08.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/__init__.py
--rw-rw-rw-   0        0        0      917 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_aim.py
--rw-rw-rw-   0        0        0     1644 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_button_box.py
--rw-rw-rw-   0        0        0     1360 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_category.py
--rw-rw-rw-   0        0        0     1873 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_filename.py
--rw-rw-rw-   0        0        0     5178 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_flexible_amount_option.py
--rw-rw-rw-   0        0        0     2246 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_float_box.py
--rw-rw-rw-   0        0        0     1424 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_function_button.py
--rw-rw-rw-   0        0        0     2067 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_int_box.py
--rw-rw-rw-   0        0        0     2047 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_list_box.py
--rw-rw-rw-   0        0        0     1187 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_page.py
--rw-rw-rw-   0        0        0     1311 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_repr.py
--rw-rw-rw-   0        0        0     2076 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_result_export.py
--rw-rw-rw-   0        0        0     1428 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_figure.py
--rw-rw-rw-   0        0        0     1362 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_text.py
--rw-rw-rw-   0        0        0     1366 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_text_box.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.596021 ScenarioGUI-0.2.1/tests/test_main_window_functions/
--rw-rw-rw-   0        0        0        0 2023-04-05 13:00:55.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/__init__.py
--rw-rw-rw-   0        0        0     2414 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_auto_save.py
--rw-rw-rw-   0        0        0     2354 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_backup.py
--rw-rw-rw-   0        0        0     3698 2023-04-11 14:05:28.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_change_font_size.py
--rw-rw-rw-   0        0        0     2946 2023-04-11 14:12:17.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_close.py
--rw-rw-rw-   0        0        0     1309 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_datastorage.py
--rw-rw-rw-   0        0        0     2121 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_double_naming.py
--rw-rw-rw-   0        0        0     6263 2023-04-11 14:05:28.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_global_settings.py
--rw-rw-rw-   0        0        0     2100 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_move_scenario.py
--rw-rw-rw-   0        0        0     6100 2023-04-11 14:11:35.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_new_save_load.py
--rw-rw-rw-   0        0        0     1414 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_no_file.py
--rw-rw-rw-   0        0        0     1908 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_push_button_change.py
--rw-rw-rw-   0        0        0     4332 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_rename_scenario.py
--rw-rw-rw-   0        0        0     5156 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_run.py
--rw-rw-rw-   0        0        0     6402 2023-03-28 11:53:59.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_change.py
--rw-rw-rw-   0        0        0     1961 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_properties.py
--rw-rw-rw-   0        0        0     2876 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_main_window_functions/test_toggle_buttons.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:17:15.615015 ScenarioGUI-0.2.1/tests/test_translations/
--rw-rw-rw-   0        0        0        0 2023-03-20 10:23:09.000000 ScenarioGUI-0.2.1/tests/test_translations/__init__.py
--rw-rw-rw-   0        0        0      913 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.1/tests/test_translations/test_language_change.py
--rw-rw-rw-   0        0        0      624 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.1/tests/test_translations/test_translation_csv_2_py.py
--rw-rw-rw-   0        0        0     8795 2023-04-11 14:13:13.000000 ScenarioGUI-0.2.1/tests/test_translations/translation_class.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.886669 ScenarioGUI-0.2.2/
+-rw-rw-rw-   0        0        0     1550 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    13284 2023-04-18 15:09:58.887667 ScenarioGUI-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12599 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.687529 ScenarioGUI-0.2.2/ScenarioGUI/
+-rw-rw-rw-   0        0        0      275 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/__init__.py
+-rw-rw-rw-   0        0        0     2240 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.740058 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:05.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/__init__.py
+-rw-rw-rw-   0        0        0    29676 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_base_class.py
+-rw-rw-rw-   0        0        0     2756 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_calculation_thread.py
+-rw-rw-rw-   0        0        0    59800 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_combine_window.py
+-rw-rw-rw-   0        0        0     4824 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_data_storage.py
+-rw-rw-rw-   0        0        0     8424 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.817520 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/
+-rw-rw-rw-   0        0        0     1154 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py
+-rw-rw-rw-   0        0        0     6293 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/aim.py
+-rw-rw-rw-   0        0        0     9824 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py
+-rw-rw-rw-   0        0        0    10352 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/category.py
+-rw-rw-rw-   0        0        0     3535 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py
+-rw-rw-rw-   0        0        0     7930 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py
+-rw-rw-rw-   0        0        0    15816 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py
+-rw-rw-rw-   0        0        0     9418 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py
+-rw-rw-rw-   0        0        0     9427 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/float_box_with_units.py
+-rw-rw-rw-   0        0        0     5772 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py
+-rw-rw-rw-   0        0        0     5028 2023-04-11 11:30:06.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/functions.py
+-rw-rw-rw-   0        0        0     4526 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/hint.py
+-rw-rw-rw-   0        0        0     8894 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py
+-rw-rw-rw-   0        0        0     8619 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/int_box_with_units.py
+-rw-rw-rw-   0        0        0     8149 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
+-rw-rw-rw-   0        0        0    10937 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/option.py
+-rw-rw-rw-   0        0        0    15225 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/page.py
+-rw-rw-rw-   0        0        0     2915 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
+-rw-rw-rw-   0        0        0    10750 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
+-rw-rw-rw-   0        0        0     4670 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
+-rw-rw-rw-   0        0        0     5841 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
+-rw-rw-rw-   0        0        0     1569 2023-04-11 11:53:51.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/status_bar_logger.py
+-rw-rw-rw-   0        0        0     8448 2023-03-27 13:57:20.000000 ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/translation_class.py
+-rw-rw-rw-   0        0        0     1513 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/ScenarioGUI/translation_csv_to_py.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.822517 ScenarioGUI-0.2.2/ScenarioGUI/utils/
+-rw-rw-rw-   0        0        0      183 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/utils/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/utils/change_font_size.py
+-rw-rw-rw-   0        0        0     1520 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/utils/load_config_file.py
+-rw-rw-rw-   0        0        0      838 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/ScenarioGUI/utils/set_default_font.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.729056 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/
+-rw-rw-rw-   0        0        0    13284 2023-04-18 15:09:58.000000 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4224 2023-04-18 15:09:58.000000 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 15:09:58.000000 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-18 15:09:58.000000 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-18 15:09:58.000000 ScenarioGUI-0.2.2/ScenarioGUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1777 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      985 2023-04-18 15:09:58.897663 ScenarioGUI-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      113 2023-03-28 09:15:55.000000 ScenarioGUI-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.826517 ScenarioGUI-0.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-03 14:37:38.000000 ScenarioGUI-0.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     7943 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/gui_structure_for_tests.py
+-rw-rw-rw-   0        0        0     1618 2023-04-03 11:52:45.000000 ScenarioGUI-0.2.2/tests/result_creating_class_for_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.851576 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:08.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/__init__.py
+-rw-rw-rw-   0        0        0      917 2023-04-11 09:28:17.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_aim.py
+-rw-rw-rw-   0        0        0     1644 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_button_box.py
+-rw-rw-rw-   0        0        0     1360 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_category.py
+-rw-rw-rw-   0        0        0     1875 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_filename.py
+-rw-rw-rw-   0        0        0     5400 2023-04-18 10:08:47.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_flexible_amount_option.py
+-rw-rw-rw-   0        0        0     2246 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_float_box.py
+-rw-rw-rw-   0        0        0     2752 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_float_box_with_units.py
+-rw-rw-rw-   0        0        0     1424 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_function_button.py
+-rw-rw-rw-   0        0        0     2067 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_int_box.py
+-rw-rw-rw-   0        0        0     2547 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_int_box_with_units.py
+-rw-rw-rw-   0        0        0     2047 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_list_box.py
+-rw-rw-rw-   0        0        0     1557 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_page.py
+-rw-rw-rw-   0        0        0     1311 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_repr.py
+-rw-rw-rw-   0        0        0     1978 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_result_export.py
+-rw-rw-rw-   0        0        0     1330 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_results_figure.py
+-rw-rw-rw-   0        0        0     1264 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_results_text.py
+-rw-rw-rw-   0        0        0     1366 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_text_box.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.880125 ScenarioGUI-0.2.2/tests/test_main_window_functions/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:00:55.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/__init__.py
+-rw-rw-rw-   0        0        0     2479 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_auto_save.py
+-rw-rw-rw-   0        0        0     2354 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_backup.py
+-rw-rw-rw-   0        0        0     4222 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_change_font_size.py
+-rw-rw-rw-   0        0        0     2512 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_close.py
+-rw-rw-rw-   0        0        0     1309 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_datastorage.py
+-rw-rw-rw-   0        0        0     2121 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_double_naming.py
+-rw-rw-rw-   0        0        0     6489 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_global_settings.py
+-rw-rw-rw-   0        0        0     2100 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_move_scenario.py
+-rw-rw-rw-   0        0        0     6102 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_new_save_load.py
+-rw-rw-rw-   0        0        0     1414 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_no_file.py
+-rw-rw-rw-   0        0        0     1908 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_push_button_change.py
+-rw-rw-rw-   0        0        0     4332 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_rename_scenario.py
+-rw-rw-rw-   0        0        0     4666 2023-04-18 13:20:47.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_run.py
+-rw-rw-rw-   0        0        0     6402 2023-04-17 11:50:10.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_scenario_change.py
+-rw-rw-rw-   0        0        0     1961 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_scenario_properties.py
+-rw-rw-rw-   0        0        0     2876 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_main_window_functions/test_toggle_buttons.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:09:58.885666 ScenarioGUI-0.2.2/tests/test_translations/
+-rw-rw-rw-   0        0        0        0 2023-03-20 10:23:09.000000 ScenarioGUI-0.2.2/tests/test_translations/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-03-28 09:31:05.000000 ScenarioGUI-0.2.2/tests/test_translations/test_language_change.py
+-rw-rw-rw-   0        0        0      626 2023-04-18 15:09:45.000000 ScenarioGUI-0.2.2/tests/test_translations/test_translation_csv_2_py.py
+-rw-rw-rw-   0        0        0     8900 2023-04-18 13:25:09.000000 ScenarioGUI-0.2.2/tests/test_translations/translation_class.py
```

### Comparing `ScenarioGUI-0.2.1/LICENSE` & `ScenarioGUI-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/PKG-INFO` & `ScenarioGUI-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScenarioGUI
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package for a scenario based GUI
 Home-page: https://github.com/tblanke/ScenarioGUI
 Author: Tobias Blanke
 Author-email: blanke@fh-aachen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -116,14 +116,16 @@
         super().__init__(default_parent, translations)
         # add a first page called "Inputs" and has a button name of "Input" and has an icon "Add.svg"
         self.page_inputs = els.Page(name="Inputs", button_name="Input", icon="Add.svg")
         # Then several aims can be added to the page with different names and icons
         self.aim_add = els.Aim(label="Adding", icon="Add", page=self.page_inputs)
         self.aim_sub = els.Aim(label="Substract", icon="Delete", page=self.page_inputs)
         self.aim_plot = els.Aim(label="Plot", icon="Parameters", page=self.page_inputs)
+        # this three aims can appear in one row by setting:
+        self.page_inputs.aims_in_row = 3
         # a category with the label "Inputs" can be added to the inputs page like:
         self.category_inputs = els.Category(label="Inputs", page=self.page_inputs)
         # an integer box can be added with different options like this (some of these options are optional):
         self.int_a = els.IntBox(label="a",default_value=2,minimal_value=0,maximal_value=200,step=2,category=self.category_inputs)
         # a float box can be added with different options like this (some of these options are optional):
         self.float_b = els.FloatBox(
             label="b",
```

### Comparing `ScenarioGUI-0.2.1/README.md` & `ScenarioGUI-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
         super().__init__(default_parent, translations)
         # add a first page called "Inputs" and has a button name of "Input" and has an icon "Add.svg"
         self.page_inputs = els.Page(name="Inputs", button_name="Input", icon="Add.svg")
         # Then several aims can be added to the page with different names and icons
         self.aim_add = els.Aim(label="Adding", icon="Add", page=self.page_inputs)
         self.aim_sub = els.Aim(label="Substract", icon="Delete", page=self.page_inputs)
         self.aim_plot = els.Aim(label="Plot", icon="Parameters", page=self.page_inputs)
+        # this three aims can appear in one row by setting:
+        self.page_inputs.aims_in_row = 3
         # a category with the label "Inputs" can be added to the inputs page like:
         self.category_inputs = els.Category(label="Inputs", page=self.page_inputs)
         # an integer box can be added with different options like this (some of these options are optional):
         self.int_a = els.IntBox(label="a",default_value=2,minimal_value=0,maximal_value=200,step=2,category=self.category_inputs)
         # a float box can be added with different options like this (some of these options are optional):
         self.float_b = els.FloatBox(
             label="b",
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_base_class.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_base_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import PySide6.QtCore as QtC
 import PySide6.QtGui as QtG
 import PySide6.QtWidgets as QtW
 
 import ScenarioGUI.global_settings as globs
 
-from .status_bar_logger import StatusBar
 from ..utils import set_default_font
+from .status_bar_logger import StatusBar
 
 
 class BaseUI:
     """
     This class contains the framework of the GUI, with the top bar,
     the scenario/run/ ... buttons and the shortcuts.
     """
@@ -308,23 +308,25 @@
         ghe_tool.setStatusBar(self.status_bar_progress_bar)
 
         self.frame_progress_bar = QtW.QFrame(self.central_widget)
         self.horizontal_layout_progress_bar = QtW.QHBoxLayout(self.frame_progress_bar)
         self.horizontal_layout_progress_bar.setObjectName("horizontalLayout_progress_bar")
         self.label_status = QtW.QLabel(self.central_widget)
         self.label_status.setObjectName("label_Status")
+        self.label_status.setFont(font)
         self.horizontal_layout_progress_bar.addWidget(self.label_status)
 
         self.progress_bar = QtW.QProgressBar(self.central_widget)
         self.progress_bar.setObjectName("progress_bar")
         self.progress_bar.setStyleSheet(
             f"QProgressBar{'{'}border: 1px solid {globs.WHITE};border-radius: 10px;text-align: center;color: {globs.WHITE};{'}'}\n"
             f"QProgressBar::chunk{'{'}background-color: {globs.LIGHT}; border-radius: 10px;{'}'}"
         )
         self.progress_bar.setValue(0)
+        self.progress_bar.setFont(font)
         self.horizontal_layout_progress_bar.addWidget(self.progress_bar)
 
         self.vertical_layout_main.addWidget(self.frame_progress_bar)
 
         self.horizontal_layout_start_buttons = QtW.QHBoxLayout()
         self.horizontal_layout_start_buttons.setObjectName("horizontalLayout_2")
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_calculation_thread.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_calculation_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             function to create the results class and a function to be called in the thread
         """
         super().__init__(parent)  # init parent class
         # set datastorage and index
         self.d_s = d_s
         self.idx = idx
         self.data_2_results_function = data_2_results_function
+        self.calculated = False
 
     def run(self) -> None:
         """
         This function contains the actual code to run the different calculations.
         For each aim in the GUI, a new if statement is used. Here, one can put all the code
         needed to run the simulation/calculation with the all the functionalities of GHEtool.
         This function should return the DataStorage as a signal.
@@ -68,19 +69,21 @@
         try:
             results, func = self.data_2_results_function(self.d_s)
             func()
         except Exception as err:
             self.d_s.debug_message = err
             # save bore field in Datastorage
             self.d_s.results = None
+            self.calculated = True
             # return Datastorage as signal
             self.any_signal.emit((self.d_s, self.idx, self))
             return
 
         # set debug message to ""
         self.d_s.debug_message = ""
 
         # save borefield in Datastorage
         self.d_s.results = results
+        self.calculated = True
         # return Datastorage as signal
         self.any_signal.emit((self.d_s, self.idx, self))
         return
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_combine_window.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_combine_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 from functools import partial as ft_partial
 from json import dump, load
 from math import isclose
 from os import makedirs, remove
 from os.path import dirname, exists, realpath
 from os.path import split as os_split
 from pathlib import Path, PurePath
@@ -13,20 +14,20 @@
 import PySide6.QtCore as QtC
 import PySide6.QtGui as QtG
 import PySide6.QtWidgets as QtW
 from matplotlib import rcParams
 
 import ScenarioGUI.global_settings as globs
 
+from ..utils import change_font_size, set_default_font
 from .gui_base_class import BaseUI
 from .gui_calculation_thread import CalcProblem
 from .gui_data_storage import DataStorage
 from .gui_structure_classes import FigureOption, Option, ResultExport
 from .gui_structure_classes.functions import check_aim_options, show_linked_options
-from ..utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:
     from collections.abc import Callable
     from typing import Protocol
 
     from ScenarioGUI.gui_classes.gui_structure import GuiStructure
 
@@ -52,15 +53,14 @@
 class MainWindow(QtW.QMainWindow, BaseUI):
     """
     This class contains the general functionalities of the GUI (e.g. the handling of creating new scenarios,
     saving documents etc.)
     """
 
     filename_default: tuple = ("", "")
-    BACKUP_FILENAME: str = f"backup.{globs.FILE_EXTENSION}BackUp"
 
     def __init__(
         self,
         dialog: QtW.QWidget,
         app: QtW.QApplication,
         gui_structure: type[GuiStructure],
         translations: type[Translations],
@@ -86,14 +86,15 @@
 
         Returns
         -------
         MainWindow
         """
         # parameter to show the end of the init function
         self.started = False
+        self._backup_filename: str = f"backup.{globs.FILE_EXTENSION}BackUp"
         # init windows of parent class
         super().__init__()
         super().setup_ui(dialog)
         # pyside6-rcc icons.qrc -o icons_rc.py
         self.translations: Translations = translations()  # init translation class
 
         self.result_creating_class = result_creating_class
@@ -111,15 +112,15 @@
         # init pop up dialog
         self.dialog: QtW.QInputDialog | None = None
         # init variables of class
         # allow checking of changes
         self.checking: bool = False
         # create backup path in home documents directory
         self.default_path: Path = Path(Path.home(), f"Documents/{globs.GUI_NAME}")
-        self.backup_file: Path = Path(self.default_path, self.BACKUP_FILENAME)
+        self.backup_file: Path = Path(self.default_path, self._backup_filename)
         # check if backup folder exits and otherwise create it
         makedirs(dirname(self.backup_file), exist_ok=True)
         makedirs(dirname(self.default_path), exist_ok=True)
         for idx, (name, icon, short_cut) in enumerate(zip(self.translations.languages, self.translations.icon, self.translations.short_cut)):
             self._create_action_language(idx, name, icon, short_cut)
         # add languages to combo box
         self.gui_structure.option_language.widget.addItems(self.translations.languages)
@@ -253,20 +254,28 @@
         self.action_open.triggered.connect(self.fun_load)
         self.action_new.triggered.connect(self.fun_new)
         self.action_rename_scenario.triggered.connect(lambda: self.fun_rename_scenario())
         self.list_widget_scenario.setDragDropMode(QtW.QAbstractItemView.InternalMove)
         self.list_widget_scenario.model().rowsMoved.connect(self.fun_move_scenario)
         self.list_widget_scenario.currentItemChanged.connect(self.scenario_is_changed)
         self.list_widget_scenario.itemSelectionChanged.connect(self._always_scenario_selected)
+        self.gui_structure.option_auto_saving.change_event(self.change_auto_saving)
         self.dia.closeEvent = self.closeEvent
 
+    def change_auto_saving(self):
+        if self.gui_structure.option_auto_saving.get_value() == 1:
+            self.push_button_save_scenario.hide()
+            return
+        self.push_button_save_scenario.show()
+
+
     def change_font_size(self):
         size = self.gui_structure.option_font_size.get_value()
         globs.FONT_SIZE = size
-        rcParams.update({'font.size': size})
+        rcParams.update({"font.size": size})
         self.gui_structure.change_font_size_2(size)
         change_font_size(self.push_button_save_scenario, size)
         change_font_size(self.push_button_add_scenario, size)
         change_font_size(self.push_button_delete_scenario, size)
         change_font_size(self.button_rename_scenario, size)
         change_font_size(self.push_button_cancel, size)
         change_font_size(self.push_button_start_single, size)
@@ -275,14 +284,16 @@
         change_font_size(self.menu_calculation, size)
         change_font_size(self.menu_file, size)
         change_font_size(self.menu_settings, size)
         change_font_size(self.menu_language, size)
         change_font_size(self.menubar, size)
         change_font_size(self.list_widget_scenario, size)
         change_font_size(self.status_bar.widget, size)
+        change_font_size(self.progress_bar, size)
+        change_font_size(self.label_status, size)
         self.remove_previous_calculated_results()
 
     def export_results(self, result_export: ResultExport):
         filename: tuple = QtW.QFileDialog.getSaveFileName(
             self.central_widget,
             caption=result_export.caption,
             filter=f".{result_export.file_extension} (*.{result_export.file_extension})",
@@ -378,26 +389,15 @@
         Returns
         -------
         None
         """
         # return if not yet started or return if checking is not allowed
         if not self.started or not self.checking:
             return
-        if self.check_values():
-            self.push_button_start_multiple.setEnabled(True)
-            self.push_button_start_single.setEnabled(True)
-            self.push_button_add_scenario.setEnabled(True)
-            self.push_button_save_scenario.setEnabled(True)
-            self.list_widget_scenario.setEnabled(True)
-        else:
-            self.push_button_start_multiple.setEnabled(False)
-            self.push_button_start_single.setEnabled(False)
-            self.push_button_add_scenario.setEnabled(False)
-            self.push_button_save_scenario.setEnabled(False)
-            self.list_widget_scenario.setEnabled(False)
+        self.check_buttons()
         # if changed File is not already True set it to True and update window title
         if self.changedFile is False:
             self.changedFile: bool = True
             self.change_window_title()
         # get current index of scenario
         idx: int = self.list_widget_scenario.currentRow()
         if self.list_ds:
@@ -422,14 +422,30 @@
             return
         # if scenario is already marked as changed return
         if text[-1] == "*":
             return
         # else add * to current item string
         self.list_widget_scenario.item(idx).setText(f"{text}*")
 
+    def check_buttons(self):
+        if self.check_values() and self.list_widget_scenario.currentRow() not in [thread.idx for thread in self.threads]:
+            self.push_button_start_multiple.setEnabled(True)
+            self.push_button_start_single.setEnabled(True)
+            self.push_button_save_scenario.setEnabled(True)
+        else:
+            self.push_button_start_multiple.setEnabled(False)
+            self.push_button_start_single.setEnabled(False)
+            self.push_button_save_scenario.setEnabled(False)
+        if self.check_values():
+            self.list_widget_scenario.setEnabled(True)
+            self.push_button_add_scenario.setEnabled(True)
+        else:
+            self.list_widget_scenario.setEnabled(False)
+            self.push_button_add_scenario.setEnabled(False)
+
     def scenario_is_changed(self, new_row_item: QtW.QListWidgetItem, old_row_item: QtW.QListWidgetItem) -> None:
         """
         This function handles the changing of scenarios.
         If the auto-save ButtonBox is set to auto-save, the previous scenario is changed an the new item is selected.
         If not, a messagebox is shown to ask if the 'old' scenario should be saved.
 
         Parameters
@@ -442,14 +458,15 @@
         Returns
         -------
         None
         """
         # return if not checking
         if not self.checking:
             return
+        self.check_buttons()
         # if no old item is selected do nothing and return
         if old_row_item is None:
             # change entries to new scenario values
             self.change_scenario(self.list_widget_scenario.row(new_row_item))
             return
 
         def return_2_old_item():
@@ -474,14 +491,15 @@
         # check if the auto saving should be performed and then save the last selected scenario
         if self.gui_structure.option_auto_saving.get_value() == 1:
             self.check_values()
             # save old scenario
             if (
                 len(self.list_ds) - 1 >= self.list_widget_scenario.row(old_row_item)
                 and DataStorage(self.gui_structure) != self.list_ds[self.list_widget_scenario.row(old_row_item)]
+                and self.push_button_save_scenario.isEnabled()
             ):
                 self.list_ds[self.list_widget_scenario.row(old_row_item)].close_figures()
                 self.list_ds[self.list_widget_scenario.row(old_row_item)] = DataStorage(self.gui_structure)
             # update backup fileImport
             self.fun_save_auto()
             # change values to new scenario values
             self.change_scenario(self.list_widget_scenario.row(new_row_item))
@@ -1140,19 +1158,21 @@
         Returns
         -------
         None
         """
         # show label and progress bar if calculation started otherwise hide them
         self.status_bar_progress_bar.show()
         # calculate percentage of calculated scenario
-        val = val / len(self.threads)
+        val = val / max(len(self.threads), 1)
         # set percentage to progress bar
         self.progress_bar.setValue(round(val * 100))
         # hide labels and progressBar if all scenarios are calculated
-        if isclose(val, 1):
+        if all(thread.calculated for thread in self.threads):
+            self.threads = []
+            self.progress_bar.setValue(100)
             self.status_bar_progress_bar.hide()
             # show message that calculation is finished
             globs.LOGGER.info(self.translations.Calculation_Finished[self.gui_structure.option_language.get_value()[0]])
 
     def thread_function(self, results: tuple[DataStorage, int, CalcProblem]) -> None:
         """
         This function closes the thread of the old calculation and stores it results.
@@ -1173,31 +1193,29 @@
 
         try:
             self.list_ds[results[1]] = results[0]
         except IndexError:
             return
 
         # count number of finished calculated scenarios
-        open_threads = [thread for thread in self.threads if not thread.isRunning() and not thread.isFinished()]
+        idx_list = [thread.idx for thread in self.threads]
+        open_threads = [thread for thread in self.threads if not thread.calculated]
         n_closed_threads = len(self.threads) - len(open_threads)
         # update progress bar
         self.update_bar(n_closed_threads)
         # if number of finished is the number that has to be calculated enable buttons and actions and change page to
         # results page
         if open_threads:        # start new thread
             open_threads[0].start()
             open_threads[0].any_signal.connect(self.thread_function)
             return
         # display results
-        self.push_button_start_multiple.setEnabled(True)
-        self.push_button_start_single.setEnabled(True)
-        self.push_button_save_scenario.setEnabled(True)
-        self.action_start_single.setEnabled(True)
-        self.action_start_multiple.setEnabled(True)
-        self.gui_structure.page_result.button.click()
+        self.check_buttons()
+        if self.list_widget_scenario.currentRow() in idx_list:
+            self.gui_structure.page_result.button.click()
 
     def start_multiple_scenarios_calculation(self) -> None:
         """
         This function starts the calculation of all the scenarios that do not have a results attribute in their
         DS, when check_values() is True.
 
         Returns
@@ -1205,27 +1223,26 @@
         None
         """
         if not self.check_values():
             return
         # add scenario if no list of scenarios exits else save current scenario
         self.add_scenario() if not self.list_ds else self.save_scenario()
         # create list of threads with scenarios that have not been calculated
-        self.threads = [CalcProblem(DS, idx, data_2_results_function=self.data_2_results_function) for idx, DS in enumerate(self.list_ds) if DS.results is None]
+        self.threads += [CalcProblem(DS, idx, data_2_results_function=self.data_2_results_function) for idx, DS in enumerate(self.list_ds) if DS.results is
+                         None]
         # set number of to calculate scenarios
         if len(self.threads) < 1:
             return
         # disable buttons and actions to avoid two calculation at once
-        self.push_button_start_multiple.setEnabled(False)
-        self.push_button_start_single.setEnabled(False)
-        self.push_button_save_scenario.setEnabled(False)
-        self.action_start_single.setEnabled(False)
-        self.action_start_multiple.setEnabled(False)
+        self.check_buttons()
         # update progress bar
         self.update_bar(0)
         # start calculation if at least one scenario has to be calculated
+        if [thread for thread in self.threads if thread.isRunning()]:  # pragma: no cover
+            return
         for thread in self.threads[:self.gui_structure.option_n_threads.get_value()]:
             thread.start()
             thread.any_signal.connect(self.thread_function)
 
     def start_current_scenario_calculation(self, no_run: bool = False) -> None:
         """
         This function starts the calculation of the selected/current scenario, when check_values() is True.
@@ -1246,30 +1263,24 @@
 
         # get index of selected scenario
         idx: int = self.list_widget_scenario.currentRow()
         # get Datastorage of selected scenario
         ds: DataStorage = self.list_ds[idx]
         # if calculation is already done just show results
         if ds.results is not None:
-            self.threads = []
             self.gui_structure.page_result.button.click()
             return
-        # return to thermal demands page if no file is selected
-        # disable buttons and actions to avoid two calculation at once
-        self.push_button_start_multiple.setEnabled(False)
-        self.push_button_start_single.setEnabled(False)
-        self.push_button_save_scenario.setEnabled(False)
-        self.action_start_single.setEnabled(False)
-        self.action_start_multiple.setEnabled(False)
         # create list of threads with calculation to be made
-        self.threads = [CalcProblem(ds, idx, data_2_results_function=self.data_2_results_function)]
+        self.threads += [CalcProblem(ds, idx, data_2_results_function=self.data_2_results_function)]
+        # disable buttons and actions to avoid two calculation at once
+        self.check_buttons()
         # update progress bar
         self.update_bar(0)
         # start calculation
-        if not no_run:
+        if not no_run and len(self.threads) == 1:
             self.threads[0].start()
             self.threads[0].any_signal.connect(self.thread_function)
 
     def display_results(self) -> None:
         """
         This function displays the results (of the selected scenario) on the results page.
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_data_storage.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_data_storage.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 It contains all the options, categories etc. that should appear on the GUI.
 """
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
+from ScenarioGUI import global_settings as globs
 from ScenarioGUI.gui_classes.gui_structure_classes import (
     Aim,
     ButtonBox,
     Category,
     FunctionButton,
     Hint,
     IntBox,
     ListBox,
     Option,
     Page,
-    ResultExport, ResultFigure,
+    ResultExport,
+    ResultFigure,
     ResultText,
 )
-from ScenarioGUI import global_settings as globs
 
 if TYPE_CHECKING:
     import PySide6.QtWidgets as QtW
 
     from ScenarioGUI.gui_classes.translation_class import Translations
 
 
@@ -108,16 +109,19 @@
             label=self.translations.option_toggle_buttons,
             default_index=1,
             entries=[" no ", " yes "],
             category=self.category_save_scenario,
         )
         self.option_toggle_buttons.change_event(self.change_toggle_button)
         self.option_n_threads = IntBox(label=self.translations.option_n_threads, default_value=2, category=self.category_save_scenario, minimal_value=1)
-        self.option_font_size = IntBox(label="Font Size", default_value= globs.FONT_SIZE, category= self.category_save_scenario, minimal_value=8,
-                                       maximal_value=14)
+        self.option_font_size = IntBox(label=self.translations.option_font_size if hasattr(self.translations, "option_font_size") else "Font Size",
+                                       default_value=globs.FONT_SIZE,
+                                       category=self.category_save_scenario,
+                                       minimal_value=8,
+                                       maximal_value=20)
         self.option_auto_saving = ButtonBox(
             label=self.translations.option_auto_saving,
             default_index=0,
             entries=[" no ", " yes "],
             category=self.category_save_scenario,
         )
         self.hint_saving = Hint(
@@ -198,8 +202,8 @@
         Page.next_label = translation.label_next[index]
         Page.previous_label = translation.label_previous[index]
         for name in [j for j in translation.__slots__ if hasattr(self, j)]:
             entry: Option | Hint | FunctionButton | Page | Category = getattr(self, name)
             try:
                 entry.translate(index)
             except IndexError:
-                logging.error(name)
+                logging.exception(name)
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,35 +7,39 @@
 from .aim import Aim
 from .button_box import ButtonBox
 from .category import Category
 from .figure_option import FigureOption
 from .filename_box import FileNameBox
 from .flexible_amount_option import FlexibleAmount
 from .float_box import FloatBox
+from .float_box_with_units import FloatBoxWithUnits
 from .function_button import FunctionButton
 from .hint import Hint
 from .int_box import IntBox
+from .int_box_with_units import IntBoxWithUnits
 from .list_box import ListBox
 from .option import Option
 from .page import Page
+from .result_export import ResultExport
 from .result_figure import ResultFigure
 from .result_text import ResultText
 from .text_box import TextBox
-from .result_export import ResultExport
 
 __all__ = [
     "Aim",
     "ButtonBox",
     "Category",
     "FigureOption",
     "FileNameBox",
     "FloatBox",
+    "FloatBoxWithUnits",
     "FunctionButton",
     "Hint",
     "IntBox",
+    "IntBoxWithUnits",
     "ListBox",
     "Option",
     "Page",
     "ResultFigure",
     "ResultText",
     "ResultExport",
     "TextBox",
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/aim.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/aim.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, Protocol
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+
 from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
@@ -133,26 +134,26 @@
         This function can be used to couple the Aim value to other options, hints, function buttons or categories.
         In the example below, 'option_example' will be shown if the Aim is selected.
 
         >>> aim_example.add_link_2_show(option=option_example)
         """
         self.list_options.append(option)
 
-    def create_widget(self, frame: QtW.QFrame, layout: QtW.QGridLayout, idx: int) -> None:
+    def create_widget(self, frame: QtW.QFrame, layout: QtW.QGridLayout, idx: tuple[int, int]) -> None:
         """
         This functions creates the Aim widget in the grid layout.
 
         Parameters
         ----------
         frame : QtW.QFrame
             The frame object in which is the parent of the current widget
         layout : QtW.QGridLayout
             The grid layout in which the widget should be created
-        idx : int
-            Index of the current Aim
+        idx : tuple[int, int]
+            position in grid layout of the current Aim
 
         Returns
         -------
         None
         """
         icon11 = QtG.QIcon()
         icon11.addFile(f"{globs.FOLDER}/icons/{self.icon}")
@@ -170,15 +171,15 @@
             f"background-color: {globs.GREY};{'}'}\n"
             f"QPushButton:disabled:hover{'{'}background-color: {globs.DARK};{'}'}"
         )
         set_default_font(push_button, bold=True)
         push_button.setIconSize(QtC.QSize(30, 30))
         push_button.setCheckable(True)
         push_button.setText(self.label[0])
-        layout.addWidget(push_button, int(idx / 2), 0 if divmod(idx, 2)[1] == 0 else 1, 1, 1)
+        layout.addWidget(push_button, idx[0], idx[1], 1, 1)
 
     def translate(self, idx: int) -> None:
         """
         Translates the label.
 
         Parameters
         ----------
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/button_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from functools import partial as ft_partial
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
-from .functions import update_opponent_not_change, update_opponent_toggle, check
+from .functions import check, update_opponent_not_change, update_opponent_toggle
 from .option import Option
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/category.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/category.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
+from ...utils import change_font_size, set_default_font
 from .hint import Hint
 from .result_text import ResultText
-from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from .function_button import FunctionButton
     from .option import Option
     from .page import Page
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
+from ...utils import change_font_size, set_default_font
 from .option import Option
-from ...utils import set_default_font, change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
 
 
@@ -32,15 +32,15 @@
         self,
         label: str | list[str],
         default_value: str,
         category: Category,
         *,
         dialog_text: str = "",
         error_text: str = "",
-        file_extension: str = "csv"
+        file_extension: str | list[str] = "csv"
     ):
         """
 
         Parameters
         ----------
         label : str | list[str]
             The labels of the FileNameBox for different languages
@@ -68,15 +68,16 @@
 
         """
         super().__init__(label, default_value, category)
         self.widget: QtW.QLineEdit = QtW.QLineEdit(self.default_parent)
         self.dialog_text: str = dialog_text
         self.error_text: str = error_text
         self.button: QtW.QPushButton = QtW.QPushButton(self.default_parent)
-        self.file_extension = file_extension
+        self.file_extension = [file_extension] if isinstance(file_extension, str) else file_extension
+        self.check_active: bool = False
 
     def get_value(self) -> str:
         """
         This function returns the filename (with path) which is put into the FileNameBox.
 
         Returns
         -------
@@ -117,15 +118,15 @@
         This function checks whether or not a value is given in the FileNameBox.
 
         Returns
         -------
         bool
             True if a value is given in the FileNameBox. False otherwise
         """
-        return exists(self.widget.text())
+        return exists(self.widget.text()) if self.check_active else True
 
     def check_linked_value(self, value: str) -> bool:
         """
         This function checks if the linked "option" should be shown.
 
         Parameters
         ----------
@@ -229,13 +230,15 @@
         This is automatically added to the FileNameBox.
 
         Returns
         -------
         None
         """
         # try to ask for a file otherwise show message in status bar
+        file_extensions = [f".{extension} (*.{extension})" for extension in self.file_extension]
+        file_extensions = ";;".join(file_extensions)
         filename = QtW.QFileDialog.getOpenFileName(self.frame, caption=self.dialog_text,
-                                                   filter=f".{self.file_extension} (*.{self.file_extension})", dir=str(Path.home()))
+                                                   filter=file_extensions, dir=str(Path.home()))
         if not filename[0]:
             logging.error(self.error_text)
             return
         self.set_value(filename[0])
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
+from ...utils import change_font_size, set_default_font
 from .option import Option
-from ...utils import set_default_font, change_font_size
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -71,15 +71,15 @@
         """
         super().__init__(label, default_length, category)
         self.category = category
         self.entry_name: str = entry_mame
         self.list_of_options: list[Option] = []
         self.option_entries: list[list[Option]] = []
         self.option_classes: list[tuple[type[Option], dict, str]] = []
-        self.func_on_change: Callable[[]] | None = None
+        self.func_on_change: list[Callable[[]]] = []
         self.len_limits: tuple[int | None, int | None] = (min_length, max_length)
         
     def add_option(self, option: type[Option], name: str, **kwargs):
         self.option_classes.append((option, kwargs, name))
 
     def _add_entry(self) -> None:
         length = len(self.option_entries)
@@ -87,15 +87,15 @@
         label.setText(f"{self.entry_name} {length + 1}")
         set_default_font(label)
         self.frame.layout().addWidget(label, length + 1, 0)
         options = []
         i = 2
         for option, kwargs, _ in self.option_classes:
             option_i = option(**kwargs, category=self, label="")
-            option_i.change_event(self.func_on_change)
+            _ = [option_i.change_event(func) for func in self.func_on_change]
             option_i.create_widget(self.frame, self.frame.layout(), column=length + 1, row=i)
             set_default_font(option_i.widget)
             options.append(option_i)
             i += 1
         self.option_entries.append(options)
         add_button: QtW.QPushButton = QtW.QPushButton(text=" + ", parent=self.frame, clicked=partial(self._add_entry_at_row, row=length))
         delete_button: QtW.QPushButton = QtW.QPushButton(text=" - ", parent=self.frame, clicked=partial(self._del_entry, row=length))
@@ -106,15 +106,15 @@
 
     def _add_entry_at_row(self, row: int):
         values = self.get_value()
         values.insert(row + 1, values[row]) if row + 1 < len(values) else values.append(values[row])
         self.set_value(values)
         for option, (min_length, max_length) in self.linked_options:
             self.show_option(option, min_length, max_length)
-        self.func_on_change()
+        _ = [func() for func in self.func_on_change]
 
     def _del_entry(self, *, row: int | None = None) -> None:
         """
         delete an entry.
 
         Parameters
         ----------
@@ -130,15 +130,15 @@
         if row == length - 1 == 0:
             return
         values = self.get_value()
         del values[row]
         self.set_value(values)
         for option, (min_length, max_length) in self.linked_options:
             self.show_option(option, min_length, max_length)
-        self.func_on_change()
+        _ = [func() for func in self.func_on_change]
 
     def get_value(self) -> list[list[str | float | int | bool]]:
         """
         This function gets the value of the FloatBox.
 
         Returns
         -------
@@ -167,15 +167,15 @@
         for idx, label in enumerate([item.widget() for item in [self.frame.layout().itemAtPosition(i, 0) for i in range(1, length + 1)] 
                                      if item is not None]):
             label.setText(f"{self.entry_name} {idx + 1}")
         for idx, name in enumerate(entry_name[2:]):
             self.frame.layout().itemAtPosition(0, idx + 2).widget().setText(name)
             self.option_classes[idx] = (self.option_classes[idx][0], self.option_classes[idx][1], name)
 
-    def set_value(self, value: list[list[str, float, int, bool]]) -> None:
+    def set_value(self, value: list[list[str | float | int | bool]] | list[tuple[str | float | int | bool]]) -> None:
         """
         This function sets the value of the Flexible Amount option.
 
         Parameters
         ----------
         value : list of list of float, int, str, bool
             Value to which the option should be set.
@@ -191,15 +191,15 @@
                              if self.frame.layout().itemAtPosition(length + 1, i) is not None]:
                     item.widget().setParent(None)
                 del self.option_entries[length]
         else:
             for _ in range(len_options, len(value)):
                 self._add_entry()
                 
-        self.func_on_change()
+        _ = [func() for func in self.func_on_change]
         self._init_links()
 
         for options, values in zip(self.option_entries, value):
             for option, val in zip(options, values):
                 option.set_value(val)
 
     def _init_links(self) -> None:
@@ -283,14 +283,36 @@
         """
         if min_length is not None and len(self.get_value()) < min_length:
             return option.show()
         if max_length is not None and len(self.get_value()) > max_length:
             return option.show()
         option.hide()
 
+    def hide(self) -> None:
+        """
+        This function makes the current frame invisible.
+
+        Returns
+        -------
+        None
+        """
+        super().hide()
+        self.label.hide()
+
+    def show(self) -> None:
+        """
+        This function makes the current frame visible.
+
+        Returns
+        -------
+        None
+        """
+        super().show()
+        self.label.show()
+
     def check_linked_value(self, value: tuple[float | None, float | None]) -> bool:
         """
         This function checks if the linked "option" should be shown.
 
         Parameters
         ----------
         value : tuple of 2 optional floats
@@ -317,15 +339,15 @@
         function_to_be_called : callable
             Function which should be called
 
         Returns
         -------
         None
         """
-        self.func_on_change = function_to_be_called
+        self.func_on_change.append(function_to_be_called)
         for option in self.list_of_options:
             option.change_event(function_to_be_called)
 
     def set_font_size(self, size: int) -> None:
         """
         set the new font size to button
 
@@ -376,15 +398,15 @@
         layout_parent_i = QtW.QVBoxLayout(frame_i)
         layout_parent_i.setSpacing(0)
         layout_parent_i.setContentsMargins(0, 0, 0, 0)
         self.label.setParent(frame_i)
         self.label.setText(self.label_text[0])
         self.label.setStyleSheet(
             f"QLabel {'{'}border: 1px solid  {globs.LIGHT};border-top-left-radius: 15px;border-top-right-radius: 15px;"
-            f"border-bottom-left-radius: 0px;border-top-right-radius: 0px;"
+            f"border-bottom-left-radius: 0px;border-bottom-right-radius: 0px;"
             f"background-color:  {globs.LIGHT};padding: 5px 0px;\n"
             f"	color:  {globs.WHITE};{'}'}"
         )
         set_default_font(self.label, bold=True)
         self.label.setAlignment(QtC.Qt.AlignCenter | QtC.Qt.AlignVCenter)
         layout_parent_i.addWidget(self.label)
         self.frame.setParent(frame_i)
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/float_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
-from .option import Option
 from ...utils import set_default_font
+from .option import Option
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -157,15 +157,15 @@
         --------
         This function can be used to couple the FloatBox value to other options, hints, function buttons or categories.
         In the example below, 'option linked' will be shown if the float value is below 0.1 or above 0.9.
 
         >>> option_float.add_link_2_show(option=option_linked, below=0.1, above=0.9)
         """
         self.linked_options.append((option, (below, above)))
-        self.widget.valueChanged.connect(ft_partial(self.show_option, option, below, above))
+        self.change_event(ft_partial(self.show_option, option, below, above))
 
     def show_option(
         self,
         option: Option | Category | FunctionButton | Hint,
         below: float | None,
         above: float | None,
         args=None,
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/function_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+
 from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from ..gui_structure_classes import Category
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/functions.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/functions.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/hint.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/hint.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
+
 from ...utils import change_font_size, set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from .category import Category
 
 
 class Hint:
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/int_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import TYPE_CHECKING
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
-from .option import Option
 from ...utils import set_default_font
+from .option import Option
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -107,15 +107,15 @@
         Function on how the links for the IntBox should be set.
 
         Returns
         -------
         None
         """
         current_value: int = self.get_value()
-        self.set_value(self.minimal_value if current_value == self.minimal_value else self.minimal_value)
+        self.set_value(self.maximal_value if current_value == self.minimal_value else self.minimal_value)
         self.set_value(current_value)
 
     def _check_value(self) -> bool:
         """
         This function checks if the value of the IntBox is between the minimal_value
         and maximal_value.
 
@@ -173,15 +173,15 @@
         Examples
         --------
         This function can be used to couple the IntBox value to other options, hints, function buttons or categories.
         So in the example `option_linked` will be shown if the integer value is below 1 or above 10.
 
         >>> option_int.add_link_2_show(option=option_linked, below=1, above=10)
         """
-        self.widget.valueChanged.connect(ft_partial(self.show_option, option, below, above))
+        self.change_event(ft_partial(self.show_option, option, below, above))
 
     def show_option(
         self,
         option: Option | Category | FunctionButton | Hint,
         below: int | None,
         above: int | None,
         args=None,
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/list_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from functools import partial as ft_partial
 from typing import TYPE_CHECKING
 
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
+from ...utils import set_default_font
 from .functions import check
 from .option import Option
-from ...utils import set_default_font
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
     from .function_button import FunctionButton
     from .hint import Hint
@@ -224,14 +224,16 @@
         None
         """
         layout = self.create_frame(frame, layout_parent)
         self.widget.setParent(self.frame)
         self.widget.setStyleSheet(
             f"QFrame {'{'}border: 1px solid {globs.WHITE};border-bottom-left-radius: 0px;border-bottom-right-radius: 0px;{'}'}"
             f"QComboBox{'{'}border: 1px solid {globs.WHITE};border-bottom-left-radius: 0px;border-bottom-right-radius: 0px;{'}'}"
+            f"QComboBox QAbstractItemView::item:hover{'{'}color: {globs.WHITE};background-color: {globs.LIGHT_SELECT};{'}'}"
+            f"QComboBox QAbstractItemView::item:selected{'{'}color: {globs.WHITE};background-color: {globs.LIGHT_SELECT};{'}'}"
         )
         self.widget.addItems(self.entries)
         self.widget.setCurrentIndex(self.default_value)
         if self.limit_size:
             # self.widget.setMaximumWidth(100)
             self.widget.setMinimumWidth(100)
         self.widget.currentIndexChanged.connect(ft_partial(check, self.linked_options, self))  # pylint: disable=E1101
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/option.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,22 @@
 
         Returns
         -------
         None
         """
 
     def set_font_size(self, size: int) -> None:
+        """
+        scale the font size
+
+        Parameters
+        ----------
+        size: int
+            new font size
+        """
         if self.label is not None:
             change_font_size(self.label, size, False)
         if isinstance(self.widget, list):
             for widget in self.widget:
                 change_font_size(widget, size, True)
             return
         change_font_size(self.widget, size, True)
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/page.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
 
 import ScenarioGUI.global_settings as globs
 
+from ...utils import change_font_size, set_default_font
 from .aim import Aim
-from .functions import update_opponent_not_change, update_opponent_toggle, check_aim_options
-from ...utils import set_default_font, change_font_size
+from .functions import check_aim_options, update_opponent_not_change, update_opponent_toggle
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
     from .category import Category
 
 
@@ -66,14 +66,15 @@
         self.label: QtW.QLabel = QtW.QLabel(self.default_parent)
         self.label_gap: QtW.QLabel = QtW.QLabel(self.default_parent)
         self.page: QtW.QWidget = QtW.QWidget(self.default_parent)
         self.previous_page: Page | None = None
         self.next_page: Page | None = None
         self.upper_frame: list[Aim] = []
         self.functions_button_clicked: list[Callable] = []
+        self.aims_in_row: int = 2
 
     def add_function_called_if_button_clicked(self, function_to_be_called: Callable) -> None:
         """
         This function calls the function_to_be_called whenever the Page is changed.
 
         Parameters
         ----------
@@ -262,16 +263,17 @@
         upper_frame.setFrameShape(QtW.QFrame.StyledPanel)
         upper_frame.setFrameShadow(QtW.QFrame.Raised)
         upper_frame.setSizePolicy(QtW.QSizePolicy.Minimum, QtW.QSizePolicy.Minimum)
         grid_layout = QtW.QGridLayout(upper_frame)
         grid_layout.setVerticalSpacing(6)
         grid_layout.setHorizontalSpacing(6)
         scroll_area_layout.addWidget(upper_frame)
+        rows = list(range(self.aims_in_row)) * len(self.upper_frame)
         for idx, option in enumerate(self.upper_frame):
-            option.create_widget(upper_frame, grid_layout, idx)
+            option.create_widget(upper_frame, grid_layout, (int(idx / self.aims_in_row), rows[idx]))
 
         list_aims: list[Aim] = [aim for aim in self.upper_frame if isinstance(aim, Aim)]
         if list_aims:
             for idx, aim in enumerate(list_aims):
                 default_value = 1 if idx == 0 else 0
                 aim.widget.clicked.connect(
                     ft_partial(
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
 function button class script
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import PySide6.QtCore as QtC  # type: ignore
-import PySide6.QtGui as QtG  # type: ignore
-import PySide6.QtWidgets as QtW  # type: ignore
-
-import ScenarioGUI.global_settings as globs
 from . import FunctionButton
 
 if TYPE_CHECKING:  # pragma: no cover
     from collections.abc import Callable
 
+    import PySide6.QtWidgets as QtW  # type: ignore
+
     from ..gui_structure_classes import Category
 
 
 class ResultExport(FunctionButton):
     """
     This class contains all the functionalities of the FunctionButton option in the GUI.
     The FunctionButton can be used to couple a button press to a function call.
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import copy
 from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import PySide6.QtCore as QtC  # type: ignore
 import PySide6.QtGui as QtG  # type: ignore
 import PySide6.QtWidgets as QtW  # type: ignore
-import ScenarioGUI.global_settings as globs
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-from .category import Category
+import ScenarioGUI.global_settings as globs
+
 from ...utils import change_font_size
+from .category import Category
 
 if TYPE_CHECKING:  # pragma: no cover
     from .page import Page
 
 
 class ResultFigure(Category):
     """
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/result_text.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/gui_structure_classes/text_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/status_bar_logger.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/status_bar_logger.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/gui_classes/translation_class.py` & `ScenarioGUI-0.2.2/ScenarioGUI/gui_classes/translation_class.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/translation_csv_to_py.py` & `ScenarioGUI-0.2.2/ScenarioGUI/translation_csv_to_py.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/utils/change_font_size.py` & `ScenarioGUI-0.2.2/ScenarioGUI/utils/change_font_size.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    import PySide6.QtWidgets as QtW
     import PySide6.QtGui as QtG
+    import PySide6.QtWidgets as QtW
 
 
 def change_font_size(widget: QtW.QWidget | QtG.QAction, size: int, scale_min_height: bool = False) -> None:
     """
     change the font size of the widget
 
     Parameters
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI/utils/set_default_font.py` & `ScenarioGUI-0.2.2/ScenarioGUI/utils/set_default_font.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
-import ScenarioGUI.global_settings as globs
-
 from typing import TYPE_CHECKING
 
+import ScenarioGUI.global_settings as globs
+
 if TYPE_CHECKING:
-    import PySide6.QtWidgets as QtW
     import PySide6.QtGui as QtG
+    import PySide6.QtWidgets as QtW
 
 
 def set_default_font(widget: QtW.QWidget | QtG.QAction, *, bold: bool = False, add_2_size: int = 0) -> None:
     """
     change the font size of the widget
 
     Parameters
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI.egg-info/PKG-INFO` & `ScenarioGUI-0.2.2/ScenarioGUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScenarioGUI
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package for a scenario based GUI
 Home-page: https://github.com/tblanke/ScenarioGUI
 Author: Tobias Blanke
 Author-email: blanke@fh-aachen.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -116,14 +116,16 @@
         super().__init__(default_parent, translations)
         # add a first page called "Inputs" and has a button name of "Input" and has an icon "Add.svg"
         self.page_inputs = els.Page(name="Inputs", button_name="Input", icon="Add.svg")
         # Then several aims can be added to the page with different names and icons
         self.aim_add = els.Aim(label="Adding", icon="Add", page=self.page_inputs)
         self.aim_sub = els.Aim(label="Substract", icon="Delete", page=self.page_inputs)
         self.aim_plot = els.Aim(label="Plot", icon="Parameters", page=self.page_inputs)
+        # this three aims can appear in one row by setting:
+        self.page_inputs.aims_in_row = 3
         # a category with the label "Inputs" can be added to the inputs page like:
         self.category_inputs = els.Category(label="Inputs", page=self.page_inputs)
         # an integer box can be added with different options like this (some of these options are optional):
         self.int_a = els.IntBox(label="a",default_value=2,minimal_value=0,maximal_value=200,step=2,category=self.category_inputs)
         # a float box can be added with different options like this (some of these options are optional):
         self.float_b = els.FloatBox(
             label="b",
```

### Comparing `ScenarioGUI-0.2.1/ScenarioGUI.egg-info/SOURCES.txt` & `ScenarioGUI-0.2.2/ScenarioGUI.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,40 +23,45 @@
 ScenarioGUI/gui_classes/gui_structure_classes/aim.py
 ScenarioGUI/gui_classes/gui_structure_classes/button_box.py
 ScenarioGUI/gui_classes/gui_structure_classes/category.py
 ScenarioGUI/gui_classes/gui_structure_classes/figure_option.py
 ScenarioGUI/gui_classes/gui_structure_classes/filename_box.py
 ScenarioGUI/gui_classes/gui_structure_classes/flexible_amount_option.py
 ScenarioGUI/gui_classes/gui_structure_classes/float_box.py
+ScenarioGUI/gui_classes/gui_structure_classes/float_box_with_units.py
 ScenarioGUI/gui_classes/gui_structure_classes/function_button.py
 ScenarioGUI/gui_classes/gui_structure_classes/functions.py
 ScenarioGUI/gui_classes/gui_structure_classes/hint.py
 ScenarioGUI/gui_classes/gui_structure_classes/int_box.py
+ScenarioGUI/gui_classes/gui_structure_classes/int_box_with_units.py
 ScenarioGUI/gui_classes/gui_structure_classes/list_box.py
 ScenarioGUI/gui_classes/gui_structure_classes/option.py
 ScenarioGUI/gui_classes/gui_structure_classes/page.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_export.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_figure.py
 ScenarioGUI/gui_classes/gui_structure_classes/result_text.py
 ScenarioGUI/gui_classes/gui_structure_classes/text_box.py
 ScenarioGUI/utils/__init__.py
 ScenarioGUI/utils/change_font_size.py
+ScenarioGUI/utils/load_config_file.py
 ScenarioGUI/utils/set_default_font.py
 tests/__init__.py
 tests/gui_structure_for_tests.py
 tests/result_creating_class_for_tests.py
 tests/test_gui_structure_elements/__init__.py
 tests/test_gui_structure_elements/test_aim.py
 tests/test_gui_structure_elements/test_button_box.py
 tests/test_gui_structure_elements/test_category.py
 tests/test_gui_structure_elements/test_filename.py
 tests/test_gui_structure_elements/test_flexible_amount_option.py
 tests/test_gui_structure_elements/test_float_box.py
+tests/test_gui_structure_elements/test_float_box_with_units.py
 tests/test_gui_structure_elements/test_function_button.py
 tests/test_gui_structure_elements/test_int_box.py
+tests/test_gui_structure_elements/test_int_box_with_units.py
 tests/test_gui_structure_elements/test_list_box.py
 tests/test_gui_structure_elements/test_page.py
 tests/test_gui_structure_elements/test_repr.py
 tests/test_gui_structure_elements/test_result_export.py
 tests/test_gui_structure_elements/test_results_figure.py
 tests/test_gui_structure_elements/test_results_text.py
 tests/test_gui_structure_elements/test_text_box.py
```

### Comparing `ScenarioGUI-0.2.1/pyproject.toml` & `ScenarioGUI-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 build-backend = "setuptools.build_meta"
 
 [pytest]
 collect_ignore = ["GHEtool/gui/start_gui.py"]
 collect_ignore_glob = ["*start_gui.py"]
 timeout = 20
 
+[tool.pytest.ini_options]
+qt_api="pyside6"
 
 [tool.black]
 line-length = 160
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
```

### Comparing `ScenarioGUI-0.2.1/setup.cfg` & `ScenarioGUI-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 6365 6e61 7269 6f47 5549 0d0a   = ScenarioGUI..
-00000020: 7665 7273 696f 6e20 3d20 302e 322e 310d  version = 0.2.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 322e 320d  version = 0.2.2.
 00000030: 0a61 7574 686f 7220 3d20 546f 6269 6173  .author = Tobias
 00000040: 2042 6c61 6e6b 650d 0a61 7574 686f 725f   Blanke..author_
 00000050: 656d 6169 6c20 3d20 626c 616e 6b65 4066  email = blanke@f
 00000060: 682d 6161 6368 656e 2e64 650d 0a64 6573  h-aachen.de..des
 00000070: 6372 6970 7469 6f6e 203d 2050 7974 686f  cription = Pytho
 00000080: 6e20 7061 636b 6167 6520 666f 7220 6120  n package for a 
 00000090: 7363 656e 6172 696f 2062 6173 6564 2047  scenario based G
```

### Comparing `ScenarioGUI-0.2.1/tests/gui_structure_for_tests.py` & `ScenarioGUI-0.2.2/tests/gui_structure_for_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from ScenarioGUI import GuiStructure
+from ScenarioGUI import elements as els
 from ScenarioGUI.gui_classes.gui_structure_classes import (
     Aim,
     ButtonBox,
     Category,
     FigureOption,
     FileNameBox,
     FlexibleAmount,
@@ -32,14 +33,16 @@
 class GUI(GuiStructure):
     def __init__(self, default_parent: QtW.QWidget, translations: Translations):
         super().__init__(default_parent, translations)
         self.page_inputs = Page(name="Inputs", button_name="Inputs", icon="Add.svg")
         self.aim_add = Aim(label=self.translations.aim_add, icon="Add", page=self.page_inputs)
         self.aim_sub = Aim(label=self.translations.aim_sub, icon="Delete", page=self.page_inputs)
         self.aim_plot = Aim(label="Plot", icon="Parameters", page=self.page_inputs)
+        # set three aims per row
+        self.page_inputs.aims_in_row = 3
         self.category_inputs = Category(page=self.page_inputs, label="Inputs")
         self.int_a = IntBox(
             label="a",
             default_value=2,
             minimal_value=0,
             maximal_value=200,
             category=self.category_inputs,
@@ -49,17 +52,37 @@
             label="b",
             default_value=100,
             minimal_value=0,
             maximal_value=1000,
             decimal_number=2,
             category=self.category_inputs,
         )
+        self.int_units = els.IntBoxWithUnits(
+            label="IntBoxWithUnits",
+            default_value=2,
+            minimal_value=0,
+            maximal_value=2_000_000,
+            category=self.category_inputs,
+            units=[("kW", 1), ("W", 0.001), ("MW", 1_000)]
+        )
+
+        self.float_units = els.FloatBoxWithUnits(
+            label="FloatBoxWithUnits",
+            default_value=2,
+            minimal_value=0,
+            maximal_value=2_000_000,
+            decimal_number=2,
+            category=self.category_inputs,
+            units=[("kW", 1), ("W", 0.001), ("MW", 1_000)]
+        )
+        self.float_units.activate_scale_decimals()
         folder: Path = Path(__file__).parent
         file = f'{folder.joinpath("./example_data.csv")}'
         self.filename = FileNameBox(label="Filename", default_value=file, category=self.category_inputs, dialog_text="Hello", error_text="no file found")
+        self.filename.check_active = True
 
         self.function_button = FunctionButton(button_text=translations.function_button, icon="Add", category=self.category_inputs)
 
         self.button_box = ButtonBox(label="a or b?", default_index=0, entries=["a", "b"], category=self.category_inputs)
 
         self.list_box = ListBox(
             label="List box",
```

### Comparing `ScenarioGUI-0.2.1/tests/result_creating_class_for_tests.py` & `ScenarioGUI-0.2.2/tests/result_creating_class_for_tests.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_aim.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_aim.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_button_box.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_button_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_category.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_category.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_filename.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_filename.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import partial
 from pathlib import Path
 
 import PySide6.QtWidgets as QtW
+
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
 from ..gui_structure_for_tests import GUI
 from ..result_creating_class_for_tests import ResultsClass, data_2_results
 from ..test_translations.translation_class import Translations
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_flexible_amount_option.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_flexible_amount_option.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,8 +78,15 @@
     flex_option.set_text("label_text,row,str,float,int,list")
     assert flex_option.label.text() == "label_text"
     assert flex_option.frame.layout().itemAtPosition(1, 0).widget().text() == "row 1"
     assert flex_option.frame.layout().itemAtPosition(0, 2).widget().text() == "str"
     assert flex_option.frame.layout().itemAtPosition(0, 3).widget().text() == "float"
     assert flex_option.frame.layout().itemAtPosition(0, 4).widget().text() == "int"
     assert flex_option.frame.layout().itemAtPosition(0, 5).widget().text() == "list"
+
+    flex_option.hide()
+    assert flex_option.frame.isHidden()
+    assert flex_option.label.isHidden()
+    flex_option.show()
+    assert not flex_option.frame.isHidden()
+    assert not flex_option.label.isHidden()
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_float_box.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_float_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_function_button.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_function_button.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_int_box.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_int_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_list_box.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_list_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_page.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_results_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 from tests.gui_structure_for_tests import GUI
 from tests.result_creating_class_for_tests import ResultsClass, data_2_results
 from tests.test_translations.translation_class import Translations
 
 
-def test_page(qtbot):
+def test_results_text(qtbot):
     # init gui window
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     main_window.delete_backup()
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
-
-    main_window.gui_structure.page_result.set_text("button name,Name")
-    assert main_window.gui_structure.page_result.button.text() == "button name"
-    assert main_window.gui_structure.page_result.label.text() == "Name"
-
-    # test linked function which counts the counter every time button is clicked
-    assert main_window.gui_structure.counter == 1
-    main_window.gui_structure.page_inputs.button.click()
-    assert main_window.gui_structure.counter == 2
+    # get sum
+    sum_ab = main_window.gui_structure.int_a.get_value() + main_window.gui_structure.float_b.get_value()
+    main_window.gui_structure.result_text_add.set_text("Hello,kW")
+    # calc sum from gui
+    main_window.save_scenario()
+    main_window.start_current_scenario_calculation(False)
+    qtbot.wait(1500)
+    assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
+    # check text output
+    assert main_window.gui_structure.result_text_add.label.text() == f"Hello{sum_ab}kW"
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_repr.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_repr.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_result_export.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_result_export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
 from functools import partial
 from pathlib import Path
 
 import PySide6.QtWidgets as QtW
-from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
+from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 from tests.gui_structure_for_tests import GUI
 from tests.result_creating_class_for_tests import ResultsClass, data_2_results
 from tests.test_translations.translation_class import Translations
 
 
 def test_results_export(qtbot):
     # init gui window
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     main_window.delete_backup()
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
+    qtbot.wait(1500)
     folder = Path(__file__).parent.parent
     file = f'{folder.joinpath("./test_export.txt")}'
     # delete files if they already exists
     if os.path.exists(main_window.default_path.joinpath(file)):  # pragma: no cover
         os.remove(main_window.default_path.joinpath(file))
 
     def get_save_file_name(*args, **kwargs):
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_figure.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_results_figure.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     main_window.delete_backup()
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     # get sum
     main_window.gui_structure.figure_results.set_text("Hello,Y-Values,X-Values")
     # calc sum from gui
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
+    qtbot.wait(1500)
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
     # check text output
     assert main_window.gui_structure.figure_results.label.text() == "Hello"
     assert main_window.gui_structure.figure_results.a_x.get_ylabel() == "Y-Values"
     assert main_window.gui_structure.figure_results.a_x.get_xlabel() == "X-Values"
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_results_text.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_no_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import PySide6.QtWidgets as QtW
 
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
-from tests.gui_structure_for_tests import GUI
-from tests.result_creating_class_for_tests import ResultsClass, data_2_results
-from tests.test_translations.translation_class import Translations
 
+from ..gui_structure_for_tests import GUI
+from ..result_creating_class_for_tests import ResultsClass, data_2_results
+from ..test_translations.translation_class import Translations
+
+
+def test_no_load_save_file(qtbot):
+    """
+    test if the GUI handles wrong load and save inputs correctly
+
+    Parameters
+    ----------
+    qtbot: qtbot
+        bot for the GUI
+    """
 
-def test_results_text(qtbot):
     # init gui window
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     main_window.delete_backup()
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
-    # get sum
-    sum_ab = main_window.gui_structure.int_a.get_value() + main_window.gui_structure.float_b.get_value()
-    main_window.gui_structure.result_text_add.set_text("Hello,kW")
-    # calc sum from gui
-    main_window.save_scenario()
-    main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
-    assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
-    # check text output
-    assert main_window.gui_structure.result_text_add.label.text() == f"Hello{sum_ab}kW"
+    # check if an import error has been raises with a wrong load file
+    main_window._load_from_data("not_there.GHEtool")
+    assert main_window.status_bar.widget.currentMessage() == main_window.translations.no_file_selected[0]
+    # check if the current error message is shown with a wrong save file/folder
+    main_window._save_to_data("hello/not_there.GHEtool")
+    assert main_window.status_bar.widget.currentMessage() == main_window.translations.no_file_selected[main_window.gui_structure.option_language.get_value()[0]]
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_gui_structure_elements/test_text_box.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_text_box.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_auto_save.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_auto_save.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,8 +51,10 @@
         main_window.delete_scenario()
         assert len(main_window.list_ds) == 10 - i
         assert main_window.list_widget_scenario.count() == 10 - i
     # check if deleting the last scenario is ignored so at least one exists
     main_window.delete_scenario()
     assert len(main_window.list_ds) == 1
     assert main_window.list_widget_scenario.count() == 1
+
+    main_window.gui_structure.option_auto_saving.set_value(0)
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_backup.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_backup.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_change_font_size.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_change_font_size.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
+
 from pathlib import Path
 
-import PySide6.QtWidgets as QtW
 import PySide6.QtGui as QtG
+import PySide6.QtWidgets as QtW
+
 from ScenarioGUI import load_config
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
 from ..gui_structure_for_tests import GUI
 from ..result_creating_class_for_tests import ResultsClass, data_2_results
 from ..test_translations.translation_class import Translations
 
@@ -38,34 +40,43 @@
     check_font_size(main_window.status_bar.widget, 8)
     check_font_size(main_window.menu_settings, 8)
     check_font_size(main_window.menubar, 8)
     check_font_size(main_window.menu_scenario, 8)
     check_font_size(main_window.menu_calculation, 8)
     check_font_size(main_window.menu_language, 8)
     check_font_size(main_window.menu_file, 8)
+    check_font_size(main_window.progress_bar, 8)
+    check_font_size(main_window.label_status, 8)
     # test page settings
     check_font_size(main_window.gui_structure.page_result.label, 8 + 4)
     check_font_size(main_window.gui_structure.page_result.button, 8)
     check_font_size(main_window.gui_structure.page_result.push_button_previous, 8)
     check_font_size(main_window.gui_structure.page_result.push_button_next, 8)
     # test option settings
     check_font_size(main_window.gui_structure.int_a.label, 8)
     check_font_size(main_window.gui_structure.int_a.widget, 8)
     check_font_size(main_window.gui_structure.float_b.label, 8)
     check_font_size(main_window.gui_structure.float_b.widget, 8)
     check_font_size(main_window.gui_structure.filename.label, 8)
     check_font_size(main_window.gui_structure.filename.widget, 8)
     check_font_size(main_window.gui_structure.list_box.label, 8)
     check_font_size(main_window.gui_structure.list_box.widget, 8)
+    check_font_size(main_window.gui_structure.float_units.label, 8)
+    check_font_size(main_window.gui_structure.float_units.widget, 8)
+    check_font_size(main_window.gui_structure.float_units.unit_widget, 8)
+    check_font_size(main_window.gui_structure.int_units.label, 8)
+    check_font_size(main_window.gui_structure.int_units.widget, 8)
+    check_font_size(main_window.gui_structure.int_units.unit_widget, 8)
     check_font_size(main_window.gui_structure.function_button.button, 8)
     check_font_size(main_window.gui_structure.button_box.label, 8)
     [check_font_size(widget, 8) for widget in main_window.gui_structure.button_box.widget]
     check_font_size(main_window.gui_structure.hint_flex.label, 8)
     check_font_size(main_window.gui_structure.aim_add.widget, 8)
     check_font_size(main_window.gui_structure.category_inputs.label, 8)
     check_font_size(main_window.gui_structure.flex_option.label, 8)
     [check_font_size(widget, 8) for widget in main_window.gui_structure.flex_option.frame.children() if isinstance(widget, QtW.QWidget)]
-    
+
+
 def check_font_size(widget: QtW.QWidget | QtG.QAction, size: int):
     font = widget.font()
     assert font.pointSize() == size
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_close.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_close.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from functools import partial
 
 import PySide6.QtCore as QtC
 import PySide6.QtWidgets as QtW
+
 import ScenarioGUI.global_settings as globs
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
 from ..gui_structure_for_tests import GUI
 from ..result_creating_class_for_tests import ResultsClass, data_2_results
 from ..test_translations.translation_class import Translations
 
@@ -30,37 +31,29 @@
     # set filenames
     filename_1 = f"test_1.{globs.FILE_EXTENSION}"
     # delete files if they already exists
     if os.path.exists(main_window.default_path.joinpath(filename_1)):  # pragma: no cover
         os.remove(main_window.default_path.joinpath(filename_1))
 
     def close():
-        while main_window.dialog is None:  # pragma: no cover
-            QtW.QApplication.processEvents()
         # handle dialog now
         if isinstance(main_window.dialog, QtW.QMessageBox):
             main_window.dialog.close()
 
     def cancel():
-        while main_window.dialog is None:  # pragma: no cover
-            QtW.QApplication.processEvents()
         # handle dialog now
         if isinstance(main_window.dialog, QtW.QMessageBox):
             main_window.dialog.buttons()[2].click()
 
     def exit_window():
-        while main_window.dialog is None:  # pragma: no cover
-            QtW.QApplication.processEvents()
         # handle dialog now
         if isinstance(main_window.dialog, QtW.QMessageBox):
             main_window.dialog.buttons()[1].click()
 
     def save():
-        while main_window.dialog is None:  # pragma: no cover
-            QtW.QApplication.processEvents()
         # handle dialog now
         if isinstance(main_window.dialog, QtW.QMessageBox):
             main_window.dialog.buttons()[0].click()
 
     QtC.QTimer.singleShot(500, close)
     main_window.close()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_datastorage.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_datastorage.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_double_naming.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_double_naming.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_global_settings.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_global_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
+
 from pathlib import Path
 from platform import system
 
-import PySide6.QtWidgets as QtW
 import PySide6.QtGui as QtG
+import PySide6.QtWidgets as QtW
 from pytest import raises
+
 from ScenarioGUI import global_settings as globs
 from ScenarioGUI import load_config
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
 from ..gui_structure_for_tests import GUI
 from ..result_creating_class_for_tests import ResultsClass, data_2_results
 from ..test_translations.translation_class import Translations
@@ -37,36 +39,38 @@
     assert globs.LIGHT_SELECT == "rgb(42, 126, 179)"
     assert globs.DARK == "rgb(0, 64, 122)"
     assert globs.GREY == "rgb(100, 100, 100)"
     assert globs.WARNING == "rgb(255, 200, 87)"
     assert globs.BLACK == "rgb(0, 0, 0)"
 
     assert globs.FILE_EXTENSION == "scenario"
+    assert main_window._backup_filename == "backup.scenarioBackUp"
     assert globs.GUI_NAME == "Scenario GUI"
     assert globs.ICON_NAME == "icon.svg"
     assert globs.path.joinpath(".").parent if "tests" in f"{Path('.').absolute()}" else globs.path.joinpath(".") == globs.FOLDER
     # test get_path_for_file function
     assert globs.get_path_for_file(globs.path.joinpath("./ScenarioGUI/gui_classes/gui_structure_classes"), "gui_config.ini")  in [globs.path.parent.joinpath(
         "." if "tests" in f"{Path('.').absolute()}" else "./examples"), globs.path.parent.joinpath("." if "tests" in f"{Path('.').absolute()}" else "./tests")]
     # test combine window settings
-
     check_font(main_window.push_button_cancel, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.push_button_start_single, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.push_button_start_multiple, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.push_button_add_scenario, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.push_button_delete_scenario, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.push_button_save_scenario, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.button_rename_scenario, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.status_bar.widget, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menu_settings, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menubar, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menu_scenario, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menu_calculation, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menu_language, globs.FONT_SIZE, globs.FONT, False)
     check_font(main_window.menu_file, globs.FONT_SIZE, globs.FONT, False)
+    check_font(main_window.progress_bar, globs.FONT_SIZE, globs.FONT, False)
+    check_font(main_window.label_status, globs.FONT_SIZE, globs.FONT, False)
     # test page settings
     check_font(main_window.gui_structure.page_result.label, globs.FONT_SIZE + 4, globs.FONT, True)
     check_font(main_window.gui_structure.page_result.button, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.gui_structure.page_result.push_button_previous, globs.FONT_SIZE, globs.FONT, True)
     check_font(main_window.gui_structure.page_result.push_button_next, globs.FONT_SIZE, globs.FONT, True)
     # test option settings
     check_font(main_window.gui_structure.int_a.label, globs.FONT_SIZE, globs.FONT, False)
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_move_scenario.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_move_scenario.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_new_save_load.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_new_save_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from functools import partial
 from pathlib import Path
 
 import numpy as np
 import PySide6.QtWidgets as QtW
+
 import ScenarioGUI.global_settings as global_vars
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
 
 from ..gui_structure_for_tests import GUI
 from ..result_creating_class_for_tests import ResultsClass, data_2_results
 from ..test_translations.translation_class import Translations
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_no_file.py` & `ScenarioGUI-0.2.2/tests/test_gui_structure_elements/test_page.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import PySide6.QtWidgets as QtW
 
 from ScenarioGUI.gui_classes.gui_combine_window import MainWindow
+from tests.gui_structure_for_tests import GUI
+from tests.result_creating_class_for_tests import ResultsClass, data_2_results
+from tests.test_translations.translation_class import Translations
 
-from ..gui_structure_for_tests import GUI
-from ..result_creating_class_for_tests import ResultsClass, data_2_results
-from ..test_translations.translation_class import Translations
-
-
-def test_no_load_save_file(qtbot):
-    """
-    test if the GUI handles wrong load and save inputs correctly
-
-    Parameters
-    ----------
-    qtbot: qtbot
-        bot for the GUI
-    """
 
+def test_page(qtbot):
     # init gui window
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
     main_window.delete_backup()
     main_window = MainWindow(QtW.QMainWindow(), qtbot, GUI, Translations, result_creating_class=ResultsClass, data_2_results_function=data_2_results)
-    # check if an import error has been raises with a wrong load file
-    main_window._load_from_data("not_there.GHEtool")
-    assert main_window.status_bar.widget.currentMessage() == main_window.translations.no_file_selected[0]
-    # check if the current error message is shown with a wrong save file/folder
-    main_window._save_to_data("hello/not_there.GHEtool")
-    assert main_window.status_bar.widget.currentMessage() == main_window.translations.no_file_selected[main_window.gui_structure.option_language.get_value()[0]]
+
+    main_window.gui_structure.page_result.set_text("button name,Name")
+    assert main_window.gui_structure.page_result.button.text() == "button name"
+    assert main_window.gui_structure.page_result.label.text() == "Name"
+
+    # test linked function which counts the counter every time button is clicked
+    assert main_window.gui_structure.counter == 1
+    main_window.gui_structure.page_inputs.button.click()
+    assert main_window.gui_structure.counter == 2
+    # check that 3 aim are in a row
+    scroll_area = [widget for widget in main_window.gui_structure.page_inputs.page.children() if isinstance(widget, QtW.QScrollArea)][0]
+    assert scroll_area.children()[0].children()[0].children()[1].children()[0].rowCount() == 1
+    assert scroll_area.children()[0].children()[0].children()[1].children()[0].columnCount() == 3
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_push_button_change.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_push_button_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_rename_scenario.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_rename_scenario.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_run.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,76 +32,74 @@
     main_window.start_multiple_scenarios_calculation()
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is None
     main_window.gui_structure.filename.set_value(file)
 
     main_window.gui_structure.aim_add.widget.click()
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
+    qtbot.wait(1500)
 
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
 
     main_window.remove_previous_calculated_results()
 
     main_window.gui_structure.aim_sub.widget.click()
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
+    qtbot.wait(1500)
 
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
     main_window.start_current_scenario_calculation(False)
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
     main_window.start_multiple_scenarios_calculation()
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
 
     main_window.remove_previous_calculated_results()
 
     main_window.gui_structure.aim_plot.widget.click()
     assert main_window.gui_structure.aim_plot.widget.isChecked()
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(False)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        QtW.QApplication.processEvents()
+    qtbot.wait(1500)
 
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
     item = main_window.list_widget_scenario.currentItem()
     main_window.add_scenario()
     main_window.gui_structure.int_a.set_value(main_window.gui_structure.int_a.get_value() + 5)
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(True)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        main_window.threads[0].run()
-        main_window.threads[0].any_signal.connect(main_window.thread_function)
-        main_window.display_results()
+    main_window.threads[-1].run()
+    main_window.threads[-1].any_signal.connect(main_window.thread_function)
+    qtbot.wait(1500)
+    main_window.display_results()
 
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
     main_window.list_widget_scenario.setCurrentItem(item)
     main_window.display_results()
     main_window.gui_structure.legend_figure_results.set_value(("", 1))
 
     main_window.remove_previous_calculated_results()
     # test value error results
     main_window.gui_structure.aim_sub.widget.click()
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(True)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        main_window.threads[0].run()
-        main_window.threads[0].any_signal.connect(main_window.thread_function)
-        main_window.display_results()
+    main_window.threads[-1].run()
+    main_window.threads[-1].any_signal.connect(main_window.thread_function)
+    qtbot.wait(1500)
+    main_window.display_results()
+
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is not None
 
     main_window.gui_structure.int_a.set_value(192)
     main_window.save_scenario()
     main_window.start_current_scenario_calculation(True)
-    with qtbot.waitSignal(main_window.threads[0].any_signal, raising=False):
-        main_window.threads[0].run()
-        main_window.threads[0].any_signal.connect(main_window.thread_function)
-        main_window.display_results()
+    main_window.threads[-1].run()
+    main_window.threads[-1].any_signal.connect(main_window.thread_function)
+    qtbot.wait(1500)
+    main_window.display_results()
 
     assert f"{main_window.list_ds[main_window.list_widget_scenario.currentRow()].debug_message}" == "Value above 190"
 
     assert main_window.list_ds[main_window.list_widget_scenario.currentRow()].results is None
 
     main_window.remove_previous_calculated_results()
     main_window.delete_backup()
```

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_change.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_scenario_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_scenario_properties.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_scenario_properties.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_main_window_functions/test_toggle_buttons.py` & `ScenarioGUI-0.2.2/tests/test_main_window_functions/test_toggle_buttons.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_translations/test_language_change.py` & `ScenarioGUI-0.2.2/tests/test_translations/test_language_change.py`

 * *Files identical despite different names*

### Comparing `ScenarioGUI-0.2.1/tests/test_translations/test_translation_csv_2_py.py` & `ScenarioGUI-0.2.2/tests/test_translations/test_translation_csv_2_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import pandas as pd
+
 from ScenarioGUI.translation_csv_to_py import translate_csv_2_class
 
 
 def test_csv_2_py():
     folder: Path = Path(__file__).parent
     translate_csv_2_class(folder.joinpath("Translations.csv"), folder)
     d_f = pd.read_csv(folder.joinpath("Translations.csv"), sep=";")
```

### Comparing `ScenarioGUI-0.2.1/tests/test_translations/translation_class.py` & `ScenarioGUI-0.2.2/tests/test_translations/translation_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         "category_save_scenario",
         "option_auto_saving",
         "hint_saving",
         "aim_add",
         "aim_sub",
         "float_b",
         "function_button",
+        "option_font_size",
         "languages",
     )
 
     def __init__(self):
         self.languages: list[str] = ["English", "German"]
         self.action_add_scenario: list[str] = ["Add scenario", "Szenario hinzufügen"]
         self.action_delete_scenario: list[str] = ["Delete scenario", "Szenario löschen"]
@@ -149,7 +150,8 @@
             "If Auto saving is selected the scenario will automatically saved if a scenario is changed. Otherwise the scenario has to be saved with the Update scenario button in the upper left corner if the changes should not be lost.",
             "Wenn Automatisch speichern ausgewählt ist, wird das Szenario automatisch gespeichert, wenn ein Szenario geändert wird. Andernfalls muss das Szenario mit der Schaltfläche Szenario aktualisieren in der oberen linken Ecke gespeichert werden, wenn die Änderungen nicht verloren gehen sollen.",
         ]
         self.aim_add: list[str] = ["Adding", "Addieren"]
         self.aim_sub: list[str] = ["Substract", "Subtrahieren"]
         self.float_b: list[str] = ["nothing", "nothing"]
         self.function_button: list[str] = ["call function", "Rufe Funktion"]
+        self.option_font_size: list[str] = ["Font Size", "Schriftgröße"]
```

