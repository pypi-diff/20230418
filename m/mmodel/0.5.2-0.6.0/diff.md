# Comparing `tmp/mmodel-0.5.2.tar.gz` & `tmp/mmodel-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmodel-0.5.2.tar", max compression
+gzip compressed data, was "mmodel-0.6.0.tar", max compression
```

## Comparing `mmodel-0.5.2.tar` & `mmodel-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1718 2022-08-01 16:13:58.303654 mmodel-0.5.2/LICENSE
--rw-r--r--   0        0        0     5711 2023-03-30 19:59:00.773081 mmodel-0.5.2/README.rst
--rw-r--r--   0        0        0      113 2023-03-15 22:52:47.247592 mmodel-0.5.2/mmodel/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-30 19:23:40.631819 mmodel-0.5.2/mmodel/draw.py
--rw-r--r--   0        0        0     1260 2023-03-30 19:59:00.773890 mmodel-0.5.2/mmodel/filter.py
--rw-r--r--   0        0        0     8348 2023-03-30 19:59:00.774309 mmodel-0.5.2/mmodel/graph.py
--rw-r--r--   0        0        0     6474 2023-03-30 19:59:00.774754 mmodel-0.5.2/mmodel/handler.py
--rw-r--r--   0        0        0     5390 2023-03-30 19:59:00.775071 mmodel-0.5.2/mmodel/metadata.py
--rw-r--r--   0        0        0     5770 2023-03-30 19:59:00.775472 mmodel-0.5.2/mmodel/model.py
--rw-r--r--   0        0        0     4169 2023-03-15 22:52:47.248660 mmodel-0.5.2/mmodel/modifier.py
--rw-r--r--   0        0        0     4526 2023-03-30 19:59:00.775802 mmodel-0.5.2/mmodel/parser.py
--rw-r--r--   0        0        0     9227 2023-03-29 22:29:58.922230 mmodel-0.5.2/mmodel/utility.py
--rw-r--r--   0        0        0     2768 2023-03-30 19:59:00.776114 mmodel-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7313 1970-01-01 00:00:00.000000 mmodel-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1752 2022-06-13 02:17:06.103534 mmodel-0.6.0/LICENSE
+-rw-r--r--   0        0        0       86 2023-04-18 00:38:09.813978 mmodel-0.6.0/mmodel/__init__.py
+-rw-r--r--   0        0        0     2376 2023-03-29 22:27:21.446475 mmodel-0.6.0/mmodel/draw.py
+-rw-r--r--   0        0        0     1304 2023-04-09 00:12:09.150527 mmodel-0.6.0/mmodel/filter.py
+-rw-r--r--   0        0        0     8647 2023-04-18 00:38:09.814981 mmodel-0.6.0/mmodel/graph.py
+-rw-r--r--   0        0        0     6691 2023-04-18 00:38:09.818981 mmodel-0.6.0/mmodel/handler.py
+-rw-r--r--   0        0        0     7320 2023-04-18 00:38:09.819978 mmodel-0.6.0/mmodel/metadata.py
+-rw-r--r--   0        0        0     5961 2023-04-18 00:38:09.820977 mmodel-0.6.0/mmodel/model.py
+-rw-r--r--   0        0        0     6646 2023-04-18 00:38:09.821978 mmodel-0.6.0/mmodel/modifier.py
+-rw-r--r--   0        0        0     6202 2023-04-18 00:38:09.821978 mmodel-0.6.0/mmodel/parser.py
+-rw-r--r--   0        0        0      401 2023-04-18 00:38:09.821978 mmodel-0.6.0/mmodel/shortcut.py
+-rw-r--r--   0        0        0     9538 2023-04-18 00:38:09.828008 mmodel-0.6.0/mmodel/utility.py
+-rw-r--r--   0        0        0     2590 2023-04-18 00:38:09.828977 mmodel-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5887 2023-04-18 00:38:09.805977 mmodel-0.6.0/README.rst
+-rw-r--r--   0        0        0     6863 2023-04-18 00:42:10.481212 mmodel-0.6.0/setup.py
+-rw-r--r--   0        0        0     7227 2023-04-18 00:42:10.481212 mmodel-0.6.0/PKG-INFO
```

### Comparing `mmodel-0.5.2/LICENSE` & `mmodel-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-MModel is distributed with the 3-clause BSD license.::
-
-    Copyright (C) 2022
-    Peter Sun <hs859@cornell.edu>
-    John Marohn <jam99@cornell.edu>
-    All rights reserved.
-
-    Redistribution and use in source and binary forms, with or without
-    modification, are permitted provided that the following conditions are
-    met:
-
-    * Redistributions of source code must retain the above copyright
-        notice, this list of conditions and the following disclaimer.
-
-    * Redistributions in binary form must reproduce the above
-        copyright notice, this list of conditions and the following
-        disclaimer in the documentation and/or other materials provided
-        with the distribution.
-
-    * Neither the name of the NetworkX Developers nor the names of its
-        contributors may be used to endorse or promote products derived
-        from this software without specific prior written permission.
-
-    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-    "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-    LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-    A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-    OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-    SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-    LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-    DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-    THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+MModel is distributed with the 3-clause BSD license.::
+
+    Copyright (C) 2022
+    Peter Sun <hs859@cornell.edu>
+    John Marohn <jam99@cornell.edu>
+    All rights reserved.
+
+    Redistribution and use in source and binary forms, with or without
+    modification, are permitted provided that the following conditions are
+    met:
+
+    * Redistributions of source code must retain the above copyright
+        notice, this list of conditions and the following disclaimer.
+
+    * Redistributions in binary form must reproduce the above
+        copyright notice, this list of conditions and the following
+        disclaimer in the documentation and/or other materials provided
+        with the distribution.
+
+    * Neither the name of the NetworkX Developers nor the names of its
+        contributors may be used to endorse or promote products derived
+        from this software without specific prior written permission.
+
+    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+    "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+    LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+    A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+    OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+    SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+    LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+    DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+    THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mmodel-0.5.2/README.rst` & `mmodel-0.6.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-MModel
-======
-
-|GitHub version| |PyPI version shields.io| |PyPI pyversions| |Unittests|
-|Docs|
-
-MModel is a lightweight and modular model-building framework
-for small-scale and nonlinear models. The package aims to solve
-scientific program prototyping and distribution difficulties, making
-it easier to create modular, fast, and user-friendly packages.
-
-Quickstart
-----------
-
-To create a nonlinear model that has the result of
-`(x + y)log(x + y, base)`:
-
-.. code-block:: python
-
-    from mmodel import ModelGraph, Model, MemHandler
-    import math
-    import numpy as np
-
-    def func(sum_xy, log_xy):
-        """Function that adds a value to the multiplied inputs."""
-        return sum_xy * log_xy + 6
-
-The graph is defined using grouped edges (the ``networkx`` syntax of edge
-the definition also works.)
-
-.. code-block:: python
-
-    # create graph edges
-    grouped_edges = [
-        ("add", ["log", "function node"]),
-        ("log", "function node"),
-    ]
-
-The functions are then added to node attributes. The order of definition
-is node_name, node_func, output, input (if different from original function),
-and modifiers.
-
-.. code-block:: python
-
-    # define note objects
-    node_objects = [
-        ("add", np.add, "sum_xy", ["x", "y"]),
-        ("log", math.log, "log_xy", ["sum_xy", "log_base"]),
-        ("function node", func, "result"),
-    ]
-
-    G = ModelGraph(name="example_graph")
-    G.add_grouped_edges_from(grouped_edges)
-    G.set_node_objects_from(node_objects)
-
-To define the model, the name, graph, and handler need to be specified. Additional
-parameters include modifiers, descriptions, and returns lists. The input parameters
-of the model are determined based on the node information.
-
-.. code-block:: python
-
-    example_model = Model("example_model", G, handler=(MemHandler, {}), description="Test model.")
-
-The model behaves like a Python function, with additional metadata. The graph can
-be plotted using the ``draw`` method.
-
-.. code-block:: python
-
-    >>> print(example_model)
-    example_model(log_base, x, y)
-    returns: z
-    graph: example_graph
-    handler: MemHandler()
-
-    Test model.
-
-    >>> example_model(2, 5, 3) # (5 + 3)log(5 + 3, 2) + 6
-    30.0
-
-    >>> example_model.draw()
-
-The resulting graph contains the model metadata and detailed node information.
-
-.. .. |br| raw:: html
-    
-..     <br/>
-
-.. .. image:: example.png
-..   :width: 300
-..   :alt: example model graph
-
-One key feature of ``mmodel`` that differs from other workflow is modifiers, 
-which modify callables post definition. Modifiers work on both the node level
-and model level.
-
-Example: Use ``loop_modifier`` on the graph to loop the nodes that require the
-"log_base" parameter.
-
-.. code-block:: python 
-
-    from mmodel import loop_modifier
-
-    H = G.subgraph(inputs=["log_base"])
-    H.name = "example_subgraph"
-    loop_node = Model("submodel", H, handler=(MemHandler, {}))
-
-    looped_G = G.replace_subgraph(
-        H,
-        "loop_node",
-        loop_node,
-        output="looped_z",
-        modifiers=[(loop_modifier, {"parameter": "log_base"})],
-    )
-    looped_G.name = "looped_graph"
-
-    looped_model = Model("looped_model", looped_G, loop_node.handler)
-
-
-We can inspect the loop node as well as the new model.
-
-.. code-block:: python 
-
-    >>> print(loop_node)
-    loop_submodel(log_base, sum_xy)
-    returns: z
-    graph: example_subgraph
-    handler: MemHandler()
-    modifiers:
-      - loop_modifier('log_base')
-
-    >>> print(looped_model)
-    looped_model(log_base, x, y)
-    returns: looped_z
-    graph: looped_graph
-    handler: MemHandler()
-    
-    >>> looped_model([2, 4], 5, 3) # (5 + 3)log(5 + 3, 2) + 6
-    [30.0, 18.0]
-
-
-Use the ``draw`` method to draw the graph. There are three styles
-"plain", "short", and "verbose", which differ by the level of detail of the
-node information. A graph output is displayed in Jupyter Notebook
-or can be saved using the export option.
-
-.. code-block:: python
-
-    G.draw(style="short")
-    example_model.draw(style="plain", export="example.pdf") # default to draw_graph
-
-Installation
-------------
-
-Graphviz installation
-^^^^^^^^^^^^^^^^^^^^^
-
-To view the graph, Graphviz needs to be installed:
-`Graphviz Installation <https://graphviz.org/download/>`_
-For windows installation, please choose "add Graphviz to the
-system PATH for all users/current users" during the setup.
-
-MModel installation
-^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block::
-
-    pip install mmodel
-
-Development installation
-^^^^^^^^^^^^^^^^^^^^^^^^
-MModel uses `poetry <https://python-poetry.org/docs/>`_ as
-the build system. The package works with both pip and poetry
-installation. For macos systems, sometimes `brew install` results
-in unexpected installation path, it is recommended to install
-with conda::
-
-    conda install -c conda-forge pygraphviz
-
-To install test and docs, despondencies run::
-
-    pip install .[test] .[docs]
-
-To run the tests in different python environments and cases 
-(py38, py39, py310, py311, coverage and docs)::
-
-    tox
-
-To create the documentation, run under the "/docs" directory::
-
-    make html
-
-
-.. |GitHub version| image:: https://badge.fury.io/gh/peterhs73%2FMModel.svg
-   :target: https://github.com/Marohn-Group/mmodel
-
-.. |PyPI version shields.io| image:: https://img.shields.io/pypi/v/mmodel.svg
-   :target: https://pypi.python.org/pypi/mmodel/
-
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/mmodel.svg
-
-.. |Unittests| image:: https://github.com/Marohn-Group/mmodel/actions/workflows/tox.yml/badge.svg
-    :target: https://github.com/Marohn-Group/mmodel/actions
-
-.. |Docs| image:: https://img.shields.io/badge/Documentation--brightgreen.svg
-    :target: https://github.com/Marohn-Group/mmodel-docs/
+MModel
+======
+
+|GitHub version| |PyPI version shields.io| |PyPI pyversions| |Unittests|
+|Docs|
+
+MModel is a lightweight and modular model-building framework
+for small-scale and nonlinear models. The package aims to solve
+scientific program prototyping and distribution difficulties, making
+it easier to create modular, fast, and user-friendly packages.
+
+Quickstart
+----------
+
+To create a nonlinear model that has the result of
+`(x + y)log(x + y, base)`:
+
+.. code-block:: python
+
+    import math
+    import numpy as np
+
+    def func(sum_xy, log_xy):
+        """Function that adds a value to the multiplied inputs."""
+
+        return sum_xy * log_xy + 6
+
+The graph is defined using grouped edges (the ``networkx`` syntax of edge
+the definition also works.)
+
+.. code-block:: python
+
+    from mmodel import ModelGraph, Model, MemHandler
+    # create graph edges
+    grouped_edges = [
+        ("add", ["log", "function node"]),
+        ("log", "function node"),
+    ]
+
+The functions are then added to node attributes. The order of definition
+is node_name, node_func, output, input (if different from original function),
+and modifiers.
+
+.. code-block:: python
+
+    # define note objects
+    node_objects = [
+        ("add", np.add, "sum_xy", ["x", "y"]),
+        ("log", math.log, "log_xy", ["sum_xy", "log_base"]),
+        ("function node", func, "result"),
+    ]
+
+    G = ModelGraph(name="example_graph")
+    G.add_grouped_edges_from(grouped_edges)
+    G.set_node_objects_from(node_objects)
+
+To define the model, the name, graph, and handler need to be specified. Additional
+parameters include modifiers, descriptions, and returns lists. The input parameters
+of the model are determined based on the node information.
+
+.. code-block:: python
+
+    example_model = Model("example_model", G, handler=MemHandler, description="Test model.")
+
+The model behaves like a Python function, with additional metadata. The graph can
+be plotted using the ``draw`` method.
+
+.. code-block:: python
+
+    >>> print(example_model)
+    example_model(log_base, x, y)
+    returns: z
+    graph: example_graph
+    handler: MemHandler
+
+    Test model.
+
+    >>> example_model(2, 5, 3) # (5 + 3)log(5 + 3, 2) + 6
+    30.0
+
+    >>> example_model.draw()
+
+The resulting graph contains the model metadata and detailed node information.
+
+.. .. |br| raw:: html
+    
+..     <br/>
+
+.. .. image:: example.png
+..   :width: 300
+..   :alt: example model graph
+
+One key feature of ``mmodel`` that differs from other workflow is modifiers, 
+which modify callables post definition. Modifiers work on both the node level
+and model level.
+
+Example: Use ``loop_input`` modifier on the graph to loop the nodes that require the
+"log_base" parameter.
+
+.. code-block:: python 
+
+    from mmodel import loop_input
+
+    H = G.subgraph(inputs=["log_base"])
+    H.name = "example_subgraph"
+    loop_node = Model("submodel", H, handler=MemHandler)
+
+    looped_G = G.replace_subgraph(
+        H,
+        "loop_node",
+        loop_node,
+        output="looped_z",
+        modifiers=[loop_input("log_base")],
+    )
+    looped_G.name = "looped_graph"
+
+    looped_model = Model("looped_model", looped_G, loop_node.handler)
+
+
+We can inspect the loop node as well as the new model.
+
+.. code-block:: python 
+
+    >>> print(looped_model)
+    looped_model(log_base, x, y)
+    returns: looped_z
+    graph: looped_graph
+    handler: MemHandler()
+    
+    >>> print(looped_model.node_metadata("loop_node"))
+    submodel(log_base, sum_xy)
+    return: looped_z
+    functype: mmodel.Model
+    modifiers:
+      - loop_input('log_base')
+
+    >>> looped_model([2, 4], 5, 3) # (5 + 3)log(5 + 3, 2) + 6
+    [30.0, 18.0]
+
+
+Use the ``draw`` method to draw the graph. There are three styles
+"plain", "short", and "verbose", which differ by the level of detail of the
+node information. A graph output is displayed in Jupyter Notebook
+or can be saved using the export option.
+
+.. code-block:: python
+
+    G.draw(style="short")
+    example_model.draw(style="plain", export="example.pdf") # default to draw_graph
+
+Installation
+------------
+
+Graphviz installation
+^^^^^^^^^^^^^^^^^^^^^
+
+To view the graph, Graphviz needs to be installed:
+`Graphviz Installation <https://graphviz.org/download/>`_
+For windows installation, please choose "add Graphviz to the
+system PATH for all users/current users" during the setup.
+
+MModel installation
+^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block::
+
+    pip install mmodel
+
+Development installation
+^^^^^^^^^^^^^^^^^^^^^^^^
+MModel uses `poetry <https://python-poetry.org/docs/>`_ as
+the build system. The package works with both pip and poetry
+installation. For macos systems, sometimes `brew install` results
+in unexpected installation path, it is recommended to install
+with conda::
+
+    conda install -c conda-forge pygraphviz
+
+To install test and docs, despondencies run::
+
+    pip install .[test] .[docs]
+
+To run the tests in different python environments and cases 
+(py38, py39, py310, py311, coverage and docs)::
+
+    tox
+
+To create the documentation, run under the "/docs" directory::
+
+    make html
+
+
+.. |GitHub version| image:: https://badge.fury.io/gh/peterhs73%2FMModel.svg
+   :target: https://github.com/Marohn-Group/mmodel
+
+.. |PyPI version shields.io| image:: https://img.shields.io/pypi/v/mmodel.svg
+   :target: https://pypi.python.org/pypi/mmodel/
+
+.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/mmodel.svg
+
+.. |Unittests| image:: https://github.com/Marohn-Group/mmodel/actions/workflows/tox.yml/badge.svg
+    :target: https://github.com/Marohn-Group/mmodel/actions
+
+.. |Docs| image:: https://img.shields.io/badge/Documentation--brightgreen.svg
+    :target: https://github.com/Marohn-Group/mmodel-docs/
```

### Comparing `mmodel-0.5.2/mmodel/draw.py` & `mmodel-0.6.0/mmodel/draw.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import graphviz
-from copy import deepcopy
-from mmodel.metadata import textwrap50, nodeformatter
-
-DEFAULT_SETTINGS = {
-    "graph_attr": {
-        "labelloc": "t",
-        "labeljust": "l",
-        "splines": "ortho",
-        "ordering": "out",
-    },
-    "node_attr": {"shape": "box"},
-}
-
-
-def draw_graph(
-    G, label, style, export=None, formatter=nodeformatter, textwrapper=textwrap50
-):
-    """Draw a detailed graph with options.
-
-    :param str name: name of the graph
-    :param str label: title of the graph
-    :param str style: there are three valid styles, plain
-        short and verbose. Each style corresponds to node-only,
-        function-only, and detailed note metadata graph
-    :param str export: filename to export to
-    """
-
-    label = label.replace("\n", "\l") + "\l"
-    settings = deepcopy(DEFAULT_SETTINGS)
-    settings["graph_attr"].update({"label": label})
-
-    dot_graph = graphviz.Digraph(name=G.name, **settings)
-
-    if style == "plain":
-        for node in G.nodes:
-            dot_graph.node(node)
-
-        for u, v in G.edges:
-            dot_graph.edge(u, v)
-
-    else:
-        if style == "short":
-            for node, ndict in G.nodes(data=True):
-                if "func" in ndict:
-                    metadata = G.node_metadata(node, False, formatter, textwrapper)
-                    nlabel = metadata.replace("\n", "\l") + "\l"
-                else:
-                    nlabel = node
-
-                dot_graph.node(node, label=nlabel)
-
-        elif style == "verbose":
-            for node, ndict in G.nodes(data=True):
-                if "func" in ndict:
-                    metadata = G.node_metadata(node, True, formatter, textwrapper)
-                    nlabel = metadata.replace("\n", "\l") + "\l"
-                else:
-                    nlabel = node
-
-                dot_graph.node(node, label=nlabel)
-
-        else:
-            raise Exception(
-                f"Invalid style {repr(style)}: must be one of plain, short, or verbose."
-            )
-
-        for u, v, edict in G.edges(data=True):
-
-            if "var" in edict:
-                xlabel = edict["var"]
-            else:
-                xlabel = ""
-
-            dot_graph.edge(u, v, xlabel=xlabel)
-
-    if export:
-        dot_graph.render(outfile=export)
-
-    return dot_graph
+import graphviz
+from copy import deepcopy
+from mmodel.metadata import textwrap50, nodeformatter
+
+DEFAULT_SETTINGS = {
+    "graph_attr": {
+        "labelloc": "t",
+        "labeljust": "l",
+        "splines": "ortho",
+        "ordering": "out",
+    },
+    "node_attr": {"shape": "box"},
+}
+
+
+def draw_graph(
+    G, label, style, export=None, formatter=nodeformatter, textwrapper=textwrap50
+):
+    """Draw a detailed graph with options.
+
+    :param str name: name of the graph
+    :param str label: title of the graph
+    :param str style: there are three valid styles, plain
+        short and verbose. Each style corresponds to node-only,
+        function-only, and detailed note metadata graph
+    :param str export: filename to export to
+    """
+
+    label = label.replace("\n", "\l") + "\l"
+    settings = deepcopy(DEFAULT_SETTINGS)
+    settings["graph_attr"].update({"label": label})
+
+    dot_graph = graphviz.Digraph(name=G.name, **settings)
+
+    if style == "plain":
+        for node in G.nodes:
+            dot_graph.node(node)
+
+        for u, v in G.edges:
+            dot_graph.edge(u, v)
+
+    else:
+        if style == "short":
+            for node, ndict in G.nodes(data=True):
+                if "func" in ndict:
+                    metadata = G.node_metadata(node, False, formatter, textwrapper)
+                    nlabel = metadata.replace("\n", "\l") + "\l"
+                else:
+                    nlabel = node
+
+                dot_graph.node(node, label=nlabel)
+
+        elif style == "verbose":
+            for node, ndict in G.nodes(data=True):
+                if "func" in ndict:
+                    metadata = G.node_metadata(node, True, formatter, textwrapper)
+                    nlabel = metadata.replace("\n", "\l") + "\l"
+                else:
+                    nlabel = node
+
+                dot_graph.node(node, label=nlabel)
+
+        else:
+            raise Exception(
+                f"Invalid style {repr(style)}: must be one of plain, short, or verbose."
+            )
+
+        for u, v, edict in G.edges(data=True):
+
+            if "var" in edict:
+                xlabel = edict["var"]
+            else:
+                xlabel = ""
+
+            dot_graph.edge(u, v, xlabel=xlabel)
+
+    if export:
+        dot_graph.render(outfile=export)
+
+    return dot_graph
```

### Comparing `mmodel-0.5.2/mmodel/graph.py` & `mmodel-0.6.0/mmodel/graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,246 +1,248 @@
-import networkx as nx
-from mmodel.draw import draw_graph
-from copy import deepcopy
-from mmodel.filter import subnodes_by_inputs, subnodes_by_outputs
-from mmodel.utility import (
-    modelgraph_signature,
-    modelgraph_returns,
-    replace_subgraph,
-    modify_node,
-)
-from mmodel.metadata import nodeformatter, format_metadata, textwrap80
-from mmodel.parser import node_parser
-
-
-class ModelGraph(nx.DiGraph):
-
-    """Create model graphs.
-
-    ModelGraph inherits from `networkx.DiGraph()`, which has all `DiGraph`
-    methods.
-
-    The class adds the "type" attribute to the graph attribute. The factory method
-    returns a copy of the dictionary. It is equivalent to
-    ``{"type": "ModelGraph"}.copy()`` when called.
-
-    The additional graph operations are added:
-    - add_grouped_edges and set_node_objects.
-    - Method ``add_grouped_edges``, cannot have both edges list.
-    - Method ``set_node_object`` updates nodes with the node callable "func" and output.
-    - The method adds callable signature 'sig' to the node attribute.
-    """
-
-    # Add the default parser to the graph attribute dictionary.
-    # To change the parser, subclass ModelGraph and change the attribute.
-    graph_attr_dict_factory = {"type": "ModelGraph", "parser": node_parser}.copy
-
-    def set_node_object(
-        self,
-        node: str,
-        func: callable,
-        output: str = None,
-        inputs: list = None,
-        modifiers: list = None,
-    ):
-        """Add or update the functions of an existing node.
-
-        In the end, the edge attributes are re-determined
-        Modifiers are applied directly onto the node. The parser checks the
-        function type and returns (at least) three dictionary entries:
-        _func, functype, doc.
-        """
-
-        node_dict = self.nodes[node]
-        parser = self.graph["parser"]
-
-        modifiers = modifiers or list()
-        attr_dict = parser(node, func, output, inputs, modifiers)
-        node_dict.update(attr_dict)
-
-        self.update_graph()
-
-    def set_node_objects_from(self, node_objects: list):
-        """Update the functions of existing nodes.
-
-        The method is the same as adding a node object.
-        """
-
-        for node_obj in node_objects:
-            # unzipping works for input with or without modifiers
-            self.set_node_object(*node_obj)
-
-    def add_edge(self, u_of_edge, v_of_edge, **attr):
-        """Modify add_edge to update the edge attribute in the end."""
-
-        super().add_edge(u_of_edge, v_of_edge, **attr)
-        self.update_graph()
-
-    def add_edges_from(self, ebunch_to_add, **attr):
-        """Modify add_edges_from to update the edge attributes."""
-
-        super().add_edges_from(ebunch_to_add, **attr)
-        self.update_graph()
-
-    def add_grouped_edge(self, u, v):
-        """Add linked edge.
-
-        For mmodel, a group edge (u, v) allows u or v
-        to be a list of nodes. Represents several nodes
-        flowing into one node or the other way around.
-        """
-
-        if isinstance(u, list) and isinstance(v, list):
-            raise Exception("only one edge node can be a list")
-
-        # use add edges from to run less update graph
-        # currently a compromise
-        if isinstance(u, list):
-            self.add_edges_from([(_u, v) for _u in u])
-        elif isinstance(v, list):
-            self.add_edges_from([(u, _v) for _v in v])
-        else:  # neither is a list
-            self.add_edge(u, v)
-
-    def add_grouped_edges_from(self, group_edges: list):
-        """Add edges from grouped values."""
-
-        for u, v in group_edges:
-            self.add_grouped_edge(u, v)
-
-    def update_graph(self):
-        """Update edge attributes based on node objects and edges."""
-
-        for u, v in self.edges:
-            # the edge "var" is not defined if the parent node does not
-            # have "output" attribute or the child node does not have
-            # the parameter
-
-            # extract the parameter dictionary
-            v_sig = getattr(self.nodes[v].get("sig", None), "parameters", {})
-            if "output" in self.nodes[u] and self.nodes[u]["output"] in v_sig:
-                self.edges[u, v]["var"] = self.nodes[u]["output"]
-
-    def _node_metadata_dict(self, node: str, verbose: bool):
-        """Return node metadata as a dictionary."""
-
-        node_dict = self.nodes[node]
-
-        short_dict = {
-            "node": node,
-            "func": node_dict["func"],
-            "return": node_dict["output"],
-        }
-
-        additional_dict = {
-            "functype": node_dict["functype"],
-            "modifiers": node_dict["modifiers"],
-            "doc": node_dict["doc"],
-        }
-        if verbose:
-            return {**short_dict, **additional_dict}
-        else:
-            return short_dict
-
-    def node_metadata(
-        self, node: str, verbose=True, formatter=nodeformatter, textwrapper=textwrap80
-    ):
-        """Printout node metadata.
-
-        The metadata includes the node information and the node function
-        information.
-        """
-        str_list = format_metadata(
-            self._node_metadata_dict(node, verbose), formatter, textwrapper
-        )
-        return "\n".join(str_list).rstrip()
-
-    # graph properties
-    @property
-    def signature(self):
-        """Graph signature.
-
-        :rtype: inspect.Signature object
-        """
-        return modelgraph_signature(self)
-
-    @property
-    def returns(self):
-        """Graph returns.
-
-        :rtype: list
-        """
-        return modelgraph_returns(self)
-
-    # graph operations
-    def subgraph(self, nodes=None, inputs=None, outputs=None):
-        """Extract subgraph by nodes, inputs, and output.
-
-        If multiple parameters are specified, the result is a union
-        of the selection. The subgraph is a deep copy of the original graph.
-        The behavior is different from the parent class method, where the subgraph
-        returns a view of the original graph.
-        """
-
-        nodes = nodes or []
-        node_inputs = subnodes_by_inputs(self, inputs or [])
-        node_outputs = subnodes_by_outputs(self, outputs or [])
-
-        # convert nodes to list because the parent class method accepts generator
-        # for nodes.
-        # may consider not using the same name as the parent class to avoid collision
-        subgraph_nodes = set(list(nodes) + node_inputs + node_outputs)  # unique nodes
-
-        return super().subgraph(subgraph_nodes).deepcopy()
-
-    def replace_subgraph(
-        self, subgraph, name, func, output=None, inputs=None, modifiers=None
-    ):
-        """Replace subgraph with a node."""
-        return replace_subgraph(self, subgraph, name, func, output, inputs, modifiers)
-
-    def modify_node(
-        self, node, func=None, output=None, inputs=None, modifiers=None, inplace=False
-    ):
-        """Modify node attributes."""
-        return modify_node(self, node, func, output, inputs, modifiers, inplace)
-
-    def draw(self, style="verbose", export=None):
-        """Draw the graph.
-
-        Draws the default styled graph.
-
-        :param str style: there are three styles, plain, short, and verbose.
-            Plain shows nodes only, short shows part of the metadata, and
-            long shows all the metadata.
-        :param str export: filename to save the graph as. The file extension
-            is needed.
-        """
-
-        return draw_graph(self, str(self), style, export)
-
-    def deepcopy(self):
-        """Deepcopy graph.
-
-        The graph.copy method is a shallow copy. Deepcopy creates copy for the
-        attributes dictionary.
-        `graph.copy<https://networkx.org/documentation/stable/reference/classes
-        /generated/networkx.Graph.copy.html>_`
-
-        However, for subgraphs, deepcopy is incredibly inefficient because
-        subgraph contains '_graph', which stores the original graph.
-        An alternative method is to copy the code from the copy method,
-        but use deepcopy for the items.
-
-        The parser is redefined in the new graph.
-        """
-
-        G = self.__class__()
-        G.graph.update(deepcopy(self.graph))
-        G.add_nodes_from((n, deepcopy(d)) for n, d in self._node.items())
-        G.add_edges_from(
-            (u, v, deepcopy(datadict))
-            for u, nbrs in self._adj.items()
-            for v, datadict in nbrs.items()
-        )
-
-        return G
+import networkx as nx
+from mmodel.draw import draw_graph
+from copy import deepcopy
+from mmodel.filter import subnodes_by_inputs, subnodes_by_outputs
+from mmodel.utility import (
+    modelgraph_signature,
+    modelgraph_returns,
+    replace_subgraph,
+    modify_node,
+)
+from mmodel.metadata import nodeformatter, format_metadata, textwrap80
+from mmodel.parser import node_parser
+
+
+class ModelGraph(nx.DiGraph):
+
+    """Create model graphs.
+
+    ModelGraph inherits from `networkx.DiGraph()`, which has all `DiGraph`
+    methods.
+
+    The class adds the "type" attribute to the graph attribute. The factory method
+    returns a copy of the dictionary. It is equivalent to
+    ``{"type": "ModelGraph"}.copy()`` when called.
+
+    The additional graph operations are added:
+    - add_grouped_edges and set_node_objects.
+    - Method ``add_grouped_edges``, cannot have both edges list.
+    - Method ``set_node_object`` updates nodes with the node callable "func" and output.
+    - The method adds callable signature 'sig' to the node attribute.
+    """
+
+    # Add the default parser to the graph attribute dictionary.
+    # To change the parser, subclass ModelGraph and change the attribute.
+    graph_attr_dict_factory = {"type": "ModelGraph", "parser": node_parser}.copy
+
+    def set_node_object(
+        self,
+        node: str,
+        func: callable,
+        output: str = None,
+        inputs: list = None,
+        modifiers: list = None,
+        **kwargs,
+    ):
+        """Add or update the functions of an existing node.
+
+        In the end, the edge attributes are re-determined
+        Modifiers are applied directly onto the node. The parser checks the
+        function type and returns (at least) three dictionary entries:
+        _func, functype, doc.
+        """
+
+        node_dict = self.nodes[node]
+        parser = self.graph["parser"]
+
+        modifiers = modifiers or list()
+        attr_dict = parser(node, func, output, inputs, modifiers)
+        node_dict.update(attr_dict)
+        node_dict.update(kwargs)
+
+        self.update_graph()
+
+    def set_node_objects_from(self, node_objects: list):
+        """Update the functions of existing nodes.
+
+        The method is the same as adding a node object.
+        """
+
+        for node_obj in node_objects:
+            # unzipping works for input with or without modifiers
+            self.set_node_object(*node_obj)
+
+    def add_edge(self, u_of_edge, v_of_edge, **attr):
+        """Modify add_edge to update the edge attribute in the end."""
+
+        super().add_edge(u_of_edge, v_of_edge, **attr)
+        self.update_graph()
+
+    def add_edges_from(self, ebunch_to_add, **attr):
+        """Modify add_edges_from to update the edge attributes."""
+
+        super().add_edges_from(ebunch_to_add, **attr)
+        self.update_graph()
+
+    def add_grouped_edge(self, u, v):
+        """Add linked edge.
+
+        For mmodel, a group edge (u, v) allows u or v
+        to be a list of nodes. Represents several nodes
+        flowing into one node or the other way around.
+        """
+
+        if isinstance(u, list) and isinstance(v, list):
+            raise Exception("only one edge node can be a list")
+
+        # use add edges from to run less update graph
+        # currently a compromise
+        if isinstance(u, list):
+            self.add_edges_from([(_u, v) for _u in u])
+        elif isinstance(v, list):
+            self.add_edges_from([(u, _v) for _v in v])
+        else:  # neither is a list
+            self.add_edge(u, v)
+
+    def add_grouped_edges_from(self, group_edges: list):
+        """Add edges from grouped values."""
+
+        for u, v in group_edges:
+            self.add_grouped_edge(u, v)
+
+    def update_graph(self):
+        """Update edge attributes based on node objects and edges."""
+
+        for u, v in self.edges:
+            # the edge "var" is not defined if the parent node does not
+            # have "output" attribute or the child node does not have
+            # the parameter
+
+            # extract the parameter dictionary
+            v_sig = getattr(self.nodes[v].get("sig", None), "parameters", {})
+            if "output" in self.nodes[u] and self.nodes[u]["output"] in v_sig:
+                self.edges[u, v]["var"] = self.nodes[u]["output"]
+
+    def _node_metadata_dict(self, node: str, verbose: bool):
+        """Return node metadata as a dictionary."""
+
+        node_dict = self.nodes[node]
+
+        short_dict = {
+            "node": node,
+            "func": node_dict["func"],
+            "return": node_dict["output"],
+        }
+
+        additional_dict = {
+            "functype": node_dict["functype"],
+            "modifiers": node_dict["modifiers"],
+            "doc": node_dict["doc"],
+        }
+        if verbose:
+            return {**short_dict, **additional_dict}
+        else:
+            return short_dict
+
+    def node_metadata(
+        self, node: str, verbose=True, formatter=nodeformatter, textwrapper=textwrap80
+    ):
+        """Printout node metadata.
+
+        The metadata includes the node information and the node function
+        information.
+        """
+        str_list = format_metadata(
+            self._node_metadata_dict(node, verbose), formatter, textwrapper
+        )
+        return "\n".join(str_list).rstrip()
+
+    # graph properties
+    @property
+    def signature(self):
+        """Graph signature.
+
+        :rtype: inspect.Signature object
+        """
+        return modelgraph_signature(self)
+
+    @property
+    def returns(self):
+        """Graph returns.
+
+        :rtype: list
+        """
+        return modelgraph_returns(self)
+
+    # graph operations
+    def subgraph(self, nodes=None, inputs=None, outputs=None):
+        """Extract subgraph by nodes, inputs, and output.
+
+        If multiple parameters are specified, the result is a union
+        of the selection. The subgraph is a deep copy of the original graph.
+        The behavior is different from the parent class method, where the subgraph
+        returns a view of the original graph.
+        """
+
+        nodes = nodes or []
+        node_inputs = subnodes_by_inputs(self, inputs or [])
+        node_outputs = subnodes_by_outputs(self, outputs or [])
+
+        # convert nodes to list because the parent class method accepts generator
+        # for nodes.
+        # may consider not using the same name as the parent class to avoid collision
+        subgraph_nodes = set(list(nodes) + node_inputs + node_outputs)  # unique nodes
+
+        return super().subgraph(subgraph_nodes).deepcopy()
+
+    def replace_subgraph(
+        self, subgraph, name, func, output=None, inputs=None, modifiers=None
+    ):
+        """Replace subgraph with a node."""
+        return replace_subgraph(self, subgraph, name, func, output, inputs, modifiers)
+
+    def modify_node(
+        self, node, func=None, output=None, inputs=None, modifiers=None, inplace=False
+    ):
+        """Modify node attributes."""
+        return modify_node(self, node, func, output, inputs, modifiers, inplace)
+
+    def draw(self, style="verbose", export=None):
+        """Draw the graph.
+
+        Draws the default styled graph.
+
+        :param str style: there are three styles, plain, short, and verbose.
+            Plain shows nodes only, short shows part of the metadata, and
+            long shows all the metadata.
+        :param str export: filename to save the graph as. The file extension
+            is needed.
+        """
+
+        return draw_graph(self, str(self), style, export)
+
+    def deepcopy(self):
+        """Deepcopy graph.
+
+        The graph.copy method is a shallow copy. Deepcopy creates copy for the
+        attributes dictionary.
+        `graph.copy<https://networkx.org/documentation/stable/reference/classes
+        /generated/networkx.Graph.copy.html>_`
+
+        However, for subgraphs, deepcopy is incredibly inefficient because
+        subgraph contains '_graph', which stores the original graph.
+        An alternative method is to copy the code from the copy method,
+        but use deepcopy for the items.
+
+        The parser is redefined in the new graph.
+        """
+
+        G = self.__class__()
+        G.graph.update(deepcopy(self.graph))
+        G.add_nodes_from((n, deepcopy(d)) for n, d in self._node.items())
+        G.add_edges_from(
+            (u, v, deepcopy(datadict))
+            for u, nbrs in self._adj.items()
+            for v, datadict in nbrs.items()
+        )
+
+        return G
```

### Comparing `mmodel-0.5.2/mmodel/handler.py` & `mmodel-0.6.0/mmodel/handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-from collections import UserDict
-from mmodel.utility import graph_topological_sort, param_counter
-from datetime import datetime
-import h5py
-import string
-import random
-
-ERROR_FORMAT = """\
-An exception occurred for node '{node}':
---- node info ---
-{node_str}
---- input info ---
-{input_str}
-"""
-
-
-class TopologicalHandler:
-    """Base class for executing graph nodes in topological order.
-
-    "Returns" specifies the output order. If there is only one return
-    the value is outputted, otherwise a tuple is outputted. This
-    behavior is similar to the Python function.
-
-    The topological handler assumes each node has exactly one output.
-
-    :param str name: name of the handler (same as the model instance)
-    :param networkx.digraph graph: graph
-    :param list returns: handler returns order
-        The list should have the same or more elements than the graph returns.
-        See Model constructor definition.
-    """
-
-    DataClass: type = callable
-
-    def __init__(self, name, graph, returns: list, **datacls_kwargs):
-
-        self.__name__ = name
-        # __signature__ allows the inspect module to properly generate the signature
-        self.__signature__ = graph.signature
-        self.returns = returns
-        self.order = graph_topological_sort(graph)
-        self.graph = graph
-        self.datacls_kwargs = datacls_kwargs
-
-    def __call__(self, **kwargs):
-        """Execute graph model by layer."""
-
-        data = self.DataClass(kwargs, **self.datacls_kwargs)
-
-        for node, node_attr in self.order:
-            self.run_node(data, node, node_attr)
-
-        result = self.finish(data, self.returns)
-
-        return result
-
-    def run_node(self, data, node, node_attr):
-        """Run the individual node."""
-
-        # Only parameters without defaults are applied
-
-        kwargs = {
-            key: data[key]
-            for key, param in node_attr["sig"].parameters.items()
-            if (param.default is param.empty)
-        }
-        try:
-            # execute
-            func_result = node_attr["func"](**kwargs)
-            output = node_attr["output"]
-            if output:  # skip the None
-                data[output] = func_result
-
-        except:  # exception occurred while running the node
-
-            if hasattr(data, "close"):
-                data.close()
-            # format the error message
-            node_str = self.graph.node_metadata(node)
-            input_str = "\n".join(
-                [f"{key} = {repr(value)}" for key, value in kwargs.items()]
-            )
-            msg = ERROR_FORMAT.format(node=node, input_str=input_str, node_str=node_str)
-            raise Exception(msg)
-
-    def finish(self, data, returns):
-        """Finish execution."""
-
-        if len(returns) == 0:
-            result = None
-        elif len(returns) == 1:
-            result = data[returns[0]]
-        else:
-            result = tuple(data[rt] for rt in returns)
-
-        # if the data class needs to be closed
-        if hasattr(data, "close"):
-            data.close()
-
-        return result
-
-
-class MemData(UserDict):
-    """Modified dictionary that checks the counter every time a value is accessed."""
-
-    def __init__(self, data, counter):
-        """Counter is a copy of the counter dictionary."""
-        self.counter = counter.copy()
-        super().__init__(data)
-
-    def __getitem__(self, key):
-        """When a key is accessed, reduce the counter.
-
-        If the counter has reached zero, pop the value (key is deleted)
-        else wise return the key.
-        """
-
-        self.counter[key] -= 1
-
-        if self.counter[key] == 0:
-            # return the value and delete the key in the dictionary
-            value = super().__getitem__(key)
-            del self[key]
-            return value
-
-        else:
-            return super().__getitem__(key)
-
-
-class H5Data:
-    """Data class to interact with underlying h5 file.
-
-    The "timestamp-uuid" is used to ensure unique entries to the H5 group.
-    The randomly generated short uuid has 36^5, which is roughly 2e9
-    possibilities (picoseconds range).
-    """
-
-    def __init__(self, data, fname, gname):
-
-        self.fname = fname
-
-        self.f = h5py.File(self.fname, "a")
-
-        alphabet = string.ascii_lowercase + string.digits
-        shortuuid = "".join(random.choices(alphabet, k=6))
-        self.gname = f"{gname} {datetime.now().strftime('%y%m%d-%H%M%S')}-{shortuuid}"
-        self.group = self.f.create_group(self.gname)
-        self.update(data)
-
-    def update(self, data):
-        """Write key values in bulk."""
-        for key, value in data.items():
-            self[key] = value
-
-    def __getitem__(self, key):
-        """Read dataset/attribute by the group.
-
-        :param str key: value name
-        :param h5py.group group: open h5py group object
-        """
-
-        return self.group[key][()]
-
-    def __setitem__(self, key, value):
-        """Write h5 dataset/attribute by the group.
-
-        If the object type cannot be recognized by HDF5, the string representation
-        of the object is written as an attribute
-        :param dict value_dict: the dictionary of values to write
-        :param h5py.group group: open h5py group object
-        """
-        try:
-            self.group.create_dataset(key, data=value)
-        except TypeError:
-            # TypeError: Object dtype dtype('O') has no native HDF5 equivalent
-            self.group.attrs[key] = str(value)
-
-    def close(self):
-        """Close the data object."""
-        self.f.close()
-
-
-class BasicHandler(TopologicalHandler):
-    """Basic handler, use the dictionary as a data class."""
-
-    DataClass = dict
-
-
-class MemHandler(TopologicalHandler):
-    """Memory optimized handler, delete intermediate values when necessary.
-
-    The process works by keeping a record of the parameter counter.
-    See MemData class for more details.
-    """
-
-    DataClass = MemData
-
-    def __init__(self, name, graph, returns: list):
-        """Add counter to the object"""
-
-        counter = param_counter(graph, returns)
-
-        super().__init__(name, graph, returns, counter=counter)
-
-
-class H5Handler(TopologicalHandler):
-    """H5 Handler, saves all calculation values to an h5 file.
-
-    :param str fname: h5 file name
-    :param str gname: group name for the data entry
-    """
-
-    DataClass = H5Data
-
-    def __init__(self, name, graph, returns, fname: str, gname: str = ""):
-        super().__init__(name, graph, returns, fname=fname, gname=gname)
+from collections import UserDict
+from mmodel.utility import graph_topological_sort, param_counter
+from datetime import datetime
+import h5py
+import string
+import random
+
+ERROR_FORMAT = """\
+An exception occurred for node '{node}':
+--- node info ---
+{node_str}
+--- input info ---
+{input_str}
+"""
+
+
+class TopologicalHandler:
+    """Base class for executing graph nodes in topological order.
+
+    "Returns" specifies the output order. If there is only one return
+    the value is outputted, otherwise a tuple is outputted. This
+    behavior is similar to the Python function.
+
+    The topological handler assumes each node has exactly one output.
+
+    :param str name: name of the handler (same as the model instance)
+    :param networkx.digraph graph: graph
+    :param list returns: handler returns order
+        The list should have the same or more elements than the graph returns.
+        See Model constructor definition.
+    """
+
+    DataClass: type = callable
+
+    def __init__(self, name, graph, returns: list, **datacls_kwargs):
+
+        self.__name__ = name
+        # __signature__ allows the inspect module to properly generate the signature
+        self.__signature__ = graph.signature
+        self.returns = returns
+        self.order = graph_topological_sort(graph)
+        self.graph = graph
+        self.datacls_kwargs = datacls_kwargs
+
+    def __call__(self, **kwargs):
+        """Execute graph model by layer."""
+
+        data = self.DataClass(kwargs, **self.datacls_kwargs)
+
+        for node, node_attr in self.order:
+            self.run_node(data, node, node_attr)
+
+        result = self.finish(data, self.returns)
+
+        return result
+
+    def run_node(self, data, node, node_attr):
+        """Run the individual node."""
+
+        # Only parameters without defaults are applied
+
+        kwargs = {
+            key: data[key]
+            for key, param in node_attr["sig"].parameters.items()
+            if (param.default is param.empty)
+        }
+        try:
+            # execute
+            func_result = node_attr["func"](**kwargs)
+            output = node_attr["output"]
+            if output:  # skip the None
+                data[output] = func_result
+
+        except:  # exception occurred while running the node
+
+            if hasattr(data, "close"):
+                data.close()
+            # format the error message
+            node_str = self.graph.node_metadata(node)
+            input_str = "\n".join(
+                [f"{key} = {repr(value)}" for key, value in kwargs.items()]
+            )
+            msg = ERROR_FORMAT.format(node=node, input_str=input_str, node_str=node_str)
+            raise Exception(msg)
+
+    def finish(self, data, returns):
+        """Finish execution."""
+
+        if len(returns) == 0:
+            result = None
+        elif len(returns) == 1:
+            result = data[returns[0]]
+        else:
+            result = tuple(data[rt] for rt in returns)
+
+        # if the data class needs to be closed
+        if hasattr(data, "close"):
+            data.close()
+
+        return result
+
+
+class MemData(UserDict):
+    """Modified dictionary that checks the counter every time a value is accessed."""
+
+    def __init__(self, data, counter):
+        """Counter is a copy of the counter dictionary."""
+        self.counter = counter.copy()
+        super().__init__(data)
+
+    def __getitem__(self, key):
+        """When a key is accessed, reduce the counter.
+
+        If the counter has reached zero, pop the value (key is deleted)
+        else wise return the key.
+        """
+
+        self.counter[key] -= 1
+
+        if self.counter[key] == 0:
+            # return the value and delete the key in the dictionary
+            value = super().__getitem__(key)
+            del self[key]
+            return value
+
+        else:
+            return super().__getitem__(key)
+
+
+class H5Data:
+    """Data class to interact with underlying h5 file.
+
+    The "timestamp-uuid" is used to ensure unique entries to the H5 group.
+    The randomly generated short uuid has 36^5, which is roughly 2e9
+    possibilities (picoseconds range).
+    """
+
+    def __init__(self, data, fname, gname):
+
+        self.fname = fname
+
+        self.f = h5py.File(self.fname, "a")
+
+        alphabet = string.ascii_lowercase + string.digits
+        shortuuid = "".join(random.choices(alphabet, k=6))
+        self.gname = f"{gname} {datetime.now().strftime('%y%m%d-%H%M%S')}-{shortuuid}"
+        self.group = self.f.create_group(self.gname)
+        self.update(data)
+
+    def update(self, data):
+        """Write key values in bulk."""
+        for key, value in data.items():
+            self[key] = value
+
+    def __getitem__(self, key):
+        """Read dataset/attribute by the group.
+
+        :param str key: value name
+        :param h5py.group group: open h5py group object
+        """
+
+        return self.group[key][()]
+
+    def __setitem__(self, key, value):
+        """Write h5 dataset/attribute by the group.
+
+        If the object type cannot be recognized by HDF5, the string representation
+        of the object is written as an attribute
+        :param dict value_dict: the dictionary of values to write
+        :param h5py.group group: open h5py group object
+        """
+        try:
+            self.group.create_dataset(key, data=value)
+        except TypeError:
+            # TypeError: Object dtype dtype('O') has no native HDF5 equivalent
+            self.group.attrs[key] = str(value)
+
+    def close(self):
+        """Close the data object."""
+        self.f.close()
+
+
+class BasicHandler(TopologicalHandler):
+    """Basic handler, use the dictionary as a data class."""
+
+    DataClass = dict
+
+
+class MemHandler(TopologicalHandler):
+    """Memory optimized handler, delete intermediate values when necessary.
+
+    The process works by keeping a record of the parameter counter.
+    See MemData class for more details.
+    """
+
+    DataClass = MemData
+
+    def __init__(self, name, graph, returns: list):
+        """Add counter to the object."""
+
+        counter = param_counter(graph, returns)
+
+        super().__init__(name, graph, returns, counter=counter)
+
+
+class H5Handler(TopologicalHandler):
+    """H5 Handler, saves all calculation values to an h5 file.
+
+    :param str fname: h5 file name
+    :param str gname: group name for the data entry
+    """
+
+    DataClass = H5Data
+
+    def __init__(self, name, graph, returns, fname: str, gname: str = ""):
+        super().__init__(name, graph, returns, fname=fname, gname=gname)
```

### Comparing `mmodel-0.5.2/mmodel/metadata.py` & `mmodel-0.6.0/mmodel/metadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,195 +1,256 @@
-"""Handle node, graph and model metadata.
-
-The two core types of functions are formatter and wrapper. The formatter
-takes care of the formatting of the metadata, and the wrapper takes care
-of the wrapping of the metadata.
-"""
-
-import inspect
-from textwrap import TextWrapper
-
-
-class MetaDataFormatter:
-    """Metadata Formatter."""
-
-    def __init__(self, formatter: dict, metaorder: list = None):
-        """Initiate the formatter."""
-
-        self.frommatter = formatter
-        self.metaorder = metaorder
-
-    def __call__(self, metadata):
-        """Convert metadata dictionary to string.
-
-        The process returns a list of metadata by lines.
-        If the formatter is not found in the formatter dictionary,
-        the default string output is "key: value".
-
-        :param dict metadata: metadata dictionary
-        :param list metaorder: metadata key order, entry is None if linebreak needed.
-            Defaults to dictionary key order.
-        """
-        metaorder = self.metaorder if self.metaorder is not None else metadata.keys()
-        metadata_str_list = []
-        for key in metaorder:
-            if key is None:
-                metadata_str_list.append("")
-                continue
-            elif key not in metadata:
-                continue
-            if key in self.frommatter:
-                metadata_str_list.extend(self.frommatter[key](key, metadata[key]))
-            else:
-                metadata_str_list.extend([f"{key}: {metadata[key]}"])
-
-        return metadata_str_list
-
-
-def format_func(key, value):
-    """Format the metadata value that has a function.
-
-    The key name is not shown in the string output.
-    The result is func(args1, args2, ...)"""
-
-    return [f"{value.__name__}{inspect.signature(value)}"]
-
-
-def format_listargs(key, value):
-    """Format the metadata value that has a list of (func, kwargs).
-
-    The formatter is for modifiers and other metadata that have a
-    list of (func, kwargs), and kwargs is a dictionary.
-    """
-
-    if value:
-        str_list = [f"{key}:"]
-
-        for func, kwargs in value:
-            str_value = [repr(v) for v in kwargs.values()]
-            mod_str = f"\t- {func.__name__}({', '.join(str_value)})"
-            str_list.append(mod_str)
-
-        return str_list
-
-    else:
-        return []
-
-
-def format_args(key, value):
-    """Format the metadata value that has the value of (func, kwargs).
-
-    The formatter is for the handler metadata.
-    """
-    if value:
-        func, kwargs = value
-        return [
-            f"{key}: {func.__name__}({', '.join(repr(v) for v in kwargs.values())})"
-        ]
-    else:
-        return []
-
-
-def format_returns(key, value):
-    """Format the metadata value that has a list of returns.
-
-    The formatter is for the returns metadata. If the "returns" value is empty,
-    the output is None. If the returns only have 1 value, return the value, else
-    return the values separated by commas in a tuple representation.
-    """
-
-    return_len = len(value)
-
-    if return_len == 0:
-        returns_str = "None"
-    elif return_len == 1:
-        returns_str = value[0]
-    else:
-        returns_str = f"({', '.join(value)})"
-
-    return [f"{key}: {returns_str}"]
-
-
-def format_value(key, value):
-    """Format the metadata without displaying key."""
-    if value:
-        return [value]
-    else:
-        return []
-
-
-def format_obj(key, value):
-    """Format the metadata value that is an object.
-
-    Only show the name of the object. This is used for graph objects.
-    The object needs to have __name__ or name attribute defined.
-    """
-
-    name = getattr(value, "__name__", getattr(value, "name", None))
-    if name:
-        return [f"{key}: {name}"]
-    else:
-        return []
-
-
-modelformatter = MetaDataFormatter(
-    {
-        "model": format_func,
-        "returns": format_returns,
-        "graph": format_obj,
-        "handler": format_args,
-        "modifiers": format_listargs,
-        "description": format_value,
-    },
-    ["model", "returns", "graph", "handler", "modifiers", None, "description"],
-)
-
-nodeformatter = MetaDataFormatter(
-    {
-        "node": format_value,
-        "func": format_func,
-        "modifiers": format_listargs,
-        "doc": format_value,
-    },
-    ["node", None, "func", "return", "functype", "modifiers", None, "doc"],
-)
-
-
-def textwrapper(width: int = 80, indent: int = 2):
-    """Wrap metadata content.
-
-    The width defaults to 80 characters. The resulting wrapping has no
-    initial indentation. The indent parameter is the subsequent indent
-    parameter in the wrap function. The tabsize is the same as
-    the indent.
-    """
-
-    return TextWrapper(
-        width=width,
-        subsequent_indent=" " * indent,
-        replace_whitespace=False,
-        expand_tabs=True,
-        tabsize=indent,
-    )
-
-
-# Standard textwrapper with 80 characters.
-textwrap80 = textwrapper(80, 2)
-# shorted textwarpper with 5o characters for nodes.
-textwrap50 = textwrapper(50, 2)
-
-
-def format_metadata(metadata, formatter, textwrapper):
-    """Format and wrap the metadata."""
-
-    metadata_list = formatter(metadata)
-
-    if textwrapper:
-        metadata_wrapped = []
-        for line in metadata_list:
-            if line:
-                metadata_wrapped.extend(textwrapper.wrap(line))
-            else:
-                metadata_wrapped.append("")
-        return metadata_wrapped
-
-    return metadata_list
+"""Handle node, graph and model metadata.
+
+The two core types of functions are formatter and wrapper. The formatter
+takes care of the formatting of the metadata, and the wrapper takes care
+of the wrapping of the metadata.
+"""
+
+import inspect
+from textwrap import TextWrapper
+
+
+class MetaDataFormatter:
+    """Metadata Formatter."""
+
+    def __init__(self, formatter: dict, metaorder: list = None):
+        """Initiate the formatter."""
+
+        self.formatter = formatter
+        self.metaorder = metaorder
+
+    def __call__(self, metadata):
+        """Convert metadata dictionary to string.
+
+        The process returns a list of metadata by lines.
+        If the formatter is not found in the formatter dictionary,
+        the default string output is "key: value".
+
+        :param dict metadata: metadata dictionary
+        :param list metaorder: metadata key order, entry is None if linebreak needed.
+            Defaults to dictionary key order.
+        """
+        metaorder = self.metaorder if self.metaorder is not None else metadata.keys()
+        metadata_str_list = []
+        for key in metaorder:
+            if key is None:
+                metadata_str_list.append("")
+                continue
+            elif key not in metadata:
+                continue
+            if key in self.formatter:
+                metadata_str_list.extend(self.formatter[key](key, metadata[key]))
+            else:
+                metadata_str_list.extend([f"{key}: {metadata[key]}"])
+
+        return metadata_str_list
+
+
+def format_func(key, value):
+    """Format the metadata value that has a function.
+
+    The key name is not shown in the string output.
+    The result is func(args1, args2, ...)"""
+
+    return [f"{value.__name__}{inspect.signature(value)}"]
+
+
+def format_list(key, value):
+    """Format the metadata value that is a list."""
+
+    if value:
+        str_list = [f"{key}:"]
+        for v in value:
+            str_list.append(f"\t- {v}")
+        return str_list
+    else:
+        return []
+
+
+def modifier_metadata(closure):
+    """Extract metadata from closure, including the name and the arguments.
+
+    The order of extraction:
+    1. If the object has the "metadata" attribute defined.
+    2. If the closure takes no arguments, the name is the function name.
+    3. If the closure takes arguments, the "metadata" attribute is not defined.
+
+    Note::
+
+        inspect.getclosurevars(closure).nonlocals can only parse values
+        if the value is used in the closure.
+    """
+
+    if hasattr(closure, "metadata"):
+        return closure.metadata
+    elif not inspect.getclosurevars(closure).nonlocals:
+        return closure.__name__
+
+    else:  # closure takes arguments
+
+        # In some rare cases, the closure is a nested function.
+        # For example, in the tests, the nested closure reflects the
+        # path of the parent function. Here we remove the nested
+        # parent function name.
+
+        name = closure.__qualname__.rsplit(".<locals>.")[-2]
+        kwargs = inspect.getclosurevars(closure).nonlocals
+        kwargs_str = ", ".join(f"{k}={repr(v)}" for k, v in kwargs.items())
+        return f"{name}({kwargs_str})"
+
+
+def format_modifierlist(key, value):
+    """Format the metadata that is a list of modifiers.
+
+    The metadata of the modifier is extracted by the modifier_metadata function.
+    The resulting list is formatted by the format_list function.
+    """
+
+    modifier_str_list = [modifier_metadata(modifier) for modifier in value]
+
+    return format_list(key, modifier_str_list)
+
+
+def format_dictargs(key, value):
+    """Format the metadata value that is a dictionary."""
+
+    if value:
+        str_list = [f"{key}:"]
+
+        for k, v in value.items():
+            mod_str = f"\t- {k}: {v}"
+            str_list.append(mod_str)
+
+        return str_list
+
+    else:
+        return []
+
+
+def format_args(key, value):
+    """Format the metadata value that has the value of (func, kwargs).
+
+    The formatter is for the handler metadata.
+    """
+    if value:
+        func, kwargs = value
+        return [
+            f"{key}: {func.__name__}({', '.join(repr(v) for v in kwargs.values())})"
+        ]
+    else:
+        return []
+
+
+def format_returns(key, value):
+    """Format the metadata value that has a list of returns.
+
+    The formatter is for the returns metadata. If the "returns" value is empty,
+    the output is None. If the returns only have 1 value, return the value, else
+    return the values separated by commas in a tuple representation.
+    """
+
+    return_len = len(value)
+
+    if return_len == 0:
+        returns_str = "None"
+    elif return_len == 1:
+        returns_str = value[0]
+    else:
+        returns_str = f"({', '.join(value)})"
+
+    return [f"{key}: {returns_str}"]
+
+
+def format_value(key, value):
+    """Format the metadata without displaying key."""
+    if value:
+        return [value]
+    else:
+        return []
+
+
+def format_obj(key, value):
+    """Format the metadata value that is an object.
+
+    Only show the name of the object. This is used for graph objects.
+    The object needs to have __name__ or name attribute defined.
+    """
+
+    name = getattr(value, "__name__", getattr(value, "name", None))
+    if name:
+        return [f"{key}: {name}"]
+    else:
+        return []
+
+
+modelformatter = MetaDataFormatter(
+    {
+        "model": format_func,
+        "returns": format_returns,
+        "graph": format_obj,
+        "handler": format_obj,
+        "handler args": format_dictargs,
+        "modifiers": format_modifierlist,
+        "description": format_value,
+    },
+    [
+        "model",
+        "returns",
+        "graph",
+        "handler",
+        "handler args",
+        "modifiers",
+        None,
+        "description",
+    ],
+)
+
+nodeformatter = MetaDataFormatter(
+    {
+        "node": format_value,
+        "func": format_func,
+        "modifiers": format_modifierlist,
+        "doc": format_value,
+    },
+    ["node", None, "func", "return", "functype", "modifiers", None, "doc"],
+)
+
+
+def textwrapper(width: int = 80, indent: int = 2):
+    """Wrap metadata content.
+
+    The width defaults to 80 characters. The resulting wrapping has no
+    initial indentation. The indent parameter is the subsequent indent
+    parameter in the wrap function. The tabsize is the same as
+    the indent.
+    """
+
+    return TextWrapper(
+        width=width,
+        subsequent_indent=" " * indent,
+        replace_whitespace=False,
+        expand_tabs=True,
+        tabsize=indent,
+    )
+
+
+# Standard textwrapper with 80 characters.
+textwrap80 = textwrapper(80, 2)
+# shorted textwarpper with 5o characters for nodes.
+textwrap50 = textwrapper(50, 2)
+
+
+def format_metadata(metadata, formatter, textwrapper):
+    """Format and wrap the metadata."""
+
+    metadata_list = formatter(metadata)
+
+    if textwrapper:
+        metadata_wrapped = []
+        for line in metadata_list:
+            if line:
+                metadata_wrapped.extend(textwrapper.wrap(line))
+            else:
+                metadata_wrapped.append("")
+        return metadata_wrapped
+
+    return metadata_list
```

### Comparing `mmodel-0.5.2/mmodel/model.py` & `mmodel-0.6.0/mmodel/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,172 @@
-from mmodel.utility import parse_input, is_node_attr_defined, is_edge_attr_defined
-from mmodel.metadata import modelformatter, textwrap80, format_metadata
-from mmodel.draw import draw_graph
-import networkx as nx
-
-
-class Model:
-    """Create model callable.
-
-    :param str name: Model name
-    :param object graph: ModelGraph instance (digraph)
-    :param class handler: Handler class that handles model execution and
-        the keyword arguments. The parameter format is (HandlerClass, {})
-        By default, the handler takes the graph as the first parameter.
-        For additional arguments, add an argument to the dictionary afterward.
-    :param list modifiers: modifiers used for the whole graph model executable.
-        The parameter is Optional and defaults to an empty list. For each modifier,
-        the format is (modifier, {}). All modifiers should have the function as
-        the first argument.
-    :param str description: model description
-    :param list returns: The order of returns of the model; defaults to the
-        topological search.
-    """
-
-    _model_keys = ["name", "graph", "handler", "modifiers", "description", "returns"]
-
-    def __init__(
-        self,
-        name,
-        graph,
-        handler,
-        modifiers: list = None,
-        description: str = "",
-        returns: list = None,
-    ):
-
-        assert self._is_valid_graph(graph)
-        self.name = self.__name__ = name
-
-        # create a copy of the graph
-        self._graph = nx.freeze(graph.deepcopy())
-        self.returns = returns or self._graph.returns  # tuples
-        self.modifiers = modifiers or list()
-        self.handler = handler
-        self.description = description
-
-        handler_class, handler_kwargs = handler
-
-        executor = handler_class(name, self._graph, self.returns, **handler_kwargs)
-        self.execution_order = [node for node, _ in executor.order]
-
-        for mdf, kwargs in self.modifiers:
-            executor = mdf(executor, **kwargs)
-
-        self.__signature__ = executor.__signature__
-
-        # final callable
-        self._executor = executor
-
-    def __call__(self, *args, **kwargs):
-        """Execute the model.
-
-        The inputs from the keyword arguments are parsed and passed to the
-        the handler class.
-        """
-
-        # process inputs
-        inputs = parse_input(self.__signature__, *args, **kwargs)
-
-        return self._executor(**inputs)
-
-    def _metadata_dict(self, verbose):
-        """Return a dictionary with metadata keys."""
-
-        short_dict = {"model": self, "returns": self.returns}
-
-        additonal_dict = {
-            "graph": self._graph,
-            "handler": self.handler,
-            "modifiers": self.modifiers,
-            "description": self.description,
-        }
-
-        if verbose:
-            return {**short_dict, **additonal_dict}
-        else:
-            return short_dict
-
-    def metadata_str(
-        self, verbose=True, formatter=modelformatter, textwrapper=textwrap80
-    ):
-        """Parse metadata string of the Model instance."""
-        return format_metadata(self._metadata_dict(verbose), formatter, textwrapper)
-
-    def __str__(self):
-        """Output callable information."""
-
-        str_list = self.metadata_str()
-        return "\n".join(str_list).rstrip()
-
-    @staticmethod
-    def _is_valid_graph(G):
-        """Check if the model graph is valid to build an executable.
-
-        ``mmodel`` does not allow cycle graphs, graphs with isolated nodes,
-        and all nodes have callable attributes defined.
-        The method is bound to the Model class because the features
-        are specific to ``Model`` class.
-        """
-
-        assert nx.is_directed(G), f"invalid graph ({G.name}): undirected graph."
-        assert not nx.recursive_simple_cycles(
-            G
-        ), f"invalid graph ({G.name}): graph contains cycles."
-
-        assert is_node_attr_defined(G, "func", "callable")
-        # the following might occur when the node object is incorrectly constructed
-        assert is_node_attr_defined(G, "output")
-        assert is_node_attr_defined(G, "sig", "signature")
-        assert is_edge_attr_defined(G, "var", "variable")
-
-        return True
-
-    @property
-    def graph(self):
-        """The graph attribute output a copy of the graph."""
-        return self._graph.deepcopy()
-
-    def get_node(self, node):
-        """Quick access to node within the model."""
-
-        return self._graph.nodes[node]
-
-    def get_node_func(self, node):
-        """Quick access to node base callable within the model.
-
-        The function helps extract the original function within
-        the node.
-        """
-
-        return self._graph.nodes[node]["_func"]
-
-    def node_metadata(self, *args, **kwargs):
-        """View a specific node."""
-
-        return self._graph.node_metadata(*args, **kwargs)
-
-    def draw(self, style="verbose", export=None):
-        """Draw the graph of the model.
-
-        Draws the default styled graph.
-
-        :param str style: there are three styles, plain, short, and verbose.
-            Plain shows nodes only, short shows part of the metadata, and
-            long shows all the metadata.
-        :param str export: filename to save the graph as. The file extension
-            is needed.
-        """
-
-        return draw_graph(self._graph, str(self), style, export)
-
-    def edit(self, **kwargs):
-        """Edit components of the model to create a new model.
-
-        It is not recommended to edit the graph component of the model.
-        Although it does create a new model, but "edit" is for creating
-        a new model with the same graph.
-        """
-
-        model_dict = {key: getattr(self, key) for key in self._model_keys}
-        return self.__class__(**{**model_dict, **kwargs})
+from mmodel.utility import parse_input, is_node_attr_defined, is_edge_attr_defined
+from mmodel.metadata import modelformatter, textwrap80, format_metadata
+from mmodel.draw import draw_graph
+import networkx as nx
+
+
+class Model:
+    """Create model callable.
+
+    :param str name: Model name
+    :param object graph: ModelGraph instance (digraph)
+    :param class handler: Handler class that handles model execution and
+        the keyword arguments. The parameter format is (HandlerClass, {})
+        By default, the handler takes the graph as the first parameter.
+        For additional arguments, add an argument to the dictionary afterward.
+    :param list modifiers: modifiers used for the whole graph model executable.
+        The parameter is Optional and defaults to an empty list. For each modifier,
+        the format is (modifier, {}). All modifiers should have the function as
+        the first argument.
+    :param str description: model description
+    :param list returns: The order of returns of the model; defaults to the
+        topological search.
+    """
+
+    _model_keys = ["name", "graph", "handler", "modifiers", "description", "returns"]
+
+    def __init__(
+        self,
+        name,
+        graph,
+        handler,
+        modifiers: list = None,
+        description: str = "",
+        returns: list = None,
+        **kwargs,
+    ):
+
+        assert self._is_valid_graph(graph)
+        self.name = self.__name__ = name
+
+        # create a copy of the graph
+        self._graph = nx.freeze(graph.deepcopy())
+        self.returns = returns or self._graph.returns  # tuples
+        self.modifiers = modifiers or list()
+        self.handler = handler
+        self.handler_args = kwargs
+        self.description = description
+
+        executor = handler(name, self._graph, self.returns, **kwargs)
+        self.execution_order = [node for node, _ in executor.order]
+
+        for mdf in self.modifiers:
+            executor = mdf(executor)
+
+        self.__signature__ = executor.__signature__
+
+        # final callable
+        self._executor = executor
+
+    def __call__(self, *args, **kwargs):
+        """Execute the model.
+
+        The inputs from the keyword arguments are parsed and passed to the
+        the handler class.
+        """
+
+        # process inputs
+        inputs = parse_input(self.__signature__, *args, **kwargs)
+
+        return self._executor(**inputs)
+
+    def _metadata_dict(self, verbose):
+        """Return a dictionary with metadata keys."""
+
+        short_dict = {"model": self, "returns": self.returns}
+
+        additonal_dict = {
+            "graph": self._graph,
+            "handler": self.handler,
+            "handler args": self.handler_args,
+            "modifiers": self.modifiers,
+            "description": self.description,
+        }
+
+        if verbose:
+            return {**short_dict, **additonal_dict}
+        else:
+            return short_dict
+
+    def metadata_str(
+        self, verbose=True, formatter=modelformatter, textwrapper=textwrap80
+    ):
+        """Parse metadata string of the Model instance."""
+        return format_metadata(self._metadata_dict(verbose), formatter, textwrapper)
+
+    def __str__(self):
+        """Output callable information."""
+
+        str_list = self.metadata_str()
+        return "\n".join(str_list).rstrip()
+
+    @staticmethod
+    def _is_valid_graph(G):
+        """Check if the model graph is valid to build an executable.
+
+        ``mmodel`` does not allow cycle graphs, graphs with isolated nodes,
+        and all nodes have callable attributes defined.
+        The method is bound to the Model class because the features
+        are specific to ``Model`` class.
+        """
+
+        assert nx.is_directed(G), f"invalid graph ({G.name}): undirected graph."
+        assert not nx.recursive_simple_cycles(
+            G
+        ), f"invalid graph ({G.name}): graph contains cycles."
+
+        assert is_node_attr_defined(G, "func", "callable")
+        # the following might occur when the node object is incorrectly constructed
+        assert is_node_attr_defined(G, "output")
+        assert is_node_attr_defined(G, "sig", "signature")
+        assert is_edge_attr_defined(G, "var", "variable")
+
+        return True
+
+    @property
+    def graph(self):
+        """The graph attribute output a copy of the graph."""
+        return self._graph.deepcopy()
+
+    def get_node(self, node):
+        """Quick access to node within the model."""
+
+        return self._graph.nodes[node]
+
+    def get_node_func(self, node):
+        """Quick access to node base callable within the model.
+
+        The function helps extract the original function within
+        the node.
+        """
+
+        return self._graph.nodes[node]["_func"]
+
+    def node_metadata(self, *args, **kwargs):
+        """View a specific node."""
+
+        return self._graph.node_metadata(*args, **kwargs)
+
+    def draw(self, style="verbose", export=None):
+        """Draw the graph of the model.
+
+        Draws the default styled graph.
+
+        :param str style: there are three styles, plain, short, and verbose.
+            Plain shows nodes only, short shows part of the metadata, and
+            long shows all the metadata.
+        :param str export: filename to save the graph as. The file extension
+            is needed.
+        """
+
+        return draw_graph(self._graph, str(self), style, export)
+
+    def edit(self, **kwargs):
+        """Edit components of the model to create a new model.
+
+        It is not recommended to edit the graph component of the model.
+        Although it does create a new model, but "edit" is for creating
+        a new model with the same graph.
+        """
+
+        model_dict = {key: getattr(self, key) for key in self._model_keys}
+        return self.__class__(**{**model_dict, **kwargs})
```

### Comparing `mmodel-0.5.2/mmodel/utility.py` & `mmodel-0.6.0/mmodel/utility.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-from inspect import Signature, Parameter
-import networkx as nx
-
-# graph properties
-def modelgraph_signature(graph):
-    """Obtain the signature from the model graph.
-
-    :param DiGraph graph: networkx.Digraph() object,
-        with 'signature', and 'output' defined for nodes
-        and "parameters" for edges.
-        The args are a dictionary of inspected signature.
-    """
-
-    parameters = {}
-    for sig in nx.get_node_attributes(graph, "sig").values():
-        for pname, param in sig.parameters.items():
-            # remove the default values
-            if param.default is param.empty and param not in parameters:
-                parameters.update({pname: param})
-
-    for output in nx.get_node_attributes(graph, "output").values():
-        parameters.pop(output, None)  # if doesn't exist return None
-
-    return Signature(sorted(parameters.values(), key=param_sorter))
-
-
-def modelgraph_returns(graph):
-    """Obtain the return parameter from the model graph.
-
-    The assumption is that all return parameter names are unique.
-    The function checks all returns values and all intermediate values (edge values)
-
-    :returns: list of variable names based on note outputs
-    :rtype: list
-    """
-
-    returns = []
-    intermediate = []
-
-    for node in graph.nodes():
-        if graph.nodes[node]["output"]:  # skip None
-            returns.append(graph.nodes[node]["output"])
-    for edge in graph.edges():
-        intermediate.append(graph.edges[edge]["var"])
-
-    final_returns = list(set(returns) - set(intermediate))
-    final_returns.sort()
-    return final_returns
-
-
-def param_sorter(parameter):
-    """Sorter for argument parameter.
-
-    The values in the tuple are compared in sequential order:
-    1. Order by parameter kind
-    2. Default parameter rank at the end of its kind
-    3. Alphabetical order
-
-    :param inspect.Parameter parameter: parameter object
-    :rtype: (bool, parameter.name, parameter.kind)
-    """
-
-    if parameter.default is not parameter.empty:
-        return parameter.kind, True, parameter.name
-    else:
-        return parameter.kind, False, parameter.name
-
-
-def replace_signature(signature, replacement_dict):
-    """Replace signature with a dictionary of (key, pair).
-
-    The function is used to replace several input parameters with an object.
-    The signature is the original signature. The dictionary key should be the
-    replacement object, and the values should be a list of the target
-    parameters to be replaced. The replacement allows unused parameters, they
-    are skipped.
-    """
-
-    params = dict(signature.parameters)
-    for func, target_list in replacement_dict.items():
-        for target in target_list:
-            # del params[target]
-            params.pop(target, None)
-        params[func] = Parameter(func, 1)
-
-    return signature.replace(parameters=sorted(params.values(), key=param_sorter))
-
-
-def graph_topological_sort(graph):
-    """Determine the topological order.
-
-    `nx.topological_generations` outputs a generator with each node list generation.
-    However, it does not carry the node attributes. The method
-    outputs a list of nodes for each generation.
-
-    :return: topological order of the graph. Returns a list of nodes and its
-        attribute.
-    :rtype: list
-
-    """
-
-    topological_order = []
-
-    for node in nx.topological_sort(graph):
-        topological_order.append((node, graph.nodes[node]))
-
-    return topological_order
-
-
-def replace_subgraph(
-    graph, subgraph, name, func, output=None, inputs=None, modifiers=None
-):
-    """Replace subgraph with a node.
-
-    Find all parent nodes, not in the subgraph but child nodes in the
-    subgraph. (All child nodes of subgraph nodes are in the subgraph).
-    The edge attribute is passed down to the new edge. Here a new graph is
-    created by deep copy the original graph.
-
-    :param graph model_graph: model_graph to modify.
-    :param graph subgraph: subgraph that is being replaced by a node
-        subgraph is a view of the original graph.
-    :param str subgraph_name: name of the subgraph.
-    :param str output: output parameter name.
-    """
-
-    graph = graph.deepcopy()
-
-    new_edges = []
-    for node in subgraph.nodes():
-        for parent in graph.predecessors(node):
-            if parent not in subgraph:
-                new_edges.append((parent, name))
-        for child in graph.successors(node):
-            if child not in subgraph:
-                new_edges.append((name, child))
-
-    graph.remove_nodes_from(subgraph.nodes)
-    # remove unique edges
-    graph.add_edges_from(set(new_edges))
-
-    graph.set_node_object(
-        name, func=func, output=output, inputs=inputs, modifiers=modifiers
-    )
-
-    return graph
-
-
-def modify_node(
-    graph, node, func=None, output=None, inputs=None, modifiers=None, inplace=False
-):
-    """Modify node.
-
-    The result is a new graph with the node object modified.
-    :param str output: change the output of the node. If the node is not
-        terminal, the output should not be changed.
-    :param bool inplace: if True, the original graph is modified.
-
-    .. Note::
-
-        If the original node has output, the node cannot be modified to None.
-        If the original node has inputs, the modification cannot remove the
-        original input (set to [] does not change anything).
-
-        For the above two cases, a copy of the graph should be created and run
-        ``set_node_object`` again to reset the node object.
-
-    """
-    if not inplace:
-        graph = graph.deepcopy()
-
-    func = func or graph.nodes[node]["_func"]
-    modifiers = modifiers or graph.nodes[node]["modifiers"]
-    output = output or graph.nodes[node]["output"]
-    graph.set_node_object(
-        node, func=func, output=output, inputs=inputs, modifiers=modifiers
-    )
-
-    return graph
-
-
-def parse_parameters(parameters):
-    """Parse a list of parameters to signatures
-
-    :param list parameters: Parameters to parse. The element can either be a string
-        as the parameter name or a tuple/list as (parameter, default).
-    :return: parameter order and signature.
-    """
-
-    param_order = []  # parameters in the correct order
-    sig_list = []  # signature values
-    sig_df_list = []  # default values
-    defultargs = {}  # default arguments dictionary
-    for var in parameters:
-        if isinstance(var, tuple) or isinstance(var, list):
-            var_name, default_value = var
-            param_order.append(var_name)
-            sig_df_list.append(Parameter(var_name, 1, default=default_value))
-            defultargs[var_name] = default_value
-        else:
-            param_order.append(var)
-            sig_list.append(Parameter(var, 1))
-
-    sig = Signature(sig_list + sig_df_list)  # the default values are ordered next
-
-    return sig, param_order, defultargs
-
-
-def param_counter(graph, returns):
-    """Count the number of times a parameter is used for graph execution.
-
-    Count all function signature parameters. For extra returns,
-    add one to each count value.
-
-    :param list returns: method returns (include extra returns)
-    :return: dictionary with parameter_name: count pair
-    :rtype: dict
-    """
-
-    value_list = []
-    for sig in nx.get_node_attributes(graph, "sig").values():
-        for key, param in sig.parameters.items():
-
-            if param.default is param.empty:
-                value_list.append(key)
-
-    # add the additional parameter to list
-    value_list += returns
-
-    count = {}
-    for value in value_list:
-        count[value] = count.get(value, 0) + 1
-
-    return count
-
-
-def parse_input(signature, *args, **kwargs):
-    """parse argument based on signature and input.
-
-    The default value is automatically filled.
-    """
-
-    values = signature.bind(*args, **kwargs)
-    values.apply_defaults()
-    return values.arguments
-
-
-def is_node_attr_defined(graph, attr: str, attr_name: str = None):
-    """Check if all graph nodes have the attribute defined.
-
-    :param str attr: attribute string.
-    :param str attr_name: the detailed name of the attribute.
-
-    Raise an exception if the attribute is undefined.
-    """
-    attr_name = attr_name or attr
-
-    if graph.name:
-        graph_str = f"graph ({graph.name})"
-    else:
-        graph_str = "graph"
-
-    node_list = []
-    for node, node_attr in graph.nodes.data():
-        if attr not in node_attr:
-            node_list.append(node)
-
-    if node_list:
-        raise Exception(
-            f"invalid {graph_str}: {attr_name} "
-            f"{repr(attr)} is not defined for node(s) {node_list}."
-        )
-
-    return True
-
-
-def is_edge_attr_defined(graph, attr: str, attr_name: str = None):
-    """Check if all graph edges have the target attribute defined.
-
-    Raise an exception if the attribute is undefined.
-    """
-    attr_name = attr_name or attr
-
-    if graph.name:
-        graph_str = f"graph ({graph.name})"
-    else:
-        graph_str = "graph"
-
-    edge_list = []
-    for u, v, edge_attr in graph.edges.data():
-        if attr not in edge_attr:
-            edge_list.append((u, v))
-    if edge_list:
-        raise Exception(
-            f"invalid {graph_str}: {attr_name} {repr(attr)}"
-            f" is not defined for edge(s) {edge_list}."
-        )
-
-    return True
+from inspect import Signature, Parameter
+import networkx as nx
+
+# graph properties
+def modelgraph_signature(graph):
+    """Obtain the signature from the model graph.
+
+    :param DiGraph graph: networkx.Digraph() object,
+        with 'signature', and 'output' defined for nodes
+        and "parameters" for edges.
+        The args are a dictionary of inspected signature.
+    """
+
+    parameters = {}
+    for sig in nx.get_node_attributes(graph, "sig").values():
+        for pname, param in sig.parameters.items():
+            # remove the default values
+            if param.default is param.empty and param not in parameters:
+                parameters.update({pname: param})
+
+    for output in nx.get_node_attributes(graph, "output").values():
+        parameters.pop(output, None)  # if doesn't exist return None
+
+    return Signature(sorted(parameters.values(), key=param_sorter))
+
+
+def modelgraph_returns(graph):
+    """Obtain the return parameter from the model graph.
+
+    The assumption is that all return parameter names are unique.
+    The function checks all returns values and all intermediate values (edge values)
+
+    :returns: list of variable names based on note outputs
+    :rtype: list
+    """
+
+    returns = []
+    intermediate = []
+
+    for node in graph.nodes():
+        if graph.nodes[node]["output"]:  # skip None
+            returns.append(graph.nodes[node]["output"])
+    for edge in graph.edges():
+        intermediate.append(graph.edges[edge]["var"])
+
+    final_returns = list(set(returns) - set(intermediate))
+    final_returns.sort()
+    return final_returns
+
+
+def param_sorter(parameter):
+    """Sorter for argument parameter.
+
+    The values in the tuple are compared in sequential order:
+    1. Order by parameter kind
+    2. Default parameter rank at the end of its kind
+    3. Alphabetical order
+
+    :param inspect.Parameter parameter: parameter object
+    :rtype: (bool, parameter.name, parameter.kind)
+    """
+
+    if parameter.default is not parameter.empty:
+        return parameter.kind, True, parameter.name
+    else:
+        return parameter.kind, False, parameter.name
+
+
+def replace_signature_with_object(signature, replacement_dict):
+    """Replace signature with a dictionary of (key, pair).
+
+    The function is used to replace several input parameters with an object.
+    The signature is the original signature. The dictionary key should be the
+    replacement object, and the values should be a list of the target
+    parameters to be replaced. The replacement allows unused parameters, they
+    are skipped.
+    """
+
+    params = dict(signature.parameters)
+    for func, target_list in replacement_dict.items():
+        for target in target_list:
+            # del params[target]
+            params.pop(target, None)
+        params[func] = Parameter(func, 1)
+
+    return signature.replace(parameters=sorted(params.values(), key=param_sorter))
+
+
+def graph_topological_sort(graph):
+    """Determine the topological order.
+
+    `nx.topological_generations` outputs a generator with each node list generation.
+    However, it does not carry the node attributes. The method
+    outputs a list of nodes for each generation.
+
+    :return: topological order of the graph. Returns a list of nodes and its
+        attribute.
+    :rtype: list
+
+    """
+
+    topological_order = []
+
+    for node in nx.topological_sort(graph):
+        topological_order.append((node, graph.nodes[node]))
+
+    return topological_order
+
+
+def replace_subgraph(
+    graph, subgraph, name, func, output=None, inputs=None, modifiers=None
+):
+    """Replace subgraph with a node.
+
+    Find all parent nodes, not in the subgraph but child nodes in the
+    subgraph. (All child nodes of subgraph nodes are in the subgraph).
+    The edge attribute is passed down to the new edge. Here a new graph is
+    created by deep copy the original graph.
+
+    :param graph model_graph: model_graph to modify.
+    :param graph subgraph: subgraph that is being replaced by a node
+        subgraph is a view of the original graph.
+    :param str subgraph_name: name of the subgraph.
+    :param str output: output parameter name.
+    """
+
+    graph = graph.deepcopy()
+
+    new_edges = []
+    for node in subgraph.nodes():
+        for parent in graph.predecessors(node):
+            if parent not in subgraph:
+                new_edges.append((parent, name))
+        for child in graph.successors(node):
+            if child not in subgraph:
+                new_edges.append((name, child))
+
+    graph.remove_nodes_from(subgraph.nodes)
+    # remove unique edges
+    graph.add_edges_from(set(new_edges))
+
+    graph.set_node_object(
+        name, func=func, output=output, inputs=inputs, modifiers=modifiers
+    )
+
+    return graph
+
+
+def modify_node(
+    graph, node, func=None, output=None, inputs=None, modifiers=None, inplace=False
+):
+    """Modify node.
+
+    The result is a new graph with the node object modified.
+    :param str output: change the output of the node. If the node is not
+        terminal, the output should not be changed.
+    :param bool inplace: if True, the original graph is modified.
+
+    .. Note::
+
+        If the original node has output, the node cannot be modified to None.
+        If the original node has inputs, the modification cannot remove the
+        original input (set to [] does not change anything).
+
+        For the above two cases, a copy of the graph should be created and run
+        ``set_node_object`` again to reset the node object.
+
+    """
+    if not inplace:
+        graph = graph.deepcopy()
+
+    func = func or graph.nodes[node]["_func"]
+    modifiers = modifiers or graph.nodes[node]["modifiers"]
+    output = output or graph.nodes[node]["output"]
+    graph.set_node_object(
+        node, func=func, output=output, inputs=inputs, modifiers=modifiers
+    )
+
+    return graph
+
+
+def parse_parameters(parameters):
+    """Parse a list of parameters to signatures
+
+    :param list parameters: Parameters to parse. The element can either be a string
+        as the parameter name or a tuple/list as (parameter, default).
+    :return: parameter order and signature.
+    """
+
+    param_order = []  # parameters in the correct order
+    sig_list = []  # signature values
+    sig_df_list = []  # default values
+    defultargs = {}  # default arguments dictionary
+    for var in parameters:
+        if isinstance(var, tuple) or isinstance(var, list):
+            var_name, default_value = var
+            param_order.append(var_name)
+            sig_df_list.append(Parameter(var_name, 1, default=default_value))
+            defultargs[var_name] = default_value
+        else:
+            param_order.append(var)
+            sig_list.append(Parameter(var, 1))
+
+    sig = Signature(sig_list + sig_df_list)  # the default values are ordered next
+
+    return sig, param_order, defultargs
+
+
+def param_counter(graph, returns):
+    """Count the number of times a parameter is used for graph execution.
+
+    Count all function signature parameters. For extra returns,
+    add one to each count value.
+
+    :param list returns: method returns (include extra returns)
+    :return: dictionary with parameter_name: count pair
+    :rtype: dict
+    """
+
+    value_list = []
+    for sig in nx.get_node_attributes(graph, "sig").values():
+        for key, param in sig.parameters.items():
+
+            if param.default is param.empty:
+                value_list.append(key)
+
+    # add the additional parameter to list
+    value_list += returns
+
+    count = {}
+    for value in value_list:
+        count[value] = count.get(value, 0) + 1
+
+    return count
+
+
+def parse_input(signature, *args, **kwargs):
+    """parse argument based on signature and input.
+
+    The default value is automatically filled.
+    """
+
+    values = signature.bind(*args, **kwargs)
+    values.apply_defaults()
+    return values.arguments
+
+
+def is_node_attr_defined(graph, attr: str, attr_name: str = None):
+    """Check if all graph nodes have the attribute defined.
+
+    :param str attr: attribute string.
+    :param str attr_name: the detailed name of the attribute.
+
+    Raise an exception if the attribute is undefined.
+    """
+    attr_name = attr_name or attr
+
+    if graph.name:
+        graph_str = f"graph ({graph.name})"
+    else:
+        graph_str = "graph"
+
+    node_list = []
+    for node, node_attr in graph.nodes.data():
+        if attr not in node_attr:
+            node_list.append(node)
+
+    if node_list:
+        raise Exception(
+            f"invalid {graph_str}: {attr_name} "
+            f"{repr(attr)} is not defined for node(s) {node_list}."
+        )
+
+    return True
+
+
+def is_edge_attr_defined(graph, attr: str, attr_name: str = None):
+    """Check if all graph edges have the target attribute defined.
+
+    Raise an exception if the attribute is undefined.
+    """
+    attr_name = attr_name or attr
+
+    if graph.name:
+        graph_str = f"graph ({graph.name})"
+    else:
+        graph_str = "graph"
+
+    edge_list = []
+    for u, v, edge_attr in graph.edges.data():
+        if attr not in edge_attr:
+            edge_list.append((u, v))
+    if edge_list:
+        raise Exception(
+            f"invalid {graph_str}: {attr_name} {repr(attr)}"
+            f" is not defined for edge(s) {edge_list}."
+        )
+
+    return True
```

### Comparing `mmodel-0.5.2/PKG-INFO` & `mmodel-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: mmodel
-Version: 0.5.2
+Version: 0.6.0
 Summary: Modular modeling framework for scientific modeling and prototyping.
 Home-page: https://peterhs73.github.io/mmodel-docs/
 License: BSD-3-Clause
 Keywords: python,scientific-modeling,prototyping
 Author: Peter Sun
 Author-email: hs859@cornell.edu
 Maintainer: Peter Sun
 Maintainer-email: hs859@cornell.edu
 Requires-Python: >=3.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: test
 Requires-Dist: graphviz (>=0.16)
 Requires-Dist: h5py (>=3.6.0)
