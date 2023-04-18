# Comparing `tmp/gluster-georep-tools-0.2.tar.gz` & `tmp/gluster-georep-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gluster-georep-tools-0.2.tar", last modified: Fri Nov 18 05:35:04 2016, max compression
+gzip compressed data, was "gluster-georep-tools-0.5.0.tar", last modified: Tue Apr 18 08:31:08 2023, max compression
```

## Comparing `gluster-georep-tools-0.2.tar` & `gluster-georep-tools-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxrwxr-x   0 aravinda  (1000) aravinda  (1000)        0 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/
-drwxrwxr-x   0 aravinda  (1000) aravinda  (1000)        0 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools/
-drwxrwxr-x   0 aravinda  (1000) aravinda  (1000)        0 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools/status/
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)     5117 2016-11-17 13:07:55.000000 gluster-georep-tools-0.2/gluster_georep_tools/status/cli.py
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)        0 2016-11-14 08:08:46.000000 gluster-georep-tools-0.2/gluster_georep_tools/status/__init__.py
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)        0 2016-11-14 08:01:21.000000 gluster-georep-tools-0.2/gluster_georep_tools/__init__.py
-drwxrwxr-x   0 aravinda  (1000) aravinda  (1000)        0 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools/setup/
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)    16739 2016-11-14 08:21:33.000000 gluster-georep-tools-0.2/gluster_georep_tools/setup/cli.py
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)      149 2016-11-14 07:14:51.000000 gluster-georep-tools-0.2/gluster_georep_tools/setup/__init__.py
-drwxrwxr-x   0 aravinda  (1000) aravinda  (1000)        0 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)        1 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)        1 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/not-zip-safe
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)      498 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)       21 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/top_level.txt
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)      760 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/PKG-INFO
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)       29 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/requires.txt
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)      139 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/gluster_georep_tools.egg-info/entry_points.txt
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)      760 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/PKG-INFO
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)       59 2016-11-18 05:35:04.000000 gluster-georep-tools-0.2/setup.cfg
--rw-rw-r--   0 aravinda  (1000) aravinda  (1000)     1458 2016-11-18 05:34:52.000000 gluster-georep-tools-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/.github/workflows/on-release-tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 08:31:07.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/setup/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/gluster_georep_tools/status/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 08:31:08.000000 gluster-georep-tools-0.5.0/gluster_georep_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/screenshots/gluster-georep-setup.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:31:08.233636 gluster-georep-tools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 08:30:57.000000 gluster-georep-tools-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gluster-georep-tools-0.2/gluster_georep_tools/status/cli.py` & `gluster-georep-tools-0.5.0/gluster_georep_tools/status/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Gluster Geo-replication Status
 """
 
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 import sys
 
-from gluster.cli import georep
+from glustercli.cli import georep
 from prettytable import PrettyTable
 
 
 def apply_filters(status_data, args):
     session_rows = []
     for session in status_data:
         # Collect the Session name and apply filter
@@ -53,95 +53,93 @@
 
     return session_rows
 
 
 def display_status(status_data):
     for session in status_data:
         # Display heading and initiate table
-        print "SESSION: " + session[0]
-        table = PrettyTable(["MASTER", "STATUS",
-                             "CRAWL STATUS", "SLAVE NODE", "LAST SYNCED",
-                             "CHKPT TIME", "CHKPT COMPLETED",
-                             "CHKPT COMPLETION TIME"])
+        print("SESSION: " + session[0])
+        table = PrettyTable([
+            "PRIMARY", "STATUS",
+            "CRAWL STATUS", "SECONDARY NODE", "LAST SYNCED"
+        ])
         for row in session[2]:
-            table.add_row([row["master_node"] + ":" + row["master_brick"],
-                           row["status"], row["crawl_status"],
-                           row["slave_node"], row["last_synced"],
-                           row["checkpoint_time"],
-                           row["checkpoint_completed"],
-                           row["checkpoint_completion_time"]])
+            table.add_row([
+                row["master_node"] + ":" + row["master_brick"],
+                row["status"], row["crawl_status"],
+                row["slave_node"], row["last_synced"]
+            ])
 
         # If Table has data
         if session[2]:
-            print table
+            print(table)
         else:
             # When no filters match
-            print "-"
+            print("-")
 
-        print ("Active: {active} | Passive: {passive} | "
+        print("Active: {active} | Passive: {passive} | "
                "Faulty: {faulty} | Created: {created} | "
                "Offline: {offline} | Stopped: {stopped} | "
                "Initializing: {initializing} | "
                "Total: {total}".format(**session[1]))
 
         # Empty line in output
-        print
+        print()
 
 
 def handle_status(args):
-    slave_user = "root"
-    slave_host = None
-    slave_vol = None
+    secondary_user = "root"
+    secondary_host = None
+    secondary_vol = None
     volname = None
 
-    if args.mastervol is not None:
-        volname = args.mastervol
+    if args.primary_vol is not None:
+        volname = args.primary_vol
 
-    if args.slave is not None:
-        if "::" not in args.slave:
-            sys.stderr.write("Invalid Slave details\n")
+    if args.secondary is not None:
+        if "::" not in args.secondary:
+            sys.stderr.write("Invalid Secondary details\n")
             sys.exit(1)
 
-        slave_host_tmp, slave_vol = args.slave.split("::")
+        secondary_host_tmp, secondary_vol = args.secondary.split("::")
 
-        slave_host_data = slave_host_tmp.split("@")
-        slave_host = slave_host_data[-1]
-        if len(slave_host_data) > 1:
-            slave_user = slave_host_data[0]
+        secondary_host_data = secondary_host_tmp.split("@")
+        secondary_host = secondary_host_data[-1]
+        if len(secondary_host_data) > 1:
+            secondary_user = secondary_host_data[0]
 
     status_data = georep.status(volname=volname,
-                                slave_host=slave_host,
-                                slave_vol=slave_vol,
-                                slave_user=slave_user)
+                                slave_host=secondary_host,
+                                slave_vol=secondary_vol,
+                                slave_user=secondary_user)
 
     if not status_data:
-        if args.slave is not None:
+        if args.secondary is not None:
             sys.stderr.write("No active Geo-replication "
                              "sessions between {0} and {1}\n".format(
-                                 args.mastervol,
-                                 args.slave))
+                                 args.primary_vol,
+                                 args.secondary))
             sys.exit(1)
-        elif args.mastervol is not None and args.slave is None:
+        elif args.primary_vol is not None and args.secondary is None:
             sys.stderr.write("No active Geo-replication "
                              "sessions for {0}\n".format(
-                                 args.mastervol))
+                                 args.primary_vol))
             sys.exit(1)
 
     status_data = apply_filters(status_data, args)
     display_status(status_data)
 
 
 def get_args():
     parser = ArgumentParser(formatter_class=RawDescriptionHelpFormatter,
                             description=__doc__)
-    parser.add_argument("mastervol", nargs="?", help="Master Volume Name")
-    parser.add_argument("slave", nargs="?", help="Slave details. "
-                        "[<slave_user>@]<slave_host>::<slave_vol>, "
-                        "Example: geoaccount@slavenode1::myvol or "
-                        "slavenode1::myvol in case of root user")
+    parser.add_argument("primary_vol", nargs="?", help="Primary Volume Name")
+    parser.add_argument("secondary", nargs="?", help="Secondary details. "
+                        "<secondary_host>::<secondary_vol>, "
+                        "Example: secondary_node1::myvol")
     parser.add_argument("--with-status",
                         help="Show only nodes with matching Status")
     parser.add_argument("--with-crawl-status",
                         help="Show only nodes with matching Crawl Status")
     return parser.parse_args()
```

### Comparing `gluster-georep-tools-0.2/gluster_georep_tools/setup/cli.py` & `gluster-georep-tools-0.5.0/gluster_georep_tools/setup/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # -*- coding: utf-8 -*-
-"""
-    georepsetup.cli.py
-    :copyright: (c) 2015 by Aravinda VK
-    :license: MIT, see LICENSE for more details.
-"""
 
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from contextlib import contextmanager
 import getpass
 import os
 import socket
 import subprocess
 import sys
 import tempfile
 
 import paramiko
 
 PROG_DESCRIPTION = """
 CLI tool to setup Gluster Geo-replication Session between
