# Comparing `tmp/carefree-drawboard-0.0.0a3.tar.gz` & `tmp/carefree-drawboard-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a3.tar", last modified: Tue Apr 18 09:58:16 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a4.tar", last modified: Tue Apr 18 10:07:58 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a3.tar` & `carefree-drawboard-0.0.0a4.tar`

### file list

```diff
@@ -1,194 +1,192 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/LICENSE
--rw-rw-rw-   0        0        0       87 2023-04-18 09:58:12.000000 carefree-drawboard-0.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     9076 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     8793 2023-04-18 02:22:15.000000 carefree-drawboard-0.0.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.146011 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     9076 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5394 2023-04-18 09:58:16.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 09:58:14.000000 carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.148005 carefree-drawboard-0.0.0a3/cfdraw/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.152988 carefree-drawboard-0.0.0a3/cfdraw/.web/
--rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/.env
--rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/.prettierrc
--rw-rw-rw-   0        0        0   888829 2023-04-17 08:28:51.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/analyze.html
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/index.html
--rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/package.json
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.155982 carefree-drawboard-0.0.0a3/cfdraw/.web/src/
--rw-rw-rw-   0        0        0      901 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/App.tsx
--rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.159967 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/download.ts
--rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/export.ts
--rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.114205 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.159967 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.160964 carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/
--rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/BoardPanel.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.163954 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/
--rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.164951 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.165947 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.166944 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useUndoRedo.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.171440 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/settings.ts
--rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.176423 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/
--rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.178416 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/
--rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
--rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.180409 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.182402 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.183399 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.184396 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/
--rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3555 2023-04-17 15:25:00.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.184396 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/
--rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.187385 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/
--rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.190375 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/
--rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/_python.ts
--rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/projects.ts
--rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.192369 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/bem.ts
--rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/event.ts
--rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.paths.json
--rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/vite.config.ts
--rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a3/cfdraw/.web/yarn.lock
--rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a3/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.193366 carefree-drawboard-0.0.0a3/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-04-18 07:46:59.000000 carefree-drawboard-0.0.0a3/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.196356 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     1944 2023-04-18 06:33:13.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/plugins.py
--rw-rw-rw-   0        0        0     5713 2023-04-17 13:23:53.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     1813 2023-04-18 02:06:49.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     3485 2023-04-18 08:00:45.000000 carefree-drawboard-0.0.0a3/cfdraw/cli.py
--rw-rw-rw-   0        0        0     2226 2023-04-18 07:55:50.000000 carefree-drawboard-0.0.0a3/cfdraw/config.py
--rw-rw-rw-   0        0        0     1479 2023-04-18 07:48:42.000000 carefree-drawboard-0.0.0a3/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.197353 carefree-drawboard-0.0.0a3/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.200343 carefree-drawboard-0.0.0a3/cfdraw/plugins/
--rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.200343 carefree-drawboard-0.0.0a3/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/factory.py
--rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.203333 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0     1090 2023-04-17 09:56:46.000000 carefree-drawboard-0.0.0a3/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.204329 carefree-drawboard-0.0.0a3/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.206322 carefree-drawboard-0.0.0a3/cfdraw/server/
--rw-rw-rw-   0        0        0     1194 2023-04-18 09:42:33.000000 carefree-drawboard-0.0.0a3/cfdraw/server/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-04-18 07:04:07.000000 carefree-drawboard-0.0.0a3/cfdraw/server/http.py
--rw-rw-rw-   0        0        0      381 2023-04-18 07:40:33.000000 carefree-drawboard-0.0.0a3/cfdraw/server/index.py
--rw-rw-rw-   0        0        0     1459 2023-04-18 07:40:19.000000 carefree-drawboard-0.0.0a3/cfdraw/server/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:58:16.210310 carefree-drawboard-0.0.0a3/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     2781 2023-04-18 07:55:53.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a3/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      113 2023-04-18 09:58:16.211306 carefree-drawboard-0.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     1054 2023-04-18 09:57:02.000000 carefree-drawboard-0.0.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0      121 2023-04-18 10:04:06.000000 carefree-drawboard-0.0.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:58.854997 carefree-drawboard-0.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     8793 2023-04-18 02:22:15.000000 carefree-drawboard-0.0.0a4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.781726 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     9076 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5363 2023-04-18 10:07:58.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 10:07:57.000000 carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.783719 carefree-drawboard-0.0.0a4/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.786709 carefree-drawboard-0.0.0a4/cfdraw/.web/
+-rw-rw-rw-   0        0        0      121 2023-04-18 05:54:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1628 2023-04-18 02:10:06.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.789699 carefree-drawboard-0.0.0a4/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      895 2023-04-18 10:06:42.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx
+-rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.750433 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.794683 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.798669 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.799667 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.800663 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFText.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.802656 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     2940 2023-04-17 06:33:19.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useUndoRedo.ts
+-rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.806643 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.810629 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/
+-rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.813619 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
+-rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.814615 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.817607 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.818604 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.819600 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     3555 2023-04-17 15:25:00.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.821593 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      880 2023-04-17 14:19:55.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.826578 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts
+-rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.832561 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     1431 2023-04-17 09:56:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.835551 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      466 2023-04-17 06:32:01.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0     1849 2023-04-18 03:53:52.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   214083 2023-04-18 03:11:54.000000 carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a4/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.837544 carefree-drawboard-0.0.0a4/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     3022 2023-04-18 07:46:59.000000 carefree-drawboard-0.0.0a4/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.840534 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     1944 2023-04-18 06:33:13.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py
+-rw-rw-rw-   0        0        0     5713 2023-04-17 13:23:53.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     1813 2023-04-18 02:06:49.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     3485 2023-04-18 08:00:45.000000 carefree-drawboard-0.0.0a4/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     2226 2023-04-18 07:55:50.000000 carefree-drawboard-0.0.0a4/cfdraw/config.py
+-rw-rw-rw-   0        0        0     1479 2023-04-18 07:48:42.000000 carefree-drawboard-0.0.0a4/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.841530 carefree-drawboard-0.0.0a4/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/
+-rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.843524 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py
+-rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/meta.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.845027 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0     1090 2023-04-17 09:56:46.000000 carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.847024 carefree-drawboard-0.0.0a4/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.849017 carefree-drawboard-0.0.0a4/cfdraw/server/
+-rw-rw-rw-   0        0        0     1194 2023-04-18 09:42:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-04-18 07:04:07.000000 carefree-drawboard-0.0.0a4/cfdraw/server/http.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 07:40:33.000000 carefree-drawboard-0.0.0a4/cfdraw/server/index.py
+-rw-rw-rw-   0        0        0     1459 2023-04-18 07:40:19.000000 carefree-drawboard-0.0.0a4/cfdraw/server/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:07:58.854001 carefree-drawboard-0.0.0a4/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     2781 2023-04-18 07:55:53.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-17 13:24:23.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a4/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-18 10:07:58.855994 carefree-drawboard-0.0.0a4/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-04-18 10:07:27.000000 carefree-drawboard-0.0.0a4/setup.py
```

