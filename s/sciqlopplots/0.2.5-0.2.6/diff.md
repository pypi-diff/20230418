# Comparing `tmp/sciqlopplots-0.2.5.tar.gz` & `tmp/sciqlopplots-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlopplots-0.2.5.tar", last modified: Tue Apr 18 08:05:31 2023, max compression
+gzip compressed data, was "sciqlopplots-0.2.6.tar", last modified: Tue Apr 18 15:47:29 2023, max compression
```

## Comparing `sciqlopplots-0.2.5.tar` & `sciqlopplots-0.2.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/.clang-format
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/.gitignore
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/COPYING
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/README.md
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/__init__.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/_QCustomPlot.hpp
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/bindings.h
--rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/bindings.xml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
--rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/src_list.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/bindings/snippets.cpp
--rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/SciQLopPlots/meson.build
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopColorMap.hpp
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopGraph.hpp
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopPlot.hpp
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopPlotItem.hpp
--rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopVerticalSpan.hpp
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/constants.hpp
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/include/SciQLopPlots/numpy_wrappers.hpp
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/meson.build
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/meson_options.txt
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/pyproject.toml
--rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/qcustomplot-source/GPL.txt
--rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/qcustomplot-source/changelog.txt
--rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/qcustomplot-source/qcustomplot.cpp
--rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/qcustomplot-source/qcustomplot.h
--rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/setup.cfg
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/SciQLopColorMap.cpp
--rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/SciQLopGraph.cpp
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/SciQLopPlot.cpp
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/SciQLopPlotItem.cpp
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/SciQLopVerticalSpan.cpp
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/src/numpy_wrappers.cpp
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/subprojects/cpp_utils.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/subprojects/hedley.wrap
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/QCP_Examples/plots/main.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/SciQLopColorMap/main.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/SciQLopGraph/main.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/SciQLopVerticalSpan/main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/StackedGraphs/main.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/manual-tests/meson.build
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/tests/meson.build
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.clang-format
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-linux.yml
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-osx.yml
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.github/workflows/pythonpublish-win.yml
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/COPYING
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/README.md
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/__init__.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/_QCustomPlot.hpp
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.h
+-rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.xml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
+-rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/src_list.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/bindings/snippets.cpp
+-rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/SciQLopPlots/meson.build
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopColorMap.hpp
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopGraph.hpp
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlot.hpp
+-rw-r--r--   0        0        0     2362 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlotItem.hpp
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopVerticalSpan.hpp
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/constants.hpp
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/include/SciQLopPlots/numpy_wrappers.hpp
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/meson_options.txt
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/pyproject.toml
+-rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/GPL.txt
+-rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/changelog.txt
+-rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.cpp
+-rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.h
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/setup.cfg
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopColorMap.cpp
+-rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopGraph.cpp
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopPlot.cpp
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopPlotItem.cpp
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/SciQLopVerticalSpan.cpp
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/src/numpy_wrappers.cpp
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/subprojects/cpp_utils.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/subprojects/hedley.wrap
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/QCP_Examples/plots/main.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopColorMap/main.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopGraph/main.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/SciQLopVerticalSpan/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/StackedGraphs/main.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/manual-tests/meson.build
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/tests/meson.build
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.6/PKG-INFO
```

### Comparing `sciqlopplots-0.2.5/.clang-format` & `sciqlopplots-0.2.6/.clang-format`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/.github/workflows/pythonpublish-linux.yml` & `sciqlopplots-0.2.6/.github/workflows/pythonpublish-linux.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/.github/workflows/pythonpublish-osx.yml` & `sciqlopplots-0.2.6/.github/workflows/pythonpublish-osx.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/.github/workflows/pythonpublish-win.yml` & `sciqlopplots-0.2.6/.github/workflows/pythonpublish-win.yml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/COPYING` & `sciqlopplots-0.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/_QCustomPlot.hpp` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/_QCustomPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/bindings.xml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/rpath-helper.py` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/rpath-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/helper_scripts/src_list.py` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/helper_scripts/src_list.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/bindings/snippets.cpp` & `sciqlopplots-0.2.6/SciQLopPlots/bindings/snippets.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/SciQLopPlots/meson.build` & `sciqlopplots-0.2.6/SciQLopPlots/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopColorMap.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopColorMap.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopGraph.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopGraph.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopPlot.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopPlotItem.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopPlotItem.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     bool _movable = false;
     QPointF _last_position;
 
 public:
     SciQLopPlotItem(QCustomPlot* plot): QCPAbstractItem_T{plot}{ }
     virtual ~SciQLopPlotItem() { }
     inline bool movable() const noexcept { return this->_movable; }