-Master Gluster Volume to Slave Gluster Volume.
+Primary Gluster Volume to Secondary Gluster Volume.
 """
 BUFFER_SIZE = 104857600  # Considering buffer_size 100MB
 SESSION_MOUNT_LOG_FILE = ("/var/log/glusterfs/geo-replication"
                           "/georepsetup.mount.log")
 SYMBOLS = ('K', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y')
 DEFAULT_GLUSTERD_WORKDIR = "/var/lib/glusterd"
 USE_CLI_COLOR = True
@@ -61,15 +56,15 @@
     """
     cmd = ["find", path,
            "-maxdepth", "1",
            "-path", os.path.join(path, ".trashcan"),
            "-prune", "-o", "-path", path, "-o", "-print0", "-quit"]
     return execute(cmd,
                    failure_msg="Unable to count number of files "
-                   "in Slave Volume")
+                   "in Secondary Volume")
 
 
 def cleanup(hostname, volname, mnt):
     """
     Unmount the Volume and Remove the temporary directory
     """
     execute(["umount", mnt],
@@ -164,15 +159,16 @@
 
 def execute(cmd, success_msg="", failure_msg="", exitcode=-1):
     """
     Generic wrapper to execute the CLI commands. Returns Output if success.
     On success it can print message in stdout if specified.
     On failure, exits after writing to stderr.
     """
-    p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    p = subprocess.Popen(cmd, universal_newlines=True,
+                         stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = p.communicate()
     if p.returncode == 0:
         if success_msg:
             output_ok(success_msg)
         return out
     else:
         err_msg = err if err else out
@@ -181,321 +177,341 @@
 
 def get_glusterd_workdir():
     """
     Command to get Glusterd working dir. If failed returns the
     default directory /var/lib/glusterd
     """
     p = subprocess.Popen(["gluster", "system::", "getwd"],
+                         universal_newlines=True,
                          stdout=subprocess.PIPE)
 
     out, _ = p.communicate()
 
     if p.returncode == 0:
         return out.strip()
     else:
         return DEFAULT_GLUSTERD_WORKDIR
 
 
-def check_host_reachable(slavehost):
+def check_host_reachable(secondary_host):
     """
-    Check if SSH port is open for given slavehost
+    Check if SSH port is open for given secondary_host
     """
-    if is_port_enabled(slavehost, 22):
-        output_ok("{0} is Reachable(Port 22)".format(slavehost))
+    if is_port_enabled(secondary_host, 22):
+        output_ok("{0} is Reachable(Port 22)".format(secondary_host))
     else:
-        output_notok("{0} is Not Reachable(Port 22)".format(slavehost))
+        output_notok("{0} is Not Reachable(Port 22)".format(secondary_host))
 
 
-def ssh_initialize(slavehost, passwd):
+def ssh_initialize(secondary_host, username, passwd):
     """
     Initialize the SSH connection
     """
     ssh = paramiko.SSHClient()
     try:
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        ssh.connect(slavehost, username="root", password=passwd)
-        output_ok("SSH Connection established root@{0}".format(slavehost))
+        ssh.connect(secondary_host, username=username, password=passwd)
+        output_ok("SSH Connection established {0}@{1}".format(username, secondary_host))
     except paramiko.ssh_exception.AuthenticationException as e:
         output_notok("Unable to establish SSH connection "
-                     "to root@{0}:\n{1}".format(slavehost, e))
+                     "to {0}@{1}:\n{2}".format(username, secondary_host, e))
 
     return ssh
 
 
 def compare_gluster_versions(ssh):
     """
-    Collect Master version by directly executing CLI command, get Slave version
-    via SSH command execution
+    Collect Primary version by directly executing CLI command, get
+    Secondary version via SSH command execution
     """
-    # Collect Gluster Version from Master
-    master_version = execute(["gluster", "--version"],
-                             failure_msg="Failed to get Gluster version "
-                             "from Master")
-    master_version = master_version.split()[1]
+    # Collect Gluster Version from Primary
+    primary_version = execute(["gluster", "--version"],
+                              failure_msg="Failed to get Gluster version "
+                              "from Primary Cluster")
+    primary_version = primary_version.split()[1]
+
+    sudo_pfx = "sudo " if ssh.use_sudo else ""
 
-    # Collect Gluster Version from Slave
-    stdin, stdout, stderr = ssh.exec_command("gluster --version")
+    # Collect Gluster Version from Secondary
+    stdin, stdout, stderr = ssh.exec_command(f"{sudo_pfx} gluster --version")
     rc = stdout.channel.recv_exit_status()
     if rc != 0:
-        output_notok("Unable to get Slave Gluster Version")
+        output_notok("Unable to get Secondary Gluster Version")
 
-    slave_version = stdout.readline().split()[1]
+    secondary_version = stdout.readline().split()[1]
 
     # Check for Version mismatch
-    if master_version == slave_version:
-        output_ok("Master Volume and Slave Volume are "
-                  "compatible (Version: {0})".format(master_version))
+    if primary_version == secondary_version:
+        output_ok("Primary Volume and Secondary Volume are "
+                  "compatible (Version: {0})".format(primary_version))
     else:
-        output_notok("Master Volume({0}) and Slave Volume({1}) "
-                     "versions not Compatible".format(master_version,
-                                                      slave_version))
+        output_notok("Primary Volume({0}) and Secondary Volume({1}) "
+                     "versions not Compatible".format(primary_version,
+                                                      secondary_version))
 
 
-def compare_disk_sizes(args, slavehost, slavevol):
+def compare_disk_sizes(args, secondary_host, secondary_vol):
     """
     Compare the disk sizes and available sizes. Also
-    Check Slave volume is empty or not
+    Check Secondary volume is empty or not
     """
-    master_disk_size = None
-    slave_disk_size = None
-    master_used_size = None
-    slave_used_size = None
+    primary_disk_size = None
+    secondary_disk_size = None
+    primary_used_size = None
+    secondary_used_size = None
 
-    with glustermount("localhost", args.mastervol) as mnt:
+    with glustermount("localhost", args.primary_vol) as mnt:
         data = os.statvfs(mnt)
-        master_disk_size = data.f_blocks * data.f_bsize
-        master_used_size = ((data.f_blocks - data.f_bavail) *
+        primary_disk_size = data.f_blocks * data.f_bsize
+        primary_used_size = ((data.f_blocks - data.f_bavail) *
                             data.f_bsize)
 
-    with glustermount(slavehost, slavevol) as mnt:
+    with glustermount(secondary_host, secondary_vol) as mnt:
         if get_number_of_files(mnt):
             if not args.force:
-                cleanup(slavehost, slavevol, mnt)
+                cleanup(secondary_host, secondary_vol, mnt)
                 output_notok("{0}::{1} is not empty. Please delete existing "
                              "files in {0}::{1} and retry, or use --force to "
                              "continue without deleting the existing "
-                             "files.".format(slavehost, slavevol))
+                             "files.".format(secondary_host, secondary_vol))
             else:
-                output_warning("{0}::{1} is not empty.".format(slavehost,
-                                                               slavevol))
+                output_warning("{0}::{1} is not empty.".format(secondary_host,
+                                                               secondary_vol))
         data = os.statvfs(mnt)
-        slave_disk_size = data.f_blocks * data.f_bsize
-        slave_used_size = ((data.f_blocks - data.f_bavail) *
-                           data.f_bsize)
+        secondary_disk_size = data.f_blocks * data.f_bsize
+        secondary_used_size = ((data.f_blocks - data.f_bavail) *
+                            data.f_bsize)
 
-    if master_disk_size is None or master_used_size is None:
-        msg = "Unable to get Disk size and Used size of Master Volume"
+    if primary_disk_size is None or primary_used_size is None:
+        msg = "Unable to get Disk size and Used size of Primary Volume"
         if not args.force:
             output_notok(msg)
         else:
             output_warning(msg)
 
-    if slave_disk_size is None or slave_used_size is None:
-        msg = "Unable to get Disk size and Used size of Slave Volume"
+    if secondary_disk_size is None or secondary_used_size is None:
+        msg = "Unable to get Disk size and Used size of Secondary Volume"
         if not args.force:
             output_notok(msg)
         else:
             output_warning(msg)
 
-    if slave_disk_size < master_disk_size:
-        msg = ("Total disk size of master({0}) is greater "
-               "than disk size of slave({1})".format(
-                   human_readable_size(master_disk_size),
-                   human_readable_size(slave_disk_size)))
+    if secondary_disk_size < primary_disk_size:
+        msg = ("Total disk size of primary({0}) is greater "
+               "than disk size of secondary({1})".format(
+                   human_readable_size(primary_disk_size),
+                   human_readable_size(secondary_disk_size)))
         if not args.force:
             output_notok(msg)
         else:
             output_warning(msg)
 
-    effective_master_used_size = master_used_size + BUFFER_SIZE
-    slave_available_size = slave_disk_size - slave_used_size
-    master_available_size = master_disk_size - effective_master_used_size
-
-    if slave_available_size < master_available_size:
-        msg = ("Total available size of master({0}) is greater "
-               "than available size of slave({1})".format(
-                   human_readable_size(master_available_size),
-                   human_readable_size(slave_available_size)))
+    effective_primary_used_size = primary_used_size + BUFFER_SIZE
+    secondary_available_size = secondary_disk_size - secondary_used_size
+    primary_available_size = primary_disk_size - effective_primary_used_size
+
+    if secondary_available_size < primary_available_size:
+        msg = ("Total available size of primary({0}) is greater "
+               "than available size of secondary({1})".format(
+                   human_readable_size(primary_available_size),
+                   human_readable_size(secondary_available_size)))
 
         if not args.force:
             output_notok(msg)
         else:
             output_warning(msg)
 
 
 def run_gsec_create(georep_dir):
     """
-    gsec_create command to generate pem keys in all the master nodes
+    gsec_create command to generate pem keys in all the primary nodes
     and collect all pub keys to single node
     """
     execute(["gluster", "system::", "execute", "gsec_create"],
             success_msg="Common secret pub file present at "
             "{0}/common_secret.pem.pub".format(georep_dir),
             failure_msg="Common secret pub file generation failed")
 
 
-def copy_to_main_slave_node(ssh, args, slavehost, georep_dir, pubfile):
+def copy_to_main_secondary_node(ssh, args, secondary_host, georep_dir, pubfile):
     """
-    Copy common_secret.pem.pub file to Main Slave node
+    Copy common_secret.pem.pub file to Main Secondary node
     """
-    # Copy common_secret.pem.pub file to Main Slave node
+    home_dir = "/root"
+    if args.secondary_user != "root":
+        home_dir = f"/home/{args.secondary_user}"
+
+    # Copy common_secret.pem.pub file to Main Secondary node
     ftp = ssh.open_sftp()
-    ftp.put("{georep_dir}/common_secret.pem.pub".format(georep_dir=georep_dir),
-            "{georep_dir}/{pubfile}".format(
-                georep_dir=georep_dir, pubfile=pubfile))
+    ftp.put(
+        f"{georep_dir}/common_secret.pem.pub",
+        f"{home_dir}/{pubfile}"
+    )
     ftp.close()
-    output_ok("common_secret.pem.pub file copied to {0}".format(slavehost))
 
+    sudo_pfx = "sudo " if ssh.use_sudo else ""
+    stdin, stdout, stderr = ssh.exec_command(
+        f"{sudo_pfx}cp {home_dir}/{pubfile} {georep_dir}/{pubfile}")
+
+    output_ok("common_secret.pem.pub file copied to {0}".format(secondary_host))
 
-def distribute_to_all_slave_nodes(ssh, pubfile):
+
+def distribute_to_all_secondary_nodes(ssh, pubfile):
     """
-    Distribute the pem.pub file to all the slave nodes using
+    Distribute the pem.pub file to all the secondary nodes using
     Glusterd copy file infrastructure
     """
+    sudo_pfx = "sudo " if ssh.use_sudo else ""
     stdin, stdout, stderr = ssh.exec_command(
-        "gluster system:: copy file /geo-replication/{pubfile}".format(
-            pubfile=pubfile))
+        f"{sudo_pfx}gluster system:: copy file /geo-replication/{pubfile}")
 
     rc = stdout.channel.recv_exit_status()
     if rc == 0:
-        output_ok("Master SSH Keys copied to all Up "
-                  "Slave nodes")
+        output_ok("Primary SSH Keys copied to all Up "
+                  "Secondary nodes")
     else:
-        output_notok("Unable to copy Master SSH Keys to all Up "
-                     "Slave nodes")
+        output_notok("Unable to copy Primary SSH Keys to all Up "
+                     "Secondary nodes")
 
 
-def add_to_authorized_keys(ssh, pubfile, slaveuser):
+def add_to_authorized_keys(ssh, pubfile, secondary_session_user):
     """
-    Add these pub keys to authorized_keys file of all Slave nodes
+    Add these pub keys to authorized_keys file of all Secondary nodes
     """
+    sudo_pfx = "sudo " if ssh.use_sudo else ""
     stdin, stdout, stderr = ssh.exec_command(
-        "gluster system:: execute add_secret_pub {slaveuser} "
-        "geo-replication/{pubfile}".format(
-            pubfile=pubfile, slaveuser=slaveuser))
+        f"{sudo_pfx}gluster system:: execute add_secret_pub {secondary_session_user} "
+        f"geo-replication/{pubfile}"
+    )
 
     rc = stdout.channel.recv_exit_status()
     if rc == 0:
-        output_ok("Updated Master SSH Keys to all Up "
-                  "Slave nodes authorized_keys file")
+        output_ok("Updated Primary SSH Keys to all Up "
+                  "Secondary nodes authorized_keys file")
     else:
-        output_notok("Unable to update Master SSH Keys to all "
-                     "Up Slave nodes authorized_keys file")
+        output_notok("Unable to update Primary SSH Keys to all "
+                     "Up Secondary nodes authorized_keys file")
 
 
-def create_georep_session(args, slaveuser, slavehost, slavevol):
+def create_georep_session(args, secondary_session_user, secondary_host, secondary_vol):
     """
     Create Geo-rep session using gluster volume geo-replication command
     """
-    slave = slavehost
-    if slaveuser != "root":
-        slave = "{0}@{1}".format(slaveuser, slavehost)
+    secondary = secondary_host
+    if secondary_session_user != "root":
+        secondary = "{0}@{1}".format(secondary_session_user, secondary_host)
 
     cmd = ["gluster", "volume", "geo-replication",
-           args.mastervol,
-           "{0}::{1}".format(slave, slavevol),
+           args.primary_vol,
+           "{0}::{1}".format(secondary, secondary_vol),
            "create",
            "no-verify"]
 
     cmd += ["force"] if args.force else []
     execute(cmd,
             success_msg="Geo-replication Session Established",
             failure_msg="Failed to Establish Geo-replication Session")
 
 
 def setup_georep():
     """
     Main function to setup Geo-replication. Steps involved are
-    1.  Collect root@SLAVEHOST's password
+    1.  Collect root@SECONDARY_HOST's password
     2.  Check if SSH port is open
     3.  Initialize SSH Client
     4.  Compare the Gluster Versions
     5.  Compare disk sizes
     6.  Run gsec_create
-    7.  Copy common_secret.pem.pub to Main Slave node
-    8.  Distribute common_secret.pem.pub to all Slave nodes
+    7.  Copy common_secret.pem.pub to Main Secondary node
+    8.  Distribute common_secret.pem.pub to all Secondary nodes
     9.  Add to authorized_keys file
     10. Create Geo-replication Session
     """
     # Parse/Validate the CLI arguments
     args = get_args()
 
     if os.getuid() != 0:
         output_notok("Only root can run this tool!")
 
     # Modify the Global Config based on User input. If no coloring required
     global USE_CLI_COLOR
     if args.no_color:
         USE_CLI_COLOR = False
 
