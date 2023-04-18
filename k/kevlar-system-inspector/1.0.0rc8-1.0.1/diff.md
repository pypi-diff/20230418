# Comparing `tmp/kevlar-system-inspector-1.0.0rc8.tar.gz` & `tmp/kevlar-system-inspector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-vfb17x5a/kevlar-system-inspector-1.0.0rc8.tar", last modified: Fri Apr 14 17:39:27 2023, max compression
+gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-y4s_az4f/kevlar-system-inspector-1.0.1.tar", last modified: Tue Apr 18 21:22:58 2023, max compression
```

## Comparing `kevlar-system-inspector-1.0.0rc8.tar` & `kevlar-system-inspector-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3682 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2650 2023-04-14 17:36:14.000000 kevlar-system-inspector-1.0.0rc8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/scripts/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/scripts/kevlar-system-inspector
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/
--rw-rw-rw-   0 root         (0) root         (0)     6110 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16848 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/console.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6470 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/output.py
--rw-rw-rw-   0 root         (0) root         (0)     8240 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/resources/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/failures.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/html5-template.txt
--rw-rw-rw-   0 root         (0) root         (0)     3215 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/report.rst
--rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/starlab.css
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/warnings.rst
--rw-rw-rw-   0 root         (0) root         (0)     9440 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_allowlisting.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6077 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_offline_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_secure_dns.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/kconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/mount.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/workdir.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3682 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/scripts/kevlar-system-inspector
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16848 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6470 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     8240 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/failures.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/html5-template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/report.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/starlab.css
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/warnings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9266 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_allowlisting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12847 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2978 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_offline_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_secure_dns.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/kconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/mount.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/top_level.txt
```

### Comparing `kevlar-system-inspector-1.0.0rc8/LICENSE` & `kevlar-system-inspector-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/PKG-INFO` & `kevlar-system-inspector-1.0.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,55 @@
-Metadata-Version: 2.1
-Name: kevlar-system-inspector
-Version: 1.0.0rc8
-Summary: A security scanner for Linux systems
-Home-page: https://www.starlab.io/explore-kevlar-system-inspector
-Author: Star Lab
-Author-email: info@starlab.io
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Security
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-License-File: LICENSE
-
 .. image:: https://inspector.starlab.io/kevlar-system-inspector-logo.svg
    :align: center
    :width: 75%
 
 ======================================================================
 Star Lab Kevlar System Inspector: A Security Scanner for Linux Systems
 ======================================================================
 
 Kevlar System Inspector is an embedded security test suite that grew out of
 `Star Lab's`_ extensive experience assessing and protecting mission-critical
 systems for the U.S. Government.  These test have been made available for
 public use to help identify security issues in a variety of Linux systems.  The
 set of tests present in Kevlar System Inspector will be expanded as adversary
-techniques and tactics change, and as we continue development of `KES`_.
+techniques and tactics change, and as we continue development of `Kevlar
+Embedded Security`_.
 
 These tests are generally more aggressive than other security scanning tools: We
 prefer to probe behavior rather than check configurations values. However, we
 do not include any actual exploit code or include any tests that could
 destabilize the system. (And of course, we check configuration values too.)
 
 .. _Star Lab's: https://www.starlab.io
-.. _KES: https://www.starlab.io/kevlar-embedded-security
+.. _Kevlar Embedded Security: https://www.starlab.io/kevlar-embedded-security
 
 
 System Requirements
 ===================
 
-Kevlar System Inspector requires Python 3.8 or higher. Our emphasis is on
-embedded Linux distros (Yocto-based), but Kevlar System Inspector is a pure
-Python project that should run on most modern Linux distros.
+Kevlar System Inspector requires Python 3.8 or higher.
+
+It is designed to be run in an embedded Linux test environment, but it is a
+Python project that can run on most modern Linux distros, including desktop
+distributions.
 
 
 Installation
 ============
 
 We provide several methods for installation:
 
 
 Install from PyPI
 -----------------
 
 If your system is capable of installing packages from PyPI, Kevlar System
