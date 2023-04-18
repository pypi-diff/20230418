# Comparing `tmp/get_certificate_chain-0.1.2.tar.gz` & `tmp/get_certificate_chain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_certificate_chain-0.1.2.tar", max compression
+gzip compressed data, was "get_certificate_chain-0.1.3.tar", max compression
```

## Comparing `get_certificate_chain-0.1.2.tar` & `get_certificate_chain-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     3944 2023-04-17 15:22:43.527867 get_certificate_chain-0.1.2/README.md
--rw-r--r--   0        0        0    15843 2023-04-17 15:08:14.586662 get_certificate_chain-0.1.2/get_certificate_chain/main.py
--rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.2/get_certificate_chain/tests/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-17 15:14:34.799742 get_certificate_chain-0.1.2/get_certificate_chain/tests/test_cert.py
--rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.2/get_certificate_chain/tests/test_data/generate_cert.sh
--rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.2/get_certificate_chain/tests/test_data/root_ca.cnf
--rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.2/get_certificate_chain/tests/test_data/server.cnf
--rw-r--r--   0        0        0      814 2023-04-17 15:13:15.404619 get_certificate_chain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 15:52:44.314027 get_certificate_chain-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     4108 2023-04-18 12:03:44.815919 get_certificate_chain-0.1.3/README.md
+-rw-r--r--   0        0        0    15854 2023-04-18 11:55:16.287746 get_certificate_chain-0.1.3/get_certificate_chain/download.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:15:58.955704 get_certificate_chain-0.1.3/get_certificate_chain/tests/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-18 11:52:31.295015 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_cert.py
+-rwxr-xr-x   0        0        0      469 2023-04-16 18:53:27.114820 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/generate_cert.sh
+-rw-r--r--   0        0        0      458 2023-04-16 18:50:45.943493 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/root_ca.cnf
+-rw-r--r--   0        0        0      613 2023-04-16 18:52:49.929303 get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/server.cnf
+-rw-r--r--   0        0        0      817 2023-04-18 11:43:18.978436 get_certificate_chain-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 get_certificate_chain-0.1.3/PKG-INFO
```

### Comparing `get_certificate_chain-0.1.2/LICENSE.md` & `get_certificate_chain-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.2/README.md` & `get_certificate_chain-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Get Certificate Chain 🌐🔐
 