### Comparing `carefree-drawboard-0.0.0a3/LICENSE` & `carefree-drawboard-0.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/PKG-INFO` & `carefree-drawboard-0.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.0a3/README.md` & `carefree-drawboard-0.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.0a3/carefree_drawboard.egg-info/SOURCES.txt` & `carefree-drawboard-0.0.0a4/carefree_drawboard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 carefree_drawboard.egg-info/top_level.txt
 cfdraw/__init__.py
 cfdraw/cli.py
 cfdraw/config.py
 cfdraw/constants.py
 cfdraw/.web/.env
 cfdraw/.web/.prettierrc
-cfdraw/.web/analyze.html
 cfdraw/.web/index.html
 cfdraw/.web/package.json
 cfdraw/.web/tsconfig.json
 cfdraw/.web/tsconfig.node.json
 cfdraw/.web/tsconfig.paths.json
 cfdraw/.web/vite.config.ts
 cfdraw/.web/yarn.lock
 cfdraw/.web/src/App.tsx
+cfdraw/.web/src/BoardPanel.tsx
 cfdraw/.web/src/_settings.ts
 cfdraw/.web/src/index.scss
 cfdraw/.web/src/index.tsx
 cfdraw/.web/src/react-app-env.d.ts
 cfdraw/.web/src/reset.d.ts
 cfdraw/.web/src/vite-env.d.ts
 cfdraw/.web/src/actions/addImage.ts