-Requires-Dist: nbsphinx (==0.9.1) ; extra == "docs"
+Requires-Dist: nbsphinx (==0.9.1); extra == "docs"
 Requires-Dist: networkx (>=2.8.3)
-Requires-Dist: pydata-sphinx-theme (==0.13.1) ; extra == "docs"
-Requires-Dist: pytest (>=7.1.1) ; extra == "test"
-Requires-Dist: pytest-cov (>=3.0.0) ; extra == "test"
-Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
-Requires-Dist: sphinx-book-theme (==1.0.0) ; extra == "docs"
+Requires-Dist: pydata-sphinx-theme (==0.13.1); extra == "docs"
+Requires-Dist: pytest (>=7.1.1); extra == "test"
+Requires-Dist: pytest-cov (>=3.0.0); extra == "test"
+Requires-Dist: sphinx (>=6.1.3,<7.0.0); extra == "docs"
+Requires-Dist: sphinx-book-theme (==1.0.0); extra == "docs"
 Requires-Dist: tox (>=3.24.5)
 Requires-Dist: tox-conda (>=0.9.2)
 Project-URL: Documentation, https://peterhs73.github.io/mmodel-docs/
 Project-URL: Repository, https://github.com/peterhs73/MModel
 Description-Content-Type: text/x-rst
 
 MModel