-    # Collect Glusterd workdir, slave information
+    # Collect Glusterd workdir, secondary information
     georep_dir = os.path.join(get_glusterd_workdir(), "geo-replication")
-    slavehost_data, slavevol = args.slave.split("::")
-    slave = slavehost_data.split("@")
-    slavehost = slave[-1]
-    slaveuser = "root" if len(slave) == 1 else slave[0]
-
-    # Get SLAVEHOST's root users password for administrative activities
-    passwd_prompt_msg = ("Geo-replication session will be established "
-                         "between {mastervol} and {slave}\n"
-                         "Root password of {slavehost} is required to complete"
-                         " the setup. NOTE: Password will not be stored.\n\n"
-                         "root@{slavehost}'s password: ".format(
-                             mastervol=args.mastervol,
-                             slave=args.slave,
-                             slavehost=slavehost))
+    secondary_host_data, secondary_vol = args.secondary.split("::")
+    secondary = secondary_host_data.split("@")
+    secondary_host = secondary[-1]
+    secondary_session_user = "root" if len(secondary) == 1 else secondary[0]
+
+    # Get SECONDARY_HOST's root users password for administrative activities
+    passwd_prompt_msg = (f"Geo-replication session will be established "
+                         f"between {args.primary_vol} and {args.secondary}\n"
+                         f"{args.secondary_user}@{secondary_host} password is "
+                         f"required to complete"
+                         f" the setup. NOTE: Password will not be stored.\n\n"
+                         f"{args.secondary_user}@{secondary_host}'s password: ")
 
     passwd = getpass.getpass(passwd_prompt_msg)
 
     # SSH Port check: Enabled/Disabled