-Inspector may be installed using ``pip``.
-
-Because Kevlar System Inspector should be run as root, we suggest using ``pip``
-to install to a virtual environment:
+Inspector may be installed using ``pip``. Because Kevlar System Inspector is
+designed to be run as root in a test environment, we suggest using ``pip`` to
+install to a virtual environment. (Note that running as root is not required.)
 
 .. code-block:: console
 
    $ python3 -m venv kevlar-venv
    $ ./kevlar-venv/bin/pip install kevlar-system-inspector
    $ sudo ./kevlar-venv/bin/kevlar-system-inspector
 
@@ -94,8 +69,45 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0rc8.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.1.tar.gz
+
+
+Running as Root
+===============
+
+Although running as root is not necessary, Kevlar System Inspector is designed
+to be run as root in a embedded test environment for two reasons:
+
+* Some tests (for example, kernel module loading) require root permissions to
+  perform.
+* The Kevlar Embedded Security threat model is a defense in depth model that
+  includes compromised root processes and malicious insiders.
+
+Kevlar System Inspector does not include any malicious code or tests that would
+destabilize the system. It uses root access to:
+
+* Probe kernel features and configurations in different ways.
+* Test the reaction of the system to (benign) files dropped in privileged
+  locations.
+* Inspect logical volume mangement configuration.
+
+
+HTML Report Output
+==================
+
+Kevlar System Inspector may be run with the option
+``--output-html=<filename.html>`` to produce a self-contained HTML report.
+
+
+Uninstalling
+============
+
+If installed through ``pip``, Kevlar System Inspector may be uninstalled using
+the command ``pip uninstall``. If it was installed in a virtual environment, or
+if the standalone tarball version was used, simply deleting the directory
+removes Kevlar System Inspector from the system. It does not permanently leave
+files anywhere else on the system.
```

### Comparing `kevlar-system-inspector-1.0.0rc8/setup.cfg` & `kevlar-system-inspector-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kevlar-system-inspector
-version = 1.0.0rc8
+version = 1.0.1
 author = Star Lab
 author_email = info@starlab.io
 url = https://www.starlab.io/explore-kevlar-system-inspector
 license = MIT
 license_files = LICENSE
 description = A security scanner for Linux systems
 long_description = file: README.rst
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__init__.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/conftest.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/conftest.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/console.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/console.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/decorators.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/decorators.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/output.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/output.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/report.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/report.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/sysinfo.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/sysinfo.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/failures.rst` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/failures.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/report.rst` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/report.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/starlab.css` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/starlab.css`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_allowlisting.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_allowlisting.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,30 +121,26 @@
     """
     A copied binary should not work
     ===============================
 
     Only official binaries should be runnable, no matter how benign. This check
     simply copies a binary such as /bin/true to a temporary directory and
     executes it.
-
-    See :kevlar-code:`200`.
     """
 
     with raises(PermissionError, "Was able to run an unauthorized binary"):
         subprocess.run([cat], stdin=subprocess.DEVNULL)
 
 
 def test_attempt_to_preload_unauthorized_library(dynamic_cat: Path, libc: Path) -> None:
     """
     Users should not be able to inject into binaries using ``LD_PRELOAD``
     =====================================================================
 
     ``LD_PRELOAD`` allows injection of arbitrary code into a process.
-
-    See :kevlar-code:`200`.
     """
     # Doesn't prevent running, just preloading the library.
     process = subprocess.Popen(
         ["cat"], env={"LD_PRELOAD": libc}, stdin=subprocess.PIPE, stdout=subprocess.PIPE
     )
 
     with process:
@@ -174,16 +170,14 @@
 def test_attempt_to_intercept_system_library(dynamic_cat: Path, libc: Path) -> None:
     """
     Users should not be able to hijack authorized shared libraries
     ==============================================================
 
     ``LD_LIBRARY_PATH`` allows injecting arbitrary code into a process by
     impersonating a legitimate library.
-
-    See :kevlar-code:`200`.
     """
 
     # Quick tests show this won't work with musl, since the loader and libc are
     # the same binary. We would need to choose another library/binary combo, which
     # comes with its own portability issues. So for now this is a TODO. The combo
     # LD_PRELOAD/LD_LIBRARY_PATH below should do it though.
 
