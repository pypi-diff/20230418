# Comparing `tmp/consulta_investimentos-4.0.1.tar.gz` & `tmp/consulta_investimentos-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consulta_investimentos-4.0.1.tar", max compression
+gzip compressed data, was "consulta_investimentos-5.0.1.tar", max compression
```

## Comparing `consulta_investimentos-4.0.1.tar` & `consulta_investimentos-5.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      274 2022-04-20 01:04:28.012265 consulta_investimentos-4.0.1/consulta_investimentos/__init__.py
--rw-r--r--   0        0        0       41 2022-03-19 01:13:13.493498 consulta_investimentos-4.0.1/consulta_investimentos/ativos_cotacoes/__init__.py
--rw-r--r--   0        0        0      970 2022-12-23 02:28:46.724644 consulta_investimentos-4.0.1/consulta_investimentos/ativos_cotacoes/cotacoes.py
--rw-r--r--   0        0        0       39 2022-03-19 01:13:36.414013 consulta_investimentos-4.0.1/consulta_investimentos/ativos_posicao/__init__.py
--rw-r--r--   0        0        0     9145 2022-11-09 14:23:10.091746 consulta_investimentos-4.0.1/consulta_investimentos/ativos_posicao/posicao.py
--rw-r--r--   0        0        0     3483 2022-04-20 01:02:49.652489 consulta_investimentos-4.0.1/consulta_investimentos/cli.py
--rw-r--r--   0        0        0       36 2022-03-19 01:13:38.744800 consulta_investimentos-4.0.1/consulta_investimentos/moeda_cotacao/__init__.py
--rw-r--r--   0        0        0     3081 2022-05-31 14:23:35.364279 consulta_investimentos-4.0.1/consulta_investimentos/moeda_cotacao/moedas.py
--rw-r--r--   0        0        0      690 2022-03-19 03:02:24.428485 consulta_investimentos-4.0.1/consulta_investimentos/moeda_cotacao/valida_moeda.py
--rw-r--r--   0        0        0      162 2022-03-31 23:06:02.326002 consulta_investimentos-4.0.1/consulta_investimentos/utils/__init__.py
--rw-r--r--   0        0        0     2056 2022-03-10 17:26:07.596808 consulta_investimentos-4.0.1/consulta_investimentos/utils/append.py
--rw-r--r--   0        0        0     4275 2022-03-15 11:27:10.852410 consulta_investimentos-4.0.1/consulta_investimentos/utils/arquivo.py
--rw-r--r--   0        0        0     1781 2022-04-01 18:13:25.921388 consulta_investimentos-4.0.1/consulta_investimentos/utils/data_functions.py
--rw-r--r--   0        0        0     2073 2022-12-23 02:08:11.804147 consulta_investimentos-4.0.1/consulta_investimentos/yfinance_exemple.py
--rw-r--r--   0        0        0    35823 2022-03-07 20:12:52.680608 consulta_investimentos-4.0.1/LICENSE
--rw-r--r--   0        0        0      743 2022-12-23 02:30:03.825027 consulta_investimentos-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     1212 2022-12-23 02:30:09.449333 consulta_investimentos-4.0.1/setup.py
--rw-r--r--   0        0        0      780 2022-12-23 02:30:09.449333 consulta_investimentos-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-18 01:24:08.758535 consulta_investimentos-5.0.1/consulta_investimentos/__init__.py
+-rw-r--r--   0        0        0       41 2022-03-19 01:13:13.493498 consulta_investimentos-5.0.1/consulta_investimentos/ativos_cotacoes/__init__.py
+-rw-r--r--   0        0        0      970 2022-12-23 02:28:46.724644 consulta_investimentos-5.0.1/consulta_investimentos/ativos_cotacoes/cotacoes.py
+-rw-r--r--   0        0        0       39 2022-03-19 01:13:36.414013 consulta_investimentos-5.0.1/consulta_investimentos/ativos_posicao/__init__.py
+-rw-r--r--   0        0        0     9259 2023-04-18 15:31:32.847977 consulta_investimentos-5.0.1/consulta_investimentos/ativos_posicao/posicao.py
+-rw-r--r--   0        0        0     3322 2023-04-18 16:35:56.202443 consulta_investimentos-5.0.1/consulta_investimentos/cli.py
+-rw-r--r--   0        0        0       36 2022-03-19 01:13:38.744800 consulta_investimentos-5.0.1/consulta_investimentos/moeda_cotacao/__init__.py
+-rw-r--r--   0        0        0     3081 2022-05-31 14:23:35.364279 consulta_investimentos-5.0.1/consulta_investimentos/moeda_cotacao/moedas.py
+-rw-r--r--   0        0        0      690 2022-03-19 03:02:24.428485 consulta_investimentos-5.0.1/consulta_investimentos/moeda_cotacao/valida_moeda.py
+-rw-r--r--   0        0        0      162 2022-03-31 23:06:02.326002 consulta_investimentos-5.0.1/consulta_investimentos/utils/__init__.py
+-rw-r--r--   0        0        0     2056 2022-03-10 17:26:07.596808 consulta_investimentos-5.0.1/consulta_investimentos/utils/append.py
+-rw-r--r--   0        0        0     4275 2022-03-15 11:27:10.852410 consulta_investimentos-5.0.1/consulta_investimentos/utils/arquivo.py
+-rw-r--r--   0        0        0     1781 2022-04-01 18:13:25.921388 consulta_investimentos-5.0.1/consulta_investimentos/utils/data_functions.py
+-rw-r--r--   0        0        0     2073 2022-12-23 02:08:11.804147 consulta_investimentos-5.0.1/consulta_investimentos/yfinance_exemple.py
+-rw-r--r--   0        0        0    35823 2022-03-07 20:12:52.680608 consulta_investimentos-5.0.1/LICENSE
+-rw-r--r--   0        0        0      743 2023-04-18 16:43:15.608771 consulta_investimentos-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:43:27.968702 consulta_investimentos-5.0.1/setup.py
+-rw-r--r--   0        0        0      780 2023-04-18 16:43:27.968702 consulta_investimentos-5.0.1/PKG-INFO
```

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/ativos_cotacoes/cotacoes.py` & `consulta_investimentos-5.0.1/consulta_investimentos/ativos_cotacoes/cotacoes.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/ativos_posicao/posicao.py` & `consulta_investimentos-5.0.1/consulta_investimentos/ativos_posicao/posicao.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,20 @@
     driver = webdriver.Chrome()
     driver.maximize_window()
     wdw = WebDriverWait(driver, 15)
     driver.get('https://www.investidor.b3.com.br/')
 
     # espera aparecer o elemento do login (CPF)
 
-    locator = (By.ID, 'DOC_INPUT')
+    locator = (By.ID, 'cpf_mask')
     elemento = wdw.until(ec.element_to_be_clickable(locator))
 
     if login:
         elemento.send_keys(login)
-        locator = (By.ID, 'Btn_CONTINUE')
+        locator = (By.XPATH,"/html/body/app-root/app-landing-page/div/div[2]/aside/div[1]/button")
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
     if senha:    
         locator = (By.ID, 'PASS_INPUT')
         elemento = wdw.until(ec.element_to_be_clickable(locator))
         elemento.send_keys(senha)
     
@@ -185,42 +185,42 @@
         else:
             dt_max = dt2
 
         # navegação no pop-up de filtros
         locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-tabela-filtro/div/div/button[1]')
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
-        locator = (By.XPATH, "//input[@data-placeholder='Data final']")
+        locator = (By.XPATH, '//*[@class="form-control input-end b3-ga-datepicker"]')
         elemento = wdw.until(ec.element_to_be_clickable(locator))
         for _ in range(10):
             elemento.send_keys(Keys.BACKSPACE)
         elemento.send_keys(dt_max.strftime('%d/%m/%Y'))
 
-        locator = (By.XPATH, "//input[@data-placeholder='Data inicial']")
+        locator = (By.XPATH, '//*[@class="form-control input-start b3-ga-datepicker"]')
         elemento = wdw.until(ec.element_to_be_clickable(locator))
         for _ in range(10):
             elemento.send_keys(Keys.BACKSPACE)
         elemento.send_keys(dt_min.strftime('%d/%m/%Y'))
 
-        locator = (By.XPATH, "//input[@data-placeholder='Data final']") # volta à data final -> aplica a conferencia do campo na data inicial
+        locator = (By.XPATH, '//*[@class="form-control input-end b3-ga-datepicker"]') # volta à data final -> aplica a conferencia do campo na data inicial
         elemento = wdw.until(ec.element_to_be_clickable(locator)).click()
 
         locator = (By.ID, 'botao-filtrar-movimentacao')
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
         # Futuro !
         # procurar se houve erro de data
 
         locator = (By.XPATH, '//button[@label="Baixar extrato"]')
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
-        locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-modal-download/b3-modal-drawer/div[1]/div[2]/div/div/div/app-opcoes-selecao-download/label[2]/div')
+        locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-modal-download-extrato/b3-modal-drawer/div[1]/div[2]/div/div/div/app-opcoes-selecao-download/label[2]/div')
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
-        locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-modal-download/b3-modal-drawer/div[1]/div[2]/div/div/button')
+        locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-modal-download-extrato/b3-modal-drawer/div[1]/div[2]/div/div/button')
         wdw.until(ec.element_to_be_clickable(locator)).click()
 
         import time
         time.sleep(2)
         download_concluido(path_download)
 
         locator = (By.XPATH, '//*[@id="b3i-conteudo"]/app-extrato/div/div/div[3]/app-movimentacoes/app-modal-download/b3-modal-drawer/div[1]/div[2]/div/div/div/button')
```

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/cli.py` & `consulta_investimentos-5.0.1/consulta_investimentos/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import click
 import pandas as pd
 
 from consulta_investimentos.ativos_cotacoes.cotacoes import consulta_cotacoes