-    check_host_reachable(slavehost)
+    check_host_reachable(secondary_host)
 
     # Initiate SSH Client
-    ssh = ssh_initialize(slavehost, passwd)
+    ssh = ssh_initialize(secondary_host, args.secondary_user, passwd)
+
+    # Use sudo while running commands in secondary node
+    ssh.use_sudo = args.secondary_user != "root"
 
-    # Compare Gluster Version in Master Cluster and Slave Cluster
+    # Compare Gluster Version in Primary Cluster and Secondary Cluster
     compare_gluster_versions(ssh)
 
-    # Compare disk size and used size to decide Master and Slave are compatible
-    # Also check if Slave is empty or not
-    compare_disk_sizes(args, slavehost, slavevol)
+    # Compare disk size and used size to decide
+    # Primary and Secondary are compatible
+    # Also check if Secondary is empty or not
+    compare_disk_sizes(args, secondary_host, secondary_vol)
 
     # Run gsec_create command
     run_gsec_create(georep_dir)
 
     # Target name for Pubfile
-    pubfile = "{mastervol}_{slavevol}_common_secret.pem.pub".format(
-        mastervol=args.mastervol, slavevol=slavevol)
+    pubfile = "{primary_vol}_{secondary_vol}_common_secret.pem.pub".format(
+        primary_vol=args.primary_vol, secondary_vol=secondary_vol)
 
