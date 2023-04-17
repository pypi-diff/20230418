# Comparing `tmp/avsos-0.0.2.tar.gz` & `tmp/avsos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.2.tar", last modified: Mon Apr 17 21:51:43 2023, max compression
+gzip compressed data, was "avsos-0.0.3.tar", last modified: Mon Apr 17 22:08:54 2023, max compression
```

## Comparing `avsos-0.0.2.tar` & `avsos-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.825697 avsos-0.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:51:43.825697 avsos-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1469 2023-04-17 20:18:08.000000 avsos-0.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.821695 avsos-0.0.2/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.2/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.2/avsos/config.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.2/avsos/encryption.py
--rw-r--r--   0 kali      (1000) kali      (1000)    17220 2023-04-17 20:20:28.000000 avsos-0.0.2/avsos/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.2/avsos/osint.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5574 2023-04-17 10:41:29.000000 avsos-0.0.2/avsos/portscan.py
--rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.2/avsos/setup.py
--rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.2/avsos/start_zap.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.2/avsos/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5521 2023-04-17 20:22:12.000000 avsos-0.0.2/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.825697 avsos-0.0.2/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      108 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 21:51:43.825697 avsos-0.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-17 21:51:37.000000 avsos-0.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.061499 avsos-0.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 22:08:54.061499 avsos-0.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1469 2023-04-17 20:18:08.000000 avsos-0.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.053503 avsos-0.0.3/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.3/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.3/avsos/config.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.3/avsos/encryption.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    17539 2023-04-17 22:03:35.000000 avsos-0.0.3/avsos/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.3/avsos/osint.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5577 2023-04-17 22:07:00.000000 avsos-0.0.3/avsos/portscan.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.3/avsos/setup.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.3/avsos/start_zap.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.3/avsos/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5485 2023-04-17 22:04:18.000000 avsos-0.0.3/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.061499 avsos-0.0.3/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      117 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 22:08:54.061499 avsos-0.0.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-17 22:07:25.000000 avsos-0.0.3/setup.py
```

### Comparing `avsos-0.0.2/README.md` & `avsos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `avsos-0.0.2/avsos/config.py` & `avsos-0.0.3/avsos/config.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.2/avsos/encryption.py` & `avsos-0.0.3/avsos/encryption.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.2/avsos/main.py` & `avsos-0.0.3/avsos/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -217,87 +217,86 @@
 
     if args.subdomains_file:
         try:
             with open(args.subdomains_file, "r") as f:
                 subdomains = f.read().splitlines()
                 if not target:  # If the target is None, use the first subdomain from the file
                     target = subdomains[0]
-                logging.debug("Running Amass on subdomains...") # run amass on domains in file
+                logging.debug("Running Amass on subdomains...")  # run amass on domains in file
                 print("\nRunning Amass on subdomains...")
                 # Run Amass on subdomains file
                 amass_output = subprocess.run(["amass", "enum", "-df", args.subdomains_file], check=True, text=True)
                 amass_results = amass_output.stdout.splitlines()
                 subdomains = amass_results
                 report_data["File Subdomains"] = subdomains
         except FileNotFoundError:
             print(f"Error: File {args.subdomains_file} not found.")
 
     if args.enum or args.all:  # subdomain enumeration
         try:
-		    if args.whois or args.all:
-		        # Run Amass and Whois concurrently
-		        with concurrent.futures.ThreadPoolExecutor() as executor:
-		            amass_future = executor.submit(osint.amass, target)
-		            whois_future = executor.submit(osint.get_whois_info, target)
-
-		        subdomains = amass_future.result()
-		        whois_info = whois_future.result()
-		        report_data["Subdomains"] = subdomains
-		        formatted_whois_info = osint.format_whois_output(whois_info)
-		        print(formatted_whois_info)
-		        domains_at_risk_list = osint.check_domain_hijacking(whois_info)
-		        domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
-		        report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
-		        report_data["Domains at risk of hijacking"] = domains_at_risk_text
-		    else:
-		        logging.debug("Running Amass...")
-		        print("\nRunning Amass...")
-		        subdomains = osint.amass(target)
-		        report_data["Subdomains"] = subdomains
-		 except Exception as e:
-		 	print(f"Error running the selected scans: {e}")
+            if args.whois or args.all:
+                # Run Amass and Whois concurrently
+                with concurrent.futures.ThreadPoolExecutor() as executor:
+                    amass_future = executor.submit(osint.amass, target)
+                    whois_future = executor.submit(osint.get_whois_info, target)
+
+                subdomains = amass_future.result()
+                whois_info = whois_future.result()
+                report_data["Subdomains"] = subdomains
+                formatted_whois_info = osint.format_whois_output(whois_info)
+                print(formatted_whois_info)
+                domains_at_risk_list = osint.check_domain_hijacking(whois_info)
+                domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
+                report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
+                report_data["Domains at risk of hijacking"] = domains_at_risk_text
+            else:
+                logging.debug("Running Amass...")
+                print("\nRunning Amass...")
+                subdomains = osint.amass(target)
+                report_data["Subdomains"] = subdomains
+        except Exception as e:
+            print(f"Error running the selected scans: {e}")
     elif args.whois or args.all:
         try:
-		    logging.debug("Running WHOIS...")
-		    print("\nRunning Whois...")
-		    whois_info = osint.get_whois_info(target)
-		    formatted_whois_info = osint.format_whois_output(whois_info)
-		    print(formatted_whois_info)
-		    domains_at_risk_list = osint.check_domain_hijacking(whois_info)
-		    domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
-		    report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
-		    report_data["Domains at risk of hijacking"] = domains_at_risk_text
+            logging.debug("Running WHOIS...")
+            print("\nRunning Whois...")
+            whois_info = osint.get_whois_info(target)
+            formatted_whois_info = osint.format_whois_output(whois_info)
+            print(formatted_whois_info)
+            domains_at_risk_list = osint.check_domain_hijacking(whois_info)
+            domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
+            report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
+            report_data["Domains at risk of hijacking"] = domains_at_risk_text
         except Exception as e:
-		 	print(f"Error running the selected scans: {e}")
+            print(f"Error running the selected scans: {e}")
 
     if args.zap or args.all:
         try:
-		    logging.debug("Running ZAP...")
-		    print("\nRunning ZAP Scan...")
-		    if api_key is None:
-		        print("Error retrieving ZAP API key.")
-		        return
-		    zap_process = zapscan.start_zap(zap_path)
-		    if zap_process is None:
-		        print("Error starting ZAP.")
-		        return
-		    zap = zapscan.run_zap_scan(target, api_key,
-		                               subdomains)  # add option of adding api key to config file and using that
-		    print("\nZAP Complete")
-
-		    zap_results_str, zap_alerts = zapscan.zap_report(zap)
-		    report_data['ZAP Scan'] = zap_results_str  # Add ZAP scan results to report_data
-		    # Generate the graph file name using the target and a timestamp
-		    graph_file = f"{target}_graph_{datetime.now().strftime('%H%M%S')}.png"
-		    # Plot the graph
-		    severity_counts = utils.count_severity(zap_alerts)
-		    zapscan.plot_graph(severity_counts, graph_file)
+            logging.debug("Running ZAP...")
+            print("\nRunning ZAP Scan...")
+            if api_key is None:
+                print("Error retrieving ZAP API key.")
+                return
+            zap_process = zapscan.start_zap(zap_path)
+            if zap_process is None:
+                print("Error starting ZAP.")
+                return
+            zap = zapscan.run_zap_scan(target, api_key,
+                                       subdomains)  # add option of adding api key to config file and using that
+            print("\nZAP Complete")
+
+            zap_results_str, zap_alerts = zapscan.zap_report(zap)
+            report_data['ZAP Scan'] = zap_results_str  # Add ZAP scan results to report_data
+            # Generate the graph file name using the target and a timestamp
+            graph_file = f"{target}_graph_{datetime.now().strftime('%H%M%S')}.png"
+            # Plot the graph
+            severity_counts = utils.count_severity(zap_alerts)
+            zapscan.plot_graph(severity_counts, graph_file)
         except Exception as e:
-		 	print(f"Error running the selected scans: {e}")
-                
+            print(f"Error running the selected scans: {e}")
 
     if args.nmap or args.all:
         logging.debug("Running NMAP...")
         print("\nRunning Nmap on the main domain...")
         try:
             all_open_ports, all_vulnerabilities, all_headers = portscan.run_nmap(target, only_vulners=False)
             unexpected_services = portscan.compare_services(target, all_open_ports)
@@ -314,42 +313,44 @@
         except Exception as e:
             print(f"Error running Nmap on {target}: {e}")
             traceback.print_exc()
 
         # Run Nmap on subdomains if they exist
         if subdomains:
             logging.debug("\nRunning Nmap on subdomains...")
-		        try:
-		        print("\nRunning Nmap on subdomains...")
-		        subdomain_all_open_ports, subdomain_all_vulnerabilities, subdomain_all_headers = portscan.run_nmap(subdomains,
-		                                                                                                           only_vulners=True)
-		        subdomain_nmap_data = {
-		            'open_ports': subdomain_all_open_ports,
-		            'vulnerabilities': subdomain_all_vulnerabilities,
-		            'headers': subdomain_all_headers
-		        }
-		        # Add the subdomains Nmap scan results to the report_data
-		        subdomain_nmap_report_str = portscan.print_report(subdomain_nmap_data)
-		        print(subdomain_nmap_report_str)
-		        report_data['Port Scan']['Subdomains'] = subdomain_nmap_report_str
+            try:
+                print("\nRunning Nmap on subdomains...")
+                subdomain_all_open_ports, subdomain_all_vulnerabilities, subdomain_all_headers = portscan.run_nmap(
+                    subdomains,
+                    only_vulners=True)
+                subdomain_nmap_data = {
+                    'open_ports': subdomain_all_open_ports,
+                    'vulnerabilities': subdomain_all_vulnerabilities,
+                    'headers': subdomain_all_headers
+                }
+                # Add the subdomains Nmap scan results to the report_data
+                subdomain_nmap_report_str = portscan.print_report(subdomain_nmap_data)
+                print(subdomain_nmap_report_str)
+                report_data['Port Scan']['Subdomains'] = subdomain_nmap_report_str
             except Exception as e:
-		 		print(f"Error running the selected scans: {e}")
+                print(f"Error running the selected scans: {e}")
+
 
     if args.debug:
         utils.enable_debugging()
 
     if args.encrypt_file:
         encryption.encrypt_existing_file(args.encrypt_file)
         return
 
     if args.decrypt:  # Check if the user wants to decrypt a file
         try:
-        	encryption.decrypt_report(args.encrypted_file, args.decrypted_file, args.key)
+            encryption.decrypt_report(args.encrypted_file, args.decrypted_file, args.key)
         except Exception as e:
-		 	print(f"Error: {e}")
+            print(f"Error: {e}")
         return  # Exit the program after decryption
 
     if args.output or args.all:
         if report_data:
             output_file = args.output
             encrypted_output_file = f"{args.output}_encrypted.txt"
 
@@ -368,14 +369,15 @@
                 # Save report in user-specified format
                 save_report(report_data, file_format, output_file, graph_file=graph_file)
                 print(f"\nReport saved as {output_file}")
         else:
             print("No previous scans were run. Please run OSINT or Vulnerabilty scans before generating reports!")
     return report_data
 
+
 def main():
     global api_key
     args = parse_arguments()
     logging.debug("Parsed arguments: %s", args)
 
     config = configparser.ConfigParser()
     config.read("config.ini")
```