@@ -37,15 +37,14 @@
 cfdraw/.web/src/actions/export.ts
 cfdraw/.web/src/actions/importMeta.ts
 cfdraw/.web/src/actions/managePlugins.ts
 cfdraw/.web/src/actions/manageProjects.ts
 cfdraw/.web/src/actions/update.ts
 cfdraw/.web/src/actions/uploadImage.ts
 cfdraw/.web/src/assets/icons/arrow-down.svg
-cfdraw/.web/src/board/BoardPanel.tsx
 cfdraw/.web/src/components/CFButton.tsx
 cfdraw/.web/src/components/CFDivider.tsx
 cfdraw/.web/src/components/CFHeading.tsx
 cfdraw/.web/src/components/CFImageUploader.tsx
 cfdraw/.web/src/components/CFInput.tsx
 cfdraw/.web/src/components/CFSlider.tsx
 cfdraw/.web/src/components/CFSwitch.tsx
```

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/package.json` & `carefree-drawboard-0.0.0a4/cfdraw/.web/package.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/App.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/App.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import { Flex } from "@chakra-ui/react";
 import { observer } from "mobx-react-lite";
 
 import { langStore } from "@carefree0910/business";
 
-import BoardPanel from "@/board/BoardPanel";
 import { useInitBoard } from "./hooks/useInitBoard";
 import { useFileDropper } from "./hooks/useFileDropper";
 import { useGridLines } from "./hooks/useGridLines";
 import { usePreventDefaults } from "./hooks/usePreventDefaults";
 import { useUndoRedo } from "./hooks/useUndoRedo";
 import { useSyncPython } from "./hooks/usePython";
+import BoardPanel from "./BoardPanel";
 
 function App() {
   useSyncPython();
   useInitBoard();
   useFileDropper(langStore.tgt);
   useGridLines();
   useUndoRedo();
```

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/_settings.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/_settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/addText.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/download.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/export.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/importMeta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/board/BoardPanel.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/hooks/usePython.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/add.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/brush.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/download.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/index.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/projects.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/settings.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/toast.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/lang/ui.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/AddPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/BrushPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DeletePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/DownloadPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/ProjectPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/SettingsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/TextEditorPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/index.tsx` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/actions.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/hooks.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/_python.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/meta.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/metaFields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/schema/requests.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/_python.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/meta.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/projects.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/theme.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/theme.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/stores/ui.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/event.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/misc.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/src/utils/toast.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/tsconfig.json` & `carefree-drawboard-0.0.0a4/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/vite.config.ts` & `carefree-drawboard-0.0.0a4/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/.web/yarn.lock` & `carefree-drawboard-0.0.0a4/cfdraw/.web/yarn.lock`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/plugins.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/upload.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/endpoints/websocket.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/app/schema.py` & `carefree-drawboard-0.0.0a4/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/cli.py` & `carefree-drawboard-0.0.0a4/cfdraw/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/config.py` & `carefree-drawboard-0.0.0a4/cfdraw/config.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/constants.py` & `carefree-drawboard-0.0.0a4/cfdraw/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a4/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a4/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/base.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/meta.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/meta.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/fields.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/text_area.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/text_area.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a4/cfdraw/plugins/sync.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a4/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.0a4/cfdraw/schema/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/server/__init__.py` & `carefree-drawboard-0.0.0a4/cfdraw/server/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/server/http.py` & `carefree-drawboard-0.0.0a4/cfdraw/server/http.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/server/socket.py` & `carefree-drawboard-0.0.0a4/cfdraw/server/socket.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/exec.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a4/cfdraw/utils/template.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a3/setup.py` & `carefree-drawboard-0.0.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.3"
+VERSION = "0.0.0-alpha.4"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

