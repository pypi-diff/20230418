# Comparing `tmp/etradebot-1.0.1.tar.gz` & `tmp/etradebot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etradebot-1.0.1.tar", last modified: Thu Apr 13 02:02:05 2023, max compression
+gzip compressed data, was "etradebot-1.0.2.tar", last modified: Tue Apr 18 19:17:27 2023, max compression
```

## Comparing `etradebot-1.0.1.tar` & `etradebot-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.654000 etradebot-1.0.1/
--rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4799 2023-04-13 02:02:05.647000 etradebot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4253 2023-04-13 02:00:43.000000 etradebot-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.154000 etradebot-1.0.1/authentication/
--rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.1/authentication/__init__.py
--rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.1/authentication/authentication.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.176000 etradebot-1.0.1/etrade/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/etrade/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.1/etrade/etrade.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.236000 etradebot-1.0.1/etradebot.egg-info/
--rw-rw-rw-   0        0        0     4799 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 02:02:04.000000 etradebot-1.0.1/etradebot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.258000 etradebot-1.0.1/execute/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/execute/__init__.py
--rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.1/execute/execute.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.293000 etradebot-1.0.1/model/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/model/__init__.py
--rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.1/model/investor_views.py
--rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.1/model/model.py
--rw-rw-rw-   0        0        0       42 2023-04-13 02:02:05.652000 etradebot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-04-13 02:00:43.000000 etradebot-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.343000 etradebot-1.0.1/strategies/
--rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.1/strategies/__init__.py
--rw-rw-rw-   0        0        0     2961 2023-04-01 01:26:39.000000 etradebot-1.0.1/strategies/cape_strategy.py
--rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.1/strategies/example_strategy.py
--rw-rw-rw-   0        0        0     1192 2023-04-02 17:50:45.000000 etradebot-1.0.1/strategies/strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.577000 etradebot-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.1/tests/mock_responses.py
--rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.1/tests/test_authentication.py
--rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.1/tests/test_etrade.py
--rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.1/tests/test_execute.py
--rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.1/tests/test_model.py
--rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.1/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:02:05.637000 etradebot-1.0.1/utils/
--rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.1/utils/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-04-12 17:27:13.000000 etradebot-1.0.1/utils/credentials.py
--rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.1/utils/fake_data.py
--rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.1/utils/logging_config.py
--rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.1/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:27.823000 etradebot-1.0.2/
+-rw-rw-rw-   0        0        0     1097 2023-03-20 03:24:40.000000 etradebot-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4944 2023-04-18 19:17:27.818000 etradebot-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4398 2023-04-16 01:46:23.000000 etradebot-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:26.863000 etradebot-1.0.2/authentication/
+-rw-rw-rw-   0        0        0       31 2023-02-19 07:12:36.000000 etradebot-1.0.2/authentication/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-02 17:21:30.000000 etradebot-1.0.2/authentication/authentication.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:26.884000 etradebot-1.0.2/etrade/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.2/etrade/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-04-02 17:36:50.000000 etradebot-1.0.2/etrade/etrade.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:26.913000 etradebot-1.0.2/etradebot.egg-info/
+-rw-rw-rw-   0        0        0     4944 2023-04-18 19:17:26.000000 etradebot-1.0.2/etradebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-04-18 19:17:26.000000 etradebot-1.0.2/etradebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-04-18 19:17:26.000000 etradebot-1.0.2/etradebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      267 2023-04-18 19:17:26.000000 etradebot-1.0.2/etradebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       59 2023-04-18 19:17:26.000000 etradebot-1.0.2/etradebot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:26.938000 etradebot-1.0.2/execute/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.2/execute/__init__.py
+-rw-rw-rw-   0        0        0    15723 2023-04-11 04:37:00.000000 etradebot-1.0.2/execute/execute.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:27.452000 etradebot-1.0.2/model/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.2/model/__init__.py
+-rw-rw-rw-   0        0        0     3144 2023-03-29 05:54:46.000000 etradebot-1.0.2/model/investor_views.py
+-rw-rw-rw-   0        0        0    30850 2023-04-12 05:02:10.000000 etradebot-1.0.2/model/model.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 19:17:27.822000 etradebot-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-04-15 21:20:03.000000 etradebot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:27.489000 etradebot-1.0.2/strategies/
+-rw-rw-rw-   0        0        0        0 2023-02-18 02:52:24.000000 etradebot-1.0.2/strategies/__init__.py
+-rw-rw-rw-   0        0        0     3038 2023-04-18 19:12:36.000000 etradebot-1.0.2/strategies/cape_strategy.py
+-rw-rw-rw-   0        0        0     3050 2023-03-18 21:04:05.000000 etradebot-1.0.2/strategies/example_strategy.py
+-rw-rw-rw-   0        0        0     1397 2023-04-18 19:13:26.000000 etradebot-1.0.2/strategies/strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:27.585000 etradebot-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-19 06:56:31.000000 etradebot-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0    25834 2023-03-16 04:10:47.000000 etradebot-1.0.2/tests/mock_responses.py
+-rw-rw-rw-   0        0        0     3857 2023-03-03 23:39:46.000000 etradebot-1.0.2/tests/test_authentication.py
+-rw-rw-rw-   0        0        0     7079 2023-02-26 05:02:38.000000 etradebot-1.0.2/tests/test_etrade.py
+-rw-rw-rw-   0        0        0     5658 2023-03-04 00:28:00.000000 etradebot-1.0.2/tests/test_execute.py
+-rw-rw-rw-   0        0        0     7062 2023-03-16 04:10:47.000000 etradebot-1.0.2/tests/test_model.py
+-rw-rw-rw-   0        0        0        0 2023-02-19 00:45:57.000000 etradebot-1.0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 19:17:27.812000 etradebot-1.0.2/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-17 04:26:08.000000 etradebot-1.0.2/utils/__init__.py
+-rw-rw-rw-   0        0        0     1126 2023-04-17 04:03:16.000000 etradebot-1.0.2/utils/credentials.py
+-rw-rw-rw-   0        0        0     2185 2023-04-03 02:19:14.000000 etradebot-1.0.2/utils/fake_data.py
+-rw-rw-rw-   0        0        0      989 2023-02-19 02:01:31.000000 etradebot-1.0.2/utils/logging_config.py
+-rw-rw-rw-   0        0        0     3763 2023-02-20 04:32:22.000000 etradebot-1.0.2/utils/portfolio.py
```

### Comparing `etradebot-1.0.1/LICENSE` & `etradebot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/PKG-INFO` & `etradebot-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etradebot
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python-based trading bot for the E-Trade platform
 Home-page: https://github.com/nathanramoscfa/etradebot
 Author: Nathan Ramos, CFA®
 Author-email: info@nrcapitalmanagement.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,31 +16,33 @@
 
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
--   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Fetches real-time market data from E-Trade API
+-   Accesses market data from the Bloomberg API or Yahoo Finance API
+-   Executes trade types: buy, sell, sell short, and short cover
 -   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