### Comparing `avsos-0.0.2/avsos/osint.py` & `avsos-0.0.3/avsos/osint.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.2/avsos/portscan.py` & `avsos-0.0.3/avsos/portscan.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             port = port_info["port"]
             service = port_info["service"]
             if port in expected_services and expected_services[port] != service.lower():
                 unexpected_services.append({"port": port, "service": service})
 
     if not unexpected_services:
         for ports in all_open_ports.items():
-        	print(f"- Port: {port}, Service: {service}")
+            print(f"- Port: {port}, Service: {service}")
         print(f"\nAll open ports on {url} match expected services.")
     else:
         print(f"\nFound {len(unexpected_services)} unexpected service(s) on {url}:")
         for service_info in unexpected_services:
             port = service_info["port"]
             service = service_info["service"]
             print(f"- Port: {port}, Service: {service}")
```

### Comparing `avsos-0.0.2/avsos/utils.py` & `avsos-0.0.3/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.2/avsos/zapscan.py` & `avsos-0.0.3/avsos/zapscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import time
 from zapv2 import ZAPv2
 import subprocess
-import json
 import utils
 import matplotlib.pyplot as plt
 import datetime
 import logging
-import os
-import signal
 import sys
 
 logging.basicConfig(filename="zapscan.log", level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
 
 def start_zap(zap_path):
     python_executable = sys.executable
     zap_process = subprocess.Popen([python_executable, zap_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
```

