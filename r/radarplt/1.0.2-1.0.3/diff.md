# Comparing `tmp/radarplt-1.0.2.tar.gz` & `tmp/radarplt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radarplt-1.0.2.tar", max compression
+gzip compressed data, was "radarplt-1.0.3.tar", max compression
```

## Comparing `radarplt-1.0.2.tar` & `radarplt-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-10 20:29:07.994168 radarplt-1.0.2/LICENSE
--rw-r--r--   0        0        0     4717 2023-02-10 20:28:50.078055 radarplt-1.0.2/README.md
--rw-r--r--   0        0        0      504 2023-02-10 20:42:04.622620 radarplt-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10074 2023-02-10 19:47:46.478652 radarplt-1.0.2/radarplt/__init__.py
--rw-r--r--   0        0        0     3782 2023-02-10 19:15:10.801166 radarplt-1.0.2/radarplt/factory.py
--rw-r--r--   0        0        0      327 2023-02-10 19:15:10.765166 radarplt-1.0.2/radarplt/helpers.py
--rw-r--r--   0        0        0     5570 1970-01-01 00:00:00.000000 radarplt-1.0.2/setup.py
--rw-r--r--   0        0        0     5261 1970-01-01 00:00:00.000000 radarplt-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-18 18:40:56.926019 radarplt-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4749 2023-04-18 18:40:56.926223 radarplt-1.0.3/README.md
+-rw-r--r--   0        0        0      504 2023-04-18 18:40:56.936745 radarplt-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10094 2023-04-18 18:40:56.936981 radarplt-1.0.3/radarplt/__init__.py
+-rw-r--r--   0        0        0     3782 2023-04-18 18:40:56.937136 radarplt-1.0.3/radarplt/factory.py
+-rw-r--r--   0        0        0      327 2023-04-18 18:40:56.937259 radarplt-1.0.3/radarplt/helpers.py
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 radarplt-1.0.3/PKG-INFO
```

### Comparing `radarplt-1.0.2/LICENSE` & `radarplt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radarplt-1.0.2/README.md` & `radarplt-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 fig, ax = radarplt.plot(
     df,
     label_column="property",
     value_column="value",
     hue_column="item",
     value_ranges=value_ranges,
     plot_labels=plot_labels,
+    target_ranges=target_ranges
 )
 legend = ax.legend(loc=(0.9, 0.95))
 plt.tight_layout()
 plt.show()
 ```
 
 Resulting in the following image
```

### Comparing `radarplt-1.0.2/radarplt/__init__.py` & `radarplt-1.0.3/radarplt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,20 +230,20 @@
         # plot ranges for values
         for i in range(len(self.ordered_labels)):
             offset = 0
             theta = label_angles[i] * np.pi / 180 + offset
 
             r = 0.25
             lower, upper = self.value_ranges[self.ordered_labels[i]]
-            text = round(r * upper + lower, 2)
+            text = round(r * (upper - lower) + lower, 2)
             plt.text(theta, r, text, fontsize=8)
 
             r = 0.75
             lower, upper = self.value_ranges[self.ordered_labels[i]]
