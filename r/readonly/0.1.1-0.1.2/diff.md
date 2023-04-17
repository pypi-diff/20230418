# Comparing `tmp/readonly-0.1.1.tar.gz` & `tmp/readonly-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readonly-0.1.1.tar", max compression
+gzip compressed data, was "readonly-0.1.2.tar", max compression
```

## Comparing `readonly-0.1.1.tar` & `readonly-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1614 2023-04-17 21:40:45.487797 readonly-0.1.1/LICENSE
--rw-r--r--   0        0        0     4222 2023-04-17 22:17:01.092830 readonly-0.1.1/README.rst
--rw-r--r--   0        0        0     1101 2023-04-17 22:17:22.477102 readonly-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      195 2023-04-17 22:17:27.353163 readonly-0.1.1/readonly/__init__.py
--rw-r--r--   0        0        0      588 2023-04-17 21:52:10.872217 readonly-0.1.1/readonly/readonly.py
--rw-r--r--   0        0        0     5015 1970-01-01 00:00:00.000000 readonly-0.1.1/setup.py
--rw-r--r--   0        0        0     5156 1970-01-01 00:00:00.000000 readonly-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1614 2023-04-17 21:40:45.487797 readonly-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4215 2023-04-17 22:24:18.613751 readonly-0.1.2/README.rst
+-rw-r--r--   0        0        0     1101 2023-04-17 22:24:47.698042 readonly-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      195 2023-04-17 22:24:53.446099 readonly-0.1.2/readonly/__init__.py
+-rw-r--r--   0        0        0      588 2023-04-17 21:52:10.872217 readonly-0.1.2/readonly/readonly.py
+-rw-r--r--   0        0        0     5007 1970-01-01 00:00:00.000000 readonly-0.1.2/setup.py
+-rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 readonly-0.1.2/PKG-INFO
```

### Comparing `readonly-0.1.1/LICENSE` & `readonly-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readonly-0.1.1/README.rst` & `readonly-0.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,15 @@
    :target: https://github.com/wiseaidev/readonly/
    :alt: Repo Size
 
 .. image:: https://circleci.com/gh/wiseaidev/readonly/tree/main.svg?style=svg
    :target: https://circleci.com/gh/wiseaidev/readonly/tree/main
    :alt: Circle ci Build Status
 
-**readonly** is a python package that acts as an alternative to frozenset, but for dictionaries.
-
+**readonly** is a simple package to make any given module attributes into read only mode. 
 
 🛠️ Requirements
 ---------------
 
 **readonly** requires Python 3.9 or above.
 
 To install Python 3.9, I recommend using `pyenv`_.
```

### Comparing `readonly-0.1.1/pyproject.toml` & `readonly-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readonly"
-version = "0.1.1"
+version = "0.1.2"
 description = "Make any module attributes read only."
 authors = [
     "Mahmoud Harmouch <business@wiseai.dev>"
 ]
 license = "GNU General Public License v3.0"
 readme = "README.rst"
 repository = "https://github.com/wiseaidev/readonly"