+[![PyTests](https://github.com/cdot65/get_certificate_chain/actions/workflows/tests.yml/badge.svg)](https://github.com/cdot65/get_certificate_chain/actions/workflows/tests.yml)
+
 This Python script retrieves the certificate chain from a website, allowing you to analyze and verify the SSL/TLS certificates of the website. This project is a custom fork of the [getCertificateChain project](https://github.com/TheScriptGuy/getCertificateChain), and the overwhelming majority of credit goes to [TheScriptGuy](https://github.com/TheScriptGuy).
 
 ## Table of Contents
 
 - [Get Certificate Chain 🌐🔐](#get-certificate-chain-)
   - [Table of Contents](#table-of-contents)
   - [Requirements 📋](#requirements-)
@@ -15,15 +17,15 @@
     - [Command Line CLI](#command-line-cli)
       - [Arguments](#arguments)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Requirements 📋
 
-- Python 3.10+
+- Python 3.9+
 - Poetry (optional) - [Python Poetry](https://python-poetry.org/docs/)
 
 ## Installation
 
 ### PyPi
 
 To install the package from PyPi, simply run the appropriate command.
@@ -52,65 +54,63 @@
 
 To use the package in your script, simply import the package and create an instance of the `SSLCertificateChainDownloader` object.
 
 To pass arguments into the object, you can use the `argparse` library:
 
 1. Import the argparse library.
 2. Import the SSLCertificateChainDownloader object from the package.
-3. Create an argument parser with a description.
-4. Add your arguments.
-5. Parse the arguments.
-6. Create an instance of the SSLCertificateChainDownloader object.
-7. Run the downloader object with the parsed arguments.
+3. Create a python dictionary with the "url" key and value of the domain.
+4. Create an instance of the SSLCertificateChainDownloader object.
+5. Run the downloader object with the parsed arguments.
 
 ```python
-from get_certificate_chain import SSLCertificateChainDownloader
+from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
 # Use the downloader object for your needs
 ```
 
-To pass arguments into the object, you can use the `argparse` library:
+You can pass the arguments directly into the object:
 
 ```python
-import argparse
-from get_certificate_chain import SSLCertificateChainDownloader
-
-# Add your arguments
-args = parser.parse_args()
+from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
-downloader.run(args)
+downloader.run({'url': 'www.google.com'})
 ```
 
-Or pass the arguments directly into the object:
+![import](images/import.png)
+
+Or pass you can use the `argparse` library to parse the arguments:
 
 ```python
-from get_certificate_chain import SSLCertificateChainDownloader
-args = {'domain': 'www.google.com'}
+import argparse
+from get_certificate_chain.download import SSLCertificateChainDownloader
+
+# Add your arguments
+args = parser.parse_args()
+
 downloader = SSLCertificateChainDownloader()
 downloader.run(args)
 ```
 
-![import](images/import.png)
-
 ### Command Line CLI
 
 To use the script from the command line, run the following command:
 
 ```bash
-get-certificate-chain --domain www.google.com
+get-certificate-chain --url www.google.com
 ```
 
 ![cli](images/cli.png)
 
 #### Arguments
 
-- `--domain`: The domain:port pair that the script should connect to. Defaults to www.google.com:443.
-- `--rm-ca-files`: Remove the certificate files in the current working directory (*.crt, *.pem).
+- `--url`: The url:port pair that the script should connect to. Defaults to www.google.com:443.
+- `--rm-ca-files`: Remove the certificate files in the current working directory (`*.crt`, `*.pem`).
 - `--get-ca-cert-pem`: Get cacert.pem from the curl.se website to help find Root CA.
 
 ## Contributing
 
 Contributions are welcome! To contribute, please follow these guidelines:
 
 1. Write tests for your code using `pytest`. Make sure your tests follow the standards set by the existing tests.
```

### Comparing `get_certificate_chain-0.1.2/get_certificate_chain/main.py` & `get_certificate_chain-0.1.3/get_certificate_chain/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 import logging
 import re
 import ssl
 import socket
 import sys
 from typing import Any, Dict, List, Union
 from urllib.request import urlopen
+from urllib.error import HTTPError, URLError
 
 # Third-party library imports
 import argparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.x509.oid import ExtensionOID
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 CERT_CHAIN = []
 
 # Configure logging
 logging.basicConfig(
     level=logging.WARNING, format="%(asctime)s [%(levelname)s] %(message)s"
 )
 
 
 # parse arguments
-def parse_arguments():
+def parse_arguments() -> argparse.Namespace:
     """
     Parse command line arguments.
 
     Returns:
         argparse.Namespace: Parsed arguments.
     """
     parser = argparse.ArgumentParser(
@@ -54,18 +55,18 @@
     parser.add_argument(
         "--get-ca-cert-pem",
         dest="get_ca_cert_pem",
         action="store_true",
         help="Get cacert.pem from curl.se website to help find Root CA.",
     )
     parser.add_argument(
-        "--domain",
-        dest="domain",
+        "--url",
+        dest="url",
         default="www.google.com",
-        help="The hostname to connect to. (default: %(default)s)",
+        help="The url to connect to. (default: %(default)s)",
     )
     return parser.parse_args()
 
 
 class SSLCertificateChainDownloader:
     def __init__(self):
         self.cert_chain = []
@@ -96,58 +97,58 @@
                     response.getcode(),
                 )
                 sys.exit(1)
             data = response.read()
             out_file.write(data)
         logging.info("Downloaded %s to %s", cacert_pem_url, cacert_pem_file)
 
-    def check_domain(self) -> Dict[str, Any]:
+    def check_url(self) -> Dict[str, Any]:
         """
-        Check and parse the domain provided by the user.
+        Check and parse the url provided by the user.
 
         Args:
-            domain (str): The domain provided by the user.
+            url (str): The url provided by the user.
 
         Returns:
-            Dict[str, Any]: A dictionary containing the hostname and port.
+            Dict[str, Any]: A dictionary containing the url and port.
         """
-        hostname, _, port = self.domain.partition(":")
-        return {"hostname": hostname, "port": int(port) if port else 443}
+        url, _, port = self.url.partition(":")
+        return {"url": url, "port": int(port) if port else 443}
 
-    def get_certificate(self, hostname: str, port: int) -> x509.Certificate:
+    def get_certificate(self, url: str, port: int) -> x509.Certificate:
         """
         Connect to a server and retrieve the SSL certificate.
 
         Args:
-            hostname (str): The hostname to connect to.
+            url (str): The url to connect to.
             port (int): The port to connect to.
 
         Returns:
             x509.Certificate: The SSL certificate of the server.
         """
         try:
             context = ssl.create_default_context()
-            with socket.create_connection((hostname, port)) as sock:
-                with context.wrap_socket(sock, server_hostname=hostname) as ssl_socket:
+            with socket.create_connection((url, port)) as sock:
+                with context.wrap_socket(sock, server_hostname=url) as ssl_socket:
                     cert_pem = ssl.DER_cert_to_PEM_cert(ssl_socket.getpeercert(True))
                     cert = x509.load_pem_x509_certificate(
                         cert_pem.encode(), default_backend()
                     )
             return cert
         except ConnectionRefusedError:
-            print(f"Connection refused to {hostname}:{port}")
+            logging.error("Connection refused to %s:%s", url, port)
             sys.exit(1)
         except ssl.SSLError as e:
-            print(f"SSL error: {e}")
+            logging.error("SSL error: %s", e)
             sys.exit(1)
         except socket.timeout:
-            print(f"Connection timed out to {hostname}:{port}")
+            logging.error("Connection timed out to %s:%s", url, port)
             sys.exit(1)
         except socket.gaierror:
-            print(f"Hostname could not be resolved: {hostname}")
+            logging.error("Hostname could not be resolved: %s", url)
             sys.exit(1)
 
     def normalize_subject(self, subject: str) -> str:
         """
         Normalize the subject of a certificate.
 
         Args:
@@ -230,15 +231,15 @@
                     return None
                 aia_content = response.read()
                 ssl_certificate = ssl.DER_cert_to_PEM_cert(aia_content)
                 cert = x509.load_pem_x509_certificate(
                     ssl_certificate.encode("ascii"), default_backend()
                 )
                 return cert
-        except Exception:
+        except (HTTPError, URLError):
             return None
 
     def return_cert_aia_list(self, ssl_certificate: x509.Certificate) -> list:
         """
         Get the list of AIA URIs from a certificate.
 
         Args:
@@ -342,15 +343,15 @@
                 )
                 root_ca_name = cert.subject.rfc4514_string()
 
                 ca_root_store[root_ca_name] = root_ca_cert
             else:
                 index += 1
 
-        print(f"Number of Root CA's loaded: {len(ca_root_store)}")
+        logging.info("Number of Root CAs loaded: %d", len(ca_root_store))
         return ca_root_store
 
     def walk_the_chain(
         self,
         ssl_certificate: x509.Certificate,
         depth: int,
         max_depth: int = 4,
@@ -406,23 +407,23 @@
 
                     if root_ca_cn is None:
                         logging.error("Root CA NOT found.")
                         sys.exit(1)
 
     def run(self, args: Union[argparse.Namespace, dict]):
         if isinstance(args, argparse.Namespace):
-            self.domain = args.domain
+            self.url = args.url
         elif isinstance(args, dict):
-            self.domain = args.get("domain")
+            self.url = args.get("url")
         else:
             raise ValueError(
                 "Invalid argument type. Expected argparse.Namespace or dict."
             )
 
-        self.parsed_domain = self.check_domain()
+        self.parsed_url = self.check_url()
 
         if isinstance(args, argparse.Namespace):
             remove_ca_files = args.remove_ca_files
             get_ca_cert_pem = args.get_ca_cert_pem
         else:
             remove_ca_files = args.get("remove_ca_files")
             get_ca_cert_pem = args.get("get_ca_cert_pem")
@@ -430,15 +431,15 @@
         if remove_ca_files:
             self.remove_ca_files()
 
         if get_ca_cert_pem:
             self.get_ca_cert_pem()
 
         ssl_certificate = self.get_certificate(
-            self.parsed_domain["hostname"], self.parsed_domain["port"]
+            self.parsed_url["url"], self.parsed_url["port"]
         )
 
         aia = self.return_cert_aia(ssl_certificate)
 
         if aia is not None and not self.return_cert_aia(ssl_certificate):
             logging.error(
                 "Could not find AIA, possible decryption taking place upstream?"
```

### Comparing `get_certificate_chain-0.1.2/get_certificate_chain/tests/test_cert.py` & `get_certificate_chain-0.1.3/get_certificate_chain/tests/test_cert.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 def cert_data(root_ca_cert, server_cert):
     return {
         "ca_cert_text": root_ca_cert,
         "cert_text": server_cert,
     }
 
 
-def test_check_domain():
+def test_check_url():
     downloader = SSLCertificateChainDownloader()
 
     # Test without port
-    downloader.domain = "www.google.com"
-    domain = downloader.check_domain()
-    assert domain == {"hostname": "www.google.com", "port": 443}
+    downloader.url = "www.google.com"
+    url = downloader.check_url()
+    assert url == {"url": "www.google.com", "port": 443}
 
     # Test with port
-    downloader.domain = "www.google.com:8443"
-    domain = downloader.check_domain()
-    assert domain == {"hostname": "www.google.com", "port": 8443}
+    downloader.url = "www.google.com:8443"
+    url = downloader.check_url()
+    assert url == {"url": "www.google.com", "port": 8443}
 
 
 def test_normalize_subject():
     downloader = SSLCertificateChainDownloader()
 
     subject = "/C=US/ST=California/L=Mountain View/O=Google LLC/CN=www.google.com"
     assert (
```

### Comparing `get_certificate_chain-0.1.2/get_certificate_chain/tests/test_data/server.cnf` & `get_certificate_chain-0.1.3/get_certificate_chain/tests/test_data/server.cnf`

 * *Files identical despite different names*

### Comparing `get_certificate_chain-0.1.2/pyproject.toml` & `get_certificate_chain-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "get_certificate_chain"
-version = "0.1.2"
+version = "0.1.3"
 description = "Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files."
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>", " TheScriptGuy <@nolanrumble>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-cryptography = "^40.0.2"
+python = "^3.9"
+cryptography = "^40.0.1"
 argparse = "^1.4.0"
 pytest = "^7.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 pytest-black = "^0.3.12"
@@ -20,12 +20,12 @@
 ipython = "^8.12.0"
 ipdb = "^0.13.13"
 requests = "^2.28.2"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 
 [tool.poetry.scripts]
-get-certificate-chain = "get_certificate_chain.main:main"
+get-certificate-chain = "get_certificate_chain.download:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `get_certificate_chain-0.1.2/PKG-INFO` & `get_certificate_chain-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: get-certificate-chain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Project to help use the breadcrumbs that are left by the certificate to build the chain and output it into files.
 License: MIT
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: cryptography (>=40.0.1,<41.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Get Certificate Chain 🌐🔐
 
+[![PyTests](https://github.com/cdot65/get_certificate_chain/actions/workflows/tests.yml/badge.svg)](https://github.com/cdot65/get_certificate_chain/actions/workflows/tests.yml)
+
 This Python script retrieves the certificate chain from a website, allowing you to analyze and verify the SSL/TLS certificates of the website. This project is a custom fork of the [getCertificateChain project](https://github.com/TheScriptGuy/getCertificateChain), and the overwhelming majority of credit goes to [TheScriptGuy](https://github.com/TheScriptGuy).
 
 ## Table of Contents
 
 - [Get Certificate Chain 🌐🔐](#get-certificate-chain-)
   - [Table of Contents](#table-of-contents)
   - [Requirements 📋](#requirements-)
@@ -31,15 +35,15 @@
     - [Command Line CLI](#command-line-cli)
       - [Arguments](#arguments)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Requirements 📋
 
-- Python 3.10+
+- Python 3.9+
 - Poetry (optional) - [Python Poetry](https://python-poetry.org/docs/)
 
 ## Installation
 
 ### PyPi
 
 To install the package from PyPi, simply run the appropriate command.
@@ -68,65 +72,63 @@
 
 To use the package in your script, simply import the package and create an instance of the `SSLCertificateChainDownloader` object.
 
 To pass arguments into the object, you can use the `argparse` library:
 
 1. Import the argparse library.
 2. Import the SSLCertificateChainDownloader object from the package.
-3. Create an argument parser with a description.
-4. Add your arguments.
-5. Parse the arguments.
-6. Create an instance of the SSLCertificateChainDownloader object.
-7. Run the downloader object with the parsed arguments.
+3. Create a python dictionary with the "url" key and value of the domain.
+4. Create an instance of the SSLCertificateChainDownloader object.
+5. Run the downloader object with the parsed arguments.
 
 ```python
-from get_certificate_chain import SSLCertificateChainDownloader
+from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
 # Use the downloader object for your needs
 ```
 
-To pass arguments into the object, you can use the `argparse` library:
+You can pass the arguments directly into the object:
 
 ```python
-import argparse
-from get_certificate_chain import SSLCertificateChainDownloader
-
-# Add your arguments
-args = parser.parse_args()
+from get_certificate_chain.download import SSLCertificateChainDownloader
 
 downloader = SSLCertificateChainDownloader()
-downloader.run(args)
+downloader.run({'url': 'www.google.com'})
 ```
 
-Or pass the arguments directly into the object:
+![import](images/import.png)
+
+Or pass you can use the `argparse` library to parse the arguments:
 
 ```python
-from get_certificate_chain import SSLCertificateChainDownloader
-args = {'domain': 'www.google.com'}
+import argparse
+from get_certificate_chain.download import SSLCertificateChainDownloader
+
+# Add your arguments
+args = parser.parse_args()
+
 downloader = SSLCertificateChainDownloader()
 downloader.run(args)
 ```
 
-![import](images/import.png)
-
 ### Command Line CLI
 
 To use the script from the command line, run the following command:
 
 ```bash
-get-certificate-chain --domain www.google.com
+get-certificate-chain --url www.google.com
 ```
 
 ![cli](images/cli.png)
 
 #### Arguments
 
-- `--domain`: The domain:port pair that the script should connect to. Defaults to www.google.com:443.
-- `--rm-ca-files`: Remove the certificate files in the current working directory (*.crt, *.pem).
+- `--url`: The url:port pair that the script should connect to. Defaults to www.google.com:443.
+- `--rm-ca-files`: Remove the certificate files in the current working directory (`*.crt`, `*.pem`).
 - `--get-ca-cert-pem`: Get cacert.pem from the curl.se website to help find Root CA.
 
 ## Contributing
 
 Contributions are welcome! To contribute, please follow these guidelines:
 
 1. Write tests for your code using `pytest`. Make sure your tests follow the standards set by the existing tests.
```

