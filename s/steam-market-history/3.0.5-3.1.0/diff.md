# Comparing `tmp/steam_market_history-3.0.5.tar.gz` & `tmp/steam_market_history-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam_market_history-3.0.5.tar", max compression
+gzip compressed data, was "steam_market_history-3.1.0.tar", max compression
```

## Comparing `steam_market_history-3.0.5.tar` & `steam_market_history-3.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-17 18:30:10.067003 steam_market_history-3.0.5/LICENSE
--rw-r--r--   0        0        0     6545 2023-04-17 18:30:10.067003 steam_market_history-3.0.5/README.md
--rw-r--r--   0        0        0      706 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/pyproject.toml
--rw-r--r--   0        0        0      196 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/__init__.py
--rw-r--r--   0        0        0     2693 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/main.py
--rw-r--r--   0        0        0        0 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/modules/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/modules/exporter.py
--rw-r--r--   0        0        0     3572 2023-04-17 18:30:10.077003 steam_market_history-3.0.5/steam_market_history/modules/steam.py
--rw-r--r--   0        0        0     6175 2023-04-17 18:30:10.077003 steam_market_history-3.0.5/steam_market_history/templates/index.html
--rw-r--r--   0        0        0     7441 1970-01-01 00:00:00.000000 steam_market_history-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-18 20:49:45.785180 steam_market_history-3.1.0/LICENSE
+-rw-r--r--   0        0        0     6631 2023-04-18 20:49:45.785180 steam_market_history-3.1.0/README.md
+-rw-r--r--   0        0        0      706 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/__init__.py
+-rw-r--r--   0        0        0     2897 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/main.py
+-rw-r--r--   0        0        0        0 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/__init__.py
+-rw-r--r--   0        0        0     1699 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/exporter.py
+-rw-r--r--   0        0        0     3572 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/steam.py
+-rw-r--r--   0        0        0     6175 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/templates/index.html
+-rw-r--r--   0        0        0     7527 1970-01-01 00:00:00.000000 steam_market_history-3.1.0/PKG-INFO
```

### Comparing `steam_market_history-3.0.5/LICENSE` & `steam_market_history-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.0.5/README.md` & `steam_market_history-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
 ## About The Project
 
 steam-market-history is a command line tool written in Python which allows you to extract your entire Steam Market History with all transaction (sales/purchases) in a CSV or HTML file.
 
 ### Key features
 