-    # Copy Pub file to Main Slave node
-    copy_to_main_slave_node(ssh, args, slavehost, georep_dir, pubfile)
+    # Copy Pub file to Main Secondary node
+    copy_to_main_secondary_node(ssh, args, secondary_host, georep_dir, pubfile)
 
-    # Distribute SSH Keys to All the Slave nodes
-    distribute_to_all_slave_nodes(ssh, pubfile)
+    # Distribute SSH Keys to All the Secondary nodes
+    distribute_to_all_secondary_nodes(ssh, pubfile)
 
-    # Add the SSH Keys to authorized_keys file of all Slave nodes
-    add_to_authorized_keys(ssh, pubfile, slaveuser)
+    # Add the SSH Keys to authorized_keys file of all Secondary nodes
+    add_to_authorized_keys(ssh, pubfile, secondary_session_user)
 
     # Last Step: Create Geo-rep Session
-    create_georep_session(args, slaveuser, slavehost, slavevol)
+    create_georep_session(args, secondary_session_user, secondary_host, secondary_vol)
 
 
 def get_args():
     """
     Parse the CLI arguments
     """
     parser = ArgumentParser(formatter_class=RawDescriptionHelpFormatter,
                             description=PROG_DESCRIPTION)
 
-    parser.add_argument("mastervol", help="Master Volume Name",
-                        metavar="MASTERVOL")
-    parser.add_argument("slave",
-                        help="Slave, HOSTNAME or root@HOSTNAME::SLAVEVOL "
-                        "or user@HOSTNAME::SLAVEVOL",
-                        metavar="SLAVE")
+    parser.add_argument("primary_vol", help="Primary Volume Name",
+                        metavar="PRIMARY_VOL")
+    parser.add_argument("secondary",
+                        help="Secondary, HOSTNAME or "
+                        "HOSTNAME::SECONDARY_VOL",
+                        metavar="SECONDARY")
+    parser.add_argument(
+        "--secondary-user", default="root",
+        help="Admin user in one of the node of the secondary cluster"
+    )
     parser.add_argument("--force", help="Force",
                         action="store_true")
     parser.add_argument("--no-color", help="No Terminal Colors",
                         action="store_true")
 
     return parser.parse_args()