-2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
-3. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
-4. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
-5. [Configure](https://etradebot.readthedocs.io/en/latest/configure.html) batch file to run ETradeBot.
-6. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
-7. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
+1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
+3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
+4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
+5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
+6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
+7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
+8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
 
 ## Example
 
 The following example shows ETradeBot being run in Anaconda Prompt:
 
 ![Execute Trades](https://github.com/nathanramoscfa/etradebot/blob/main/docs/source/_static/execute_trades.gif)
```

### Comparing `etradebot-1.0.1/README.md` & `etradebot-1.0.2/etradebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,48 @@
+Metadata-Version: 2.1
+Name: etradebot
+Version: 1.0.2
+Summary: A Python-based trading bot for the E-Trade platform
+Home-page: https://github.com/nathanramoscfa/etradebot
+Author: Nathan Ramos, CFA®
+Author-email: info@nrcapitalmanagement.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
--   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Fetches real-time market data from E-Trade API
+-   Accesses market data from the Bloomberg API or Yahoo Finance API
+-   Executes trade types: buy, sell, sell short, and short cover
 -   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
-2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
-3. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
-4. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
-5. [Configure](https://etradebot.readthedocs.io/en/latest/configure.html) batch file to run ETradeBot.
-6. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
-7. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
+1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
+3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
+4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
+5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
+6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
+7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
+8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
 
 ## Example
 
 The following example shows ETradeBot being run in Anaconda Prompt:
 
 ![Execute Trades](https://github.com/nathanramoscfa/etradebot/blob/main/docs/source/_static/execute_trades.gif)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `etradebot-1.0.1/authentication/authentication.py` & `etradebot-1.0.2/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/etrade/etrade.py` & `etradebot-1.0.2/etrade/etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/etradebot.egg-info/PKG-INFO` & `etradebot-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-Metadata-Version: 2.1
-Name: etradebot
-Version: 1.0.1
-Summary: A Python-based trading bot for the E-Trade platform
-Home-page: https://github.com/nathanramoscfa/etradebot
-Author: Nathan Ramos, CFA®
-Author-email: info@nrcapitalmanagement.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ETradeBot
 
 ETradeBot is an automated trading software written in Python for E-Trade accounts that allows users to execute trades based on custom trading strategies. ETradeBot is strategy-agnostic and will execute any strategy given to it. This project is not affiliated with E-Trade or any other financial institution. By using ETradeBot, you agree to the [disclaimer](https://etradebot.readthedocs.io/en/latest/disclaimer.html).
 
 ## Features
 
--   Fetches real-time market data from E-Trade API used to execute trades
--   Executes trade types: buy, sell, sell short, and short cover trade types
+-   Fetches real-time market data from E-Trade API
+-   Accesses market data from the Bloomberg API or Yahoo Finance API
+-   Executes trade types: buy, sell, sell short, and short cover
 -   Submits price type: market orders to E-Trade API
 -   Manages portfolio: tracks positions, balance, and performance
 -   Trades: common stocks and ETFs
 
 ## Getting Started
 
 Refer to the [ETradeBot documentation](https://etradebot.readthedocs.io/en/latest/index.html) for instructions on installing, configuring, and using the software. 
 
-1. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
-2. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
-3. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
-4. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
-5. [Configure](https://etradebot.readthedocs.io/en/latest/configure.html) batch file to run ETradeBot.
-6. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
-7. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
+1. [Install](https://etradebot.readthedocs.io/en/latest/bloomberg.html) the Bloomberg SDK and C++ Build Tools.
+2. [Create](https://etradebot.readthedocs.io/en/latest/environment.html) your Python environment and install ETradeBot.
+3. [Configure](https://etradebot.readthedocs.io/en/latest/selenium.html) Selenium to work with your browser.
+4. [Obtain](https://etradebot.readthedocs.io/en/latest/credentials.html) and securely store your E-Trade credentials.
+5. [Insert](https://etradebot.readthedocs.io/en/latest/strategies.html) your strategy into the strategies directory as a .py file.
+6. [Configure](https://etradebot.readthedocs.io/en/latest/batch.html) a batch file to run ETradeBot.
+7. [Run](https://etradebot.readthedocs.io/en/latest/running.html) ETradeBot in either preview or live trading mode.
+8. [Schedule](https://etradebot.readthedocs.io/en/latest/scheduling.html) ETradeBot to run automatically.
 
 ## Example
 
 The following example shows ETradeBot being run in Anaconda Prompt:
 
 ![Execute Trades](https://github.com/nathanramoscfa/etradebot/blob/main/docs/source/_static/execute_trades.gif)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `etradebot-1.0.1/etradebot.egg-info/SOURCES.txt` & `etradebot-1.0.2/etradebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/execute/execute.py` & `etradebot-1.0.2/execute/execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/model/investor_views.py` & `etradebot-1.0.2/model/investor_views.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/model/model.py` & `etradebot-1.0.2/model/model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/setup.py` & `etradebot-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='etradebot',
-    version='1.0.1',
+    version='1.0.2',
     url='https://github.com/nathanramoscfa/etradebot',
     license='MIT',
     author='Nathan Ramos, CFA®',
     author_email='info@nrcapitalmanagement.com',
     description='A Python-based trading bot for the E-Trade platform',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `etradebot-1.0.1/strategies/cape_strategy.py` & `etradebot-1.0.2/strategies/cape_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,20 @@
         (equity_etf_csv['FWD_RETURN_FORECAST'] >= min_long_return) |
         (equity_etf_csv['FWD_RETURN_FORECAST'] <= max_short_return)
         ]
 
     return df
 
 
-def strategy(etf_path):
+def strategy():
     """
-    :description: Strategy
+    :description: Strategy to be run by the backtester
+
+    :return: Portfolio weights
+    :rtype: pd.Series
     """
     etf_path = 'https://raw.githubusercontent.com/nathanramoscfa/nrcapital/main/data/etf_cape_return_forecast.csv'
     selected_equity_etfs = get_nrcapital_forecast(etf_path)
     symbols = list(selected_equity_etfs.TICKER)
 
     model = Model(
         symbols,
```

### Comparing `etradebot-1.0.1/strategies/example_strategy.py` & `etradebot-1.0.2/strategies/example_strategy.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/strategies/strategy.py` & `etradebot-1.0.2/strategies/strategy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import warnings
 import importlib
 
 
 class Strategy:
     """
     :description: This class is the main strategy class that will be used to run the strategy.
@@ -31,8 +32,13 @@
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
 
             # Import the strategy function from the specified module
             strategy_module = importlib.import_module("strategies." + self.strategy_name)
             strategy_function = strategy_module.strategy
 
-            return strategy_function(self.prints)
+            num_parameters = len(inspect.signature(strategy_function).parameters)
+
+            if num_parameters == 1:
+                return strategy_function(self.prints)
+            else:
+                return strategy_function()
```

### Comparing `etradebot-1.0.1/tests/mock_responses.py` & `etradebot-1.0.2/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/tests/test_authentication.py` & `etradebot-1.0.2/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/tests/test_etrade.py` & `etradebot-1.0.2/tests/test_etrade.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/tests/test_execute.py` & `etradebot-1.0.2/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/tests/test_model.py` & `etradebot-1.0.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/utils/credentials.py` & `etradebot-1.0.2/utils/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 consumer_key = keyring.get_password("etrade", "consumer_key")
 consumer_secret = keyring.get_password("etrade", "consumer_secret")
 sandbox_key = keyring.get_password("etrade", "sandbox_key")
 sandbox_secret = keyring.get_password("etrade", "sandbox_secret")
 web_username = keyring.get_password("etrade", "web_username")
 web_password = keyring.get_password("etrade", "web_password")
 account_id = keyring.get_password("etrade", "account_id")
-etrade_cookie = ast.literal_eval(keyring.get_password("etrade", "cookie"))
+etrade_cookie = ast.literal_eval(keyring.get_password("etrade", "etrade_cookie"))
 account_id_key = keyring.get_password("etrade", "account_id_key")
 
 
 # Show the credentials
 def show_credentials():
     print("consumer_key: " + consumer_key)
     print("consumer_secret: " + consumer_secret)
```

### Comparing `etradebot-1.0.1/utils/fake_data.py` & `etradebot-1.0.2/utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/utils/logging_config.py` & `etradebot-1.0.2/utils/logging_config.py`

 * *Files identical despite different names*

### Comparing `etradebot-1.0.1/utils/portfolio.py` & `etradebot-1.0.2/utils/portfolio.py`

 * *Files identical despite different names*