-    inline void setMovable(bool movable) noexcept { this->_movable = movable; }
+    inline virtual void setMovable(bool movable) noexcept { this->_movable = movable; }
 
     virtual void move(double dx, double dy) = 0;
     inline void replot() { this->layer()->replot(); }
 
     inline void mousePressEvent(QMouseEvent* event, const QVariant& details) override
     {
         this->_last_position = event->pos();
```

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/SciQLopVerticalSpan.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/SciQLopVerticalSpan.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,21 @@
                 emit this->range_changed(this->range());
             });
 
         this->set_left_pos(std::min(horizontal_range.lower, horizontal_range.upper));
         this->set_right_pos(std::max(horizontal_range.lower, horizontal_range.upper));
     }
 
+    inline virtual void setMovable(bool movable) noexcept override
+    {
+        SciQLopPlotItem::setMovable(movable);
+        this->_border1->setMovable(movable);
+        this->_border2->setMovable(movable);
+    }
+
     ~VerticalSpan()
     {
         this->parentPlot()->removeItem(this->_border1);
         this->parentPlot()->removeItem(this->_border2);
     }
 
     inline void set_range(const QCPRange horizontal_range)
@@ -269,8 +276,10 @@
     {
         this->_impl->set_range(horizontal_range);
     }
 
     inline void set_color(const QColor& color) { this->_impl->set_color(color); }
 
     inline void set_selected(bool selected) { this->_impl->setSelected(selected); }
+
+    inline void set_read_only(bool read_only) { this->_impl->setMovable(!read_only); }
 };
```

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/constants.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/constants.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/include/SciQLopPlots/numpy_wrappers.hpp` & `sciqlopplots-0.2.6/include/SciQLopPlots/numpy_wrappers.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/meson.build` & `sciqlopplots-0.2.6/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.5')
+project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.6')
 add_project_arguments(
             '-DCATCH_CONFIG_NO_POSIX_SIGNALS', # workaround for this https://github.com/catchorg/Catch2/issues/2192
             language: 'cpp',
             native: true
 )
 qt_sdk='qt6'
```

### Comparing `sciqlopplots-0.2.5/pyproject.toml` & `sciqlopplots-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/qcustomplot-source/GPL.txt` & `sciqlopplots-0.2.6/qcustomplot-source/GPL.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/qcustomplot-source/changelog.txt` & `sciqlopplots-0.2.6/qcustomplot-source/changelog.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/qcustomplot-source/qcustomplot.cpp` & `sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/qcustomplot-source/qcustomplot.h` & `sciqlopplots-0.2.6/qcustomplot-source/qcustomplot.h`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/SciQLopColorMap.cpp` & `sciqlopplots-0.2.6/src/SciQLopColorMap.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/SciQLopGraph.cpp` & `sciqlopplots-0.2.6/src/SciQLopGraph.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/SciQLopPlot.cpp` & `sciqlopplots-0.2.6/src/SciQLopPlot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/SciQLopPlotItem.cpp` & `sciqlopplots-0.2.6/src/SciQLopPlotItem.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/SciQLopVerticalSpan.cpp` & `sciqlopplots-0.2.6/src/SciQLopVerticalSpan.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/src/numpy_wrappers.cpp` & `sciqlopplots-0.2.6/src/numpy_wrappers.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/QCP_Examples/plots/main.py` & `sciqlopplots-0.2.6/tests/manual-tests/QCP_Examples/plots/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/SciQLopColorMap/main.py` & `sciqlopplots-0.2.6/tests/manual-tests/SciQLopColorMap/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/SciQLopGraph/main.py` & `sciqlopplots-0.2.6/tests/manual-tests/SciQLopGraph/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/SciQLopVerticalSpan/main.py` & `sciqlopplots-0.2.6/tests/manual-tests/SciQLopVerticalSpan/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/StackedGraphs/main.py` & `sciqlopplots-0.2.6/tests/manual-tests/StackedGraphs/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/tests/manual-tests/meson.build` & `sciqlopplots-0.2.6/tests/manual-tests/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.5/PKG-INFO` & `sciqlopplots-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.2.5
+Version: 0.2.6
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
```

