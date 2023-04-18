# Comparing `tmp/flask-htmx-0.2.0.tar.gz` & `tmp/flask_htmx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-htmx-0.2.0.tar", max compression
+gzip compressed data, was "flask_htmx-0.3.0.tar", max compression
```

## Comparing `flask-htmx-0.2.0.tar` & `flask_htmx-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2022-03-09 07:34:22.895630 flask-htmx-0.2.0/LICENSE
--rw-r--r--   0        0        0     3636 2022-03-09 07:34:22.895630 flask-htmx-0.2.0/README.rst
--rw-r--r--   0        0        0       23 2022-03-09 07:34:22.899629 flask-htmx-0.2.0/flask_htmx/__init__.py
--rw-r--r--   0        0        0     2662 2022-03-09 07:34:22.899629 flask-htmx-0.2.0/flask_htmx/htmx.py
--rw-r--r--   0        0        0     1018 2022-03-09 07:34:22.899629 flask-htmx-0.2.0/flask_htmx/responses.py
--rw-r--r--   0        0        0     1268 2022-03-09 07:35:17.340573 flask-htmx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4439 2022-03-09 07:35:18.122143 flask-htmx-0.2.0/setup.py
--rw-r--r--   0        0        0     4788 2022-03-09 07:35:18.122476 flask-htmx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4648 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/README.rst
+-rw-r--r--   0        0        0      108 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/constants.py
+-rw-r--r--   0        0        0     2680 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/htmx.py
+-rw-r--r--   0        0        0     4767 2023-04-18 10:24:38.347851 flask_htmx-0.3.0/flask_htmx/responses.py
+-rw-r--r--   0        0        0     1430 2023-04-18 10:25:16.752200 flask_htmx-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5851 1970-01-01 00:00:00.000000 flask_htmx-0.3.0/PKG-INFO
```

### Comparing `flask-htmx-0.2.0/LICENSE` & `flask_htmx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-htmx-0.2.0/flask_htmx/htmx.py` & `flask_htmx-0.3.0/flask_htmx/htmx.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,31 +23,33 @@
 
     def init_app(self, app: Flask):
         """Initialise the extension with the Flask app object."""
         app.htmx = self
 
     @property
     def boosted(self) -> bool:
-        """:py:obj:`True` if the request came from an element with the `hx-boost` attribute.
+        """:py:obj:`True` if the request came from an element with the `hx-boost`
+        attribute.
 
         Based on the :code:`HX-Boosted` header.
         """
-        return request.headers.get("HX-Boost") == "true"
+        return request.headers.get("HX-Boosted") == "true"
 
     @property
     def current_url(self) -> Optional[str]:
         """The current URL of the browser, or :py:obj:`None` for non-HTMX requests.
 
         Based on the :code:`HX-Current-URL` header.
         """
         return request.headers.get("HX-Current-URL")
 
     @property
     def history_restore_request(self) -> bool:
-        """:py:obj:`True` if the request is for history restoration after a miss in the local history cache.
+        """:py:obj:`True` if the request is for history restoration after a miss in the
+        local history cache.
 
         Based on the :code:`HX-History-Restore-Request` header.
         """
         return request.headers.get("HX-History-Restore-Request") == "true"
 
     @property
     def prompt(self) -> Optional[str]:
```

### Comparing `flask-htmx-0.2.0/pyproject.toml` & `flask_htmx-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flask-htmx"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Flask extension to work with HTMX."
 authors = ["Edmond Chuc <edmond.chuc@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/edmondchuc/flask-htmx"
 repository = "https://github.com/edmondchuc/flask-htmx"
 documentation = "https://flask-htmx.readthedocs.io"
@@ -24,22 +24,32 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
-black = "^21.12b0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.6.1"
 Sphinx = "^4.4.0"
 furo = "^2022.1.2"
 sphinx-autobuild = "^2021.3.14"
 sphinx-copybutton = "^0.4.0"
+pre-commit = ">=2.20.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/edmondchuc/flask-htmx/issues"
+"Bug Tracker" = "https://github.com/edmondchuc/flask-htmx/issues"
+
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+line_length = 88
+
+[tool.black]
+line_length = 88
```

### Comparing `flask-htmx-0.2.0/PKG-INFO` & `flask_htmx-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: flask-htmx
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Flask extension to work with HTMX.
 Home-page: https://github.com/edmondchuc/flask-htmx
 License: MIT
 Keywords: Flask,HTMX,Python,Web
 Author: Edmond Chuc
 Author-email: edmond.chuc@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2.0.2,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/edmondchuc/flask-htmx/issues
 Project-URL: Documentation, https://flask-htmx.readthedocs.io
 Project-URL: Repository, https://github.com/edmondchuc/flask-htmx
 Description-Content-Type: text/x-rst
@@ -44,15 +45,15 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 .. image:: https://img.shields.io/badge/License-MIT-red.svg
     :target: https://github.com/edmondchuc/flask-htmx/blob/main/LICENSE
 
-.. image:: https://static.pepy.tech/personalized-badge/flask-htmx?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week
+.. image:: https://static.pepy.tech/personalized-badge/flask-htmx?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week
     :target: https://pepy.tech/project/flask-htmx
 
 .. image:: https://static.pepy.tech/personalized-badge/flask-htmx?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/flask-htmx
 
 .. image:: https://static.pepy.tech/personalized-badge/flask-htmx?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads
     :target: https://pepy.tech/project/flask-htmx
@@ -74,14 +75,17 @@
 
 Or perhaps you use Poetry.
 
 .. code-block:: bash
 
     poetry add flask-htmx
 
+HTMX Request
+------------
+
 You can register the HTMX object by passing the Flask
 :code:`app` object via the constructor.
 
 .. code-block:: python
 
     htmx = HTMX(app)
 
@@ -128,19 +132,58 @@
     def home():
         current_url = htmx.current_url
         return render_template("index.html", current_url=current_url)
 
 Other HTMX request headers are also available.
 See https://htmx.org/reference/#request_headers.
 
-Continue to the next section of the docs,
-`The HTMX Class <https://flask-htmx.readthedocs.io/en/latest/flask_htmx.htmx.html>`_.
+HTMX Response
+-------------
+
+You might be interested on adding
+`htmx response headers <https://htmx.org/reference/#response_headers>`_ to your response.
+Use :code:`flask_htmx.make_response` for that. For example, instead of:
+
+.. code-block:: python
+
+    import json
+    from flask import make_response
+    from my_app import app
+
+    @app.route("/hola-mundo")
+    def hola_mundo():
+        body = "Hola Mundo!"
+        response = make_response(body)
+        response.headers["HX-Push-URL"] = "false"
+        trigger_string = json.dumps({"event1":"A message", "event2":"Another message"})
+        response.headers["HX-Trigger"] = trigger_string
+        return response
+
+You can do:
+
+.. code-block:: python
+
+    from flask_htmx import make_response
+    from my_app import app
+
+    @app.route("/hola-mundo")
+    def hola_mundo():
+        body = "Hola Mundo!"
+        return make_response(
+            body,
+            push_url=False,
+            trigger={"event1": "A message", "event2": "Another message"},
+        )
 
 .. quickstart-endblock
 
+Documentation
+=============
+Visit the `full documentation <https://flask-htmx.readthedocs.io>`_.
+
 Development
 ===========
 
 Installation
 ------------
 
 .. code-block:: bash
```