@@ -202,16 +196,14 @@
 ) -> None:
     """
     Users should not be able to inject code with environment variables
     ==================================================================
 
     ``LD_LIBRARY_PATH`` and ``LD_PRELOAD`` allow injecting arbitrary code into
     a process. This test uses them together.
-
-    See :kevlar-code:`200`.
     """
 
     libz_name = "libz.so.1"
     libz_src = _resolve_system_lib(libz_name)
     if not libz_src:
         warnings.warn("Unable to find libz for testing.")
         pytest.skip()
@@ -246,16 +238,14 @@
 
 
 @pytest.mark.requires_root
 def test_attempt_to_overwrite_system_binary() -> None:
     """
     Users should not be able to modify protected locations
     ======================================================
-
-    See :kevlar-code:`200`.
     """
     # Can get different errors depending on what other defenses are enabled
     # (i.e., dm-verity)
 
     # Don't trust shutil.copy for two reasons:
     #   1) It does not guarantee an atomic operation, and we don't want to
     #   brick the system if we can't complete the write.
@@ -284,11 +274,9 @@
 
 
 @full_version_only
 def test_attempt_to_run_new_binary() -> None:
     """
     Users should not be able to drop and execute a crafted binary
     =============================================================
-
-    See :kevlar-code:`200`.
     """
     ...
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_config.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 --------------------------------------
 Kernel Hardening: Kernel Configuration
 --------------------------------------
 
 The Linux kernel should be configured to minimize the potential attack surface
 and provide exploit mitigations where possible.
 
+See :kevlar-code:`300`.
 """
 
 from collections import defaultdict
 import errno
 import subprocess
 import warnings
 import os
@@ -287,16 +288,14 @@
     =============================================
 
     There are many knobs to turn when configuring the Linux kernel for your
     needs. Many of these knobs provide extra security or have subtle security
     implications.
 
     {{description | dedent}}
-
-    See :kevlar-code:`300`.
     """
 
     if not value:
         config = f"# {name} is not set"
         message = f"{name} should not be configured"
     else:
         config = f"{name}={value}"
@@ -319,16 +318,14 @@
     flag: str, reason: str, kernel_cmdline: List[str], kconfig: KconfigSet
 ) -> None:
     """
     Enable kernel heap checks
     =========================
 
     Kernel heap checking must be enabled both via config and via command line.
-
-    See :kevlar-code:`300`.
     """
 
     if "CONFIG_SLUB_DEBUG=y" not in kconfig:
         pytest.skip("Prerequisites not met")
 
     for arg in kernel_cmdline:
         if arg.startswith("slub_debug="):
@@ -345,16 +342,14 @@
     """
     ``/proc/kcore`` should not be present
     =====================================
 
     Linux provides a core file of the running system, which allows a user with
     root access to view all kernel pointers and secrets, paving the way for
     further kernel exploits.
-
-    See :kevlar-code:`300`.
     """
 
     assert not os.path.exists("/proc/kcore"), "/proc/kcore attack surface detected"
 
 
 DeviceVals = Tuple[int, int, int]
 
@@ -377,16 +372,14 @@
 ) -> None:
     """
     Device path ``{{device_path}}`` should not be present
     ==============================================================
 
     Device files, such as ``{{device_path}}`` are an unnecessary attack surface
     that can be disabled.
-
-    See :kevlar-code:`300`.
     """
 
     try:
         info = os.stat(device_path)
     except FileNotFoundError:
         return
 
@@ -418,16 +411,14 @@
     """
     ``{{device_path}}`` should be inaccessible even through indirect means
     ============================================================================
 
     Deleting a device file path is not enough to render a device inaccessible.
     It needs to be removed from the kernel entirely. This test attempts to use
     ``mknod()`` to access a device without using it's standard file path.
-
-    See :kevlar-code:`300`.
     """
 
     new_path = workdir / "device"
 
     if module:
         result = run_kmod(["modprobe", module], stderr=subprocess.DEVNULL)
         assert result.returncode == 0, f"Could not load module {module}"
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_modules.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 ----------------------------------
 Kernel Hardening: Loadable Modules
 ----------------------------------
 
 Kernel modules allow runtime modification of the kernel. To prevent their use
 as a malware vector, only vetted, signed modules should be loadable.