-from consulta_investimentos.ativos_dividendos.dividendos import consulta_dividendos
-from consulta_investimentos.ativos_eventos.eventos import consulta_eventos
 from consulta_investimentos.ativos_posicao.posicao import consulta_posicao
 from consulta_investimentos.moeda_cotacao.moedas import consulta_moedas
 
 
 @click.group('cli')
 def cli():
     ...
```

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/moeda_cotacao/moedas.py` & `consulta_investimentos-5.0.1/consulta_investimentos/moeda_cotacao/moedas.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/moeda_cotacao/valida_moeda.py` & `consulta_investimentos-5.0.1/consulta_investimentos/moeda_cotacao/valida_moeda.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/utils/append.py` & `consulta_investimentos-5.0.1/consulta_investimentos/utils/append.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/utils/arquivo.py` & `consulta_investimentos-5.0.1/consulta_investimentos/utils/arquivo.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/utils/data_functions.py` & `consulta_investimentos-5.0.1/consulta_investimentos/utils/data_functions.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/consulta_investimentos/yfinance_exemple.py` & `consulta_investimentos-5.0.1/consulta_investimentos/yfinance_exemple.py`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/LICENSE` & `consulta_investimentos-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consulta_investimentos-4.0.1/pyproject.toml` & `consulta_investimentos-5.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "consulta_investimentos"
-version = "4.0.1"
+version = "5.0.1"
 description = "Baixa infos diversas de ativos financeiros."
 authors = ["Vinicius Maciel <vinimaciel01@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.4.1"
 requests = "^2.27.1"
```

### Comparing `consulta_investimentos-4.0.1/setup.py` & `consulta_investimentos-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'yfinance>=0.2.3,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['consulta_investimentos = consulta_investimentos.cli:cli']}
 
 setup_kwargs = {
     'name': 'consulta-investimentos',
-    'version': '4.0.1',
+    'version': '5.0.1',
     'description': 'Baixa infos diversas de ativos financeiros.',
     'long_description': None,
     'author': 'Vinicius Maciel',
     'author_email': 'vinimaciel01@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `consulta_investimentos-4.0.1/PKG-INFO` & `consulta_investimentos-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consulta-investimentos
-Version: 4.0.1
+Version: 5.0.1
 Summary: Baixa infos diversas de ativos financeiros.
 Author: Vinicius Maciel
 Author-email: vinimaciel01@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