-            text = round(r * upper + lower, 2)
+            text = round(r * (upper - lower) + lower, 2)
             plt.text(theta, r, text, fontsize=8)
 
 
 def plot(
     df: pd.DataFrame,
     label_column: str,
     value_column: str,
```

### Comparing `radarplt-1.0.2/radarplt/factory.py` & `radarplt-1.0.3/radarplt/factory.py`

 * *Files identical despite different names*

### Comparing `radarplt-1.0.2/setup.py` & `radarplt-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,197 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: radarplt
+Version: 1.0.3
+Summary: 
+Home-page: https://github.com/jdkern11/radar_plot.git
+Author: jdkern11
+Author-email: josephdanielkern@gmail.com
+Requires-Python: >=3.9,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
+Requires-Dist: pandas (>=1.4.4,<2.0.0)
+Project-URL: Repository, https://github.com/jdkern11/radar_plot.git
+Description-Content-Type: text/markdown
+
+# Radar plot
+This package creates radar plots. It can generate typical radar plots and 
+plot ranges of values.
+
+- [Data formatting](#data-formatting)
+- [Basic usage](#basic-usage)
+- [Chaning ranges](#changing-ranges)
+- [Chaning labels](#changing-labels)
+- [Plotting target ranges](#plotting-target-ranges)
+
+![example 0](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_0.png)
+
+## Data formatting
+Data you want to plot must have a tidy format. For instance, if I wanted to plot
+three properties (let's say prop1, prop2, and prop3 with values 
+12, 3.5, and 42 respectively) then you should load a csv file into a pandas 
+dataframe that has the following format:
+
+| property | value | item  |
+| -------- | ----- | ----- |
+| prop1    | 12.0  | item1 |
+| prop2    | 3.5   | item1 |
+| prop3    | 42    | item1 |
+
+If you wanted to plot several items (e.g., item1, item2, and item3)
+with different values for the properties, then format the data like this:
+
+| property | value | item  |
+| -------- | ----- | ----- |
+| prop1    | 12.0  | item1 |
+| prop2    | 3.5   | item1 |
+| prop3    | 42    | item1 |
+| prop1    | 14.0  | item2 |
+| prop2    | 4.0   | item2 |
+| prop3    | 36    | item2 |
+| prop1    | 15    | item3 |
+| prop2    | 2     | item3 |
+| prop3    | 40    | item3 |
+
+## Basic Usage
+Following [that formatting scheme](#data-formatting), you can plot the data as follows
+```Python
+import pandas as pd
+import matplotlib.pyplot as plt
+import radarplt
+
+# see tables above
+df = pd.read_csv('example_data.csv')
+fig, ax = radarplt.plot(
+    df,
+    label_column="property",
+    value_column="value",
+    hue_column="item",
+)
+legend = ax.legend(loc=(0.9, 0.95))
+plt.tight_layout()
+plt.show()
+```
+Resulting in the following image
+![example 1 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_1.png)
+
+Additional lines are plotted at the .25, .50, and .75 marks on the image. The value at the
+.25 and .75 line for each property is labeled and values increase/decrease linearly
+between these points. For instance, the 0.5 mark for property 2 would be 4, the 1 
+mark would be 6 and the 0 mark would be 2.
+
+### Changing Ranges 
+Let's say you don't like that the prop2 ranges from 1 to 6. To change
+these value ranges create a dictionary of the ranges you want for each property and 
+pass it to the function via the `value_ranges` parameter.
+For instance: 
+```Python
+import pandas as pd
+import matplotlib.pyplot as plt
+import radarplt
+
+value_ranges = {
+  "prop1": [0, 20],
+  "prop2": [0, 5],
+  "prop3": [0, 50],
+}
+
+# see tables above
+df = pd.read_csv('example_data.csv')
+fig, ax = radarplt.plot(
+    df,
+    label_column="property",
+    value_column="value",
+    hue_column="item",
+    value_ranges=value_ranges,
+)
+legend = ax.legend(loc=(0.9, 0.95))
+plt.tight_layout()
+plt.show()
+```
+Resulting in the following image
+![example 2 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_2.png)
+
+### Changing labels
+If you don't want the labels for the properties to be the property names, 
+you can change those as well with the `plot_labels` parameter.
+
+```Python
+import pandas as pd
+import matplotlib.pyplot as plt
+import radarplt
+
+value_ranges = {
+  "prop1": [0, 20],
+  "prop2": [0, 5],
+  "prop3": [0, 50],
+}
+
+plot_labels = {
+  "prop1": "$\sigma^{2}$",
+  "prop2": "Property 2 (seconds)",
+  "prop3": "p3"
+}
 
-packages = \
-['radarplt']
+# see tables above
+df = pd.read_csv('example_data.csv')
+fig, ax = radarplt.plot(
+    df,
+    label_column="property",
+    value_column="value",
+    hue_column="item",
+    value_ranges=value_ranges,
+    plot_labels=plot_labels,
+)
+legend = ax.legend(loc=(0.9, 0.95))
+plt.tight_layout()
+plt.show()
+```
+Resulting in the following image
+![example 3 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_3.png)
+
+### Plotting target ranges
+If you want to see if your items' values fall within a certain range, you 
+can add those ranges as well
+```Python
+import pandas as pd
+import matplotlib.pyplot as plt
+import radarplt
+
+target_ranges = {
+  "prop1": [10, 20],
+  "prop2": [0, 2],
+  "prop3": [25, 35]
+}
 
-package_data = \
-{'': ['*']}
+value_ranges = {
+  "prop1": [0, 20],
+  "prop2": [0, 5],
+  "prop3": [0, 50],
+}
 
-install_requires = \
-['matplotlib>=3.6.3,<4.0.0', 'pandas>=1.4.4,<2.0.0']
-
-setup_kwargs = {
-    'name': 'radarplt',
-    'version': '1.0.2',
-    'description': '',
-    'long_description': '# Radar plot\nThis package creates radar plots. It can generate typical radar plots and \nplot ranges of values.\n\n- [Data formatting](#data-formatting)\n- [Basic usage](#basic-usage)\n- [Chaning ranges](#changing-ranges)\n- [Chaning labels](#changing-labels)\n- [Plotting target ranges](#plotting-target-ranges)\n\n![example 0](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_0.png)\n\n## Data formatting\nData you want to plot must have a tidy format. For instance, if I wanted to plot\nthree properties (let\'s say prop1, prop2, and prop3 with values \n12, 3.5, and 42 respectively) then you should load a csv file into a pandas \ndataframe that has the following format:\n\n| property | value | item  |\n| -------- | ----- | ----- |\n| prop1    | 12.0  | item1 |\n| prop2    | 3.5   | item1 |\n| prop3    | 42    | item1 |\n\nIf you wanted to plot several items (e.g., item1, item2, and item3)\nwith different values for the properties, then format the data like this:\n\n| property | value | item  |\n| -------- | ----- | ----- |\n| prop1    | 12.0  | item1 |\n| prop2    | 3.5   | item1 |\n| prop3    | 42    | item1 |\n| prop1    | 14.0  | item2 |\n| prop2    | 4.0   | item2 |\n| prop3    | 36    | item2 |\n| prop1    | 15    | item3 |\n| prop2    | 2     | item3 |\n| prop3    | 40    | item3 |\n\n## Basic Usage\nFollowing [that formatting scheme](#data-formatting), you can plot the data as follows\n```Python\nimport pandas as pd\nimport matplotlib.pyplot as plt\nimport radarplt\n\n# see tables above\ndf = pd.read_csv(\'example_data.csv\')\nfig, ax = radarplt.plot(\n    df,\n    label_column="property",\n    value_column="value",\n    hue_column="item",\n)\nlegend = ax.legend(loc=(0.9, 0.95))\nplt.tight_layout()\nplt.show()\n```\nResulting in the following image\n![example 1 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_1.png)\n\nAdditional lines are plotted at the .25, .50, and .75 marks on the image. The value at the\n.25 and .75 line for each property is labeled and values increase/decrease linearly\nbetween these points. For instance, the 0.5 mark for property 2 would be 4, the 1 \nmark would be 6 and the 0 mark would be 2.\n\n### Changing Ranges \nLet\'s say you don\'t like that the prop2 ranges from 1 to 6. To change\nthese value ranges create a dictionary of the ranges you want for each property and \npass it to the function via the `value_ranges` parameter.\nFor instance: \n```Python\nimport pandas as pd\nimport matplotlib.pyplot as plt\nimport radarplt\n\nvalue_ranges = {\n  "prop1": [0, 20],\n  "prop2": [0, 5],\n  "prop3": [0, 50],\n}\n\n# see tables above\ndf = pd.read_csv(\'example_data.csv\')\nfig, ax = radarplt.plot(\n    df,\n    label_column="property",\n    value_column="value",\n    hue_column="item",\n    value_ranges=value_ranges,\n)\nlegend = ax.legend(loc=(0.9, 0.95))\nplt.tight_layout()\nplt.show()\n```\nResulting in the following image\n![example 2 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_2.png)\n\n### Changing labels\nIf you don\'t want the labels for the properties to be the property names, \nyou can change those as well with the `plot_labels` parameter.\n\n```Python\nimport pandas as pd\nimport matplotlib.pyplot as plt\nimport radarplt\n\nvalue_ranges = {\n  "prop1": [0, 20],\n  "prop2": [0, 5],\n  "prop3": [0, 50],\n}\n\nplot_labels = {\n  "prop1": "$\\sigma^{2}$",\n  "prop2": "Property 2 (seconds)",\n  "prop3": "p3"\n}\n\n# see tables above\ndf = pd.read_csv(\'example_data.csv\')\nfig, ax = radarplt.plot(\n    df,\n    label_column="property",\n    value_column="value",\n    hue_column="item",\n    value_ranges=value_ranges,\n    plot_labels=plot_labels,\n)\nlegend = ax.legend(loc=(0.9, 0.95))\nplt.tight_layout()\nplt.show()\n```\nResulting in the following image\n![example 3 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_3.png)\n\n### Plotting target ranges\nIf you want to see if your items\' values fall within a certain range, you \ncan add those ranges as well\n```Python\nimport pandas as pd\nimport matplotlib.pyplot as plt\nimport radarplt\n\ntarget_ranges = {\n  "prop1": [10, 20],\n  "prop2": [0, 2],\n  "prop3": [25, 35]\n}\n\nvalue_ranges = {\n  "prop1": [0, 20],\n  "prop2": [0, 5],\n  "prop3": [0, 50],\n}\n\nplot_labels = {\n  "prop1": "$\\sigma^{2}$",\n  "prop2": "Property 2 (seconds)",\n  "prop3": "p3"\n}\n\n# see tables above\ndf = pd.read_csv(\'example_data.csv\')\nfig, ax = radarplt.plot(\n    df,\n    label_column="property",\n    value_column="value",\n    hue_column="item",\n    value_ranges=value_ranges,\n    plot_labels=plot_labels,\n)\nlegend = ax.legend(loc=(0.9, 0.95))\nplt.tight_layout()\nplt.show()\n```\n\nResulting in the following image\n![example 4 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_4.png)\n',
-    'author': 'jdkern11',
-    'author_email': 'josephdanielkern@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/jdkern11/radar_plot.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.11',
+plot_labels = {
+  "prop1": "$\sigma^{2}$",
+  "prop2": "Property 2 (seconds)",
+  "prop3": "p3"
 }
 
+# see tables above
+df = pd.read_csv('example_data.csv')
+fig, ax = radarplt.plot(
+    df,
+    label_column="property",
+    value_column="value",
+    hue_column="item",
+    value_ranges=value_ranges,
+    plot_labels=plot_labels,
+    target_ranges=target_ranges
+)
+legend = ax.legend(loc=(0.9, 0.95))
+plt.tight_layout()
+plt.show()
+```
+
+Resulting in the following image
+![example 4 plotted](https://raw.githubusercontent.com/jdkern11/radar_plot/main/images/example_4.png)
 
-setup(**setup_kwargs)
```

