# Comparing `tmp/zenoml-0.4.7.tar.gz` & `tmp/zenoml-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenoml-0.4.7.tar", max compression
+gzip compressed data, was "zenoml-0.4.8.tar", max compression
```

## Comparing `zenoml-0.4.7.tar` & `zenoml-0.4.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1081 2022-02-24 19:12:18.966638 zenoml-0.4.7/LICENSE.md
--rw-r--r--   0        0        0     4488 2023-04-17 23:18:23.305935 zenoml-0.4.7/README.md
--rw-r--r--   0        0        0     1321 2023-04-17 23:18:35.286697 zenoml-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-17 23:18:23.328202 zenoml-0.4.7/zeno/__init__.py
--rw-r--r--   0        0        0       53 2023-04-16 15:12:31.655723 zenoml-0.4.7/zeno/__main__.py
--rwxr-xr-x   0        0        0     5943 2023-04-16 15:12:31.814437 zenoml-0.4.7/zeno/api.py
--rw-r--r--   0        0        0    21519 2023-04-16 15:12:31.891037 zenoml-0.4.7/zeno/backend.py
--rw-r--r--   0        0        0     1543 2023-04-16 15:12:31.667539 zenoml-0.4.7/zeno/classes/base.py
--rw-r--r--   0        0        0     1340 2023-04-16 15:12:31.756077 zenoml-0.4.7/zeno/classes/classes.py
--rw-r--r--   0        0        0      821 2023-04-16 15:12:31.639350 zenoml-0.4.7/zeno/classes/metadata.py
--rw-r--r--   0        0        0      487 2023-04-16 15:12:31.638895 zenoml-0.4.7/zeno/classes/projection.py
--rw-r--r--   0        0        0      692 2023-04-16 15:12:31.736743 zenoml-0.4.7/zeno/classes/report.py
--rw-r--r--   0        0        0      650 2023-04-16 15:12:31.677226 zenoml-0.4.7/zeno/classes/slice.py
--rw-r--r--   0        0        0     6148 2023-02-07 21:13:15.301646 zenoml-0.4.7/zeno/frontend/.DS_Store
--rw-r--r--   0        0        0  1844175 2023-04-17 23:19:05.657730 zenoml-0.4.7/zeno/frontend/build/assets/main.5a7a7111.js
--rw-r--r--   0        0        0    57544 2023-04-17 23:19:05.657204 zenoml-0.4.7/zeno/frontend/build/assets/main.6757dad9.css
--rw-r--r--   0        0        0     1173 2023-04-17 23:19:04.384539 zenoml-0.4.7/zeno/frontend/build/favicon.png
--rw-r--r--   0        0        0     1016 2023-04-17 23:19:04.385260 zenoml-0.4.7/zeno/frontend/build/global.css
--rw-r--r--   0        0        0      255 2023-04-17 23:19:05.657268 zenoml-0.4.7/zeno/frontend/build/manifest.json
--rw-r--r--   0        0        0   370831 2023-04-17 23:19:04.388186 zenoml-0.4.7/zeno/frontend/build/smui.css
--rw-r--r--   0        0        0    17353 2023-04-17 23:19:04.389588 zenoml-0.4.7/zeno/frontend/build/zeno.png
--rw-r--r--   0        0        0      863 2023-04-17 23:19:06.058249 zenoml-0.4.7/zeno/frontend/index.html
--rw-r--r--   0        0        0      881 2023-03-08 02:24:41.317296 zenoml-0.4.7/zeno/frontend/index_og.html
--rw-r--r--   0        0        0     6519 2023-04-16 15:12:31.752207 zenoml-0.4.7/zeno/processing/data_processing.py
--rw-r--r--   0        0        0     2980 2023-04-16 15:12:31.700099 zenoml-0.4.7/zeno/processing/filtering.py
--rw-r--r--   0        0        0     6985 2023-04-16 15:12:31.830529 zenoml-0.4.7/zeno/processing/histogram_processing.py
--rw-r--r--   0        0        0     3585 2023-04-16 15:12:31.727047 zenoml-0.4.7/zeno/processing/projection_processing.py
--rwxr-xr-x   0        0        0     2946 2023-04-17 23:18:23.328661 zenoml-0.4.7/zeno/runner.py
--rw-r--r--   0        0        0     8672 2023-04-16 15:12:31.796712 zenoml-0.4.7/zeno/server.py
--rw-r--r--   0        0        0     2834 2023-04-16 15:12:31.713471 zenoml-0.4.7/zeno/setup.py
--rw-r--r--   0        0        0     7275 2023-04-16 15:12:31.824953 zenoml-0.4.7/zeno/util.py
--rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 zenoml-0.4.7/setup.py
--rw-r--r--   0        0        0     5701 1970-01-01 00:00:00.000000 zenoml-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-02-24 19:12:18.966638 zenoml-0.4.8/LICENSE.md
+-rw-r--r--   0        0        0     4488 2023-04-17 23:18:23.305935 zenoml-0.4.8/README.md
+-rw-r--r--   0        0        0     1321 2023-04-17 23:50:53.917446 zenoml-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-17 23:18:23.328202 zenoml-0.4.8/zeno/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-16 15:12:31.655723 zenoml-0.4.8/zeno/__main__.py
+-rwxr-xr-x   0        0        0     5943 2023-04-16 15:12:31.814437 zenoml-0.4.8/zeno/api.py
+-rw-r--r--   0        0        0    21519 2023-04-16 15:12:31.891037 zenoml-0.4.8/zeno/backend.py
+-rw-r--r--   0        0        0     1543 2023-04-16 15:12:31.667539 zenoml-0.4.8/zeno/classes/base.py
+-rw-r--r--   0        0        0     1340 2023-04-16 15:12:31.756077 zenoml-0.4.8/zeno/classes/classes.py
+-rw-r--r--   0        0        0      821 2023-04-16 15:12:31.639350 zenoml-0.4.8/zeno/classes/metadata.py
+-rw-r--r--   0        0        0      487 2023-04-16 15:12:31.638895 zenoml-0.4.8/zeno/classes/projection.py
+-rw-r--r--   0        0        0      692 2023-04-16 15:12:31.736743 zenoml-0.4.8/zeno/classes/report.py
+-rw-r--r--   0        0        0      650 2023-04-16 15:12:31.677226 zenoml-0.4.8/zeno/classes/slice.py
+-rw-r--r--   0        0        0     6148 2023-02-07 21:13:15.301646 zenoml-0.4.8/zeno/frontend/.DS_Store
+-rw-r--r--   0        0        0    57544 2023-04-17 23:51:23.258796 zenoml-0.4.8/zeno/frontend/build/assets/main.6757dad9.css
+-rw-r--r--   0        0        0  1844244 2023-04-17 23:51:23.259457 zenoml-0.4.8/zeno/frontend/build/assets/main.f60e39ea.js
+-rw-r--r--   0        0        0     1173 2023-04-17 23:51:22.045382 zenoml-0.4.8/zeno/frontend/build/favicon.png
+-rw-r--r--   0        0        0     1016 2023-04-17 23:51:22.046319 zenoml-0.4.8/zeno/frontend/build/global.css
+-rw-r--r--   0        0        0      255 2023-04-17 23:51:23.258724 zenoml-0.4.8/zeno/frontend/build/manifest.json
+-rw-r--r--   0        0        0   370831 2023-04-17 23:51:22.049558 zenoml-0.4.8/zeno/frontend/build/smui.css
+-rw-r--r--   0        0        0    17353 2023-04-17 23:51:22.051391 zenoml-0.4.8/zeno/frontend/build/zeno.png
+-rw-r--r--   0        0        0      863 2023-04-17 23:51:23.647365 zenoml-0.4.8/zeno/frontend/index.html
+-rw-r--r--   0        0        0      881 2023-03-08 02:24:41.317296 zenoml-0.4.8/zeno/frontend/index_og.html
+-rw-r--r--   0        0        0     6519 2023-04-16 15:12:31.752207 zenoml-0.4.8/zeno/processing/data_processing.py
+-rw-r--r--   0        0        0     2980 2023-04-16 15:12:31.700099 zenoml-0.4.8/zeno/processing/filtering.py
+-rw-r--r--   0        0        0     6985 2023-04-16 15:12:31.830529 zenoml-0.4.8/zeno/processing/histogram_processing.py
+-rw-r--r--   0        0        0     3585 2023-04-16 15:12:31.727047 zenoml-0.4.8/zeno/processing/projection_processing.py
+-rwxr-xr-x   0        0        0     2946 2023-04-17 23:18:23.328661 zenoml-0.4.8/zeno/runner.py
+-rw-r--r--   0        0        0     8672 2023-04-16 15:12:31.796712 zenoml-0.4.8/zeno/server.py
+-rw-r--r--   0        0        0     2834 2023-04-16 15:12:31.713471 zenoml-0.4.8/zeno/setup.py
+-rw-r--r--   0        0        0     7275 2023-04-16 15:12:31.824953 zenoml-0.4.8/zeno/util.py
+-rw-r--r--   0        0        0     5800 1970-01-01 00:00:00.000000 zenoml-0.4.8/setup.py
+-rw-r--r--   0        0        0     5701 1970-01-01 00:00:00.000000 zenoml-0.4.8/PKG-INFO
```

### Comparing `zenoml-0.4.7/LICENSE.md` & `zenoml-0.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/README.md` & `zenoml-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/pyproject.toml` & `zenoml-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zenoml"
-version = "0.4.7"
+version = "0.4.8"
 description = "Interactive Evaluation Framework for Machine Learning"
 license = "MIT"
 authors = ["Ángel Alexander Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/zeno-ml/zeno"
 homepage = "https://zenoml.com"
 keywords = ["ml", "testing", "evaluation", "machine learning", "ai"]
```

### Comparing `zenoml-0.4.7/zeno/api.py` & `zenoml-0.4.8/zeno/api.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/backend.py` & `zenoml-0.4.8/zeno/backend.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/classes/base.py` & `zenoml-0.4.8/zeno/classes/base.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/classes/classes.py` & `zenoml-0.4.8/zeno/classes/classes.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/classes/metadata.py` & `zenoml-0.4.8/zeno/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/classes/report.py` & `zenoml-0.4.8/zeno/classes/report.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/classes/slice.py` & `zenoml-0.4.8/zeno/classes/slice.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/.DS_Store` & `zenoml-0.4.8/zeno/frontend/.DS_Store`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/build/assets/main.5a7a7111.js` & `zenoml-0.4.8/zeno/frontend/build/assets/main.f60e39ea.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5022,15 +5022,15 @@
                 this._cancelHandlers.length = 0, this._reject?.(new Wse("Request aborted"))
             }
         }
         get isCancelled() {
             return this._isCancelled
         }
     }
-    const Cs = {
+    const ys = {
         BASE: "/api",
         VERSION: "0.1.0",
         WITH_CREDENTIALS: !1,
         CREDENTIALS: "include",
         TOKEN: void 0,
         USERNAME: void 0,
         PASSWORD: void 0,
@@ -5160,200 +5160,200 @@
                 }
             } catch (s) {
                 i(s)
             }
         });
     class rs {
         static getSettings() {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/settings"
             })
         }
         static getInitialInfo() {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/initialize"
             })
         }
         static getSlices() {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/slices"
             })
         }
         static getReports() {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/reports"
             })
         }
         static updateReports(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/reports",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static setFolders(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/folders",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static getFilteredIds(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/filtered-ids",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static getFilteredTable(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/filtered-table",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static refreshData() {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/refresh"
             })
         }
         static getHistogramBuckets(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/histograms",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static calculateHistogramCounts(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/histogram-counts",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static calculateHistogramMetrics(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/histogram-metrics",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static createNewSlice(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/slice",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static deleteSlice(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "DELETE",
                 url: "/slice",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static filterStringMetadata(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/string-filter",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static getMetricsForSlices(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/slice-metrics",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static embedExists(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "GET",
                 url: "/embed-exists/{model}",
                 path: {
                     model: t
                 },
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static projectEmbedInto2D(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/embed-project",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static getProjectionColors(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/colors-project",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
             })
         }
         static getDfRowEntry(t) {
-            return Ts(Cs, {
+            return Ts(ys, {
                 method: "POST",
                 url: "/entry",
                 body: t,
                 mediaType: "application/json",
                 errors: {
                     422: "Validation Error"
                 }
@@ -8887,18 +8887,18 @@
         e_ = {
             TRANSITION_OPEN_DURATION: 120,
             TRANSITION_CLOSE_DURATION: 75,
             MARGIN_TO_EDGE: 32,
             ANCHOR_TO_MENU_SURFACE_WIDTH_RATIO: .67,
             TOUCH_EVENT_WAIT_MS: 30
         },
-        Es;
+        Ss;
     (function(e) {
         e[e.BOTTOM = 1] = "BOTTOM", e[e.CENTER = 2] = "CENTER", e[e.RIGHT = 4] = "RIGHT", e[e.FLIP_RTL = 8] = "FLIP_RTL"
-    })(Es || (Es = {}));
+    })(Ss || (Ss = {}));
     var Rm;
     (function(e) {
         e[e.TOP_LEFT = 0] = "TOP_LEFT", e[e.TOP_RIGHT = 4] = "TOP_RIGHT", e[e.BOTTOM_LEFT = 1] = "BOTTOM_LEFT", e[e.BOTTOM_RIGHT = 5] = "BOTTOM_RIGHT", e[e.TOP_START = 8] = "TOP_START", e[e.TOP_END = 12] = "TOP_END", e[e.BOTTOM_START = 9] = "BOTTOM_START", e[e.BOTTOM_END = 13] = "BOTTOM_END"
     })(Rm || (Rm = {}));
     /**
      * @license
      * Copyright 2018 Google Inc.
@@ -8964,15 +8964,15 @@
     .` + np[Hi.LIST_ITEM_CLASS] + ` a,
     .` + np[Hi.LIST_ITEM_CLASS] + ` input[type="radio"]:not(:disabled),
     .` + np[Hi.LIST_ITEM_CLASS] + ` input[type="checkbox"]:not(:disabled)
   `,
             RADIO_SELECTOR: 'input[type="radio"]',
             SELECTED_ITEM_SELECTOR: '[aria-selected="true"], [aria-current="true"]'
         },
