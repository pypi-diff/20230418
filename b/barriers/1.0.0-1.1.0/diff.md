# Comparing `tmp/barriers-1.0.0.tar.gz` & `tmp/barriers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barriers-1.0.0.tar", last modified: Sat Sep  3 04:30:04 2022, max compression
+gzip compressed data, was "barriers-1.1.0.tar", last modified: Tue Apr 18 05:36:15 2023, max compression
```

## Comparing `barriers-1.0.0.tar` & `barriers-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-03 04:30:04.197549 barriers-1.0.0/
--rw-rw-rw-   0        0        0     1087 2022-08-17 18:40:24.000000 barriers-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     8686 2022-09-03 04:30:04.197296 barriers-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8078 2022-09-03 04:28:00.000000 barriers-1.0.0/README.rst
--rw-rw-rw-   0        0        0     1045 2022-08-31 04:45:16.000000 barriers-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-03 04:30:04.197651 barriers-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-03 04:30:04.183971 barriers-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-09-03 04:30:04.187638 barriers-1.0.0/src/barriers/
--rw-rw-rw-   0        0        0       98 2022-08-17 18:45:16.000000 barriers-1.0.0/src/barriers/__init__.py
--rw-rw-rw-   0        0        0    20772 2022-08-31 05:09:45.000000 barriers-1.0.0/src/barriers/barriers.py
-drwxrwxrwx   0        0        0        0 2022-09-03 04:30:04.196155 barriers-1.0.0/src/barriers.egg-info/
--rw-rw-rw-   0        0        0     8686 2022-09-03 04:30:03.000000 barriers-1.0.0/src/barriers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-09-03 04:30:04.000000 barriers-1.0.0/src/barriers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-03 04:30:03.000000 barriers-1.0.0/src/barriers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-09-03 04:30:04.000000 barriers-1.0.0/src/barriers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-03 04:30:04.000000 barriers-1.0.0/src/barriers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:15.749079 barriers-1.1.0/
+-rw-rw-rw-   0        0        0     1087 2022-08-17 18:40:24.000000 barriers-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9615 2023-04-18 05:36:15.749079 barriers-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9007 2023-04-18 05:22:05.000000 barriers-1.1.0/README.rst
+-rw-rw-rw-   0        0        0     1046 2023-04-18 04:41:54.000000 barriers-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:36:15.749079 barriers-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:15.737307 barriers-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:15.739310 barriers-1.1.0/src/barriers/
+-rw-rw-rw-   0        0        0       98 2022-08-17 18:45:16.000000 barriers-1.1.0/src/barriers/__init__.py
+-rw-rw-rw-   0        0        0    20964 2023-04-18 04:47:06.000000 barriers-1.1.0/src/barriers/barriers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:15.747741 barriers-1.1.0/src/barriers.egg-info/
+-rw-rw-rw-   0        0        0     9615 2023-04-18 05:36:15.000000 barriers-1.1.0/src/barriers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-18 05:36:15.000000 barriers-1.1.0/src/barriers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:36:15.000000 barriers-1.1.0/src/barriers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-04-18 05:36:15.000000 barriers-1.1.0/src/barriers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 05:36:15.000000 barriers-1.1.0/src/barriers.egg-info/top_level.txt
```

### Comparing `barriers-1.0.0/LICENSE` & `barriers-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barriers-1.0.0/PKG-INFO` & `barriers-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barriers
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python decorators for including/excluding type checks, value/bounds checks, and other code blocks within the compiled bytecode of functions and methods.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/reity/barriers
 Project-URL: Documentation, https://barriers.readthedocs.io
 Requires-Python: >=3.7
@@ -38,155 +38,207 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/reity/barriers/badge.svg?branch=main
    :target: https://coveralls.io/github/reity/barriers?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__:
+
+.. code-block:: bash
 
     python -m pip install barriers
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import barriers
     from barriers import barriers
 
 Examples
 ^^^^^^^^
 
 .. |barriers| replace:: ``barriers``
-.. _barriers: https://barriers.readthedocs.io/en/1.0.0/_source/barriers.html#barriers.barriers.barriers
+.. _barriers: https://barriers.readthedocs.io/en/1.1.0/_source/barriers.html#barriers.barriers.barriers
 
 .. |globals| replace:: ``globals``
 .. _globals: https://docs.python.org/3/library/functions.html#globals
 
-Consider the function below. The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer::
+Consider the function below (defined within a file ``f.py``). The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer:
+
+.. code-block:: python
+
+    def f(x: int, y: int) -> int:
+
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
+
+We can import the module above and invoke the function to observe its behavior:
+
+.. code-block:: python
 