```

### Comparing `gluster-georep-tools-0.2/setup.py` & `gluster-georep-tools-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 # -*- coding: utf-8 -*-
-"""
-    gluster-georep-tools.setup.py
-    :copyright: (c) 2016 by Aravinda VK
-    :license: MIT, see LICENSE for more details.
-"""
-
 from setuptools import setup
+from importlib.metadata import version, PackageNotFoundError
 
+try:
+    __version__ = version('gluster_georep_tools')
+except PackageNotFoundError:
+    __version__ = "unknown"
 
 setup(
     name="gluster-georep-tools",
-    version="0.2",
+    version=__version__,
     packages=["gluster_georep_tools",
               "gluster_georep_tools.status",
               "gluster_georep_tools.setup"],
     include_package_data=True,
-    install_requires=['argparse', 'paramiko', 'glustercli'],
+    install_requires=['paramiko', 'glustercli', 'prettytable'],
     entry_points={
         "console_scripts": [
             "gluster-georep-setup = gluster_georep_tools.setup.cli:main",
             "gluster-georep-status = gluster_georep_tools.status.cli:main",
         ]
     },
     platforms="linux",
     zip_safe=False,
-    author="Aravinda VK",
+    author="Aravinda Vishwanathapura",
     author_email="mail@aravindavk.in",
     description="Gluster Geo-replication tools",
     license="MIT",
     keywords="gluster, tool, geo-replication",
     url="https://github.com/aravindavk/gluster-georep-tools",
     long_description="""
     Gluster Geo-replication Tools
     """,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 2 :: Only"
+        "Programming Language :: Python"
     ],
 )
```

