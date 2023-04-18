# Comparing `tmp/carefree-drawboard-0.0.0a2.tar.gz` & `tmp/carefree-drawboard-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a2.tar", last modified: Mon Apr 17 03:19:32 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a3.tar", last modified: Tue Apr 18 09:58:16 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a2.tar` & `carefree-drawboard-0.0.0a3.tar`

### file list

```diff
@@ -1,188 +1,194 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/LICENSE
--rw-rw-rw-   0        0        0       63 2023-04-17 03:16:55.000000 carefree-drawboard-0.0.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0     8807 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     8524 2023-04-17 02:49:50.000000 carefree-drawboard-0.0.0a2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.001106 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     8807 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-04-17 03:19:31.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      147 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.003449 carefree-drawboard-0.0.0a2/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.006439 carefree-drawboard-0.0.0a2/cfdraw/.web/
--rw-rw-rw-   0        0        0      119 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1526 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.009429 carefree-drawboard-0.0.0a2/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      901 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.013415 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:31.981040 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.013415 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.014413 carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/
--rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/BoardPanel.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.017402 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.017402 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.018400 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.020392 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     3048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useUndoRedo.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.024379 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.029363 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/
--rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.031355 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
--rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.032352 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.034346 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.035343 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.035343 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.036339 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      824 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.038332 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.041322 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     1431 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.043316 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      546 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0      594 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   210103 2023-04-16 17:37:05.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a2/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.044313 carefree-drawboard-0.0.0a2/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.047303 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     1907 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/plugins.py
--rw-rw-rw-   0        0        0     5653 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     1813 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     2569 2023-04-16 17:34:51.000000 carefree-drawboard-0.0.0a2/cfdraw/cli.py
--rw-rw-rw-   0        0        0     1459 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/config.py
--rw-rw-rw-   0        0        0      955 2023-04-17 03:06:49.000000 carefree-drawboard-0.0.0a2/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.048299 carefree-drawboard-0.0.0a2/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.050292 carefree-drawboard-0.0.0a2/cfdraw/plugins/
--rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.050292 carefree-drawboard-0.0.0a2/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/factory.py
--rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.052286 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0     1090 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.053282 carefree-drawboard-0.0.0a2/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     1222 2023-04-17 03:07:11.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-17 03:19:32.057269 carefree-drawboard-0.0.0a2/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-04-17 03:12:52.000000 carefree-drawboard-0.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/LICENSE
+-rw-rw-rw-   0        0        0       87 2023-04-18 09:58:12.000000 carefree-drawboard-0.0.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9076 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     8793 2023-04-18 02:22:15.000000 carefree-drawboard-0.0.0a3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.146011 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9076 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5394 2023-04-18 09:58:16.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.148005 carefree-drawboard-0.0.0a3/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.152988 carefree-drawboard-0.0.0a3/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0   888829 2023-04-17 08:28:51.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/analyze.html
+-rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.155982 carefree-drawboard-0.0.0a3/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      901 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.159967 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.114205 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.159967 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.160964 carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/
+-rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/BoardPanel.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.163954 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.164951 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.165947 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFText.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.166944 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useUndoRedo.ts
+-rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.171440 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.176423 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/
+-rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.178416 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
+-rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.180409 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.182402 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.183399 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.184396 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     3555 2023-04-17 15:25:00.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.184396 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.187385 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/metaFields.ts
+-rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.190375 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.192369 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a3/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.193366 carefree-drawboard-0.0.0a3/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-04-18 07:46:59.000000 carefree-drawboard-0.0.0a3/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.196356 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     1944 2023-04-18 06:33:13.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/plugins.py
+-rw-rw-rw-   0        0        0     5713 2023-04-17 13:23:53.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     1813 2023-04-18 02:06:49.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3485 2023-04-18 08:00:45.000000 carefree-drawboard-0.0.0a3/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2226 2023-04-18 07:55:50.000000 carefree-drawboard-0.0.0a3/cfdraw/config.py
+-rw-rw-rw-   0        0        0     1479 2023-04-18 07:48:42.000000 carefree-drawboard-0.0.0a3/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.197353 carefree-drawboard-0.0.0a3/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.200343 carefree-drawboard-0.0.0a3/cfdraw/plugins/
+-rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.200343 carefree-drawboard-0.0.0a3/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/factory.py
+-rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/meta.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.203333 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0     1090 2023-04-17 09:56:46.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.204329 carefree-drawboard-0.0.0a3/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.206322 carefree-drawboard-0.0.0a3/cfdraw/server/
+-rw-rw-rw-   0        0        0     1194 2023-04-18 09:42:33.000000 carefree-drawboard-0.0.0a3/cfdraw/server/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-04-18 07:04:07.000000 carefree-drawboard-0.0.0a3/cfdraw/server/http.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 07:40:33.000000 carefree-drawboard-0.0.0a3/cfdraw/server/index.py
+-rw-rw-rw-   0        0        0     1459 2023-04-18 07:40:19.000000 carefree-drawboard-0.0.0a3/cfdraw/server/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     2781 2023-04-18 07:55:53.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-18 09:58:16.211306 carefree-drawboard-0.0.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-04-18 09:57:02.000000 carefree-drawboard-0.0.0a3/setup.py
```

