# Comparing `tmp/watchtower_browser_testing-0.4.0.tar.gz` & `tmp/watchtower_browser_testing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.0.tar", last modified: Tue Apr 18 07:09:16 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.1.tar", last modified: Tue Apr 18 07:11:40 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.0.tar` & `watchtower_browser_testing-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.631347 watchtower_browser_testing-0.4.0/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6148 2023-04-18 07:09:05.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-18 07:08:06.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6149 2023-04-18 07:11:24.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-18 07:11:33.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:11:40.640031 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-18 07:11:40.000000 watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.0/setup.py` & `watchtower_browser_testing-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                                                 {% if test_result.css_id==event.id and not test_result.ok %}
                                                 <div class="alert alert-danger" role="alert" style="margin-top:1rem;">
                                                     <svg xmlns="http://www.w3.org/2000/svg" width="1.2rem" height="1.2rem" fill="currentColor" class="bi bi-exclamation-triangle alert_exclamation" viewBox="0 0 16 16" style="float:left;">
                                                         <path d="M7.938 2.016A.13.13 0 0 1 8.002 2a.13.13 0 0 1 .063.016.146.146 0 0 1 .054.057l6.857 11.667c.036.06.035.124.002.183a.163.163 0 0 1-.054.06.116.116 0 0 1-.066.017H1.146a.115.115 0 0 1-.066-.017.163.163 0 0 1-.054-.06.176.176 0 0 1 .002-.183L7.884 2.073a.147.147 0 0 1 .054-.057zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/>
                                                         <path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/>
                                                     </svg>
                                                     <details>
-                                                    <summary style="list-style: none">Test failed for browser <strong>{ test_result.browser }}</strong></summary>
+                                                    <summary style="list-style: none">Test failed for browser <strong>{{ test_result.browser }}</strong></summary>
                                                     {{ test_result.errors }}
                                                     </details>
                                                 </div>
                                                 {% endif %}
                                             {% endfor %}
                                         {% endif %}
                                     </div>
```

#### html2text {}

```diff
@@ -12,12 +12,12 @@
 ** Tests **
 {% for scenario in test.children %}
 {{ scenario.description }} {% if scenario.children %} {% for event in
 scenario.children %}
 {{ event.description }} {% if test_results %} {% for test_result in
 test_results.results %} {% if test_result.css_id==event.id and not
 test_result.ok %}
-     Test failed for browser { test_result.browser }} {{ test_result.errors }}
+     Test failed for browser {{ test_result.browser }} {{ test_result.errors }}
 {% endif %} {% endfor %} {% endif %}
 {% endfor %} {% endif %}
 {% endfor %}
 {% endfor %}
```

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.1/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