-        ys = {
+        Es = {
             UNSET_INDEX: -1,
             TYPEAHEAD_BUFFER_CLEAR_TIMEOUT_MS: 300
         };
     /**
      * @license
      * Copyright 2020 Google Inc.
      *
@@ -9057,15 +9057,15 @@
             i = e.focusItemAtIndex,
             r = e.sortedIndexByFirstChar,
             s = e.focusedItemIndex,
             o = e.skipFocus,
             a = e.isItemAtIndexDisabled;
         clearTimeout(t.bufferClearTimeout), t.bufferClearTimeout = setTimeout(function() {
             WV(t)
-        }, ys.TYPEAHEAD_BUFFER_CLEAR_TIMEOUT_MS), t.typeaheadBuffer = t.typeaheadBuffer + n;
+        }, Es.TYPEAHEAD_BUFFER_CLEAR_TIMEOUT_MS), t.typeaheadBuffer = t.typeaheadBuffer + n;
         var l;
         return t.typeaheadBuffer.length === 1 ? l = Lae(r, s, a, t) : l = Mae(r, a, t), l !== -1 && !o && i(l), l
     }
 
     function Lae(e, t, n, i) {
         var r = i.typeaheadBuffer[0],
             s = e.get(r);
@@ -9199,15 +9199,15 @@
         }
     }
     var xae = function(e) {
         Ho(t, e);
 
         function t(n) {
             var i = e.call(this, Zi(Zi({}, t.defaultAdapter), n)) || this;
-            return i.wrapFocus = !1, i.isVertical = !0, i.isSingleSelectionList = !1, i.areDisabledItemsFocusable = !0, i.selectedIndex = ys.UNSET_INDEX, i.focusedItemIndex = ys.UNSET_INDEX, i.useActivatedClass = !1, i.useSelectedAttr = !1, i.ariaCurrentAttrValue = null, i.isCheckboxList = !1, i.isRadioList = !1, i.lastSelectedIndex = null, i.hasTypeahead = !1, i.typeaheadState = kae(), i.sortedIndexByFirstChar = new Map, i
+            return i.wrapFocus = !1, i.isVertical = !0, i.isSingleSelectionList = !1, i.areDisabledItemsFocusable = !0, i.selectedIndex = Es.UNSET_INDEX, i.focusedItemIndex = Es.UNSET_INDEX, i.useActivatedClass = !1, i.useSelectedAttr = !1, i.ariaCurrentAttrValue = null, i.isCheckboxList = !1, i.isRadioList = !1, i.lastSelectedIndex = null, i.hasTypeahead = !1, i.typeaheadState = kae(), i.sortedIndexByFirstChar = new Map, i
         }
         return Object.defineProperty(t, "strings", {
             get: function() {
                 return gd
             },
             enumerable: !1,
             configurable: !0
@@ -9215,15 +9215,15 @@
             get: function() {
                 return Hi
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(t, "numbers", {
             get: function() {
-                return ys
+                return Es
             },
             enumerable: !1,
             configurable: !0
         }), Object.defineProperty(t, "defaultAdapter", {
             get: function() {
                 return {
                     addClassForElementIndex: function() {},
@@ -9278,20 +9278,20 @@
             this.isVertical = n
         }, t.prototype.setSingleSelection = function(n) {
             this.isSingleSelectionList = n, n && (this.maybeInitializeSingleSelection(), this.selectedIndex = this.getSelectedIndexFromDOM())
         }, t.prototype.setDisabledItemsFocusable = function(n) {
             this.areDisabledItemsFocusable = n
         }, t.prototype.maybeInitializeSingleSelection = function() {
             var n = this.getSelectedIndexFromDOM();
-            if (n !== ys.UNSET_INDEX) {
+            if (n !== Es.UNSET_INDEX) {
                 var i = this.adapter.listItemAtIndexHasClass(n, Hi.LIST_ITEM_ACTIVATED_CLASS);
                 i && this.setUseActivatedClass(!0), this.isSingleSelectionList = !0, this.selectedIndex = n
             }
         }, t.prototype.getSelectedIndexFromDOM = function() {
-            for (var n = ys.UNSET_INDEX, i = this.adapter.getListItemCount(), r = 0; r < i; r++) {
+            for (var n = Es.UNSET_INDEX, i = this.adapter.getListItemCount(), r = 0; r < i; r++) {
                 var s = this.adapter.listItemAtIndexHasClass(r, Hi.LIST_ITEM_SELECTED_CLASS),
                     o = this.adapter.listItemAtIndexHasClass(r, Hi.LIST_ITEM_ACTIVATED_CLASS);
                 if (!!(s || o)) {
                     n = r;
                     break
                 }
             }
@@ -9376,15 +9376,15 @@
                 else if (d && b([])) Cl(n), this.focusLastElement();
                 else if (f && b(["Control", "Shift"]) && this.isCheckboxList) {
                     if (Cl(n), this.isIndexDisabled(E)) return;
                     this.focusFirstElement(), this.toggleCheckboxRange(0, E, E)
                 } else if (d && b(["Control", "Shift"]) && this.isCheckboxList) {
                     if (Cl(n), this.isIndexDisabled(E)) return;
                     this.focusLastElement(), this.toggleCheckboxRange(E, this.adapter.getListItemCount() - 1, E)
-                } else if (_ && b(["Control"]) && this.isCheckboxList) n.preventDefault(), this.checkboxListToggleAll(this.selectedIndex === ys.UNSET_INDEX ? [] : this.selectedIndex, !0);
+                } else if (_ && b(["Control"]) && this.isCheckboxList) n.preventDefault(), this.checkboxListToggleAll(this.selectedIndex === Es.UNSET_INDEX ? [] : this.selectedIndex, !0);
                 else if ((h || m) && b([])) {
                     if (i) {
                         var A = n.target;
                         if (A && A.tagName === "A" && h || (Cl(n), this.isIndexDisabled(E))) return;
                         this.isTypeaheadInProgress() || (this.isSelectableList() && this.setSelectedIndexOnAction(E, !1), this.adapter.notifyAction(E))
                     }
                 } else if ((h || m) && b(["Shift"]) && this.isCheckboxList) {
@@ -9406,15 +9406,15 @@
                         }
                     };
                     p8(S, this.typeaheadState)
                 }
             }
         }, t.prototype.handleClick = function(n, i, r) {
             var s, o = _8(r);
-            n !== ys.UNSET_INDEX && (this.isIndexDisabled(n) || (o([]) ? (this.isSelectableList() && this.setSelectedIndexOnAction(n, i), this.adapter.notifyAction(n)) : this.isCheckboxList && o(["Shift"]) && (this.toggleCheckboxRange((s = this.lastSelectedIndex) !== null && s !== void 0 ? s : n, n, n), this.adapter.notifyAction(n))))
+            n !== Es.UNSET_INDEX && (this.isIndexDisabled(n) || (o([]) ? (this.isSelectableList() && this.setSelectedIndexOnAction(n, i), this.adapter.notifyAction(n)) : this.isCheckboxList && o(["Shift"]) && (this.toggleCheckboxRange((s = this.lastSelectedIndex) !== null && s !== void 0 ? s : n, n, n), this.adapter.notifyAction(n))))
         }, t.prototype.focusNextElement = function(n) {
             var i = this.adapter.getListItemCount(),
                 r = n,
                 s = null;
             do {
                 if (r++, r >= i)
                     if (this.wrapFocus) r = 0;
@@ -9443,80 +9443,80 @@
             var n = this.getFirstSelectedOrFocusedItemIndex();
             return this.focusItemAtIndex(n), n
         }, t.prototype.setEnabled = function(n, i) {
             !this.isIndexValid(n, !1) || (i ? (this.adapter.removeClassForElementIndex(n, Hi.LIST_ITEM_DISABLED_CLASS), this.adapter.setAttributeForElementIndex(n, gd.ARIA_DISABLED, "false")) : (this.adapter.addClassForElementIndex(n, Hi.LIST_ITEM_DISABLED_CLASS), this.adapter.setAttributeForElementIndex(n, gd.ARIA_DISABLED, "true")))
         }, t.prototype.setSingleSelectionAtIndex = function(n, i) {
             if (i === void 0 && (i = {}), !(this.selectedIndex === n && !i.forceUpdate)) {
                 var r = Hi.LIST_ITEM_SELECTED_CLASS;
-                this.useActivatedClass && (r = Hi.LIST_ITEM_ACTIVATED_CLASS), this.selectedIndex !== ys.UNSET_INDEX && this.adapter.removeClassForElementIndex(this.selectedIndex, r), this.setAriaForSingleSelectionAtIndex(n), this.setTabindexAtIndex(n), n !== ys.UNSET_INDEX && this.adapter.addClassForElementIndex(n, r), this.selectedIndex = n, i.isUserInteraction && !i.forceUpdate && this.adapter.notifySelectionChange([n])
+                this.useActivatedClass && (r = Hi.LIST_ITEM_ACTIVATED_CLASS), this.selectedIndex !== Es.UNSET_INDEX && this.adapter.removeClassForElementIndex(this.selectedIndex, r), this.setAriaForSingleSelectionAtIndex(n), this.setTabindexAtIndex(n), n !== Es.UNSET_INDEX && this.adapter.addClassForElementIndex(n, r), this.selectedIndex = n, i.isUserInteraction && !i.forceUpdate && this.adapter.notifySelectionChange([n])
             }
         }, t.prototype.setAriaForSingleSelectionAtIndex = function(n) {
-            this.selectedIndex === ys.UNSET_INDEX && (this.ariaCurrentAttrValue = this.adapter.getAttributeForElementIndex(n, gd.ARIA_CURRENT));
+            this.selectedIndex === Es.UNSET_INDEX && (this.ariaCurrentAttrValue = this.adapter.getAttributeForElementIndex(n, gd.ARIA_CURRENT));
             var i = this.ariaCurrentAttrValue !== null,
                 r = i ? gd.ARIA_CURRENT : gd.ARIA_SELECTED;
-            if (this.selectedIndex !== ys.UNSET_INDEX && this.adapter.setAttributeForElementIndex(this.selectedIndex, r, "false"), n !== ys.UNSET_INDEX) {
+            if (this.selectedIndex !== Es.UNSET_INDEX && this.adapter.setAttributeForElementIndex(this.selectedIndex, r, "false"), n !== Es.UNSET_INDEX) {
                 var s = i ? this.ariaCurrentAttrValue : "true";
                 this.adapter.setAttributeForElementIndex(n, r, s)
             }
         }, t.prototype.getSelectionAttribute = function() {
             return this.useSelectedAttr ? gd.ARIA_SELECTED : gd.ARIA_CHECKED
         }, t.prototype.setRadioAtIndex = function(n, i) {
             i === void 0 && (i = {});
             var r = this.getSelectionAttribute();
-            this.adapter.setCheckedCheckboxOrRadioAtIndex(n, !0), !(this.selectedIndex === n && !i.forceUpdate) && (this.selectedIndex !== ys.UNSET_INDEX && this.adapter.setAttributeForElementIndex(this.selectedIndex, r, "false"), this.adapter.setAttributeForElementIndex(n, r, "true"), this.selectedIndex = n, i.isUserInteraction && !i.forceUpdate && this.adapter.notifySelectionChange([n]))
+            this.adapter.setCheckedCheckboxOrRadioAtIndex(n, !0), !(this.selectedIndex === n && !i.forceUpdate) && (this.selectedIndex !== Es.UNSET_INDEX && this.adapter.setAttributeForElementIndex(this.selectedIndex, r, "false"), this.adapter.setAttributeForElementIndex(n, r, "true"), this.selectedIndex = n, i.isUserInteraction && !i.forceUpdate && this.adapter.notifySelectionChange([n]))
         }, t.prototype.setCheckboxAtIndex = function(n, i) {
             i === void 0 && (i = {});
-            for (var r = this.selectedIndex, s = i.isUserInteraction ? new Set(r === ys.UNSET_INDEX ? [] : r) : null, o = this.getSelectionAttribute(), a = [], l = 0; l < this.adapter.getListItemCount(); l++) {
+            for (var r = this.selectedIndex, s = i.isUserInteraction ? new Set(r === Es.UNSET_INDEX ? [] : r) : null, o = this.getSelectionAttribute(), a = [], l = 0; l < this.adapter.getListItemCount(); l++) {
                 var u = s?.has(l),
                     c = n.indexOf(l) >= 0;
                 c !== u && a.push(l), this.adapter.setCheckedCheckboxOrRadioAtIndex(l, c), this.adapter.setAttributeForElementIndex(l, o, c ? "true" : "false")
             }
             this.selectedIndex = n, i.isUserInteraction && a.length && this.adapter.notifySelectionChange(a)
         }, t.prototype.toggleCheckboxRange = function(n, i, r) {
             this.lastSelectedIndex = r;
-            for (var s = new Set(this.selectedIndex === ys.UNSET_INDEX ? [] : this.selectedIndex), o = !s?.has(r), a = Ex([n, i].sort(), 2), l = a[0], u = a[1], c = this.getSelectionAttribute(), f = [], d = l; d <= u; d++)
+            for (var s = new Set(this.selectedIndex === Es.UNSET_INDEX ? [] : this.selectedIndex), o = !s?.has(r), a = Ex([n, i].sort(), 2), l = a[0], u = a[1], c = this.getSelectionAttribute(), f = [], d = l; d <= u; d++)
                 if (!this.isIndexDisabled(d)) {
                     var h = s.has(d);
                     o !== h && (f.push(d), this.adapter.setCheckedCheckboxOrRadioAtIndex(d, o), this.adapter.setAttributeForElementIndex(d, c, "" + o), o ? s.add(d) : s.delete(d))
                 } f.length && (this.selectedIndex = yre([], Ex(s)), this.adapter.notifySelectionChange(f))
         }, t.prototype.setTabindexAtIndex = function(n) {
-            this.focusedItemIndex === ys.UNSET_INDEX && n !== 0 ? this.adapter.setAttributeForElementIndex(0, "tabindex", "-1") : this.focusedItemIndex >= 0 && this.focusedItemIndex !== n && this.adapter.setAttributeForElementIndex(this.focusedItemIndex, "tabindex", "-1"), !(this.selectedIndex instanceof Array) && this.selectedIndex !== n && this.adapter.setAttributeForElementIndex(this.selectedIndex, "tabindex", "-1"), n !== ys.UNSET_INDEX && this.adapter.setAttributeForElementIndex(n, "tabindex", "0")
+            this.focusedItemIndex === Es.UNSET_INDEX && n !== 0 ? this.adapter.setAttributeForElementIndex(0, "tabindex", "-1") : this.focusedItemIndex >= 0 && this.focusedItemIndex !== n && this.adapter.setAttributeForElementIndex(this.focusedItemIndex, "tabindex", "-1"), !(this.selectedIndex instanceof Array) && this.selectedIndex !== n && this.adapter.setAttributeForElementIndex(this.selectedIndex, "tabindex", "-1"), n !== Es.UNSET_INDEX && this.adapter.setAttributeForElementIndex(n, "tabindex", "0")
         }, t.prototype.isSelectableList = function() {
             return this.isSingleSelectionList || this.isCheckboxList || this.isRadioList
         }, t.prototype.setTabindexToFirstSelectedOrFocusedItem = function() {
             var n = this.getFirstSelectedOrFocusedItemIndex();
             this.setTabindexAtIndex(n)
         }, t.prototype.getFirstSelectedOrFocusedItemIndex = function() {
-            return this.isSelectableList() ? typeof this.selectedIndex == "number" && this.selectedIndex !== ys.UNSET_INDEX ? this.selectedIndex : Dae(this.selectedIndex) && this.selectedIndex.length > 0 ? this.selectedIndex.reduce(function(n, i) {
+            return this.isSelectableList() ? typeof this.selectedIndex == "number" && this.selectedIndex !== Es.UNSET_INDEX ? this.selectedIndex : Dae(this.selectedIndex) && this.selectedIndex.length > 0 ? this.selectedIndex.reduce(function(n, i) {
                 return Math.min(n, i)
             }) : 0 : Math.max(this.focusedItemIndex, 0)
         }, t.prototype.isIndexValid = function(n, i) {
             var r = this;
             if (i === void 0 && (i = !0), n instanceof Array) {
                 if (!this.isCheckboxList && i) throw new Error("MDCListFoundation: Array of index is only supported for checkbox based list");
                 return n.length === 0 ? !0 : n.some(function(s) {
                     return r.isIndexInRange(s)
                 })
             } else if (typeof n == "number") {
                 if (this.isCheckboxList && i) throw new Error("MDCListFoundation: Expected array of index for checkbox based list but got number: " + n);
-                return this.isIndexInRange(n) || this.isSingleSelectionList && n === ys.UNSET_INDEX
+                return this.isIndexInRange(n) || this.isSingleSelectionList && n === Es.UNSET_INDEX
             } else return !1
         }, t.prototype.isIndexInRange = function(n) {
             var i = this.adapter.getListItemCount();
             return n >= 0 && n < i
         }, t.prototype.setSelectedIndexOnAction = function(n, i) {
             this.lastSelectedIndex = n, this.isCheckboxList ? (this.toggleCheckboxAtIndex(n, i), this.adapter.notifySelectionChange([n])) : this.setSelectedIndex(n, {
                 isUserInteraction: !0
             })
         }, t.prototype.toggleCheckboxAtIndex = function(n, i) {
             var r = this.getSelectionAttribute(),
                 s = this.adapter.isCheckboxCheckedAtIndex(n),
                 o;
             i ? o = s : (o = !s, this.adapter.setCheckedCheckboxOrRadioAtIndex(n, o)), this.adapter.setAttributeForElementIndex(n, r, o ? "true" : "false");
-            var a = this.selectedIndex === ys.UNSET_INDEX ? [] : this.selectedIndex.slice();
+            var a = this.selectedIndex === Es.UNSET_INDEX ? [] : this.selectedIndex.slice();
             o ? a.push(n) : a = a.filter(function(l) {
                 return l !== n
             }), this.selectedIndex = a
         }, t.prototype.focusItemAtIndex = function(n) {
             this.adapter.focusItemAtIndex(n), this.focusedItemIndex = n
         }, t.prototype.checkboxListToggleAll = function(n, i) {
             var r = this.adapter.getListItemCount();
@@ -9679,15 +9679,15 @@
             if (!this.adapter.hasClass(i)) throw new Error(i + " class required in root element.");
             this.adapter.hasClass(r) && (this.isSurfaceOpen = !0)
         }, t.prototype.destroy = function() {
             clearTimeout(this.openAnimationEndTimerId), clearTimeout(this.closeAnimationEndTimerId), cancelAnimationFrame(this.animationRequestId)
         }, t.prototype.setAnchorCorner = function(n) {
             this.anchorCorner = n
         }, t.prototype.flipCornerHorizontally = function() {
-            this.originCorner = this.originCorner ^ Es.RIGHT
+            this.originCorner = this.originCorner ^ Ss.RIGHT
         }, t.prototype.setAnchorMargin = function(n) {
             this.anchorMargin.top = n.top || 0, this.anchorMargin.right = n.right || 0, this.anchorMargin.bottom = n.bottom || 0, this.anchorMargin.left = n.left || 0
         }, t.prototype.setIsHoisted = function(n) {
             this.isHoistedElement = n
         }, t.prototype.setFixedPosition = function(n) {
             this.isFixedPosition = n
         }, t.prototype.isFixed = function() {
@@ -9733,23 +9733,23 @@
                 s = r === "Escape" || i === 27;
             s && this.close()
         }, t.prototype.autoposition = function() {
             var n;
             this.measurements = this.getAutoLayoutmeasurements();
             var i = this.getoriginCorner(),
                 r = this.getMenuSurfaceMaxHeight(i),
-                s = this.hasBit(i, Es.BOTTOM) ? "bottom" : "top",
-                o = this.hasBit(i, Es.RIGHT) ? "right" : "left",
+                s = this.hasBit(i, Ss.BOTTOM) ? "bottom" : "top",
+                o = this.hasBit(i, Ss.RIGHT) ? "right" : "left",
                 a = this.getHorizontalOriginOffset(i),
                 l = this.getVerticalOriginOffset(i),
                 u = this.measurements,
                 c = u.anchorSize,
                 f = u.surfaceSize,
                 d = (n = {}, n[o] = a, n[s] = l, n);
-            c.width / f.width > e_.ANCHOR_TO_MENU_SURFACE_WIDTH_RATIO && (o = "center"), (this.isHoistedElement || this.isFixedPosition) && this.adjustPositionForHoistedElement(d), this.adapter.setTransformOrigin(o + " " + s), this.adapter.setPosition(d), this.adapter.setMaxHeight(r ? r + "px" : ""), this.hasBit(i, Es.BOTTOM) || this.adapter.addClass(t.cssClasses.IS_OPEN_BELOW)
+            c.width / f.width > e_.ANCHOR_TO_MENU_SURFACE_WIDTH_RATIO && (o = "center"), (this.isHoistedElement || this.isFixedPosition) && this.adjustPositionForHoistedElement(d), this.adapter.setTransformOrigin(o + " " + s), this.adapter.setPosition(d), this.adapter.setMaxHeight(r ? r + "px" : ""), this.hasBit(i, Ss.BOTTOM) || this.adapter.addClass(t.cssClasses.IS_OPEN_BELOW)
         }, t.prototype.getAutoLayoutmeasurements = function() {
             var n = this.adapter.getAnchorDimensions(),
                 i = this.adapter.getBodyDimensions(),
                 r = this.adapter.getWindowDimensions(),
                 s = this.adapter.getWindowScroll();
             return n || (n = {
                 top: this.position.y,
@@ -9774,51 +9774,51 @@
         }, t.prototype.getoriginCorner = function() {
             var n = this.originCorner,
                 i = this.measurements,
                 r = i.viewportDistance,
                 s = i.anchorSize,
                 o = i.surfaceSize,
                 a = t.numbers.MARGIN_TO_EDGE,
-                l = this.hasBit(this.anchorCorner, Es.BOTTOM),
+                l = this.hasBit(this.anchorCorner, Ss.BOTTOM),
                 u, c;
             l ? (u = r.top - a + this.anchorMargin.bottom, c = r.bottom - a - this.anchorMargin.bottom) : (u = r.top - a + this.anchorMargin.top, c = r.bottom - a + s.height - this.anchorMargin.top);
             var f = c - o.height > 0;
-            !f && u > c + this.openBottomBias && (n = this.setBit(n, Es.BOTTOM));
+            !f && u > c + this.openBottomBias && (n = this.setBit(n, Ss.BOTTOM));
             var d = this.adapter.isRtl(),
-                h = this.hasBit(this.anchorCorner, Es.FLIP_RTL),
-                m = this.hasBit(this.anchorCorner, Es.RIGHT) || this.hasBit(n, Es.RIGHT),
+                h = this.hasBit(this.anchorCorner, Ss.FLIP_RTL),
+                m = this.hasBit(this.anchorCorner, Ss.RIGHT) || this.hasBit(n, Ss.RIGHT),
                 g = !1;
             d && h ? g = !m : g = m;
             var p, _;
             g ? (p = r.left + s.width + this.anchorMargin.right, _ = r.right - this.anchorMargin.right) : (p = r.left + this.anchorMargin.left, _ = r.right + s.width - this.anchorMargin.left);
             var b = p - o.width > 0,
                 v = _ - o.width > 0,
-                S = this.hasBit(n, Es.FLIP_RTL) && this.hasBit(n, Es.RIGHT);
-            return v && S && d || !b && S ? n = this.unsetBit(n, Es.RIGHT) : (b && g && d || b && !g && m || !v && p >= _) && (n = this.setBit(n, Es.RIGHT)), n
+                S = this.hasBit(n, Ss.FLIP_RTL) && this.hasBit(n, Ss.RIGHT);
+            return v && S && d || !b && S ? n = this.unsetBit(n, Ss.RIGHT) : (b && g && d || b && !g && m || !v && p >= _) && (n = this.setBit(n, Ss.RIGHT)), n
         }, t.prototype.getMenuSurfaceMaxHeight = function(n) {
             if (this.maxHeight > 0) return this.maxHeight;
             var i = this.measurements.viewportDistance,
                 r = 0,
-                s = this.hasBit(n, Es.BOTTOM),
-                o = this.hasBit(this.anchorCorner, Es.BOTTOM),
+                s = this.hasBit(n, Ss.BOTTOM),
+                o = this.hasBit(this.anchorCorner, Ss.BOTTOM),
                 a = t.numbers.MARGIN_TO_EDGE;
             return s ? (r = i.top + this.anchorMargin.top - a, o || (r += this.measurements.anchorSize.height)) : (r = i.bottom - this.anchorMargin.bottom + this.measurements.anchorSize.height - a, o && (r -= this.measurements.anchorSize.height)), r
         }, t.prototype.getHorizontalOriginOffset = function(n) {
             var i = this.measurements.anchorSize,
-                r = this.hasBit(n, Es.RIGHT),
-                s = this.hasBit(this.anchorCorner, Es.RIGHT);
+                r = this.hasBit(n, Ss.RIGHT),
+                s = this.hasBit(this.anchorCorner, Ss.RIGHT);
             if (r) {
                 var o = s ? i.width - this.anchorMargin.left : this.anchorMargin.right;
                 return this.isHoistedElement || this.isFixedPosition ? o - (this.measurements.viewportSize.width - this.measurements.bodySize.width) : o
             }
             return s ? i.width - this.anchorMargin.right : this.anchorMargin.left
         }, t.prototype.getVerticalOriginOffset = function(n) {
             var i = this.measurements.anchorSize,
-                r = this.hasBit(n, Es.BOTTOM),
-                s = this.hasBit(this.anchorCorner, Es.BOTTOM),
+                r = this.hasBit(n, Ss.BOTTOM),
+                s = this.hasBit(this.anchorCorner, Ss.BOTTOM),
                 o = 0;
             return r ? o = s ? i.height - this.anchorMargin.top : -this.anchorMargin.bottom : o = s ? i.height + this.anchorMargin.bottom : this.anchorMargin.top, o
         }, t.prototype.adjustPositionForHoistedElement = function(n) {
             var i, r, s = this.measurements,
                 o = s.windowScroll,
                 a = s.viewportDistance,
                 l = s.surfaceSize,
@@ -17964,15 +17964,15 @@
                 Ot ? n(91, ce = Fn) : n(91, ce = Y ? Fn.map(tr => tr[yi]) : Wn.length ? Fn[yi] : null), n(59, Le = ce), n(60, Me = Fn)
             }
             e.$$.dirty[1] & 268435456 | e.$$.dirty[2] & 536870912 && ce !== Le && Ha(Le), e.$$.dirty[0] & 1073741824 | e.$$.dirty[2] & 256 && n(33, r = ve && Wn.length == ve), e.$$.dirty[0] & 2 | e.$$.dirty[1] & 12 | e.$$.dirty[2] & 1141768192 && n(32, s = r ? [] : wue(i, Ne ? null : f, Y ? gs : !1, Vt, Kt, ai)), e.$$.dirty[0] & 131072 | e.$$.dirty[1] & 10 && (o = Ye && f ? s.length : s.length - 1), e.$$.dirty[0] & 131072 | e.$$.dirty[1] & 10 | e.$$.dirty[2] & 67108864 && n(31, a = Tue(s, Ye && f, ai)), e.$$.dirty[0] & 33554432 | e.$$.dirty[1] & 1 && (qn === null ? n(25, qn = a.first) : qn > a.last ? n(25, qn = a.last) : qn < a.first && n(25, qn = a.first)), e.$$.dirty[0] & 805306368 | e.$$.dirty[1] & 134217742 | e.$$.dirty[2] & 268501248 && n(42, l = r ? Yn.max(ve) : f.length && s.length === 0 && Bt <= 1 ? Yn.nomatch : ae ? Bt <= 1 ? Yr ? Dr ? Yn.fetchInit : Yn.empty : Yn.fetchBefore : Yn.fetchQuery(Bt, f.length) : Yn.empty), e.$$.dirty[0] & 134217728 | e.$$.dirty[2] & 8 && n(41, u = typeof N == "function" ? N : kN[N] || kN.default.bind({
                 label: ui
             })), e.$$.dirty[1] & 50331656 && n(40, c = ut(f, E))
         }, [S, Y, p, _, b, v, T, C, k, I, j, W, J, fe, De, gt, Be, Ye, oe, We, Tt, G, Ft, _n, at, qn, fi, ui, Dr, Yn, Wn, a, s, r, f, Xn, xi, ur, Ws, cr, c, u, l, xn, ms, xs, Hr, Ps, Va, Vo, Xl, Bc, jc, qa, Sr, E, ut, Se, ae, Le, Me, A, y, w, D, N, z, V, U, ge, ve, _e, qe, we, ye, je, pt, ze, Bt, Vt, Kt, Ne, xt, Ot, vi, An, $t, vt, ai, Li, Yr, ce, i, m, qo, uo, Wa, Fu, g]
     }
-    class As extends Rt {
+    class ws extends Rt {
         constructor(t) {
             super(), kt(this, t, vce, _ce, At, {
                 name: 2,
                 inputId: 3,
                 required: 4,
                 hasAnchor: 5,
                 disabled: 0,
@@ -18611,15 +18611,15 @@
         let u = {
             options: e[12].filter(e[20]),
             labelAsValue: !0,
             closeAfterSelect: !0,
             multiple: !0,
             placeholder: "Select models to compare"
         };
-        e[5] !== void 0 && (u.value = e[5]), t = new As({
+        e[5] !== void 0 && (u.value = e[5]), t = new ws({
             props: u
         }), _t.push(() => Yi(t, "value", l));
         let c = e[1][e[6]] && FN(e);
         return o = new B4({
             props: {
                 slot: "paginate",
                 class: "pagination",
@@ -24836,53 +24836,53 @@
 
             function sx(P) {
                 return P.sort(function(X, le) {
                     return X === Yc ? -1 : le === Yc ? 1 : X < le ? -1 : 1
                 })
             }
 
-            function ws(P, X, le, He) {
+            function Cs(P, X, le, He) {
                 this.thisDep = P, this.contextDep = X, this.propDep = le, this.append = He
             }
 
             function fd(P) {
                 return P && !(P.thisDep || P.contextDep || P.propDep)
             }
 
             function as(P) {
-                return new ws(!1, !1, !1, P)
+                return new Cs(!1, !1, !1, P)
             }
 
             function ma(P, X) {
                 var le = P.type;
                 if (le === s3) {
                     var He = P.data.length;
-                    return new ws(!0, He >= 1, He >= 2, X)
+                    return new Cs(!0, He >= 1, He >= 2, X)
                 } else if (le === Yy) {
                     var rt = P.data;
-                    return new ws(rt.thisDep, rt.contextDep, rt.propDep, X)
+                    return new Cs(rt.thisDep, rt.contextDep, rt.propDep, X)
                 } else {
-                    if (le === LF) return new ws(!1, !1, !1, X);
+                    if (le === LF) return new Cs(!1, !1, !1, X);
                     if (le === MF) {
                         for (var Ue = !1, Ke = !1, yt = !1, bt = 0; bt < P.data.length; ++bt) {
                             var Lt = P.data[bt];
                             if (Lt.type === o3) yt = !0;
                             else if (Lt.type === a3) Ke = !0;
                             else if (Lt.type === l3) Ue = !0;
                             else if (Lt.type === s3) {
                                 Ue = !0;
                                 var Dt = Lt.data;
                                 Dt >= 1 && (Ke = !0), Dt >= 2 && (yt = !0)
                             } else Lt.type === Yy && (Ue = Ue || Lt.data.thisDep, Ke = Ke || Lt.data.contextDep, yt = yt || Lt.data.propDep)
                         }
-                        return new ws(Ue, Ke, yt, X)
-                    } else return new ws(le === l3, le === a3, le === o3, X)
+                        return new Cs(Ue, Ke, yt, X)
+                    } else return new Cs(le === l3, le === a3, le === o3, X)
                 }
             }
-            var ox = new ws(!1, !1, !1, function() {});
+            var ox = new Cs(!1, !1, !1, function() {});
 
             function aie(P, X, le, He, rt, Ue, Ke, yt, bt, Lt, Dt, Mt, Gt, St, It) {
                 var Ce = Lt.Record,
                     Xe = {
                         add: 32774,
                         subtract: 32778,
                         "reverse subtract": 32779
@@ -25065,15 +25065,15 @@
                         if (Z in Ae) {
                             var se = Ae[Z];
                             G.commandType(se, "object", "invalid " + Z, he.commandStr);
                             var Q = !0,
                                 xe = se.x | 0,
                                 Re = se.y | 0,
                                 et, lt;
-                            return "width" in se ? (et = se.width | 0, G.command(et >= 0, "invalid " + Z, he.commandStr)) : Q = !1, "height" in se ? (lt = se.height | 0, G.command(lt >= 0, "invalid " + Z, he.commandStr)) : Q = !1, new ws(!Q && q && q.thisDep, !Q && q && q.contextDep, !Q && q && q.propDep, function(Mn, un) {
+                            return "width" in se ? (et = se.width | 0, G.command(et >= 0, "invalid " + Z, he.commandStr)) : Q = !1, "height" in se ? (lt = se.height | 0, G.command(lt >= 0, "invalid " + Z, he.commandStr)) : Q = !1, new Cs(!Q && q && q.thisDep, !Q && q && q.contextDep, !Q && q && q.propDep, function(Mn, un) {
                                 var ct = Mn.shared.context,
                                     Qe = et;
                                 "width" in se || (Qe = un.def(ct, ".", $g, "-", xe));
                                 var vn = lt;
                                 return "height" in se || (vn = un.def(ct, ".", Zg, "-", Re)), [xe, Re, Qe, vn]
                             })
                         } else if (Z in Te) {
@@ -25089,23 +25089,23 @@
                                         Un = un.def('"width" in ', ct, "?", ct, ".width|0:", "(", Qe, ".", $g, "-", vn, ")"),
                                         Wi = un.def('"height" in ', ct, "?", ct, ".height|0:", "(", Qe, ".", Zg, "-", bn, ")");
                                     return G.optional(function() {
                                         Mn.assert(un, Un + ">=0&&" + Wi + ">=0", "invalid " + Z)
                                     }), [vn, bn, Un, Wi]
                                 });
                             return q && (Vn.thisDep = Vn.thisDep || q.thisDep, Vn.contextDep = Vn.contextDep || q.contextDep, Vn.propDep = Vn.propDep || q.propDep), Vn
-                        } else return q ? new ws(q.thisDep, q.contextDep, q.propDep, function(Mn, un) {
+                        } else return q ? new Cs(q.thisDep, q.contextDep, q.propDep, function(Mn, un) {
                             var ct = Mn.shared.context;
                             return [0, 0, un.def(ct, ".", $g), un.def(ct, ".", Zg)]
                         }) : null
                     }
                     var me = pe(Yc);
                     if (me) {
                         var Ee = me;
-                        me = new ws(me.thisDep, me.contextDep, me.propDep, function(Z, se) {
+                        me = new Cs(me.thisDep, me.contextDep, me.propDep, function(Z, se) {
                             var Q = Ee.append(Z, se),
                                 xe = Z.shared.context;
                             return se.set(xe, "." + Une, Q[2]), se.set(xe, "." + Hne, Q[3]), Q
                         })
                     }
                     return {
                         viewport: me,
@@ -25156,15 +25156,15 @@
                     }
                     var me = pe(q1),
                         Ee = pe(V1),
                         Z = null,
                         se;
                     return fd(me) && fd(Ee) ? (Z = Dt.program(Ee.id, me.id, null, he), se = as(function(Q, xe) {
                         return Q.link(Z)
-                    })) : se = new ws(me && me.thisDep || Ee && Ee.thisDep, me && me.contextDep || Ee && Ee.contextDep, me && me.propDep || Ee && Ee.propDep, function(Q, xe) {
+                    })) : se = new Cs(me && me.thisDep || Ee && Ee.thisDep, me && me.contextDep || Ee && Ee.contextDep, me && me.propDep || Ee && Ee.propDep, function(Q, xe) {
                         var Re = Q.shared.shader,
                             et;
                         me ? et = me.append(Q, xe) : et = xe.def(Re, ".", q1);
                         var lt;
                         Ee ? lt = Ee.append(Q, xe) : lt = xe.def(Re, ".", V1);
                         var jt = Re + ".program(" + lt + "," + et;
                         return G.optional(function() {
@@ -25230,15 +25230,15 @@
                                     Hu = Un.def("null"),
                                     dd = Un.def(Ks, "(", Kc, ")"),
                                     Xh = bn.cond(dd).then(Hu, "=", Wh, ".createStream(", Kc, ");").else(Hu, "=", Wh, ".getElements(", Kc, ");");
                                 return G.optional(function() {
                                     bn.assert(Xh.else, "!" + Kc + "||" + Hu, "invalid elements")
                                 }), Un.entry(Xh), Un.exit(bn.cond(dd).then(Wh, ".destroyStream(", Hu, ");")), bn.ELEMENTS = Hu, Hu
                             })
-                        } else if (pe) return new ws(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
+                        } else if (pe) return new Cs(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
                             return Un.def(bn.shared.vao + ".currentVAO?" + bn.shared.elements + ".getElements(" + bn.shared.vao + ".currentVAO.elements):null")
                         });
                         return null
                     }
                     var Q = se();
 
                     function xe() {
@@ -25257,19 +25257,19 @@
                                 }), vn.def(bn, "[", Un, "]")
                             })
                         } else {
                             if (Z) return fd(Q) ? Q.value ? as(function(Qe, vn) {
                                 return vn.def(Qe.ELEMENTS, ".primType")
                             }) : as(function() {
                                 return w3
-                            }) : new ws(Q.thisDep, Q.contextDep, Q.propDep, function(Qe, vn) {
+                            }) : new Cs(Q.thisDep, Q.contextDep, Q.propDep, function(Qe, vn) {
                                 var bn = Qe.ELEMENTS;
                                 return vn.def(bn, "?", bn, ".primType:", w3)
                             });
-                            if (pe) return new ws(Ee.thisDep, Ee.contextDep, Ee.propDep, function(Qe, vn) {
+                            if (pe) return new Cs(Ee.thisDep, Ee.contextDep, Ee.propDep, function(Qe, vn) {
                                 return vn.def(Qe.shared.vao + ".currentVAO?" + Qe.shared.vao + ".currentVAO.primitive:" + w3)
                             })
                         }
                         return null
                     }
 
                     function Re(un, ct) {
@@ -25286,18 +25286,18 @@
                                     bn.assert(Un, Wi + ">=0", "invalid " + un)
                                 })), Wi
                             })
                         } else if (ct) {
                             if (Z) return as(function(bn, Un) {
                                 return bn.OFFSET = 0, 0
                             });
-                            if (pe) return new ws(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
+                            if (pe) return new Cs(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
                                 return Un.def(bn.shared.vao + ".currentVAO?" + bn.shared.vao + ".currentVAO.offset:0")
                             })
-                        } else if (pe) return new ws(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
+                        } else if (pe) return new Cs(Ee.thisDep, Ee.contextDep, Ee.propDep, function(bn, Un) {
                             return Un.def(bn.shared.vao + ".currentVAO?" + bn.shared.vao + ".currentVAO.instances:-1")
                         });
                         return null
                     }
                     var et = Re($y, !0);
 
                     function lt() {
@@ -25312,39 +25312,39 @@
                                 var Ks = Un.invoke(Wi, ct);
                                 return G.optional(function() {
                                     Un.assert(Wi, "typeof " + Ks + '==="number"&&' + Ks + ">=0&&" + Ks + "===(" + Ks + "|0)", "invalid vertex count")
                                 }), Ks
                             })
                         } else if (Z)
                             if (fd(Q)) {
-                                if (Q) return et ? new ws(et.thisDep, et.contextDep, et.propDep, function(Un, Wi) {
+                                if (Q) return et ? new Cs(et.thisDep, et.contextDep, et.propDep, function(Un, Wi) {
                                     var Ks = Wi.def(Un.ELEMENTS, ".vertCount-", Un.OFFSET);
                                     return G.optional(function() {
                                         Un.assert(Wi, Ks + ">=0", "invalid vertex offset/element buffer too small")
                                     }), Ks
                                 }) : as(function(Un, Wi) {
                                     return Wi.def(Un.ELEMENTS, ".vertCount")
                                 });
                                 var Qe = as(function() {
                                     return -1
                                 });
                                 return G.optional(function() {
                                     Qe.MISSING = !0
                                 }), Qe
                             } else {
-                                var vn = new ws(Q.thisDep || et.thisDep, Q.contextDep || et.contextDep, Q.propDep || et.propDep, function(Un, Wi) {
+                                var vn = new Cs(Q.thisDep || et.thisDep, Q.contextDep || et.contextDep, Q.propDep || et.propDep, function(Un, Wi) {
                                     var Ks = Un.ELEMENTS;
                                     return Un.OFFSET ? Wi.def(Ks, "?", Ks, ".vertCount-", Un.OFFSET, ":-1") : Wi.def(Ks, "?", Ks, ".vertCount:-1")
                                 });
                                 return G.optional(function() {
                                     vn.DYNAMIC = !0
                                 }), vn
                             }
                         else if (pe) {
-                            var bn = new ws(Ee.thisDep, Ee.contextDep, Ee.propDep, function(Un, Wi) {
+                            var bn = new Cs(Ee.thisDep, Ee.contextDep, Ee.propDep, function(Un, Wi) {
                                 return Wi.def(Un.shared.vao, ".currentVAO?", Un.shared.vao, ".currentVAO.count:-1")
                             });
                             return bn
                         }
                         return null
                     }
                     var jt = xe(),
@@ -25778,15 +25778,15 @@
                                 return Vn = Vn && !!Qe, Qe
                             });
                         if (Vn && Mn.length > 0) {
                             var un = Lt.getVAO(Lt.createVAO({
                                 attributes: Mn,
                                 elements: Q.static.elements
                             }));
-                            jt.drawVAO = new ws(null, null, null, function(ct, Qe) {
+                            jt.drawVAO = new Cs(null, null, null, function(ct, Qe) {
                                 return ct.link(un)
                             }), jt.useVAO = !0
                         }
                     }
                     return Ee ? jt.useVAO = !0 : jt.attributes = _s(q, Te), jt.context = Cr(Ae), jt
                 }
 
@@ -47362,15 +47362,15 @@
     }));
     var si = 1e-6,
         XS = 1e-12,
         Bi = Math.PI,
         ds = Bi / 2,
         YS = Bi / 4,
         aa = Bi * 2,
-        Ss = 180 / Bi,
+        As = 180 / Bi,
         Ni = Bi / 180,
         Ki = Math.abs,
         Q0 = Math.atan,
         jl = Math.atan2,
         oi = Math.cos,
         H2 = Math.ceil,
         E$ = Math.exp,
@@ -47552,17 +47552,17 @@
         if (zp) {
             var i = m0(zp, n),
                 r = [i[1], -i[0], 0],
                 s = m0(r, i);
             eA(s), s = JS(s);
             var o = e - hm,
                 a = o > 0 ? 1 : -1,
-                l = s[0] * Ss * a,
+                l = s[0] * As * a,
                 u, c = Ki(o) > 180;
-            c ^ (a * hm < l && l < a * e) ? (u = s[1] * Ss, u > nl && (nl = u)) : (l = (l + 360) % 360 - 180, c ^ (a * hm < l && l < a * e) ? (u = -s[1] * Ss, u < ya && (ya = u)) : (t < ya && (ya = t), t > nl && (nl = t))), c ? e < hm ? el(is, e) > el(is, us) && (us = e) : el(e, us) > el(is, us) && (is = e) : us >= is ? (e < is && (is = e), e > us && (us = e)) : e > hm ? el(is, e) > el(is, us) && (us = e) : el(e, us) > el(is, us) && (is = e)
+            c ^ (a * hm < l && l < a * e) ? (u = s[1] * As, u > nl && (nl = u)) : (l = (l + 360) % 360 - 180, c ^ (a * hm < l && l < a * e) ? (u = -s[1] * As, u < ya && (ya = u)) : (t < ya && (ya = t), t > nl && (nl = t))), c ? e < hm ? el(is, e) > el(is, us) && (us = e) : el(e, us) > el(is, us) && (is = e) : us >= is ? (e < is && (is = e), e > us && (us = e)) : e > hm ? el(is, e) > el(is, us) && (us = e) : el(e, us) > el(is, us) && (is = e)
         } else Td.push(Nf = [is = e, us = e]);
         t < ya && (ya = t), t > nl && (nl = t), zp = n, hm = e
     }
 
     function $9() {
         af.point = I$
     }
@@ -47691,15 +47691,15 @@
 
     function wAe(e) {
         U_ = tA = nA = iA = rA = sA = oA = aA = 0, $k = new sa, Zk = new sa, Qk = new sa, df(e, gu);
         var t = +$k,
             n = +Zk,
             i = +Qk,
             r = Vk(t, n, i);
-        return r < XS && (t = sA, n = oA, i = aA, tA < si && (t = nA, n = iA, i = rA), r = Vk(t, n, i), r < XS) ? [NaN, NaN] : [jl(n, t) * Ss, xa(i / r) * Ss]
+        return r < XS && (t = sA, n = oA, i = aA, tA < si && (t = nA, n = iA, i = rA), r = Vk(t, n, i), r < XS) ? [NaN, NaN] : [jl(n, t) * As, xa(i / r) * As]
     }
 
     function Jk(e, t) {
         function n(i, r) {
             return i = e(i, r), t(i[0], i[1])
         }
         return e.invert && t.invert && (n.invert = function(i, r) {
@@ -47751,18 +47751,18 @@
         }, o
     }
 
     function CAe(e) {
         e = D$(e[0] * Ni, e[1] * Ni, e.length > 2 ? e[2] * Ni : 0);
 
         function t(n) {
-            return n = e(n[0] * Ni, n[1] * Ni), n[0] *= Ss, n[1] *= Ss, n
+            return n = e(n[0] * Ni, n[1] * Ni), n[0] *= As, n[1] *= As, n
         }
         return t.invert = function(n) {
-            return n = e.invert(n[0] * Ni, n[1] * Ni), n[0] *= Ss, n[1] *= Ss, n
+            return n = e.invert(n[0] * Ni, n[1] * Ni), n[0] *= As, n[1] *= As, n
         }, t
     }
 
     function TAe(e, t, n, i, r, s) {
         if (!!n) {
             var o = oi(t),
                 a = ti(t),
@@ -48827,39 +48827,39 @@
             A, y, w, D, T;
 
         function C(j) {
             return w(j[0] * Ni, j[1] * Ni)
         }
 
         function k(j) {
-            return j = w.invert(j[0], j[1]), j && [j[0] * Ss, j[1] * Ss]
+            return j = w.invert(j[0], j[1]), j && [j[0] * As, j[1] * As]
         }
         C.stream = function(j) {
             return D && T === j ? D : D = ZAe(QAe(c)(g(A(S(T = j)))))
         }, C.preclip = function(j) {
             return arguments.length ? (g = j, m = void 0, N()) : g
         }, C.postclip = function(j) {
             return arguments.length ? (S = j, p = _ = b = v = null, N()) : S
         }, C.clipAngle = function(j) {
-            return arguments.length ? (g = +j ? DAe(m = j * Ni) : (m = null, oB), N()) : m * Ss
+            return arguments.length ? (g = +j ? DAe(m = j * Ni) : (m = null, oB), N()) : m * As
         }, C.clipExtent = function(j) {
             return arguments.length ? (S = j == null ? (p = _ = b = v = null, xb) : P$(p = +j[0][0], _ = +j[0][1], b = +j[1][0], v = +j[1][1]), N()) : p == null ? null : [
                 [p, _],
                 [b, v]
             ]
         }, C.scale = function(j) {
             return arguments.length ? (n = +j, I()) : n
         }, C.translate = function(j) {
             return arguments.length ? (i = +j[0], r = +j[1], I()) : [i, r]
         }, C.center = function(j) {
-            return arguments.length ? (s = j[0] % 360 * Ni, o = j[1] % 360 * Ni, I()) : [s * Ss, o * Ss]
+            return arguments.length ? (s = j[0] % 360 * Ni, o = j[1] % 360 * Ni, I()) : [s * As, o * As]
         }, C.rotate = function(j) {
-            return arguments.length ? (a = j[0] % 360 * Ni, l = j[1] % 360 * Ni, u = j.length > 2 ? j[2] % 360 * Ni : 0, I()) : [a * Ss, l * Ss, u * Ss]
+            return arguments.length ? (a = j[0] % 360 * Ni, l = j[1] % 360 * Ni, u = j.length > 2 ? j[2] % 360 * Ni : 0, I()) : [a * As, l * As, u * As]
         }, C.angle = function(j) {
-            return arguments.length ? (f = j % 360 * Ni, I()) : f * Ss
+            return arguments.length ? (f = j % 360 * Ni, I()) : f * As
         }, C.reflectX = function(j) {
             return arguments.length ? (d = j ? -1 : 1, I()) : d < 0
         }, C.reflectY = function(j) {
             return arguments.length ? (h = j ? -1 : 1, I()) : h < 0
         }, C.precision = function(j) {
             return arguments.length ? (A = vB(y, E = j * j), N()) : la(E)
         }, C.fitExtent = function(j, z) {
@@ -48888,15 +48888,15 @@
 
     function L6(e) {
         var t = 0,
             n = Bi / 3,
             i = $$(e),
             r = i(t, n);
         return r.parallels = function(s) {
-            return arguments.length ? i(t = s[0] * Ni, n = s[1] * Ni) : [t * Ss, n * Ss]
+            return arguments.length ? i(t = s[0] * Ni, n = s[1] * Ni) : [t * As, n * As]
         }, r
     }
 
     function ewe(e) {
         var t = oi(e);
 
         function n(i, r) {
@@ -49243,15 +49243,15 @@
                 [c, f]
             ]
         }, v.scale = function(S) {
             return arguments.length ? (e = +S, b()) : e
         }, v.translate = function(S) {
             return arguments.length ? (t = +S[0], n = +S[1], b()) : [t, n]
         }, v.angle = function(S) {
-            return arguments.length ? (s = S % 360 * Ni, a = ti(s), o = oi(s), b()) : s * Ss
+            return arguments.length ? (s = S % 360 * Ni, a = ti(s), o = oi(s), b()) : s * As
         }, v.reflectX = function(S) {
             return arguments.length ? (i = S ? -1 : 1, b()) : i < 0
         }, v.reflectY = function(S) {
             return arguments.length ? (r = S ? -1 : 1, b()) : r < 0
         }, v.fitExtent = function(S, E) {
             return Qw(v, S, E)
         }, v.fitSize = function(S, E) {
@@ -85683,15 +85683,15 @@
                 n && F(t)
             }
         }
     }
 
     function WHe(e) {
         let t, n, i;
-        return n = new As({
+        return n = new ws({
             props: {
                 style: "width: 60px",
                 value: e[0].join,
                 resetOnBlur: !1,
                 placeholder: "",
                 valueField: "label",
                 labelField: "label",
@@ -85718,15 +85718,15 @@
                 r && F(t), ie(n)
             }
         }
     }
 
     function XHe(e) {
         let t, n;
-        return t = new As({
+        return t = new ws({
             props: {
                 options: e[5]
             }
         }), {
             c() {
                 re(t.$$.fragment)
             },
@@ -85777,15 +85777,15 @@
                 o[t].d(l), l && F(i)
             }
         }
     }
 
     function KHe(e) {
         let t, n;
-        return t = new As({
+        return t = new ws({
             props: {
                 value: e[0].operation,
                 placeholder: "Operation",
                 valueField: "label",
                 searchable: !1,
                 options: e[5]
             }
@@ -85810,15 +85810,15 @@
                 ie(t, i)
             }
         }
     }
 
     function $He(e) {
         let t, n;
-        return t = new As({
+        return t = new ws({
             props: {
                 value: e[0].operation,
                 placeholder: "Operation",
                 valueField: "label",
                 searchable: !1,
                 options: ["match", "match (regex)"]
             }
@@ -85843,15 +85843,15 @@
                 ie(t, i)
             }
         }
     }
 
     function ZHe(e) {
         let t, n;
-        return t = new As({
+        return t = new ws({
             props: {
                 value: e[0].operation,
                 placeholder: "Operation",
                 valueField: "label",
                 searchable: !1,
                 options: ["==", "!="]
             }
@@ -85876,15 +85876,15 @@
                 ie(t, i)
             }
         }
     }
 
     function QHe(e) {
         let t, n;
-        return t = new As({}), {
+        return t = new ws({}), {
             c() {
                 re(t.$$.fragment)
             },
             m(i, r) {
                 ne(t, i, r), n = !0
             },
             p: ue,
@@ -85966,15 +85966,15 @@
                 id: !0,
                 name: "true"
             }, {
                 id: !1,
                 name: "false"
             }]
         };
-        return e[0].value !== void 0 && (s.value = e[0].value), t = new As({
+        return e[0].value !== void 0 && (s.value = e[0].value), t = new ws({
             props: s
         }), _t.push(() => Yi(t, "value", r)), {
             c() {
                 re(t.$$.fragment)
             },
             m(o, a) {
                 ne(t, o, a), i = !0
@@ -86064,15 +86064,15 @@
             e[8](j)
         }
         let w = {
             placeholder: "Column",
             valueAsObject: !0,
             options: e[3].completeColumns.filter(e[7])
         };
-        e[0].column !== void 0 && (w.value = e[0].column), o = new As({
+        e[0].column !== void 0 && (w.value = e[0].column), o = new ws({
             props: w
         }), _t.push(() => Yi(o, "value", y));
         const D = [YHe, XHe],
             T = [];
 
         function C(j, z) {
             return j[0].column ? 0 : 1
@@ -86189,15 +86189,15 @@
     function eG(e, t, n) {
         const i = e.slice();
         return i[11] = t[n], i[12] = t, i[13] = n, i
     }
 
     function tG(e) {
         let t, n;
-        return t = new As({
+        return t = new ws({
             props: {
                 placeholder: "",
                 style: "width: 60px",
                 value: e[0].join,
                 valueField: "label",
                 labelField: "label",
                 options: ["&", "|"]
@@ -91992,15 +91992,15 @@
         constructor(t) {
             super(), kt(this, t, oWe, Jqe, At, {})
         }
     }
 
     function lWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[0],
                 options: e[4],
                 searchable: !1
             }
         }), r.$on("change", e[5]), {
@@ -92051,15 +92051,15 @@
         constructor(t) {
             super(), kt(this, t, uWe, lWe, At, {})
         }
     }
 
     function fWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[4],
                 options: e[3],
                 multiple: !0,
                 placeholder: "Select Slices..."
             }
@@ -92104,15 +92104,15 @@
         constructor(t) {
             super(), kt(this, t, dWe, fWe, At, {})
         }
     }
 
     function mWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[4],
                 options: e[3],
                 multiple: !0,
                 placeholder: "Select Slices..."
             }
@@ -92157,15 +92157,15 @@
         constructor(t) {
             super(), kt(this, t, gWe, mWe, At, {})
         }
     }
 
     function _We(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[1][e[0]].metrics[0],
                 options: e[2],
                 searchable: !1
             }
         }), r.$on("change", e[3]), {
@@ -92215,15 +92215,15 @@
         constructor(t) {
             super(), kt(this, t, bWe, _We, At, {})
         }
     }
 
     function yWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[3],
                 options: e[2],
                 multiple: !0,
                 placeholder: "Select Metrics..."
             }
@@ -92268,15 +92268,15 @@
         constructor(t) {
             super(), kt(this, t, EWe, yWe, At, {})
         }
     }
 
     function AWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[1][e[0]].models[0],
                 options: e[2],
                 searchable: !1
             }
         }), r.$on("change", e[3]), {
@@ -92326,15 +92326,15 @@
         constructor(t) {
             super(), kt(this, t, wWe, AWe, At, {})
         }
     }
 
     function CWe(e) {
         let t, n, i, r, s;
-        return r = new As({
+        return r = new ws({
             props: {
                 style: "width: 280px; flex:none;",
                 value: e[3],
                 options: e[2],
                 multiple: !0,
                 placeholder: "Select Models..."
             }
@@ -92576,15 +92576,15 @@
                 ie(t, i)
             }
         }
     }
 
     function HG(e) {
         let t, n, i, r, s, o, a, l;
-        return s = new As({
+        return s = new ws({
             props: {
                 style: "width: 280px; height: 30px; flex:none;",
                 value: "models",
                 options: [{
                     label: "models"
                 }],
                 searchable: !1
@@ -92634,29 +92634,29 @@
     }
 
     function DWe(e) {
         let t, n, i, r, s, o, a, l = e[4][e[1]].x + "",
             u, c, f, d, h, m, g, p, _, b, v = e[4][e[1]].y + "",
             S, E, A, y, w, D, T, C, k, I, N, j, z = e[4][e[1]].z + "",
             W, V, U, J, ge, fe, De;
-        f = new As({
+        f = new ws({
             props: {
                 style: "width: 280px; height: 30px; flex:none",
                 value: e[0].xEncoding,
                 options: e[5][e[1]].x,
                 searchable: !1
             }
         }), f.$on("change", e[10]);
         let Y = e[1] === Hn.BEESWARM && zG();
         var ve = e[2] === "x" ? e[3][e[0].xEncoding].fixed : e[3][e[0].xEncoding].multi;
 
         function gt(ae) {
             return {}
         }
-        ve && (m = Fi(ve, gt())), A = new As({
+        ve && (m = Fi(ve, gt())), A = new ws({
             props: {
                 style: "width: 280px; height: 30px; flex:none",
                 value: e[0].yEncoding,
                 options: e[5][e[1]].y,
                 searchable: !1
             }
         }), A.$on("change", e[11]);
@@ -92665,15 +92665,15 @@
             _e = [];
 
         function qe(ae, je) {
             return ae[1] === Hn.HEATMAP && ae[0].yEncoding === "slices" ? 0 : 1
         }
         D = qe(e), T = _e[D] = Ye[D](e);
         let we = e[1] === Hn.HEATMAP && e[0].xEncoding === e[0].yEncoding && HG();
-        U = new As({
+        U = new ws({
             props: {
                 style: "width: 280px; height: 30px; flex:none;",
                 value: e[0].zEncoding,
                 options: e[5][e[1]].z,
                 searchable: !1
             }
         }), U.$on("change", e[12]);
@@ -93033,24 +93033,24 @@
                 a && F(t), ie(n), ie(s)
             }
         }
     }
 
     function zWe(e, t, n) {
         let i;
-        Je(e, fs, s => n(1, i = s));
+        Je(e, fs, s => n(2, i = s));
         const r = {
             "/": BI,
             "/predict/": TGe,
             "/explore/": BI,
             "/report/": XGe,
             "/report/:id": BWe,
             "*": BI
         };
-        return ll.subscribe(s => {
+        return ys.BASE = location.protocol + "//" + location.host + location.pathname + "api", ll.subscribe(s => {
             let o = {};
             s.completeColumns.filter(a => !i.metadata[fr(a)]).forEach(a => {
                 o[fr(a)] = {
                     predicates: [],
                     join: ""
                 }
             }), fs.update(a => ({
```

### Comparing `zenoml-0.4.7/zeno/frontend/build/assets/main.6757dad9.css` & `zenoml-0.4.8/zeno/frontend/build/assets/main.6757dad9.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/build/favicon.png` & `zenoml-0.4.8/zeno/frontend/build/favicon.png`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/build/global.css` & `zenoml-0.4.8/zeno/frontend/build/global.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/build/smui.css` & `zenoml-0.4.8/zeno/frontend/build/smui.css`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/build/zeno.png` & `zenoml-0.4.8/zeno/frontend/build/zeno.png`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/frontend/index.html` & `zenoml-0.4.8/zeno/frontend/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -16,9 +16,9 @@
       href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,600,700"
     >
     
     <link       rel="stylesheet"
       href="https://fonts.googleapis.com/css?family=Roboto+Mono"
     >
   <link rel="stylesheet" href="./build/assets/main.6757dad9.css"></head>
-  <body><div id="app"></div><script type="module" src="./build/assets/main.5a7a7111.js"></script></body>
+  <body><div id="app"></div><script type="module" src="./build/assets/main.f60e39ea.js"></script></body>
 </html>
```

### Comparing `zenoml-0.4.7/zeno/frontend/index_og.html` & `zenoml-0.4.8/zeno/frontend/index_og.html`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/processing/data_processing.py` & `zenoml-0.4.8/zeno/processing/data_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/processing/filtering.py` & `zenoml-0.4.8/zeno/processing/filtering.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/processing/histogram_processing.py` & `zenoml-0.4.8/zeno/processing/histogram_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/processing/projection_processing.py` & `zenoml-0.4.8/zeno/processing/projection_processing.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/runner.py` & `zenoml-0.4.8/zeno/runner.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/server.py` & `zenoml-0.4.8/zeno/server.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/setup.py` & `zenoml-0.4.8/zeno/setup.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/zeno/util.py` & `zenoml-0.4.8/zeno/util.py`

 * *Files identical despite different names*

### Comparing `zenoml-0.4.7/setup.py` & `zenoml-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'websockets>=10.2,<12.0']
 
 entry_points = \
 {'console_scripts': ['zeno = zeno.runner:command_line']}
 
 setup_kwargs = {
     'name': 'zenoml',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'Interactive Evaluation Framework for Machine Learning',
     'long_description': '<img src="https://zenoml.com/img/zeno.png" width="250px"/>\n\n[![PyPI version](https://badge.fury.io/py/zenoml.svg)](https://badge.fury.io/py/zenoml)\n![Github Actions CI tests](https://github.com/zeno-ml/zeno/actions/workflows/test.yml/badge.svg)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/) \n[![DOI](https://img.shields.io/badge/doi-10.1145%2F3544548.3581268-red)](https://cabreraalex.com/paper/zeno)\n[![Discord](https://img.shields.io/discord/1086004954872950834)](https://discord.gg/km62pDKAkE)\n\nZeno is a general-purpose framework for evaluating machine learning models.\nIt combines a **Python API** with an **interactive UI** to allow users to discover, explore, and analyze the performance of their models across diverse use cases.\nZeno can be used for any data type or task with [modular views](https://zenoml.com/docs/views/) for everything from object detection to audio transcription.\n\n\n### Demos\n\n\n| **Image Classification**  | **Audio Transcription** | **Image Generation** | **Dataset Chatbot** | **Sensor Classification**\n|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|\n| Imagenette  | Speech Accent Archive | DiffusionDB | LangChain + Notion | MotionSense\n|[![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imagenette.hf.space/)| [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-audio-transcription.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-diffusiondb.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-langchain-qa.hf.space/) | [![Try with Zeno](https://zenoml.com/img/zeno-badge.svg)](https://zeno-ml-imu-classification.hf.space)\n| [code](https://huggingface.co/spaces/zeno-ml/imagenette/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/diffusiondb/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/audio-transcription/tree/main) | [code](https://huggingface.co/spaces/zeno-ml/imu-classification/tree/main) |\n\n<br /> \n\nhttps://user-images.githubusercontent.com/4563691/220689691-1ad7c184-02db-4615-b5ac-f52b8d5b8ea3.mp4\n\n## Quickstart\n\nInstall the Zeno Python package from PyPI:\n\n```bash\npip install zenoml\n```\n\n### Command Line\n\nTo get started, run the following command to initialize a Zeno project. It will walk you through creating the `zeno.toml` configuration file:\n\n```bash\nzeno init\n```\n\nTake a look at the [configuration documentation](https://zenoml.com/docs/configuration) for additional `toml` file options like adding model functions.\n\nStart Zeno with `zeno zeno.toml`.\n\n### Jupyter Notebook\n\nYou can also run Zeno directly from Jupyter notebooks or lab. The `zeno` command takes a dictionary of configuration options as input. See [the docs](https://zenoml.com/docs/configuration) for a full list of options. In this example we pass the minimum options for exploring a non-tabular dataset:\n\n```python\nimport pandas as pd\nfrom zeno import zeno\n\ndf = pd.read_csv("/path/to/metadata/file.csv")\n\nzeno({\n    "metadata": df, # Pandas DataFrame with a row for each instance\n    "view": "audio-transcription", # The type of view for this data/task\n    "data_path": "/path/to/raw/data/", # The folder with raw data (images, audio, etc.)\n    "data_column": "id" # The column in the metadata file that contains the relative paths of files in data_path\n})\n\n```\n\nYou can pass a list of decorated function references directly Zeno as you add models and metrics.\n\n## Citation\n\nPlease reference our [CHI\'23 paper](https://arxiv.org/pdf/2302.04732.pdf)\n\n```bibtex\n@inproceedings{cabrera23zeno,\n  author = {Cabrera, Ángel Alexander and Fu, Erica and Bertucci, Donald and Holstein, Kenneth and Talwalkar, Ameet and Hong, Jason I. and Perer, Adam},\n  title = {Zeno: An Interactive Framework for Behavioral Evaluation of Machine Learning},\n  year = {2023},\n  isbn = {978-1-4503-9421-5/23/04},\n  publisher = {Association for Computing Machinery},\n  address = {New York, NY, USA},\n  url = {https://doi.org/10.1145/3544548.3581268},\n  doi = {10.1145/3544548.3581268},\n  booktitle = {CHI Conference on Human Factors in Computing Systems},\n  location = {Hamburg, Germany},\n  series = {CHI \'23}\n}\n```\n\n## Community\n\nChat with us on our [Discord channel](https://discord.gg/km62pDKAkE) or leave an issue on this repository if you run into any issues or have a request!\n',
     'author': 'Ángel Alexander Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://zenoml.com',
```

### Comparing `zenoml-0.4.7/PKG-INFO` & `zenoml-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenoml
-Version: 0.4.7
+Version: 0.4.8
 Summary: Interactive Evaluation Framework for Machine Learning
 Home-page: https://zenoml.com
 License: MIT
 Keywords: ml,testing,evaluation,machine learning,ai
 Author: Ángel Alexander Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.8.1,<=3.11
```