@@ -52,27 +51,28 @@
 ----------
 
 To create a nonlinear model that has the result of
 `(x + y)log(x + y, base)`:
 
 .. code-block:: python
 
-    from mmodel import ModelGraph, Model, MemHandler
     import math
     import numpy as np
 
     def func(sum_xy, log_xy):
         """Function that adds a value to the multiplied inputs."""
+
         return sum_xy * log_xy + 6
 
 The graph is defined using grouped edges (the ``networkx`` syntax of edge
 the definition also works.)
 
 .. code-block:: python
 
+    from mmodel import ModelGraph, Model, MemHandler
     # create graph edges
     grouped_edges = [
         ("add", ["log", "function node"]),
         ("log", "function node"),
     ]
 
 The functions are then added to node attributes. The order of definition
@@ -94,26 +94,26 @@
 
 To define the model, the name, graph, and handler need to be specified. Additional
 parameters include modifiers, descriptions, and returns lists. The input parameters
 of the model are determined based on the node information.
 
 .. code-block:: python
 
-    example_model = Model("example_model", G, handler=(MemHandler, {}), description="Test model.")
+    example_model = Model("example_model", G, handler=MemHandler, description="Test model.")
 
 The model behaves like a Python function, with additional metadata. The graph can
 be plotted using the ``draw`` method.
 
 .. code-block:: python
 
     >>> print(example_model)
     example_model(log_base, x, y)
     returns: z
     graph: example_graph