### Comparing `carefree-drawboard-0.0.0a2/LICENSE` & `carefree-drawboard-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/PKG-INFO` & `carefree-drawboard-0.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,26 +14,29 @@
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
-[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)  
+[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
-* [Node.js 12.22.0+](https://nodejs.org/en/)
+* [Node.js 18+](https://nodejs.org/en/)
+
+> To be exact, we need `^14.13.1 || ^16 || >=18` because of the `tsconfck@2.1.1` package.
 
 ```bash
 pip install carefree-drawboard
 npm install --global yarn
 ```
 
 Although we'll always try to help you install the frontend packages, it is recommended to install them beforehands because you can receive much more verbose:
```

### Comparing `carefree-drawboard-0.0.0a2/README.md` & `carefree-drawboard-0.0.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
-[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)  
+[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
-* [Node.js 12.22.0+](https://nodejs.org/en/)
+* [Node.js 18+](https://nodejs.org/en/)
+
+> To be exact, we need `^14.13.1 || ^16 || >=18` because of the `tsconfck@2.1.1` package.
 
 ```bash
 pip install carefree-drawboard
 npm install --global yarn
 ```
 
 Although we'll always try to help you install the frontend packages, it is recommended to install them beforehands because you can receive much more verbose:
```

### Comparing `carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,26 +14,29 @@
 
 > This is the screenshot I used for the [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) example and I don't know what should be the proper banner, help!
 
 <div align="center">
 
 [![PyPI version](https://badge.fury.io/py/carefree-drawboard.svg)](https://badge.fury.io/py/carefree-drawboard.svg)
 ![Checks](https://github.com/carefree0910/carefree-drawboard/actions/workflows/checks.yml/badge.svg)
-[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)  
+[![License](https://img.shields.io/badge/License-Apache_2.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carefree0910/carefree-drawboard/blob/dev/examples/server.ipynb)
 
 ### [Wiki](https://github.com/carefree0910/carefree-drawboard/wiki) | [Examples](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples) | [Stable Diffusion](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion) | [ControlNet](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_controlnet) | [Inpainting](https://github.com/carefree0910/carefree-drawboard/tree/dev/examples/stable_diffusion_inpainting)
 
 <div align="left">
 
 ## Installation
 
 `carefree-drawboard` 🎨 requires the following to get started:
 
 * Python 3.8+
-* [Node.js 12.22.0+](https://nodejs.org/en/)
+* [Node.js 18+](https://nodejs.org/en/)
+
+> To be exact, we need `^14.13.1 || ^16 || >=18` because of the `tsconfck@2.1.1` package.
 
 ```bash
 pip install carefree-drawboard
 npm install --global yarn
 ```
 
 Although we'll always try to help you install the frontend packages, it is recommended to install them beforehands because you can receive much more verbose:
```

### Comparing `carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 carefree_drawboard.egg-info/top_level.txt
 cfdraw/__init__.py
 cfdraw/cli.py
 cfdraw/config.py
 cfdraw/constants.py
 cfdraw/.web/.env
 cfdraw/.web/.prettierrc
+cfdraw/.web/analyze.html
 cfdraw/.web/index.html
 cfdraw/.web/package.json
 cfdraw/.web/tsconfig.json
 cfdraw/.web/tsconfig.node.json
 cfdraw/.web/tsconfig.paths.json
 cfdraw/.web/vite.config.ts
 cfdraw/.web/yarn.lock
@@ -141,14 +142,18 @@
 cfdraw/plugins/middlewares/__init__.py
 cfdraw/plugins/middlewares/fields.py
 cfdraw/plugins/middlewares/text_area.py
 cfdraw/plugins/middlewares/timer.py
 cfdraw/schema/__init__.py
 cfdraw/schema/fields.py
 cfdraw/schema/plugins.py
+cfdraw/server/__init__.py
+cfdraw/server/http.py
+cfdraw/server/index.py
+cfdraw/server/socket.py
 cfdraw/utils/__init__.py
 cfdraw/utils/cache.py
 cfdraw/utils/console.py
 cfdraw/utils/exec.py
 cfdraw/utils/prerequisites.py
 cfdraw/utils/processes.py
 cfdraw/utils/server.py
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/package.json` & `carefree-drawboard-0.0.0a3/cfdraw/.web/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9559523809523809%*

 * *Differences: {"'dependencies'": "{'@carefree0910/business': '^0.4.10-alpha.2', '@carefree0910/core': "*

 * *                   "'^0.4.10-alpha.1', '@carefree0910/native': '^0.4.10-alpha.2', delete: "*

 * *                   "['vite-plugin-svgr', 'vite-tsconfig-paths']}",*

 * * "'devDependencies'": "{'rollup-plugin-visualizer': '^5.9.0', 'vite-plugin-svgr': '^2.4.0', "*

 * *                      "'vite-tsconfig-paths': '^4.0.8'}",*

 * * "'scripts'": "{'build:preview': 'tsc && vite build && vite preview'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "dependencies": {
-        "@carefree0910/business": "^0.4.10-alpha.0",
-        "@carefree0910/core": "^0.4.10-alpha.0",
-        "@carefree0910/native": "^0.4.10-alpha.0",
+        "@carefree0910/business": "^0.4.10-alpha.2",
+        "@carefree0910/core": "^0.4.10-alpha.1",
+        "@carefree0910/native": "^0.4.10-alpha.2",
         "@chakra-ui/icons": "^2.0.4",
         "@chakra-ui/react": "^2.2.4",
         "@emotion/react": "^11.9.3",
         "@emotion/styled": "^11.9.3",
         "@svgdotjs/svg.filter.js": "^3.0.8",
         "@svgdotjs/svg.js": "^3.1.1",
         "@svgdotjs/svg.topath.js": "^2.0.3",
@@ -23,32 +23,34 @@
         "mobx-react-lite": "^3.4.0",
         "next": "13.2.4",
         "opentype.js": "^1.3.4",
         "platform": "^1.3.6",
         "rc-upload": "^4.3.4",
         "react": "18.2.0",
         "react-dom": "18.2.0",
-        "uuid": "^9.0.0",
-        "vite-plugin-svgr": "^2.4.0",
-        "vite-tsconfig-paths": "^4.0.8"
+        "uuid": "^9.0.0"
     },
     "devDependencies": {
         "@total-typescript/ts-reset": "^0.4.2",
         "@types/node": "18.15.11",
         "@types/react": "18.0.33",
         "@types/react-dom": "18.0.11",
         "@types/uuid": "^9.0.1",
         "@vitejs/plugin-react": "^3.1.0",
+        "rollup-plugin-visualizer": "^5.9.0",
         "sass": "^1.60.0",
         "typescript": "^5.0.3",
-        "vite": "^4.2.0"
+        "vite": "^4.2.0",
+        "vite-plugin-svgr": "^2.4.0",
+        "vite-tsconfig-paths": "^4.0.8"
     },
     "name": "cfdraw",
     "private": true,
     "scripts": {
         "build": "tsc && vite build",
+        "build:preview": "tsc && vite build && vite preview",
         "dev": "vite",
         "preview": "vite preview"
     },
     "type": "module",
     "version": "0.0.0"
 }
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/_settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/importMeta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/BoardPanel.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,25 @@
   BoardStore,
   BoardStoresOptions,
   useFlags,
   useBoardStore,
   useIsReady,
 } from "@carefree0910/business";
 
-import { BOARD_CONTAINER_ID, ENV } from "@/utils/constants";
+import { BOARD_CONTAINER_ID, IS_PROD } from "@/utils/constants";
 import { initStore } from "@/stores/init";
 import { themeStore } from "@/stores/theme";
 
 export function useInitBoard(): void {
   async function _initialize(): Promise<void> {
     if (initStore.working) return;
     initStore.updateProperty("working", true);
 
     // pre settings
-    const isProduction = ENV === "production";
-    Logger.isDebug = !isProduction;
+    Logger.isDebug = !IS_PROD;
 
     // check cache
     const cache: { graph?: Graph; globalTransform?: Matrix2DFields } = {};
 
     // initialize board
     // TODO: make this more elegant
 
@@ -63,20 +62,18 @@
 
     //// render
     await unittest.renderGraph(cache.graph ?? new Graph(), undefined, false);
 
     //// setup options
     const storeOptions: BoardStoresOptions = {
       constantsOpt: {
-        env: ENV as BoardStoresOptions["constantsOpt"]["env"],
+        env: IS_PROD ? "production" : "development",
       },
     };
-    if (isProduction) {
-      Logger.isDebug = false;
-    } else {
+    if (!IS_PROD) {
       storeOptions.debug = {
         selecting: true,
         selectingDetails: false,
       };
     }
 
     //// setup board store
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePython.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/ui.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/AddPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/BrushPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DeletePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DownloadPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ProjectPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/SettingsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/TextEditorPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/hooks.ts`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,24 @@
 import type { ISocketCallbacks, IPythonSocketMessage } from "@/schema/_python";
 import { pythonStore } from "@/stores/_python";
 import { useInceptors } from "./interceptors";
 
 // cannot use `useMemo` here
 export function useAPI<T extends APISources>(source: T): APIs[T] {
   const timeout = pythonStore.globalSettings.timeout ?? 300000;
-  const backendPort = import.meta.env.VITE_CFDRAW_BE_PORT ?? 8123;
+  let baseURL = import.meta.env.VITE_CFDRAW_API_URL;
+  if (!baseURL) {
+    let backendPort = import.meta.env.VITE_CFDRAW_BE_PORT;
+    if (!backendPort) {
+      backendPort = 8123;
+    }
+    baseURL = `http://localhost:${backendPort}`;
+  }
   const apis = {
-    _python: axios.create({ baseURL: `http://localhost:${backendPort}`, timeout }),
+    _python: axios.create({ baseURL, timeout }),
   };
   useInceptors(apis);
   return apis[source];
 }
 
 const DEBUG = false;
 const log = (...args: any[]) => DEBUG && console.log(...args);
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import type { Interceptors } from "@/schema/requests";
 
 export const _pythonInceptors: Interceptors = {
   beforeRequest: (config) => {
     if (Logger.isDebug) {
       Logger.debug(`send to Python: ${JSON.stringify(config.data)} (${config.url})`);
     }
+    config.headers["ngrok-skip-browser-warning"] = "";
     return config;
   },
   requestError(error) {
     if (Logger.isDebug) {
       Logger.debug(`send to Python error: ${error}`);
     }
     return Promise.reject(error);
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/metaFields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/_python.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/_python.ts`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { makeObservable, observable, runInAction } from "mobx";
 
+import { getHash } from "@carefree0910/core";
 import { ABCStore } from "@carefree0910/business";
 
 import type { AvailablePythonPlugins, IMakePlugin } from "@/schema/plugins";
-import { getHash } from "@carefree0910/core";
 
 interface IGlobalSettings {
   timeout?: number;
   useStrictMode?: boolean;
   sockenEndpoint?: string;
 }
 export interface IPythonStore {
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/theme.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.0a3/cfdraw/.web/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -213,41 +213,41 @@
   resolved "https://registry.yarnpkg.com/@babel/types/-/types-7.21.4.tgz#2d5d6bb7908699b3b416409ffd3b5daa25b030d4"
   integrity sha512-rU2oY501qDxE8Pyo7i/Orqma4ziCOrby0/9mvbDUGEfvZjb279Nk9k19e2fiCxHbRRpY2ZyrgW1eq22mvmOIzA==
   dependencies:
     "@babel/helper-string-parser" "^7.19.4"
     "@babel/helper-validator-identifier" "^7.19.1"
     to-fast-properties "^2.0.0"
 
-"@carefree0910/business@^0.4.10-alpha.0":
-  version "0.4.10-alpha.0"
-  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.4.10-alpha.0.tgz#f5bdabc7c30d5165163162b56db4fb5ff9c957a4"
-  integrity sha512-zS83oOIvGnyj3keXEQc1kRSskMZq/tj8ciwceTmCn6XZ5JdwHfw4bvbJF3ZlH72JzdGH9/trnYRmx2xvNjRmbA==
-  dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.0"
-    "@carefree0910/svg" "^0.4.10-alpha.0"
-
-"@carefree0910/core@^0.4.10-alpha.0":
-  version "0.4.10-alpha.0"
-  resolved "https://registry.yarnpkg.com/@carefree0910/core/-/core-0.4.10-alpha.0.tgz#8425fd279b84ea90a7277e21a210260607c02ef1"
-  integrity sha512-/80EkHTrfugwo7YOabrcp1l+/fXEAtFj/Mflj4vK6EpJs7gY7jBdCNOwgsLqYCkMR6R/hX78JpbswAPbI9YT2A==
-
-"@carefree0910/native@^0.4.10-alpha.0":
-  version "0.4.10-alpha.0"
-  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.4.10-alpha.0.tgz#ed7d4555b37cc64968c3bed5822e9d0811a2f29f"
-  integrity sha512-5RDbbEf7z9ZMR45CStyFzK36y63tVO4oUxVV1MJenWuChnoaCYSMaBmuw3rpfZKdZ5chEZ+kZ5wZI6xKDvJmyQ==
-  dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.0"
-    "@carefree0910/svg" "^0.4.10-alpha.0"
-
-"@carefree0910/svg@^0.4.10-alpha.0":
-  version "0.4.10-alpha.0"
-  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.4.10-alpha.0.tgz#ab3b888e16432785490481d33a0cebdd1506d2b3"
-  integrity sha512-y1LfmAGvWZP3PCcSLVOAlTBZ848Py+NepxO4XdqtWKTGKIEfUdYW9Rx+3T6qHwT2OM3dX6zHowBKmo/09YTiGQ==
+"@carefree0910/business@^0.4.10-alpha.2":
+  version "0.4.10-alpha.2"
+  resolved "https://registry.yarnpkg.com/@carefree0910/business/-/business-0.4.10-alpha.2.tgz#b937f4e1a7c51ba44944dfaac375b3611f0caaae"
+  integrity sha512-tFNFwAtsEAYGOIAJuaBPcmohIlIimzeQp4LpRDhXeDctcEtoenrcfsd6r9Cdcd0Zd1LekjVj/y9CEpfQaBoXeA==
+  dependencies:
+    "@carefree0910/core" "^0.4.10-alpha.1"
+    "@carefree0910/svg" "^0.4.10-alpha.1"
+
+"@carefree0910/core@^0.4.10-alpha.1":
+  version "0.4.10-alpha.1"
+  resolved "https://registry.yarnpkg.com/@carefree0910/core/-/core-0.4.10-alpha.1.tgz#8a1c579b7073a2119c8f30dae93bc1d1a21a3dbd"
+  integrity sha512-bjKvuFAHawgNW/avS/vOh/J70MCw/Lu+04cQvlVmqzYxlOGAZPKsRFNtYgTO2CNo6vgRt3sa+WpnBXibWssw2Q==
+
+"@carefree0910/native@^0.4.10-alpha.2":
+  version "0.4.10-alpha.2"
+  resolved "https://registry.yarnpkg.com/@carefree0910/native/-/native-0.4.10-alpha.2.tgz#0a1224046dcbc8ac5864721843a61aa1643a37c0"
+  integrity sha512-NsuHU2gff2PRK0NLVUU/4sfPT87K8gHuXAYaN1L01upOcIlzu6RgwsCoKKphh1uZtl9TYYt0VxjOAVxrONHvyg==
+  dependencies:
+    "@carefree0910/core" "^0.4.10-alpha.1"
+    "@carefree0910/svg" "^0.4.10-alpha.1"
+
+"@carefree0910/svg@^0.4.10-alpha.1":
+  version "0.4.10-alpha.1"
+  resolved "https://registry.yarnpkg.com/@carefree0910/svg/-/svg-0.4.10-alpha.1.tgz#b74bad3868c50033e691659e85deeeaa30ff9a32"
+  integrity sha512-r2BweoT2kiW5IOsack9c/W3EMwUnB6K6cIn1LgUm8gjMrRxc0OB0OmtIL4IHOyUjbDsFCQGP9WrsG7EqJ8mwJA==
   dependencies:
-    "@carefree0910/core" "^0.4.10-alpha.0"
+    "@carefree0910/core" "^0.4.10-alpha.1"
 
 "@chakra-ui/accordion@2.1.11":
   version "2.1.11"
   resolved "https://registry.yarnpkg.com/@chakra-ui/accordion/-/accordion-2.1.11.tgz#c6df0100c543645d0631df3aefde2ea2b8ed6313"
   integrity sha512-mfVPmqETp9pyRDHJ33AdF19oHv/LyxVzQJtlxUByuvs8Cj9QQZ2LQLg5kejm+b3mj03A7A6yfbuo3RNaI4Bhsg==
   dependencies:
     "@chakra-ui/descendant" "3.0.14"
@@ -1799,15 +1799,15 @@
 ansi-styles@^3.2.1:
   version "3.2.1"
   resolved "https://registry.yarnpkg.com/ansi-styles/-/ansi-styles-3.2.1.tgz#41fbb20243e50b12be0f04b8dedbf07520ce841d"
   integrity sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==
   dependencies:
     color-convert "^1.9.0"
 
-ansi-styles@^4.1.0:
+ansi-styles@^4.0.0, ansi-styles@^4.1.0:
   version "4.3.0"
   resolved "https://registry.yarnpkg.com/ansi-styles/-/ansi-styles-4.3.0.tgz#edd803628ae71c04c85ae7a0906edad34b648937"
   integrity sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==
   dependencies:
     color-convert "^2.0.1"
 
 anymatch@~3.1.2:
@@ -2033,14 +2033,23 @@
   integrity sha512-CSbhY4cFEJRe6/GQzIk5qXZ4Jeg5pcsP7b5peFSDpffpe1cqjASH/n9UTjBwOp6XpMSTwQ8Za2K5V02ueA7Tmw==
 
 client-only@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/client-only/-/client-only-0.0.1.tgz#38bba5d403c41ab150bff64a95c85013cf73bca1"
   integrity sha512-IV3Ou0jSMzZrd3pZ48nLkT9DA7Ag1pnPzaiQhpW7c3RbcqqzvzzVu+L8gfqMp/8IM2MQtSiqaCxrrcfu8I8rMA==
 
+cliui@^8.0.1:
+  version "8.0.1"
+  resolved "https://registry.yarnpkg.com/cliui/-/cliui-8.0.1.tgz#0c04b075db02cbfe60dc8e6cf2f5486b1a3608aa"
+  integrity sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==
+  dependencies:
+    string-width "^4.2.0"
+    strip-ansi "^6.0.1"
+    wrap-ansi "^7.0.0"
+
 color-convert@^1.9.0:
   version "1.9.3"
   resolved "https://registry.yarnpkg.com/color-convert/-/color-convert-1.9.3.tgz#bb71850690e1f136567de629d2d5471deda4c1e8"
   integrity sha512-QfAUtd+vFdAtFQcC8CCyYt1fYWxSqAiK2cSD6zDB8N3cpsEBAvRxp9zOGg6G/SHHJYAT88/az/IuDGALsNVbGg==
   dependencies:
     color-name "1.1.3"
 
@@ -2229,14 +2238,19 @@
     esutils "^2.0.2"
 
 electron-to-chromium@^1.4.284:
   version "1.4.365"
   resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.365.tgz#ccd9e352d4493aa288d87e6ea36f3edf350c045e"
   integrity sha512-FRHZO+1tUNO4TOPXmlxetkoaIY8uwHzd1kKopK/Gx2SKn1L47wJXWD44wxP5CGRyyP98z/c8e1eBzJrgPeiBOg==
 
+emoji-regex@^8.0.0:
+  version "8.0.0"
+  resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
+  integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
+
 emoji-regex@^9.2.2:
   version "9.2.2"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-9.2.2.tgz#840c8803b0d8047f4ff0cf963176b32d4ef3ed72"
   integrity sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==
 
 enhanced-resolve@^5.12.0:
   version "5.12.0"
@@ -2740,14 +2754,19 @@
   integrity sha512-xckBUXyTIqT97tq2x2AMb+g163b5JFysYk0x4qxNFwbfQkmNZoiRHb6sPzI9/QV33WeuvVYBUIiD4NzNIyqaRQ==
 
 gensync@^1.0.0-beta.2:
   version "1.0.0-beta.2"
   resolved "https://registry.yarnpkg.com/gensync/-/gensync-1.0.0-beta.2.tgz#32a6ee76c3d7f52d46b2b1ae5d93fea8580a25e0"
   integrity sha512-3hN7NaskYvMDLQY55gnW3NQ+mesEAepTqlg+VEbj7zzqEMBVNhzcGYYeqFo/TlYz6eQiFcp1HcsCZO+nGgS8zg==
 
+get-caller-file@^2.0.5:
+  version "2.0.5"
+  resolved "https://registry.yarnpkg.com/get-caller-file/-/get-caller-file-2.0.5.tgz#4f94412a82db32f36e3b0b9741f8a97feb031f7e"
+  integrity sha512-DyFP3BM/3YHTQOCUL/w0OZHR0lpKeGrxotcHWcqNEdnltqFwXVfhEBQ94eIo34AfQpo0rGki4cyIiftY06h2Fg==
+
 get-intrinsic@^1.0.2, get-intrinsic@^1.1.1, get-intrinsic@^1.1.3, get-intrinsic@^1.2.0:
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/get-intrinsic/-/get-intrinsic-1.2.0.tgz#7ad1dc0535f3a2904bba075772763e5051f6d05f"
   integrity sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==
   dependencies:
     function-bind "^1.1.1"
     has "^1.0.3"
@@ -3067,14 +3086,19 @@
   integrity sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==
 
 is-extglob@^2.1.1:
   version "2.1.1"
   resolved "https://registry.yarnpkg.com/is-extglob/-/is-extglob-2.1.1.tgz#a88c02535791f02ed37c76a1b9ea9773c833f8c2"
   integrity sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==
 
+is-fullwidth-code-point@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.yarnpkg.com/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz#f116f8064fe90b3f7844a38997c0b75051269f1d"
+  integrity sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==
+
 is-glob@^4.0.0, is-glob@^4.0.1, is-glob@^4.0.3, is-glob@~4.0.1:
   version "4.0.3"
   resolved "https://registry.yarnpkg.com/is-glob/-/is-glob-4.0.3.tgz#64f61e42cbbb2eec2071a9dac0b28ba1e65d5084"
   integrity sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==
   dependencies:
     is-extglob "^2.1.1"
 
@@ -3835,14 +3859,19 @@
   resolved "https://registry.yarnpkg.com/regexp.prototype.flags/-/regexp.prototype.flags-1.4.3.tgz#87cab30f80f66660181a3bb7bf5981a872b367ac"
   integrity sha512-fjggEOO3slI6Wvgjwflkc4NFRCTZAu5CnNfBd5qOMYhWdn67nJBBu34/TkD++eeFmd8C9r9jfXJ27+nSiRkSUA==
   dependencies:
     call-bind "^1.0.2"
     define-properties "^1.1.3"
     functions-have-names "^1.2.2"
 
+require-directory@^2.1.1:
+  version "2.1.1"
+  resolved "https://registry.yarnpkg.com/require-directory/-/require-directory-2.1.1.tgz#8c64ad5fd30dab1c976e2344ffe7f792a6a6df42"
+  integrity sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==
+
 resize-observer-polyfill@^1.5.1:
   version "1.5.1"
   resolved "https://registry.yarnpkg.com/resize-observer-polyfill/-/resize-observer-polyfill-1.5.1.tgz#0e9020dd3d21024458d4ebd27e23e40269810464"
   integrity sha512-LwZrotdHOo12nQuZlHEmtuXdqGoOD0OhaxopaNFxWzInpEgaLWoVuAMbTzixuosCx2nEG58ngzW3vxdWoxIgdg==
 
 resolve-from@^4.0.0:
   version "4.0.0"
@@ -3875,14 +3904,24 @@
 rimraf@^3.0.2:
   version "3.0.2"
   resolved "https://registry.yarnpkg.com/rimraf/-/rimraf-3.0.2.tgz#f1a5402ba6220ad52cc1282bac1ae3aa49fd061a"
   integrity sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==
   dependencies:
     glob "^7.1.3"
 
+rollup-plugin-visualizer@^5.9.0:
+  version "5.9.0"
+  resolved "https://registry.yarnpkg.com/rollup-plugin-visualizer/-/rollup-plugin-visualizer-5.9.0.tgz#013ac54fb6a9d7c9019e7eb77eced673399e5a0b"
+  integrity sha512-bbDOv47+Bw4C/cgs0czZqfm8L82xOZssk4ayZjG40y9zbXclNk7YikrZTDao6p7+HDiGxrN0b65SgZiVm9k1Cg==
+  dependencies:
+    open "^8.4.0"
+    picomatch "^2.3.1"
+    source-map "^0.7.4"
+    yargs "^17.5.1"
+
 rollup@^3.18.0:
   version "3.20.3"
   resolved "https://registry.yarnpkg.com/rollup/-/rollup-3.20.3.tgz#932754ecadd5a03ed98e827d6ffd060936a7c986"
   integrity sha512-u6/O1X42CAZ79rbk+smyONJQLTpwFBL7InpRa/AVWia5lq60w5J/PUsVHCOgSolN0X9R2GjQ41fZm3x28Hk1lA==
   optionalDependencies:
     fsevents "~2.3.2"
 
@@ -3982,21 +4021,35 @@
   integrity sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==
 
 source-map@^0.5.7:
   version "0.5.7"
   resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.5.7.tgz#8a039d2d1021d22d1ea14c80d8ea468ba2ef3fcc"
   integrity sha512-LbrmJOMUSdEVxIKvdcJzQC+nQhe8FUZQTXQy6+I75skNgn3OoQ0DZA8YnFa7gp8tqtL3KPf1kmo0R5DoApeSGQ==
 
+source-map@^0.7.4:
+  version "0.7.4"
+  resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.7.4.tgz#a9bbe705c9d8846f4e08ff6765acf0f1b0898656"
+  integrity sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==
+
 stop-iteration-iterator@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/stop-iteration-iterator/-/stop-iteration-iterator-1.0.0.tgz#6a60be0b4ee757d1ed5254858ec66b10c49285e4"
   integrity sha512-iCGQj+0l0HOdZ2AEeBADlsRC+vsnDsZsbdSiH1yNSjcfKM7fdpCMfqAL/dwF5BLiw/XhRft/Wax6zQbhq2BcjQ==
   dependencies:
     internal-slot "^1.0.4"
 
+string-width@^4.1.0, string-width@^4.2.0, string-width@^4.2.3:
+  version "4.2.3"
+  resolved "https://registry.yarnpkg.com/string-width/-/string-width-4.2.3.tgz#269c7117d27b05ad2e536830a8ec895ef9c6d010"
+  integrity sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==
+  dependencies:
+    emoji-regex "^8.0.0"
+    is-fullwidth-code-point "^3.0.0"
+    strip-ansi "^6.0.1"
+
 string.prototype.codepointat@^0.2.1:
   version "0.2.1"
   resolved "https://registry.yarnpkg.com/string.prototype.codepointat/-/string.prototype.codepointat-0.2.1.tgz#004ad44c8afc727527b108cd462b4d971cd469bc"
   integrity sha512-2cBVCj6I4IOvEnjgO/hWqXjqBGsY+zwPmHl12Srk9IXSZ56Jwwmy+66XO5Iut/oQVR7t5ihYdLB0GMa4alEUcg==
 
 string.prototype.matchall@^4.0.8:
   version "4.0.8"
@@ -4042,15 +4095,15 @@
 string_decoder@~1.1.1:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/string_decoder/-/string_decoder-1.1.1.tgz#9cf1611ba62685d7030ae9e4ba34149c3af03fc8"
   integrity sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==
   dependencies:
     safe-buffer "~5.1.0"
 
-strip-ansi@^6.0.1:
+strip-ansi@^6.0.0, strip-ansi@^6.0.1:
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/strip-ansi/-/strip-ansi-6.0.1.tgz#9e26c63d30f53443e9489495b2105d37b67a85d9"
   integrity sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==
   dependencies:
     ansi-regex "^5.0.1"
 
 strip-bom@^3.0.0:
@@ -4335,19 +4388,33 @@
     isexe "^2.0.0"
 
 word-wrap@^1.2.3:
   version "1.2.3"
   resolved "https://registry.yarnpkg.com/word-wrap/-/word-wrap-1.2.3.tgz#610636f6b1f703891bd34771ccb17fb93b47079c"
   integrity sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==
 
+wrap-ansi@^7.0.0:
+  version "7.0.0"
+  resolved "https://registry.yarnpkg.com/wrap-ansi/-/wrap-ansi-7.0.0.tgz#67e145cff510a6a6984bdf1152911d69d2eb9e43"
+  integrity sha512-YVGIj2kamLSTxw6NsZjoBxfSwsn0ycdesmc4p+Q21c5zPuZ1pl+NfxVdxPtdHvmNVOQ6XSYG4AUtyt/Fi7D16Q==
+  dependencies:
+    ansi-styles "^4.0.0"
+    string-width "^4.1.0"
+    strip-ansi "^6.0.0"
+
 wrappy@1:
   version "1.0.2"
   resolved "https://registry.yarnpkg.com/wrappy/-/wrappy-1.0.2.tgz#b5243d8f3ec1aa35f1364605bc0d1036e30ab69f"
   integrity sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==
 
+y18n@^5.0.5:
+  version "5.0.8"
+  resolved "https://registry.yarnpkg.com/y18n/-/y18n-5.0.8.tgz#7f4934d0f7ca8c56f95314939ddcd2dd91ce1d55"
+  integrity sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==
+
 yallist@^3.0.2:
   version "3.1.1"
   resolved "https://registry.yarnpkg.com/yallist/-/yallist-3.1.1.tgz#dbb7daf9bfd8bac9ab45ebf602b8cbad0d5d08fd"
   integrity sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==
 
 yallist@^4.0.0:
   version "4.0.0"
@@ -4355,11 +4422,29 @@
   integrity sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==
 
 yaml@^1.10.0:
   version "1.10.2"
   resolved "https://registry.yarnpkg.com/yaml/-/yaml-1.10.2.tgz#2301c5ffbf12b467de8da2333a459e29e7920e4b"
   integrity sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==
 
+yargs-parser@^21.1.1:
+  version "21.1.1"
+  resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-21.1.1.tgz#9096bceebf990d21bb31fa9516e0ede294a77d35"
+  integrity sha512-tVpsJW7DdjecAiFpbIB1e3qxIQsE6NoPc5/eTdrbbIC4h0LVsWhnoa3g+m2HclBIujHzsxZ4VJVA+GUuc2/LBw==
+
+yargs@^17.5.1:
+  version "17.7.1"
+  resolved "https://registry.yarnpkg.com/yargs/-/yargs-17.7.1.tgz#34a77645201d1a8fc5213ace787c220eabbd0967"
+  integrity sha512-cwiTb08Xuv5fqF4AovYacTFNxk62th7LKJ6BL9IGUpTJrWoU7/7WdQGTP2SjKf1dUNBGzDd28p/Yfs/GI6JrLw==
+  dependencies:
+    cliui "^8.0.1"
+    escalade "^3.1.1"
+    get-caller-file "^2.0.5"
+    require-directory "^2.1.1"
+    string-width "^4.2.3"
+    y18n "^5.0.5"
+    yargs-parser "^21.1.1"
+
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,18 +18,16 @@
     return "pong"
 
 
 class App(IApp):
     def __init__(self) -> None:
         # config
         self.config = get_config()
-
         # clients
         self.http_session = ClientSession()
-
         # fastapi
         self.api = FastAPI()
         self.add_cors()
         self.add_default_endpoints()
         self.add_events()
         self.endpoints: List[IEndpoint] = [
             UploadEndpoint(self),
@@ -62,25 +60,29 @@
             allow_headers=["*"],
             allow_origins=["*"],
         )
 
     def add_events(self) -> None:
         @self.api.on_event("startup")
         async def startup() -> None:
+            def info(msg: str) -> None:
+                if not self.config.use_tornado:
+                    print_info(msg)
+
             self.hash = random_hash()
-            print_info(f"🚀 Starting Server at {self.config.api_url} ...")
-            print_info("🔨 Compiling Plugins & Endpoints...")
+            info(f"🚀 Starting Backend Server at {self.config.api_url} ...")
+            info("🔨 Compiling Plugins & Endpoints...")
             for plugin in self.plugins.values():
                 plugin.hash = self.hash
                 plugin.http_session = self.http_session
             for endpoint in self.endpoints:
                 await endpoint.on_startup()
             upload_root_path = self.config.upload_root_path
-            print_info(f"🔔 Your files will be saved to '{upload_root_path}'")
-            print_info("🎉 Server is Ready!")
+            info(f"🔔 Your files will be saved to '{upload_root_path}'")
+            info("🎉 Backend Server is Ready!")
 
         @self.api.on_event("shutdown")
         async def shutdown() -> None:
             await self.http_session.close()
             for plugin in self.plugins.values():
                 plugin.http_session = None
             for endpoint in self.endpoints:
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/plugins.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 
 def add_plugins(app: IApp) -> None:
     for identifier, plugin in app.plugins.items():
         if not isinstance(plugin, IHttpPlugin):
             continue
         endpoint = f"/{identifier}"
-        print_info(f"registering endpoint '{endpoint}'")
+        if not app.config.prod:
+            print_info(f"registering endpoint '{endpoint}'")
 
         def _register(_id: str, _p: IHttpPlugin) -> None:
             @app.api.post(
                 endpoint,
                 name=endpoint[1:].replace("/", "_"),
                 responses=get_responses(IPluginResponse),
             )
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,19 +116,17 @@
             # replace url if needed
             graph = noli.parse_graph(d["graphInfo"])
             for node in graph.all_single_nodes:
                 if node.type == noli.SingleNodeType.IMAGE:
                     if node.renderParams is None:
                         raise ValueError("`ImageNode` should have `renderParams`")
                     src = node.renderParams.src
-                    if (
-                        src
-                        and isinstance(src, str)
-                        and src.startswith(app.config.api_host)
-                    ):
+                    # TODO: this kind of transformation should be included in the
+                    # migration stage, not runtime stage. Will be fixed in the future
+                    if src and isinstance(src, str) and src.startswith("http://"):
                         pivot = constants.UPLOAD_IMAGE_FOLDER_NAME
                         _, path = src.split(pivot)
                         api_url = app.config.api_url
                         node.renderParams.src = api_url + "/" + pivot + path
             d["graphInfo"] = graph.dict()["root_nodes"]
             return ProjectModel(**d)
         except Exception as err:
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/upload.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/websocket.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/app/schema.py` & `carefree-drawboard-0.0.0a3/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/cli.py` & `carefree-drawboard-0.0.0a3/cfdraw/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,37 +22,56 @@
     module: str = typer.Option(None, help="The module to run."),
     no_frontend: bool = typer.Option(False, help="Whether not to run the frontend."),
     no_backend: bool = typer.Option(False, help="Whether not to run the backend."),
     log_level: constants.LogLevel = typer.Option(
         constants.LogLevel.ERROR,
         help="The log level to use.",
     ),
+    prod: bool = typer.Option(False, help="Whether to run in production mode."),
+    tornado: bool = typer.Option(False, help="Whether use tornado to unify servers."),
 ) -> None:
     sys.path.insert(0, os.getcwd())
-    # fetch configs
+    if tornado:
+        if not prod:
+            console.print(
+                "[bold orange1]Tornado is only available in production mode, "
+                "so `--prod` flag will be forced."
+            )
+            prod = True
+    constants.set_env(constants.Env.PROD if prod else constants.Env.DEV)
+    constants.set_tornado(tornado)
+    # fetch config
     config = get_config()
-    frontend_port = config.frontend_port
-    backend_port = config.backend_port
     # fetch module
     if module is None:
         module = constants.DEFAULT_MODULE
     if module.endswith(".py"):
         module = module[:-3]
     path_prefix = f".{os.path.sep}"
     if module.startswith(path_prefix):
         module = module[len(path_prefix) :]
     console.rule(f"[bold green]Running {module}")
     # execute
+    frontend_port = config.frontend_port
+    backend_port = config.backend_port
+    tornado_port = config.tornado_port
     if not no_frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
     if not no_backend and processes.is_process_on_port(backend_port):
         backend_port = processes.change_or_terminate_port(backend_port, "backend")
+    if tornado and not no_backend and processes.is_process_on_port(tornado_port):
+        tornado_port = processes.change_or_terminate_port(tornado_port, "tornado")
     config.frontend_port = frontend_port
     config.backend_port = backend_port
-    frontend_fn, backend_fn = exec.run_frontend, exec.run_backend
+    config.tornado_port = tornado_port
+    if not prod:
+        frontend_fn, backend_fn = exec.run_frontend, exec.run_backend
+    else:
+        frontend_fn = exec.run_frontend_prod
+        backend_fn = exec.run_tornado if tornado else exec.run_backend
     try:
         if not no_frontend:
             frontend_fn()
         if not no_backend:
             backend_fn(module, log_level=log_level)
     finally:
         console.rule("[bold]Shutting down")
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/config.py` & `carefree-drawboard-0.0.0a3/cfdraw/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+
+from typing import Optional
 from pathlib import Path
 from importlib import import_module
 from dataclasses import dataclass
 
 from cfdraw import constants
 from cfdraw.utils.cache import cache_resource
 
@@ -9,25 +12,45 @@
 @dataclass
 class Config:
     # app
     entry: str = constants.DEFAULT_ENTRY
     # frontend
     frontend_port: str = constants.FRONTEND_PORT
     # api
-    api_host: str = constants.API_HOST
     backend_port: str = constants.BACKEND_PORT
+    tornado_port: str = constants.TORNADO_PORT
+    backend_hosting_url: Optional[str] = None  # this must be provided for hosting
     # upload
     upload_root: str = str(constants.UPLOAD_ROOT)
     # misc
-    debug: bool = True
     use_react_strict_mode: bool = False
 
     @property
+    def prod(self) -> bool:
+        return constants.get_env() == constants.Env.PROD
+
+    @property
+    def use_tornado(self) -> bool:
+        return constants.use_tornado()
+
+    @property
+    def api_port(self) -> str:
+        return self.tornado_port if self.use_tornado else self.backend_port
+
+    @property
     def api_url(self) -> str:
-        return f"{self.api_host}:{self.backend_port}"
+        if self.backend_hosting_url is not None:
+            api_url = self.backend_hosting_url
+        else:
+            env_api_url = os.environ.get(constants.API_URL_KEY)
+            if env_api_url is not None:
+                api_url = env_api_url
+            else:
+                api_url = f"http://localhost:{self.api_port}"
+        return api_url.rstrip("/").rstrip("\\")
 
     @property
     def upload_root_path(self) -> Path:
         return Path(self.upload_root).absolute()
 
     @property
     def upload_image_folder(self) -> Path:
```

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a3/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a3/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/base.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/meta.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/meta.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/fields.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/text_area.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/text_area.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a3/cfdraw/plugins/sync.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a3/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.0a3/cfdraw/schema/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a3/cfdraw/utils/template.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a2/setup.py` & `carefree-drawboard-0.0.0a3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.2"
+VERSION = "0.0.0-alpha.3"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -23,14 +23,15 @@
         "websockets",
         "watchdog",
         "python-multipart",
         "carefree-toolkit>=0.3.4",
         "pillow",
         "aiohttp",
         "charset-normalizer==2.1.0",
+        "tornado",
     ],
     author="carefree0910",
     author_email="syameimaru.saki@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="python carefree-learn drawboard",
```