+
+See :kevlar-code:`400`.
 """
 
 import gzip
 import lzma
 import platform
 import os
 from typing import Generator, Any, Tuple
@@ -82,29 +84,25 @@
 def test_has_module_signing(kconfig: KconfigSet) -> None:
     """
     Kernel module signatures should be enabled
     ==========================================
 
     The Linux kernel can check the integrity of loaded modules to guard against
     corruption and malware.
-
-    See :kevlar-code:`400`.
     """
     assert "CONFIG_MODULE_SIG=y" in kconfig, "Kernel module signing is disabled."
 
 
 def test_has_strict_module_signing(kconfig: KconfigSet) -> None:
     """
     Kernel module signatures should be mandatory
     ============================================
 
     Unsigned modules should not be loadable, to guard against malware and
     corruption.
-
-    See :kevlar-code:`400`.
     """
     try:
         with open("/sys/kernel/security/lockdown", "r") as fp:
             is_locked_down = "[none]" not in fp.read()
     except OSError:
         is_locked_down = False
 
@@ -118,16 +116,14 @@
 def test_has_strong_module_signing_hash(hash: str, kconfig: KconfigSet) -> None:
     """
     Kernel module signatures should use strong hash functions
     =========================================================
 
     The kernel can be configured to check module integrity using weak or
     deprecated hash functions. These hash functions should be disabled.
-
-    See :kevlar-code:`400`.
     """
     assert (
         f'CONFIG_MODULE_SIG_HASH="{hash}"' not in kconfig
     ), f"Weak hash {hash} used for signing modules."
 
 
 def test_any_modules_unsigned() -> None:
@@ -137,16 +133,14 @@
 
     All kernel modules that come with the Linux system should have signatures.
 
     .. note::
 
        This test looks for the presence of a signature, but it does not
        validate the signatures themselves.
-
-    See :kevlar-code:`400`.
     """
     any_unsupported = False
 
     marker = b"~Module signature appended~\n"
     for module, opener in iter_modules():
         if opener is None:
             any_unsupported = True
@@ -165,52 +159,44 @@
 def test_validate_module_signatures() -> None:
     """
     All kernel modules should be validly signed
     ===========================================
 
     All kernel modules that come with the Linux system should have valid
     signatures.
-
-    See :kevlar-code:`400`.
     """
     ...
 
 
 @full_version_only
 def test_kernel_refuses_to_load_unsigned() -> None:
     """
     The kernel should not load unsigned modules
     ===========================================
 
     This test attempts to inject a benign, unsigned module into the kernel.
-
-    See :kevlar-code:`400`.
     """
     ...
 
 
 @full_version_only
 def test_kernel_refuses_to_load_corrupted_data() -> None:
     """
     The kernel should not load modules with corrupted data
     ======================================================
 
     This test attempts to inject a benign kernel module with data that does not
     match its signature.
-
-    See :kevlar-code:`400`.
     """
     ...
 
 
 @full_version_only
 def test_kernel_refuses_to_load_corrupted_sig() -> None:
     """
     The kernel should not load modules with corrupted signature
     ===========================================================
 
     This test attempts to inject a benign kernel module with a slightly altered
     signature.
-
-    See :kevlar-code:`400`.
     """
     ...
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_offline_integrity.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_offline_integrity.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ---------------------
 
 It is often a simple matter to alter files while the computer is turned off,
 allowing an attacker to alter data and executables without needing to bypass
 enforcement that happens while the system is live. It is critical to secure the
 system from offline tampering, or none of the data on the device can really be
 trusted. This is a prerequisite to secure boot.