-- Extract your **entire** Steam Market History
-- Create a CSV-File with all transactions
+- Extract your **entire** Steam Market History with all transactions to a HTML, CSV or JSON file
 - Overview of _all_ transactions on a user-friendly webpage with searchable and filterable results
 
 ### Built With
 
 - [Python](https://www.python.org/)
 - [Typer](https://typer.tiangolo.com/)
 
@@ -84,15 +83,15 @@
 
 - Python >= 3.8
 
 ### Installation
 
 Pip (recommended):
 
-```python
+```shell
 pip install steam-market-history
 ```
 
 Manual:
 
 1. Clone the repo
    ```sh
@@ -113,22 +112,23 @@
 
 ## Usage
 
 Currently, the following commands are supported:
 
 ### `export`
 
-Export your steam market history to a CSV or HTML file
+Export your steam market history to an HTML, JSON or CSV file
 
 > When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your computer. This package does not save your credentials in any way.
 
 Options:
 
-- `--csv` - Export to csv file
-- `--html` - Export to html file
+- `--csv` - Export market transactions to csv file
+- `--html` - Export market transactions to html file
+- `--json` - Export market transactions to json file
 - `--path` - Output directory for all file based operations (default: current working directory)
 - `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)
 - `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)
 - `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]
 
 Examples:
 
@@ -153,15 +153,14 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Add options of verbosity
-- [ ] Export to JSON
 
 See the [open issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
```

#### html2text {}

```diff
@@ -27,47 +27,49 @@
    5. Contributing
    6. License
    7. Contact
    8. Acknowledgments
   ## About The Project steam-market-history is a command line tool written in
 Python which allows you to extract your entire Steam Market History with all
 transaction (sales/purchases) in a CSV or HTML file. ### Key features - Extract
-your **entire** Steam Market History - Create a CSV-File with all transactions
-- Overview of _all_ transactions on a user-friendly webpage with searchable and
-filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
-(https://typer.tiangolo.com/)
+your **entire** Steam Market History with all transactions to a HTML, CSV or
+JSON file - Overview of _all_ transactions on a user-friendly webpage with
+searchable and filterable results ### Built With - [Python](https://
+www.python.org/) - [Typer](https://typer.tiangolo.com/)
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
-(recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
+(recommended): ```shell pip install steam-market-history ``` Manual: 1. Clone
 the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
 ``` 2. Install poetry (if not already installed) ```sh pip install poetry ```
 3. Install dependencies and start virtual environment ```sh poetry install &&
 poetry shell ```
                                                                   (back_to_top)
  ## Usage Currently, the following commands are supported: ### `export` Export
-your steam market history to a CSV or HTML file > When running the tool you
-will be prompted to insert your steam credentials. All processing is done
+your steam market history to an HTML, JSON or CSV file > When running the tool
+you will be prompted to insert your steam credentials. All processing is done
 locally on your computer. This package does not save your credentials in any
-way. Options: - `--csv` - Export to csv file - `--html` - Export to html file -
-`--path` - Output directory for all file based operations (default: current
-working directory) - `--launch` / `--no-launch` - Automatically open file(s)
-after export (default: `--launch`) - `--cache` / `--no-cache` - Create a file
-cache for all market transactions (default: `--no-cache`) - `--interactive` /
-`--non-interactive` - Interactive or non-interactive steam authentication
-[default: `--interactive`] Examples: Export your steam market history to a HTML
-file: ```shell steam-market-history export --html ``` Export your steam market
-history to a CSV file in a specific directory: ```shell steam-market-history
-export --csv --path /tmp/steam-market-history ``` ### `version` Display
-detailed information about this package. This includes the version, the license
-and the authors. ``` steam-market-history version ```
+way. Options: - `--csv` - Export market transactions to csv file - `--html` -
+Export market transactions to html file - `--json` - Export market transactions
+to json file - `--path` - Output directory for all file based operations
+(default: current working directory) - `--launch` / `--no-launch` -
+Automatically open file(s) after export (default: `--launch`) - `--cache` / `--
+no-cache` - Create a file cache for all market transactions (default: `--no-
+cache`) - `--interactive` / `--non-interactive` - Interactive or non-
+interactive steam authentication [default: `--interactive`] Examples: Export
+your steam market history to a HTML file: ```shell steam-market-history export
+--html ``` Export your steam market history to a CSV file in a specific
+directory: ```shell steam-market-history export --csv --path /tmp/steam-market-
+history ``` ### `version` Display detailed information about this package. This
+includes the version, the license and the authors. ``` steam-market-history
+version ```
                                                                   (back_to_top)
- ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
-issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
-list of proposed features (and known issues).
+ ## Roadmap - [ ] Add options of verbosity See the [open issues](https://
+gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed
+features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `steam_market_history-3.0.5/pyproject.toml` & `steam_market_history-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steam-market-history"
-version = "3.0.5"
+version = "3.1.0"
 description = "An easy-to-use CLI to export your steam market history to various formats"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fabieu/steam-market-history"
 keywords = ["steam", "CLI"]
```

### Comparing `steam_market_history-3.0.5/steam_market_history/main.py` & `steam_market_history-3.1.0/steam_market_history/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,29 @@
     typer.echo(f"License: {__metadata__.get('License')}")
 
 
 @app.command()
 def export(
         export_csv: bool = typer.Option(False, "--csv", help="Generate steam market history as csv file"),
         export_html: bool = typer.Option(False, "--html", help="Generate steam market history as interactive website"),
+        export_json: bool = typer.Option(False, "--json", help="Generate steam market history as json file"),
         path: Path = typer.Option(Path.cwd(), help="Path for file export"),
         launch: bool = typer.Option(True, help="Automatically open file(s) after export"),
         cache: bool = typer.Option(False, help="Cache market transactions. Use with caution!"),
         interactive: bool = typer.Option(True, "--interactive/--non-interactive",
                                          help="Interactive or non-interactive steam authentication")
 ):
     """
     Export your entire steam market history to a csv or html file. For more information use 'steam-market-history
     export --help'.
     """
     cache_path = "market_transactions.pkl"
 
     # Check if at least one export option is provided
-    if True not in {export_csv, export_html}:
+    if True not in {export_csv, export_html, export_json}:
         typer.echo(
             "Please provide at least one export option! For more information use 'steam-market-history export --help'",
             err=True)
         raise typer.Exit(1)
 
     # Login to steam
     if interactive:
@@ -68,10 +69,13 @@
 
     if export_csv:
         exporter.to_csv(market_transactions, path, launch)
 
     if export_html:
         exporter.to_html(market_transactions, path, launch)
 
+    if export_json:
+        exporter.to_json(market_transactions, path, launch)
+
 
 if __name__ == "__main__":
     app()
```

### Comparing `steam_market_history-3.0.5/steam_market_history/modules/exporter.py` & `steam_market_history-3.1.0/steam_market_history/modules/exporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 # Build-in modules
 import csv
+import json
 from datetime import datetime
 from pathlib import Path
 
 # PyPi modules
 from jinja2 import Template, select_autoescape
 import typer
 
+# Global variables
+base_name = "steam-market-history"
+
 
 def to_csv(market_transactions: list, path: Path, launch: bool) -> None:
-    filename = "steam-market-history.csv"
+    filename = base_name + ".csv"
 
     with open(filename, 'w', newline='', encoding="utf-8") as file:
         writer = csv.writer(file, delimiter=',')
         writer.writerow(market_transactions[0].keys())
         writer.writerows([x.values() for x in market_transactions])
 
     if launch:
         typer.launch(str(path / filename), locate=True)
 
 
 def to_html(market_transactions: list, path: Path, launch: bool) -> None:
-    filename = "steam-market-history.html"
+    filename = base_name + ".html"
 
     with open(Path(__file__).parent.parent / "templates/index.html", encoding="utf-8") as template_file:
         template = Template(template_file.read(), autoescape=select_autoescape())
 
     with open(filename, 'w', encoding="utf-8") as rendered_file:
         current_date = datetime.now().strftime("%d.%m.%Y %H:%M")
         summary = {
             "totalTransactions": len(market_transactions)
         }
         rendered_file.write(template.render(
             summary=summary, transactions=market_transactions, current_date=current_date))
 
     if launch:
         typer.launch(str(path / filename))
+
+
+def to_json(market_transactions: list, path: Path, launch: bool) -> None:
+    filename = base_name + ".json"
+
+    wrapper = {
+        "data": market_transactions
+    }
+
+    with open(filename, 'w', encoding="utf-8") as file:
+        file.write(json.dumps(wrapper, indent=4))
+
+    if launch:
+        typer.launch(str(path / filename))
```

### Comparing `steam_market_history-3.0.5/steam_market_history/modules/steam.py` & `steam_market_history-3.1.0/steam_market_history/modules/steam.py`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.0.5/steam_market_history/templates/index.html` & `steam_market_history-3.1.0/steam_market_history/templates/index.html`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.0.5/PKG-INFO` & `steam_market_history-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-market-history
-Version: 3.0.5
+Version: 3.1.0
 Summary: An easy-to-use CLI to export your steam market history to various formats
 Home-page: https://github.com/fabieu/steam-market-history
 License: MIT
 Keywords: steam,CLI
 Author: Fabian Eulitz
 Author-email: dev@sustineo.de
 Requires-Python: >=3.8,<4.0
@@ -82,16 +82,15 @@
 
 ## About The Project
 
 steam-market-history is a command line tool written in Python which allows you to extract your entire Steam Market History with all transaction (sales/purchases) in a CSV or HTML file.
 
 ### Key features
 
-- Extract your **entire** Steam Market History
-- Create a CSV-File with all transactions
+- Extract your **entire** Steam Market History with all transactions to a HTML, CSV or JSON file
 - Overview of _all_ transactions on a user-friendly webpage with searchable and filterable results
 
 ### Built With
 
 - [Python](https://www.python.org/)
 - [Typer](https://typer.tiangolo.com/)
 
@@ -107,15 +106,15 @@
 
 - Python >= 3.8
 
 ### Installation
 
 Pip (recommended):
 
-```python
+```shell
 pip install steam-market-history
 ```
 
 Manual:
 
 1. Clone the repo
    ```sh
@@ -136,22 +135,23 @@
 
 ## Usage
 
 Currently, the following commands are supported:
 
 ### `export`
 
-Export your steam market history to a CSV or HTML file
+Export your steam market history to an HTML, JSON or CSV file
 
 > When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your computer. This package does not save your credentials in any way.
 
 Options:
 
-- `--csv` - Export to csv file
-- `--html` - Export to html file
+- `--csv` - Export market transactions to csv file
+- `--html` - Export market transactions to html file
+- `--json` - Export market transactions to json file
 - `--path` - Output directory for all file based operations (default: current working directory)
 - `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)
 - `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)
 - `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]
 
 Examples:
 
@@ -176,15 +176,14 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Add options of verbosity
-- [ ] Export to JSON
 
 See the [open issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: steam-market-history Version: 3.0.5 Summary: An
+Metadata-Version: 2.1 Name: steam-market-history Version: 3.1.0 Summary: An
 easy-to-use CLI to export your steam market history to various formats Home-
 page: https://github.com/fabieu/steam-market-history License: MIT Keywords:
 steam,CLI Author: Fabian Eulitz Author-email: dev@sustineo.de Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -39,47 +39,49 @@
    5. Contributing
    6. License
    7. Contact
    8. Acknowledgments
   ## About The Project steam-market-history is a command line tool written in
 Python which allows you to extract your entire Steam Market History with all
 transaction (sales/purchases) in a CSV or HTML file. ### Key features - Extract
-your **entire** Steam Market History - Create a CSV-File with all transactions
-- Overview of _all_ transactions on a user-friendly webpage with searchable and
-filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
-(https://typer.tiangolo.com/)
+your **entire** Steam Market History with all transactions to a HTML, CSV or
+JSON file - Overview of _all_ transactions on a user-friendly webpage with
+searchable and filterable results ### Built With - [Python](https://
+www.python.org/) - [Typer](https://typer.tiangolo.com/)
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
-(recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
+(recommended): ```shell pip install steam-market-history ``` Manual: 1. Clone
 the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
 ``` 2. Install poetry (if not already installed) ```sh pip install poetry ```
 3. Install dependencies and start virtual environment ```sh poetry install &&
 poetry shell ```
                                                                   (back_to_top)
  ## Usage Currently, the following commands are supported: ### `export` Export
-your steam market history to a CSV or HTML file > When running the tool you
-will be prompted to insert your steam credentials. All processing is done
+your steam market history to an HTML, JSON or CSV file > When running the tool
+you will be prompted to insert your steam credentials. All processing is done
 locally on your computer. This package does not save your credentials in any
-way. Options: - `--csv` - Export to csv file - `--html` - Export to html file -
-`--path` - Output directory for all file based operations (default: current
-working directory) - `--launch` / `--no-launch` - Automatically open file(s)
-after export (default: `--launch`) - `--cache` / `--no-cache` - Create a file
-cache for all market transactions (default: `--no-cache`) - `--interactive` /
-`--non-interactive` - Interactive or non-interactive steam authentication
-[default: `--interactive`] Examples: Export your steam market history to a HTML
-file: ```shell steam-market-history export --html ``` Export your steam market
-history to a CSV file in a specific directory: ```shell steam-market-history
-export --csv --path /tmp/steam-market-history ``` ### `version` Display
-detailed information about this package. This includes the version, the license
-and the authors. ``` steam-market-history version ```
+way. Options: - `--csv` - Export market transactions to csv file - `--html` -
+Export market transactions to html file - `--json` - Export market transactions
+to json file - `--path` - Output directory for all file based operations
+(default: current working directory) - `--launch` / `--no-launch` -
+Automatically open file(s) after export (default: `--launch`) - `--cache` / `--
+no-cache` - Create a file cache for all market transactions (default: `--no-
+cache`) - `--interactive` / `--non-interactive` - Interactive or non-
+interactive steam authentication [default: `--interactive`] Examples: Export
+your steam market history to a HTML file: ```shell steam-market-history export
+--html ``` Export your steam market history to a CSV file in a specific
+directory: ```shell steam-market-history export --csv --path /tmp/steam-market-
+history ``` ### `version` Display detailed information about this package. This
+includes the version, the license and the authors. ``` steam-market-history
+version ```
                                                                   (back_to_top)
- ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
-issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
-list of proposed features (and known issues).
+ ## Roadmap - [ ] Add options of verbosity See the [open issues](https://
+gitlab.com/sustineo/steam-market-history/-/issues) for a full list of proposed
+features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