```

### Comparing `readonly-0.1.1/readonly/readonly.py` & `readonly-0.1.2/readonly/readonly.py`

 * *Files identical despite different names*

### Comparing `readonly-0.1.1/setup.py` & `readonly-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['readonly']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'readonly',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Make any module attributes read only.',
-    'long_description': '=========\nreadonly\n=========\n\n.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg\n   :target: https://github.com/wiseaidev/readonly/blob/main/LICENSE\n   :alt: License\n\n.. image:: https://img.shields.io/pypi/v/readonly.svg\n   :target: https://pypi.org/project/readonly/\n   :alt: pypi version\n\n.. image:: https://img.shields.io/github/repo-size/wiseaidev/readonly\n   :target: https://github.com/wiseaidev/readonly/\n   :alt: Repo Size\n\n.. image:: https://circleci.com/gh/wiseaidev/readonly/tree/main.svg?style=svg\n   :target: https://circleci.com/gh/wiseaidev/readonly/tree/main\n   :alt: Circle ci Build Status\n\n**readonly** is a python package that acts as an alternative to frozenset, but for dictionaries.\n\n\n🛠️ Requirements\n---------------\n\n**readonly** requires Python 3.9 or above.\n\nTo install Python 3.9, I recommend using `pyenv`_.\n\n.. code-block:: bash\n\n   # install pyenv\n   git clone https://github.com/pyenv/pyenv ~/.pyenv\n\n   # setup pyenv (you should also put these three lines in .bashrc or similar)\n   # if you are using zsh\n   cat << EOF >> ~/.zshrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n\n   # or if you using the default bash shell, do this instead:\n   cat << EOF >> ~/.bashrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n   # Close and open a new shell session\n   # install Python 3.9.10\n   pyenv install 3.9.10\n\n   # make it available globally\n   pyenv global system 3.9.10\n\n\nTo manage the Python 3.9 virtualenv, I recommend using `poetry`_.\n\n.. code-block:: bash\n\n   # install poetry\n   curl -sSL https://install.python-poetry.org | python3 -\n   poetry --version\n   Poetry version 1.1.13\n\n   # Having the python executable in your PATH, you can use it:\n   poetry env use 3.9.10\n\n   # However, you are most likely to get the following issue:\n   Creating virtualenv readonly-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs\n\n   ModuleNotFoundError\n\n   No module named \'virtualenv.seed.via_app_data\'\n\n   at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked\n\n   # To resolve it, you need to reinstall virtualenv through pip\n   sudo apt remove --purge python3-virtualenv virtualenv\n   python3 -m pip install -U virtualenv\n\n   # Now, you can just use the minor Python version in this case:\n   poetry env use 3.9.10\n   Using virtualenv: ~/.cache/pypoetry/virtualenvs/readonly-dxc671ba-py3.9\n\n\n🚨 Installation\n---------------\n\nWith :code:`pip`:\n\n.. code-block:: console\n\n   python3.9 -m pip install readonly\n\n\n🚸 Usage\n--------\n\n.. code-block:: python3\n\n   >>> from readonly import readonly\n   >>> import math\n   >>> math = readonly(math)\n\n   # raises AttributeError\n   >>> math.pi = 3.0\n\n🎉 Credits\n----------\n\nThe following projects were used to build and test :code:`readonly`.\n\n- `python`_\n- `poetry`_\n- `pytest`_\n- `flake8`_\n- `coverage`_\n- `rstcheck`_\n- `mypy`_\n- `pytestcov`_\n- `tox`_\n- `isort`_\n- `black`_\n- `precommit`_\n\n\n👋 Contribute\n-------------\n\nIf you are looking for a way to contribute to the project, please refer to the `Guideline`_.\n\n📝 License\n----------\n\nThis program and the accompanying materials are made available under the terms and conditions of the `GNU GENERAL PUBLIC LICENSE`_.\n\n.. _GNU GENERAL PUBLIC LICENSE: http://www.gnu.org/licenses/\n.. _readonly: https://pypi.org/project/readonly/\n.. _Marco Sulla: https://github.com/Marco-Sulla\n.. _Guideline: https://github.com/wiseaidev/readonly/blob/main/CONTRIBUTING.rst\n.. _pyenv: https://github.com/pyenv/pyenv\n.. _poetry: https://github.com/python-poetry/poetry\n.. _pipx: https://github.com/pypa/pipx\n.. _python: https://www.python.org/\n.. _pytest: https://docs.pytest.org/en/7.1.x/\n.. _flake8: https://flake8.pycqa.org/en/latest/\n.. _coverage: https://coverage.readthedocs.io/en/6.3.2/\n.. _rstcheck: https://pypi.org/project/rstcheck/\n.. _mypy: https://mypy.readthedocs.io/en/stable/\n.. _pytestcov: https://pytest-cov.readthedocs.io/en/latest/\n.. _tox: https://tox.wiki/en/latest/\n.. _isort: https://github.com/PyCQA/isort\n.. _black: https://black.readthedocs.io/en/stable/\n.. _precommit: https://pre-commit.com/\n',
+    'long_description': '=========\nreadonly\n=========\n\n.. image:: https://img.shields.io/badge/License-GPLv3-blue.svg\n   :target: https://github.com/wiseaidev/readonly/blob/main/LICENSE\n   :alt: License\n\n.. image:: https://img.shields.io/pypi/v/readonly.svg\n   :target: https://pypi.org/project/readonly/\n   :alt: pypi version\n\n.. image:: https://img.shields.io/github/repo-size/wiseaidev/readonly\n   :target: https://github.com/wiseaidev/readonly/\n   :alt: Repo Size\n\n.. image:: https://circleci.com/gh/wiseaidev/readonly/tree/main.svg?style=svg\n   :target: https://circleci.com/gh/wiseaidev/readonly/tree/main\n   :alt: Circle ci Build Status\n\n**readonly** is a simple package to make any given module attributes into read only mode. \n\n🛠️ Requirements\n---------------\n\n**readonly** requires Python 3.9 or above.\n\nTo install Python 3.9, I recommend using `pyenv`_.\n\n.. code-block:: bash\n\n   # install pyenv\n   git clone https://github.com/pyenv/pyenv ~/.pyenv\n\n   # setup pyenv (you should also put these three lines in .bashrc or similar)\n   # if you are using zsh\n   cat << EOF >> ~/.zshrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n\n   # or if you using the default bash shell, do this instead:\n   cat << EOF >> ~/.bashrc\n   # pyenv config\n   export PATH="${HOME}/.pyenv/bin:${PATH}"\n   export PYENV_ROOT="${HOME}/.pyenv"\n   eval "$(pyenv init -)"\n   EOF\n   # Close and open a new shell session\n   # install Python 3.9.10\n   pyenv install 3.9.10\n\n   # make it available globally\n   pyenv global system 3.9.10\n\n\nTo manage the Python 3.9 virtualenv, I recommend using `poetry`_.\n\n.. code-block:: bash\n\n   # install poetry\n   curl -sSL https://install.python-poetry.org | python3 -\n   poetry --version\n   Poetry version 1.1.13\n\n   # Having the python executable in your PATH, you can use it:\n   poetry env use 3.9.10\n\n   # However, you are most likely to get the following issue:\n   Creating virtualenv readonly-dxc671ba-py3.9 in ~/.cache/pypoetry/virtualenvs\n\n   ModuleNotFoundError\n\n   No module named \'virtualenv.seed.via_app_data\'\n\n   at <frozen importlib._bootstrap>:973 in _find_and_load_unlocked\n\n   # To resolve it, you need to reinstall virtualenv through pip\n   sudo apt remove --purge python3-virtualenv virtualenv\n   python3 -m pip install -U virtualenv\n\n   # Now, you can just use the minor Python version in this case:\n   poetry env use 3.9.10\n   Using virtualenv: ~/.cache/pypoetry/virtualenvs/readonly-dxc671ba-py3.9\n\n\n🚨 Installation\n---------------\n\nWith :code:`pip`:\n\n.. code-block:: console\n\n   python3.9 -m pip install readonly\n\n\n🚸 Usage\n--------\n\n.. code-block:: python3\n\n   >>> from readonly import readonly\n   >>> import math\n   >>> math = readonly(math)\n\n   # raises AttributeError\n   >>> math.pi = 3.0\n\n🎉 Credits\n----------\n\nThe following projects were used to build and test :code:`readonly`.\n\n- `python`_\n- `poetry`_\n- `pytest`_\n- `flake8`_\n- `coverage`_\n- `rstcheck`_\n- `mypy`_\n- `pytestcov`_\n- `tox`_\n- `isort`_\n- `black`_\n- `precommit`_\n\n\n👋 Contribute\n-------------\n\nIf you are looking for a way to contribute to the project, please refer to the `Guideline`_.\n\n📝 License\n----------\n\nThis program and the accompanying materials are made available under the terms and conditions of the `GNU GENERAL PUBLIC LICENSE`_.\n\n.. _GNU GENERAL PUBLIC LICENSE: http://www.gnu.org/licenses/\n.. _readonly: https://pypi.org/project/readonly/\n.. _Marco Sulla: https://github.com/Marco-Sulla\n.. _Guideline: https://github.com/wiseaidev/readonly/blob/main/CONTRIBUTING.rst\n.. _pyenv: https://github.com/pyenv/pyenv\n.. _poetry: https://github.com/python-poetry/poetry\n.. _pipx: https://github.com/pypa/pipx\n.. _python: https://www.python.org/\n.. _pytest: https://docs.pytest.org/en/7.1.x/\n.. _flake8: https://flake8.pycqa.org/en/latest/\n.. _coverage: https://coverage.readthedocs.io/en/6.3.2/\n.. _rstcheck: https://pypi.org/project/rstcheck/\n.. _mypy: https://mypy.readthedocs.io/en/stable/\n.. _pytestcov: https://pytest-cov.readthedocs.io/en/latest/\n.. _tox: https://tox.wiki/en/latest/\n.. _isort: https://github.com/PyCQA/isort\n.. _black: https://black.readthedocs.io/en/stable/\n.. _precommit: https://pre-commit.com/\n',
     'author': 'Mahmoud Harmouch',
     'author_email': 'business@wiseai.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wiseaidev/readonly',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `readonly-0.1.1/PKG-INFO` & `readonly-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readonly
-Version: 0.1.1
+Version: 0.1.2
 Summary: Make any module attributes read only.
 Home-page: https://github.com/wiseaidev/readonly
 License: GNU General Public License v3.0
 Keywords: python,readonly
 Author: Mahmoud Harmouch
 Author-email: business@wiseai.dev
 Requires-Python: >=3.9,<4.0
@@ -38,16 +38,15 @@
    :target: https://github.com/wiseaidev/readonly/
    :alt: Repo Size
 
 .. image:: https://circleci.com/gh/wiseaidev/readonly/tree/main.svg?style=svg
    :target: https://circleci.com/gh/wiseaidev/readonly/tree/main
    :alt: Circle ci Build Status
 
-**readonly** is a python package that acts as an alternative to frozenset, but for dictionaries.
-
+**readonly** is a simple package to make any given module attributes into read only mode. 
 
 🛠️ Requirements
 ---------------
 
 **readonly** requires Python 3.9 or above.
 
 To install Python 3.9, I recommend using `pyenv`_.
```

