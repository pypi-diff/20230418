# Comparing `tmp/domino_code_assist-1.1.4.tar.gz` & `tmp/domino_code_assist-1.2.0.tar.gz`

## Comparing `domino_code_assist-1.1.4.tar` & `domino_code_assist-1.2.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/DominoLogoGrey.svg
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/DominoLogoWhite.svg
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/__init__.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/action.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/action_ui.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/actions_store.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/app.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/app_entrypoint.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/code.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/code.vue
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/components.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/crossfilter_widgets.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/css.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/css.vue
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/df_select.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/df_select.vue
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/domino_api.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/domino_lab_mock.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/express.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/hooks.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/layout.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/logging_workaround.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/nb_app.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/py36.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/sample_project_md.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/serialize.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/settings.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/thumbnail.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/util.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/widgets.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/__init__.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/assistant.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/assistant.vue
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/drawer.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/drawer.vue
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/handle_user_install.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/menu.vue
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/mixpanel.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/mixpanel.vue
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/assistant/notebook.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/data/__init__.py
--rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/data/penguins.csv
--rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/data/small_molecule_drugbank.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/app_checker.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/app_checker.vue
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/button_clipboard.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/button_clipboard.vue
--rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/deploy-sync.png
--rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/deployer.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/filesystem_watcher.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/deploy/filesystem_watcher.vue
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/jupyter/__init__.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/jupyter/mixpanel_handler.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/jupyter/server_extension.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/__init__.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/big_query.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/data_source.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/drawer.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/object_store.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/panel.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/quick_start.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/snowflake_redshift.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/load_data/state.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/app.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/assistant.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/load_data.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/notebook.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/playwright/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/snippets/__init__.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/snippets/snippet_drawer.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/snippets/snippets.py
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/snippets/snippets_ui.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/snippets/tree.vue
--rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/app.png
--rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/code_inserted.png
--rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/hover_cell.png
--rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/hover_icon.png
--rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/load_data.png
--rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/menu.png
--rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/menu_app.png
--rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/menu_transform.png
--rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/menu_visualizations.png
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/tour.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/tour.vue
--rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/transform.png
--rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/tour/visualizations.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/column_description.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/column_description.vue
--rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/transform_action_ui.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/transform_drawer.py
--rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/transform/transform_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/viz/__init__.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/viz/drawer.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/viz/plot_builder.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/domino_code_assist/viz/state.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/app.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/app_entrypoint.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/deploy.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/express.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/layout.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/low_code_assistant/widgets.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/LICENSE.md
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 domino_code_assist-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/DominoLogoGrey.svg
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/DominoLogoWhite.svg
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/__init__.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/action.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/action_ui.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/actions_store.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/app.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/app_entrypoint.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/code.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/code.vue
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/components.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/crossfilter_widgets.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/css.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/css.vue
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/df_select.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/df_select.vue
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/domino_api.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/domino_lab_mock.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/express.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/hooks.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/layout.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/logging_workaround.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/nb_app.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/py36.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/sample_project_md.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/serialize.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/settings.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/thumbnail.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/util.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/widgets.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/__init__.py
+-rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.vue
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.vue
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/handle_user_install.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/menu.vue
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.vue
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/notebook.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/__init__.py
+-rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/penguins.csv
+-rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/small_molecule_drugbank.csv
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/stocks_long.parquet
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.vue
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.vue
+-rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/deploy-sync.png
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/deployer.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.vue
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/mixpanel_handler.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/server_extension.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/__init__.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/big_query.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/data_source.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/drawer.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/object_store.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/panel.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/quick_start.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/snowflake_redshift.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/state.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/app.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/assistant.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/load_data.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/notebook.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippet_drawer.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippets.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippets_ui.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/tree.vue
+-rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/app.png
+-rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/code_inserted.png
+-rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/hover_cell.png
+-rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/hover_icon.png
+-rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/load_data.png
+-rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu.png
+-rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_app.png
+-rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_transform.png
+-rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_visualizations.png
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/tour.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/tour.vue
+-rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/transform.png
+-rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/visualizations.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/column_description.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/column_description.vue
+-rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_action_ui.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_drawer.py
+-rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/__init__.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/drawer.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/plot_builder.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/state.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/app.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/app_entrypoint.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/deploy.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/express.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/layout.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/widgets.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/PKG-INFO
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/DominoLogoGrey.svg` & `domino_code_assist-1.2.0/domino_code_assist/DominoLogoGrey.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/DominoLogoWhite.svg` & `domino_code_assist-1.2.0/domino_code_assist/DominoLogoWhite.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/__init__.py` & `domino_code_assist-1.2.0/domino_code_assist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dominocode"""
 
-__version__ = "1.1.4"
+__version__ = "1.2.0"
 
 import os
 
 # isort: skip_file
 
 import domino_code_assist.logging_workaround
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/action.py` & `domino_code_assist-1.2.0/domino_code_assist/action.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/action_ui.py` & `domino_code_assist-1.2.0/domino_code_assist/action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/actions_store.py` & `domino_code_assist-1.2.0/domino_code_assist/actions_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/app.py` & `domino_code_assist-1.2.0/domino_code_assist/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/app_entrypoint.py` & `domino_code_assist-1.2.0/domino_code_assist/app_entrypoint.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/code.py` & `domino_code_assist-1.2.0/domino_code_assist/code.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/code.vue` & `domino_code_assist-1.2.0/domino_code_assist/code.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/components.py` & `domino_code_assist-1.2.0/domino_code_assist/components.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/crossfilter_widgets.py` & `domino_code_assist-1.2.0/domino_code_assist/crossfilter_widgets.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/df_select.py` & `domino_code_assist-1.2.0/domino_code_assist/df_select.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/domino_api.py` & `domino_code_assist-1.2.0/domino_code_assist/domino_api.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/domino_lab_mock.py` & `domino_code_assist-1.2.0/domino_code_assist/domino_lab_mock.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/layout.py` & `domino_code_assist-1.2.0/domino_code_assist/layout.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/nb_app.py` & `domino_code_assist-1.2.0/domino_code_assist/nb_app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/py36.py` & `domino_code_assist-1.2.0/domino_code_assist/py36.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/sample_project_md.py` & `domino_code_assist-1.2.0/domino_code_assist/sample_project_md.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/serialize.py` & `domino_code_assist-1.2.0/domino_code_assist/serialize.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/settings.py` & `domino_code_assist-1.2.0/domino_code_assist/settings.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/thumbnail.py` & `domino_code_assist-1.2.0/domino_code_assist/thumbnail.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/util.py` & `domino_code_assist-1.2.0/domino_code_assist/util.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/assistant.py` & `domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import textwrap
 import traceback
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, cast
+from typing import Any, Callable, Dict, Optional, cast
 
 import ipyvuetify as vy
 import ipywidgets
 import plotly
 import reacton
 import reacton.ipyvuetify as v
 import solara as sol
@@ -486,15 +486,14 @@
     solara.use_memo(sync_notebook_browser_path, dependencies=[notebook_path])
 
     edit_data, set_edit_data = reacton.use_state(cast(Optional[Dict["str", Any]], None))
     markdown_cells, set_markdown_cells = reacton.use_state(cast(Optional[Dict], None))
 
     snippet_saved_count, set_snippet_saved_count = reacton.use_state(0)
     snippet_edit_mode, set_snippet_edit_mode = reacton.use_state(False)
-    writable_paths, set_writable_paths = reacton.use_state(cast(Optional[List[str]], None))
 
     snippet_add_header, set_snippet_add_header = reacton.use_state(cast(Optional[str], None))
     add_dialog_open, set_add_dialog_open = reacton.use_state(False)
 
     def handle_code_up():
         if code_up and code_up.get("type_") == "markdown":
             set_edit_data({"markdown": code_up["code"]})
@@ -519,15 +518,15 @@
                 {
                     "section": selected.get("action"),
                     "edit": bool(selected.get("edit")),
                 },
             )
 
     reacton.use_memo(on_selected, [selected])
-    reacton.use_memo(lambda: set_writable_paths(snippets.get_writable_paths()), [])
+    writable_paths = reacton.use_memo(snippets.get_writable_paths, [])
 
     overwrite = bool(code_up is not None and code_up["code"].strip())
 
     overwrite_warning = sol.use_memo(
         lambda: OverWriteWarning(code_up["code"], code_up.get("type_")) if code_up and selected and not selected.get("edit") and overwrite else None
     )
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/assistant.vue` & `domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/drawer.py` & `domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/drawer.vue` & `domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/handle_user_install.py` & `domino_code_assist-1.2.0/domino_code_assist/assistant/handle_user_install.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/menu.vue` & `domino_code_assist-1.2.0/domino_code_assist/assistant/menu.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/mixpanel.py` & `domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     template_file = (__file__, "mixpanel.vue")
 
     project_token = traitlets.Unicode(allow_none=True).tag(sync=True)
     debug = traitlets.Bool(False).tag(sync=True)
     initialized = traitlets.Bool(False).tag(sync=True)
     unreachable_in_frontend = traitlets.Bool(False).tag(sync=True)
     frontend_props = traitlets.Dict().tag(sync=True)
-    mixpanel_enabled = traitlets.Bool(False).tag(sync=True)
+    mixpanel_enabled = traitlets.Bool(False, allow_none=True).tag(sync=True)
 
     def track(self, event: str, props: Optional[Dict] = None):
         self.send({"method": "track", "args": [event, props]})
 
     def identify(self, unique_id: str):
         self.send({"method": "identify", "args": [unique_id]})
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/assistant/mixpanel.vue` & `domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/data/penguins.csv` & `domino_code_assist-1.2.0/domino_code_assist/data/penguins.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/data/small_molecule_drugbank.csv` & `domino_code_assist-1.2.0/domino_code_assist/data/small_molecule_drugbank.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/app_checker.py` & `domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/app_checker.vue` & `domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/button_clipboard.vue` & `domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/deploy-sync.png` & `domino_code_assist-1.2.0/domino_code_assist/deploy/deploy-sync.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/deployer.py` & `domino_code_assist-1.2.0/domino_code_assist/deploy/deployer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/filesystem_watcher.py` & `domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/deploy/filesystem_watcher.vue` & `domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/jupyter/mixpanel_handler.py` & `domino_code_assist-1.2.0/domino_code_assist/jupyter/mixpanel_handler.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/jupyter/server_extension.py` & `domino_code_assist-1.2.0/domino_code_assist/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/big_query.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/big_query.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/data_source.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/data_source.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/drawer.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/object_store.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/object_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/panel.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/quick_start.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/quick_start.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import reacton.ipyvuetify as v
 from solara.lab import Ref
 
 from .state import load_data
 
 _items = {
     "Quick-start": ["carshare", "election", "iris", "medals_long", "medals_wide", "palmerpenguins", "tips", "wind"],
-    "Economics": ["gapminder", "stocks"],
+    "Economics": ["gapminder", "stocks", "stocks_long"],
     "Pharma": ["experiment", "small_molecule_drugbank"],
 }
 
 
 @reacton.component
 def QuickStart():
     load_data.use()
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/snowflake_redshift.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/snowflake_redshift.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/load_data/state.py` & `domino_code_assist-1.2.0/domino_code_assist/load_data/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/playwright/app.py` & `domino_code_assist-1.2.0/domino_code_assist/playwright/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/playwright/assistant.py` & `domino_code_assist-1.2.0/domino_code_assist/playwright/assistant.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/playwright/load_data.py` & `domino_code_assist-1.2.0/domino_code_assist/playwright/load_data.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/playwright/notebook.py` & `domino_code_assist-1.2.0/domino_code_assist/playwright/notebook.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/playwright/transform.py` & `domino_code_assist-1.2.0/domino_code_assist/playwright/transform.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/snippets/snippet_drawer.py` & `domino_code_assist-1.2.0/domino_code_assist/snippets/snippet_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/snippets/snippets.py` & `domino_code_assist-1.2.0/domino_code_assist/snippets/snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     return [str(p) for p in datasets_dir.glob("*") if p.is_dir() and p != local_dir]
 
 
 def get_shared_git_paths():
     path = settings.domino_repos_dir or settings.domino_imported_code_dir
     if not path:
         return []
-    return [str(p) for p in Path(path).glob("*") if p.is_dir()]
+    return [str(p) for p in Path(path).glob("*") if p.is_dir() and (p / "snippets").is_dir()]
 
 
 def get_prefix_paths():
     return [str(p) for p in settings.domino_snippet_builtin_dir.glob("*") if p.is_dir()]
 
 
 def read_snippets(sub: Path, data: str, base_path: Path) -> List[Snippet]:
@@ -128,15 +128,15 @@
 
 def get_writable_paths():
     git_paths = get_shared_git_paths()
 
     def is_writable(path):
         return 0 == subprocess.run(["git", "push", "--dry-run", "--force", "--no-verify"], cwd=path, stdout=subprocess.PIPE, stderr=subprocess.PIPE).returncode
 
-    return [str(p) for p in git_paths if is_writable(p)] + [str(settings.domino_working_dir)]
+    return [{"path": str(p), "writable": is_writable(p)} for p in git_paths] + [{"path": str(settings.domino_working_dir), "writable": True}]
 
 
 def adjust_path(snippet_map, path: List[Dict]):
     if not path:
         return path
     new_path = path[:1]
     sub_map = snippet_map
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/snippets/snippets_ui.py` & `domino_code_assist-1.2.0/domino_code_assist/snippets/snippets_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         def starts_with(a: Path, b: Path):
             try:
                 b.relative_to(a)
                 return True
             except ValueError:
                 return False
 
-        return any(starts_with(Path(p), path) for p in writable_paths)
+        return any(starts_with(Path(p), path) for p in [wp["path"] for wp in writable_paths if wp["writable"]])
 
     def delete_snippet():
         on_delete_snippet(content)
         set_delete_dialog(False)
 
     with sol.Div(style_="height: 100%; display: flex; flex-direction: column;") as main:
         with sol.Div(style_="display: flex; flex-grow: 1; min-height: 0"):
@@ -179,43 +179,53 @@
     return main
 
 
 @reacton.component
 def AddDialog(writable_paths, open, on_open, on_add_snippet, path=[{}]):
     add_name, set_add_name = reacton.use_state("")
     add_path, set_add_path = reacton.use_state("")
-    with v.Dialog(width="400px", v_model=open, on_v_model=lambda v: on_open(v)).meta(ref="add-dialog") as main:
+    with v.Dialog(width="600px", v_model=open, on_v_model=lambda v: on_open(v)).meta(ref="add-dialog") as main:
         with v.Card():
             v.CardTitle(children=["Add snippet"])
             with v.CardText():
                 sol.Div(children=["Folder: " + "/".join([p["id"] for p in path[1:] if not p["leaf"]])])
                 v.TextField(label="Name", v_model=add_name, on_v_model=set_add_name, autofocus=True)
                 sol.Div(children=["Repository"])
                 with v.List():
                     with v.ListItemGroup(v_model=add_path, on_v_model=set_add_path, color="primary"):
                         for item in writable_paths:
                             label = item
                             icon = ""
                             git_path = settings.domino_repos_dir or settings.domino_imported_code_dir
-                            if str(item).startswith(settings.domino_working_dir):
+                            if str(item["path"]).startswith(settings.domino_working_dir):
                                 label = "current project"
-                            elif git_path and str(item).startswith(git_path):
+                            elif git_path and str(item["path"]).startswith(git_path):
                                 icon = "mdi-git"
-                                label = str(item)[len(git_path) + 1 :]
-                            with v.ListItem(value=str(item)).key(str(item)):
+                                label = str(item["path"])[len(git_path) + 1 :]
+                            with v.ListItem(value=str(item["path"]), disabled=not item["writable"]).key(str(item)):
                                 with v.ListItemIcon():
                                     if icon:
                                         v.Icon(children=[icon])
                                     else:
                                         v.Img(
                                             src=util.logo_grey,
                                             style_="height: 24px; max-width: 24px; border-radius: 12px",
                                         )
                                 with v.ListItemContent():
-                                    v.ListItemTitle(children=[str(label)])
+                                    v.ListItemTitle(
+                                        children=[
+                                            str(label),
+                                            sol.Tooltip(
+                                                "Read only. The configured credentials don't have write access to this repository.",
+                                                children=[sol.Text(" (read only)", style="pointer-events: all")],
+                                            )
+                                            if not item["writable"]
+                                            else "",
+                                        ]
+                                    )
             with v.CardActions():
                 sol.Button("Cancel", outlined=True, color="primary", on_click=lambda: on_open(False), icon_name="mdi-close")
                 sol.Button(
                     "add",
                     color="primary",
                     on_click=lambda: on_add_snippet(add_path, path, add_name),
                     class_="mx-2",
```

### Comparing `domino_code_assist-1.1.4/domino_code_assist/snippets/tree.vue` & `domino_code_assist-1.2.0/domino_code_assist/snippets/tree.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/app.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/code_inserted.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/code_inserted.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/hover_cell.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/hover_cell.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/hover_icon.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/hover_icon.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/load_data.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/load_data.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/menu.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/menu.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/menu_app.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/menu_app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/menu_transform.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/menu_transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/menu_visualizations.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/menu_visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/tour.py` & `domino_code_assist-1.2.0/domino_code_assist/tour/tour.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/tour.vue` & `domino_code_assist-1.2.0/domino_code_assist/tour/tour.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/transform.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/tour/visualizations.png` & `domino_code_assist-1.2.0/domino_code_assist/tour/visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/transform/column_description.py` & `domino_code_assist-1.2.0/domino_code_assist/transform/column_description.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/transform/column_description.vue` & `domino_code_assist-1.2.0/domino_code_assist/transform/column_description.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/transform/transform_action_ui.py` & `domino_code_assist-1.2.0/domino_code_assist/transform/transform_action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/transform/transform_drawer.py` & `domino_code_assist-1.2.0/domino_code_assist/transform/transform_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/transform/transform_panel.py` & `domino_code_assist-1.2.0/domino_code_assist/transform/transform_panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/viz/drawer.py` & `domino_code_assist-1.2.0/domino_code_assist/viz/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/viz/plot_builder.py` & `domino_code_assist-1.2.0/domino_code_assist/viz/plot_builder.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/domino_code_assist/viz/state.py` & `domino_code_assist-1.2.0/domino_code_assist/viz/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/pyproject.toml` & `domino_code_assist-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.1.4/PKG-INFO` & `domino_code_assist-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-code-assist
-Version: 1.1.4
+Version: 1.2.0
 Project-URL: Home, https://github.com/cerebrotech/domino-code-assist
 License-File: LICENSE.md
 Requires-Dist: dominodatalab; python_version >= '3.8'
 Requires-Dist: humanize
 Requires-Dist: ipyvue
 Requires-Dist: ipyvuetify
 Requires-Dist: ipywidgets<8
```