-    handler: MemHandler()
+    handler: MemHandler
 
     Test model.
 
     >>> example_model(2, 5, 3) # (5 + 3)log(5 + 3, 2) + 6
     30.0
 
     >>> example_model.draw()
@@ -128,55 +128,54 @@
 ..   :width: 300
 ..   :alt: example model graph
 
 One key feature of ``mmodel`` that differs from other workflow is modifiers, 
 which modify callables post definition. Modifiers work on both the node level
 and model level.
 
-Example: Use ``loop_modifier`` on the graph to loop the nodes that require the
+Example: Use ``loop_input`` modifier on the graph to loop the nodes that require the
 "log_base" parameter.
 
 .. code-block:: python 
 
-    from mmodel import loop_modifier
+    from mmodel import loop_input
 
     H = G.subgraph(inputs=["log_base"])
     H.name = "example_subgraph"
-    loop_node = Model("submodel", H, handler=(MemHandler, {}))
+    loop_node = Model("submodel", H, handler=MemHandler)
 
     looped_G = G.replace_subgraph(
         H,
         "loop_node",
         loop_node,
         output="looped_z",
-        modifiers=[(loop_modifier, {"parameter": "log_base"})],
+        modifiers=[loop_input("log_base")],
     )
     looped_G.name = "looped_graph"
 
     looped_model = Model("looped_model", looped_G, loop_node.handler)
 
 
 We can inspect the loop node as well as the new model.
 
 .. code-block:: python 
 
-    >>> print(loop_node)
-    loop_submodel(log_base, sum_xy)
-    returns: z
-    graph: example_subgraph
-    handler: MemHandler()
-    modifiers:
-      - loop_modifier('log_base')
-
     >>> print(looped_model)
     looped_model(log_base, x, y)
     returns: looped_z
     graph: looped_graph
     handler: MemHandler()
     
+    >>> print(looped_model.node_metadata("loop_node"))
+    submodel(log_base, sum_xy)
+    return: looped_z
+    functype: mmodel.Model
+    modifiers:
+      - loop_input('log_base')
+
     >>> looped_model([2, 4], 5, 3) # (5 + 3)log(5 + 3, 2) + 6
     [30.0, 18.0]
 
 
 Use the ``draw`` method to draw the graph. There are three styles
 "plain", "short", and "verbose", which differ by the level of detail of the
 node information. A graph output is displayed in Jupyter Notebook
```