+
+See :kevlar-code:`500`
 """
 
 from typing import Dict
 from dataclasses import dataclass
 import subprocess
 import os
 import re
@@ -87,13 +89,11 @@
     The root filesystem should be protected at the block level from offline modification
     ====================================================================================
 
     The root filesystem holds system binaries and configuration and should be
     protected from offline modification. We recommend block-based schemes such
     as dm-verity, because they are higher performance and present fewer
     configuration challenges than file-based schemes.
-
-    See :kevlar-code:`500`
     """
 
     info = inspect_mountpoint("/")
     assert info.has_integrity, "Root file system is unprotected."
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_secure_dns.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_secure_dns.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Network Hardening: DNS Configuration
 ------------------------------------
 
 While the Domain Name Service (DNS) underlies all network communication, it is
 not a secure protocol. Failing to secure a device's use of DNS can allow
 malicious actors to arbitrarily spoof websites and will leak sensitive metadata
 about websites visited.
+
+See :kevlar-code:`600`.
 """
 
 import ipaddress
 import re
 import subprocess
 from typing import List
 
@@ -82,32 +84,28 @@
     ====================================
 
     DNSSEC is a standard that protects DNS lookups from spoofing or cache
     poisoning attacks. Without DNSSEC, there is no guarantee that the IP
     address the DNS server returned has not been maliciously altered. DNSSEC
     must be enabled on the DNS server, but it does no good if the client is not
     set up to verify it. When possible, the DNS client should *require* DNSSEC.
-
-    See :kevlar-code:`600`.
     """
 
     check_links_for_feature("DNSSEC", "dnssec", links_with_dns)
 
 
 def test_dns_over_tls_is_enabled(links_with_dns: List[str]) -> None:
     """
     DNS-over-TLS should be enabled
     ==============================
 
     DNS is vulnerable to eavesdropping and traffic modification. This is a
     serious side channel that can reveal to third parties what sites were
     visited, even if the connections are encrypted. By encrypting DNS using
     standard TLS, third parties cannot view or alter domain name lookups.
-
-    See :kevlar-code:`600`.
     """
 
     check_links_for_feature("DNS-over-TLS", "dnsovertls", links_with_dns)
 
 
 def test_resolv_conf_uses_loopback() -> None:
     """
@@ -116,16 +114,14 @@
 
     When ``/etc/resolv.conf`` has remote DNS server listed, most applications
     will use the system libc's rudimentary DNS client functionality to query
     them directly. There are no libc DNS implementations that implement any
     sort of security, such as DNS-over-TLS or DNSSEC. Instead,
     ``/etc/resolv.conf`` should be configured to query a more sophisticated
     resolver via a loopback address.
-
-    See :kevlar-code:`600`.
     """
 
     try:
         with open("/etc/resolv.conf") as fp:
             for line in fp:
                 fields = line.split()
                 if len(fields) == 2 and fields[0] == "nameserver":
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_systemd_syscall_filtering.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Application Sandboxing: Systemd
 -------------------------------
 
 Systemd can restrict what operations services can perform using per-service
 system call filtering. This can mitigate what an exploitable program can be
 made to do and can mitigate follow-on exploits such as local privilege
 escalations.
+
+See :kevlar-code:`700`.
 """
 
 import subprocess
 from typing import Dict
 
 import pytest
 
@@ -29,16 +31,14 @@
 def test_systemd_has_seccomp_enabled() -> None:
     """
     Systemd should be built with system call filtering support
     ==========================================================
 
     Systemd system call filtering is a compile-time option that should be
     enabled.
-
-    See :kevlar-code:`700`.
     """
 
     result = subprocess.run(
         ["systemctl", "--version"], text=True, stdout=subprocess.PIPE
     )
     assert "+SECCOMP" in result.stdout, "Systemd was not compiled with seccomp support"
 
@@ -60,16 +60,14 @@
 
 def test_has_filter_installed(basic_service: Dict[str, str]) -> None:
     """
     {{fixture_names["basic_service"]}} should have a system call filter installed
     =============================================================================
 
     This service has a system call filter available. It should be activated.