-    >>> def f(x: int, y: int) -> int:
-    ...
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     Traceback (most recent call last):
       ...
     ValueError: inputs must be nonnegative
 
-An instance of the |barriers|_ class should normally be introduced near the top of a Python module::
+An instance of the |barriers|_ class should normally be introduced near the top of a Python module using a pair of statements such as those below:
 
+.. code-block:: python
+
+    >>> from barriers import barriers
     >>> example = barriers(False) @ globals() # Remove marked code blocks (i.e., "disable barriers").
 
 The |barriers|_ instance ``example`` defined above is a decorator that transforms any decorated function by removing any designated code blocks in the body of that function.
 
 * The ``False`` argument in the expression ``barriers(False)`` above should be interpreted to mean that **this barrier is disabled** (*i.e.*, that the marked code blocks in the bodies of functions decorated by this decorator **should be removed**). The default value for this optional argument is ``True``; this should be interpreted to mean that **this barrier is enabled** (and, thus, that marked code blocks **should not be removed** from decorated functions).
 
 * The notation ``@ globals()`` ensures that the namespace returned by |globals|_ is used when compiling the abstract syntax trees of transformed functions.
 
-A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``::
+Consider the modified version of ``f.py`` below. A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``:
+
+.. code-block:: python
+
+    from barriers import barriers
+    example = barriers(False) @ globals()
+
+    @example
+    def f(x: int, y: int) -> int:
+
+        example
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
 
-    >>> @example
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     example
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
+The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs:
 
-The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs::
+.. code-block:: python
 
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     -3
 
-It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance)::
+It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance):
+
+.. code-block:: python
 
     >>> from barriers import barriers
     >>> checks = barriers(types=True, bounds=False) @ globals()
 
-Given the above definitions, it is now possible to introduce named markers such as those in the example below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**::
+Given the above definitions, it is possible to introduce named markers such as those in the variant of ``f.py`` presented below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**:
+
+.. code-block:: python
+
+    from barriers import barriers
+    checks = barriers(types=True, bounds=False) @ globals()
+
+    @checks
+    def f(x: int, y: int) -> int:
+    
+        checks.types
+        if not isinstance(x, int) and not isinstance(y, int):
+            raise TypeError('inputs must be integers')
+    
+        checks.bounds
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+    
+        return x + y
+
+The described behavior can be observed when evaluating the function:
 
-    >>> @checks
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     checks.types
-    ...     if not isinstance(x, int) and not isinstance(y, int):
-    ...         raise TypeError('inputs must be integers')
-    ...
-    ...     checks.bounds
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+.. code-block:: python
+
+    >>> from f import f
     >>> f('a', 'b')
     Traceback (most recent call last):
       ...
     TypeError: inputs must be integers
     >>> f(-1, -2)
     -3
 
-Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.0.0>`__.
+Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.1.0>`__.
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/barriers/barriers.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/barriers
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/barriers>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `barriers-1.0.0/README.rst` & `barriers-1.1.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -20,155 +20,207 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/reity/barriers/badge.svg?branch=main
    :target: https://coveralls.io/github/reity/barriers?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__:
+
+.. code-block:: bash
 
     python -m pip install barriers
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import barriers
     from barriers import barriers
 
 Examples
 ^^^^^^^^
 
 .. |barriers| replace:: ``barriers``
-.. _barriers: https://barriers.readthedocs.io/en/1.0.0/_source/barriers.html#barriers.barriers.barriers
+.. _barriers: https://barriers.readthedocs.io/en/1.1.0/_source/barriers.html#barriers.barriers.barriers
 
 .. |globals| replace:: ``globals``
 .. _globals: https://docs.python.org/3/library/functions.html#globals
 
-Consider the function below. The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer::
+Consider the function below (defined within a file ``f.py``). The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer:
+
+.. code-block:: python
+
+    def f(x: int, y: int) -> int:
+
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
+
+We can import the module above and invoke the function to observe its behavior:
+
+.. code-block:: python
 
-    >>> def f(x: int, y: int) -> int:
-    ...
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     Traceback (most recent call last):
       ...
     ValueError: inputs must be nonnegative
 
-An instance of the |barriers|_ class should normally be introduced near the top of a Python module::
+An instance of the |barriers|_ class should normally be introduced near the top of a Python module using a pair of statements such as those below:
 
+.. code-block:: python
+
+    >>> from barriers import barriers
     >>> example = barriers(False) @ globals() # Remove marked code blocks (i.e., "disable barriers").
 
 The |barriers|_ instance ``example`` defined above is a decorator that transforms any decorated function by removing any designated code blocks in the body of that function.
 
 * The ``False`` argument in the expression ``barriers(False)`` above should be interpreted to mean that **this barrier is disabled** (*i.e.*, that the marked code blocks in the bodies of functions decorated by this decorator **should be removed**). The default value for this optional argument is ``True``; this should be interpreted to mean that **this barrier is enabled** (and, thus, that marked code blocks **should not be removed** from decorated functions).
 
 * The notation ``@ globals()`` ensures that the namespace returned by |globals|_ is used when compiling the abstract syntax trees of transformed functions.
 
-A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``::
+Consider the modified version of ``f.py`` below. A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``:
+
+.. code-block:: python
+
+    from barriers import barriers
+    example = barriers(False) @ globals()
+
+    @example
+    def f(x: int, y: int) -> int:
+
+        example
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
 
-    >>> @example
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     example
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
+The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs:
 
-The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs::
+.. code-block:: python
 
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     -3
 
-It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance)::
+It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance):
+
+.. code-block:: python
 
     >>> from barriers import barriers
     >>> checks = barriers(types=True, bounds=False) @ globals()
 
-Given the above definitions, it is now possible to introduce named markers such as those in the example below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**::
+Given the above definitions, it is possible to introduce named markers such as those in the variant of ``f.py`` presented below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**:
+
+.. code-block:: python
+
+    from barriers import barriers
+    checks = barriers(types=True, bounds=False) @ globals()
+
+    @checks
+    def f(x: int, y: int) -> int:
+    
+        checks.types
+        if not isinstance(x, int) and not isinstance(y, int):
+            raise TypeError('inputs must be integers')
+    
+        checks.bounds
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+    
+        return x + y
+
+The described behavior can be observed when evaluating the function:
 
-    >>> @checks
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     checks.types
-    ...     if not isinstance(x, int) and not isinstance(y, int):
-    ...         raise TypeError('inputs must be integers')
-    ...
-    ...     checks.bounds
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+.. code-block:: python
+
+    >>> from f import f
     >>> f('a', 'b')
     Traceback (most recent call last):
       ...
     TypeError: inputs must be integers
     >>> f(-1, -2)
     -3
 
-Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.0.0>`__.
+Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.1.0>`__.
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/barriers/barriers.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/barriers
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/barriers>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `barriers-1.0.0/pyproject.toml` & `barriers-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "barriers"
-version = "1.0.0"
+version = "1.1.0"
 description = """\
     Python decorators for including/excluding type checks, \
     value/bounds checks, and other code blocks within the \
     compiled bytecode of functions and methods.\
     """
 license = {text = "MIT"}
 authors = [
@@ -21,29 +21,29 @@
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=barriers --cov-report term-missing"
```

### Comparing `barriers-1.0.0/src/barriers/barriers.py` & `barriers-1.1.0/src/barriers/barriers.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,18 @@
                 return function
 
             # Store unmodified function as an attribute of the transformed
             # function. The transformed function will be returned by the
             # last statement in this method (as is the default behavior).
             setattr(namespace[function.__name__], self._attribute[1], function)
 
-        return namespace[function.__name__]
+        result = namespace[function.__name__]
+        result.__name__ = function.__name__ # Preserve original function's name.
+        result.__doc__ = function.__doc__ # Preserve original function's docstring.
+        return result
 
     def __call__(self: barriers, function: Callable) -> Callable:
         """
         Allows this instance to behave as a decorator that parses a function
         and removes any marked code blocks (as specified within this instance).
 
         >>> from barriers import barriers
```

### Comparing `barriers-1.0.0/src/barriers.egg-info/PKG-INFO` & `barriers-1.1.0/src/barriers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barriers
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python decorators for including/excluding type checks, value/bounds checks, and other code blocks within the compiled bytecode of functions and methods.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/reity/barriers
 Project-URL: Documentation, https://barriers.readthedocs.io
 Requires-Python: >=3.7
@@ -38,155 +38,207 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/reity/barriers/badge.svg?branch=main
    :target: https://coveralls.io/github/reity/barriers?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/barriers>`__:
+
+.. code-block:: bash
 
     python -m pip install barriers
 
-The library can be imported in the usual ways::
+The library can be imported in the usual ways:
+
+.. code-block:: python
 
     import barriers
     from barriers import barriers
 
 Examples
 ^^^^^^^^
 
 .. |barriers| replace:: ``barriers``
-.. _barriers: https://barriers.readthedocs.io/en/1.0.0/_source/barriers.html#barriers.barriers.barriers
+.. _barriers: https://barriers.readthedocs.io/en/1.1.0/_source/barriers.html#barriers.barriers.barriers
 
 .. |globals| replace:: ``globals``
 .. _globals: https://docs.python.org/3/library/functions.html#globals
 
-Consider the function below. The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer::
+Consider the function below (defined within a file ``f.py``). The body of this function contains a code block that raises an exception if either of the two inputs is a negative integer:
+
+.. code-block:: python
+
+    def f(x: int, y: int) -> int:
+
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
+
+We can import the module above and invoke the function to observe its behavior:
+
+.. code-block:: python
 
-    >>> def f(x: int, y: int) -> int:
-    ...
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     Traceback (most recent call last):
       ...
     ValueError: inputs must be nonnegative
 
-An instance of the |barriers|_ class should normally be introduced near the top of a Python module::
+An instance of the |barriers|_ class should normally be introduced near the top of a Python module using a pair of statements such as those below:
 
+.. code-block:: python
+
+    >>> from barriers import barriers
     >>> example = barriers(False) @ globals() # Remove marked code blocks (i.e., "disable barriers").
 
 The |barriers|_ instance ``example`` defined above is a decorator that transforms any decorated function by removing any designated code blocks in the body of that function.
 
 * The ``False`` argument in the expression ``barriers(False)`` above should be interpreted to mean that **this barrier is disabled** (*i.e.*, that the marked code blocks in the bodies of functions decorated by this decorator **should be removed**). The default value for this optional argument is ``True``; this should be interpreted to mean that **this barrier is enabled** (and, thus, that marked code blocks **should not be removed** from decorated functions).
 
 * The notation ``@ globals()`` ensures that the namespace returned by |globals|_ is used when compiling the abstract syntax trees of transformed functions.
 
-A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``::
+Consider the modified version of ``f.py`` below. A statement can be designated for automatic removal by placing a marker -- in this case, the ``example`` variable -- on the line directly above that statement. Note that in the body of the function ``f`` defined below, the ``if`` block is immediately preceded by a line that contains the variable ``example``:
+
+.. code-block:: python
+
+    from barriers import barriers
+    example = barriers(False) @ globals()
+
+    @example
+    def f(x: int, y: int) -> int:
+
+        example
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+
+        return x + y
 
-    >>> @example
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     example
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
+The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs:
 
-The decorator ``@example`` automatically removes the ``if`` block in the function above. As a result, the function does not raise an exception when it is applied to negative inputs::
+.. code-block:: python
 
+    >>> from f import f
     >>> f(1, 2)
     3
     >>> f(-1, -2)
     -3
 
-It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance)::
+It is also possible to define and use individually named markers (which are created as attributes of the |barriers|_ instance):
+
+.. code-block:: python
 
     >>> from barriers import barriers
     >>> checks = barriers(types=True, bounds=False) @ globals()
 
-Given the above definitions, it is now possible to introduce named markers such as those in the example below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**::
+Given the above definitions, it is possible to introduce named markers such as those in the variant of ``f.py`` presented below. When a marker definition has been assigned ``True``, the statements immediately below that named marker **are not removed** (*i.e.*, the marked barrier statements are enabled). When a marker definition has been assigned ``False``, the corresponding marked statements **are removed**:
+
+.. code-block:: python
+
+    from barriers import barriers
+    checks = barriers(types=True, bounds=False) @ globals()
+
+    @checks
+    def f(x: int, y: int) -> int:
+    
+        checks.types
+        if not isinstance(x, int) and not isinstance(y, int):
+            raise TypeError('inputs must be integers')
+    
+        checks.bounds
+        if x < 0 or y < 0:
+            raise ValueError('inputs must be nonnegative')
+    
+        return x + y
+
+The described behavior can be observed when evaluating the function:
 
-    >>> @checks
-    ... def f(x: int, y: int) -> int:
-    ...
-    ...     checks.types
-    ...     if not isinstance(x, int) and not isinstance(y, int):
-    ...         raise TypeError('inputs must be integers')
-    ...
-    ...     checks.bounds
-    ...     if x < 0 or y < 0:
-    ...         raise ValueError('inputs must be nonnegative')
-    ...
-    ...     return x + y
-    ...
+.. code-block:: python
+
+    >>> from f import f
     >>> f('a', 'b')
     Traceback (most recent call last):
       ...
     TypeError: inputs must be integers
     >>> f(-1, -2)
     -3
 
-Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.0.0>`__.
+Many additional details and examples are presented in the `documentation <https://barriers.readthedocs.io/en/1.1.0>`__.
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/barriers/barriers.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/barriers
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/barriers>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 The version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/barriers>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