-
-    See :kevlar-code:`700`.
     """
 
     # Empty and ~ are equivalent.
     assert (
         basic_service.get("SystemCallFilter", "~") != "~"
     ), "No system call filter installed"
 
@@ -80,14 +78,12 @@
     ========================================================================
 
     Some architectures support multiple types of system calls. Most commonly,
     64-bit systems will support a secondary set of system calls for 32-bit
     processes. Allowing these alternate system calls can reduce the
     effectiveness of a system call filter and should be prohibited for programs
     that have system call filtering enabled.
-
-    See :kevlar-code:`700`.
     """
 
     assert (
         basic_service.get("SystemCallArchitectures") == "native"
     ), "System call filter allows non-native architectures"
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/__init__.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/elf.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/elf.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/kconfig.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/kconfig.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/modules.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/modules.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/mount.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/mount.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/systemd.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/systemd.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/workdir.py` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/workdir.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/PKG-INFO` & `kevlar-system-inspector-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.0.0rc8
+Version: 1.0.1
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -34,47 +34,49 @@
 ======================================================================
 
 Kevlar System Inspector is an embedded security test suite that grew out of
 `Star Lab's`_ extensive experience assessing and protecting mission-critical
 systems for the U.S. Government.  These test have been made available for
 public use to help identify security issues in a variety of Linux systems.  The
 set of tests present in Kevlar System Inspector will be expanded as adversary
-techniques and tactics change, and as we continue development of `KES`_.
+techniques and tactics change, and as we continue development of `Kevlar
+Embedded Security`_.
 
 These tests are generally more aggressive than other security scanning tools: We
 prefer to probe behavior rather than check configurations values. However, we
 do not include any actual exploit code or include any tests that could
 destabilize the system. (And of course, we check configuration values too.)
 
 .. _Star Lab's: https://www.starlab.io
-.. _KES: https://www.starlab.io/kevlar-embedded-security
+.. _Kevlar Embedded Security: https://www.starlab.io/kevlar-embedded-security
 
 
 System Requirements
 ===================
 
-Kevlar System Inspector requires Python 3.8 or higher. Our emphasis is on
-embedded Linux distros (Yocto-based), but Kevlar System Inspector is a pure
-Python project that should run on most modern Linux distros.
+Kevlar System Inspector requires Python 3.8 or higher.
+
+It is designed to be run in an embedded Linux test environment, but it is a
+Python project that can run on most modern Linux distros, including desktop
+distributions.
 
 
 Installation
 ============
 
 We provide several methods for installation:
 
 
 Install from PyPI
 -----------------
 
 If your system is capable of installing packages from PyPI, Kevlar System
-Inspector may be installed using ``pip``.
-
-Because Kevlar System Inspector should be run as root, we suggest using ``pip``
-to install to a virtual environment:
+Inspector may be installed using ``pip``. Because Kevlar System Inspector is
+designed to be run as root in a test environment, we suggest using ``pip`` to
+install to a virtual environment. (Note that running as root is not required.)
 
 .. code-block:: console
 
    $ python3 -m venv kevlar-venv
    $ ./kevlar-venv/bin/pip install kevlar-system-inspector
    $ sudo ./kevlar-venv/bin/kevlar-system-inspector
 
@@ -94,8 +96,45 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0rc8.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.1.tar.gz
+
+
+Running as Root
+===============
+
+Although running as root is not necessary, Kevlar System Inspector is designed
+to be run as root in a embedded test environment for two reasons:
+
+* Some tests (for example, kernel module loading) require root permissions to
+  perform.
+* The Kevlar Embedded Security threat model is a defense in depth model that
+  includes compromised root processes and malicious insiders.
+
+Kevlar System Inspector does not include any malicious code or tests that would
+destabilize the system. It uses root access to:
+
+* Probe kernel features and configurations in different ways.
+* Test the reaction of the system to (benign) files dropped in privileged
+  locations.
+* Inspect logical volume mangement configuration.
+
+
+HTML Report Output
+==================
+
+Kevlar System Inspector may be run with the option
+``--output-html=<filename.html>`` to produce a self-contained HTML report.
+
+
+Uninstalling
+============
+
+If installed through ``pip``, Kevlar System Inspector may be uninstalled using
+the command ``pip uninstall``. If it was installed in a virtual environment, or
+if the standalone tarball version was used, simply deleting the directory
+removes Kevlar System Inspector from the system. It does not permanently leave
+files anywhere else on the system.
```

### Comparing `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/SOURCES.txt` & `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

