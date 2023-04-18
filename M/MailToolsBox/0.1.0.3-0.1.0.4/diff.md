# Comparing `tmp/MailToolsBox-0.1.0.3.tar.gz` & `tmp/MailToolsBox-0.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailToolsBox-0.1.0.3.tar", last modified: Tue Apr 18 11:46:51 2023, max compression
+gzip compressed data, was "MailToolsBox-0.1.0.4.tar", last modified: Tue Apr 18 12:08:37 2023, max compression
```

## Comparing `MailToolsBox-0.1.0.3.tar` & `MailToolsBox-0.1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.702589 MailToolsBox-0.1.0.3/
--rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.662353 MailToolsBox-0.1.0.3/MailToolsBox/
--rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.3/MailToolsBox/__init__.py
--rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.3/MailToolsBox/imapClient.py
--rw-rw-rw-   0        0        0     4341 2023-04-18 11:43:35.000000 MailToolsBox-0.1.0.3/MailToolsBox/mailSender.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.699590 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/
--rw-rw-rw-   0        0        0     6059 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6059 2023-04-18 11:46:51.701589 MailToolsBox-0.1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5232 2023-04-18 11:39:35.000000 MailToolsBox-0.1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 11:46:51.703589 MailToolsBox-0.1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1388 2023-04-18 11:45:35.000000 MailToolsBox-0.1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:08:37.336949 MailToolsBox-0.1.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.4/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 12:08:37.313956 MailToolsBox-0.1.0.4/MailToolsBox/
+-rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.4/MailToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.4/MailToolsBox/imapClient.py
+-rw-rw-rw-   0        0        0     4339 2023-04-18 12:05:14.000000 MailToolsBox-0.1.0.4/MailToolsBox/mailSender.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:08:37.334949 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     6059 2023-04-18 12:08:37.000000 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-18 12:08:37.000000 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:08:37.000000 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 12:08:37.000000 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 12:08:37.000000 MailToolsBox-0.1.0.4/MailToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6059 2023-04-18 12:08:37.335948 MailToolsBox-0.1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5232 2023-04-18 11:39:35.000000 MailToolsBox-0.1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 12:08:37.337948 MailToolsBox-0.1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-04-18 12:06:50.000000 MailToolsBox-0.1.0.4/setup.py
```

### Comparing `MailToolsBox-0.1.0.3/LICENSE.txt` & `MailToolsBox-0.1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.3/MailToolsBox/imapClient.py` & `MailToolsBox-0.1.0.4/MailToolsBox/imapClient.py`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.3/MailToolsBox/mailSender.py` & `MailToolsBox-0.1.0.4/MailToolsBox/mailSender.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     attachment_part = MIMEApplication(
                         attachment_data, Name=os.path.basename(attachment))
                     attachment_part[
                         'Content-Disposition'] = f'attachment; filename="{os.path.basename(attachment)}"'
                     self.msg.attach(attachment_part)
 
             # recipients = [recipient_email] + cc if cc else [recipient_email]
-            recipients = [recipient_email]
+            recipients = recipient_email
             self.server.sendmail(
                 self.user_email, recipients, self.msg.as_string())
 
         except (smtplib.SMTPException, FileNotFoundError) as e:
             print(f"An error occurred while sending the email: {e}")
         finally:
             if server_quit:
```

### Comparing `MailToolsBox-0.1.0.3/MailToolsBox.egg-info/PKG-INFO` & `MailToolsBox-0.1.0.4/MailToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MailToolsBox
-Version: 0.1.0.3
+Version: 0.1.0.4
 Summary: Mail tools simplify mail server and sender development for developers.
 Home-page: https://www.rambod.net
 Download-URL: https://github.com/rambod/MailToolsBox/archive/0.0.4.6.tar.gz
 Author: Rambod Ghashghai
 Author-email: gh.rambod@gmail.com
 License: MIT
 Keywords: Mail,Server,smtp,send,email,tools,box
```

### Comparing `MailToolsBox-0.1.0.3/PKG-INFO` & `MailToolsBox-0.1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MailToolsBox
-Version: 0.1.0.3
+Version: 0.1.0.4
 Summary: Mail tools simplify mail server and sender development for developers.
 Home-page: https://www.rambod.net
 Download-URL: https://github.com/rambod/MailToolsBox/archive/0.0.4.6.tar.gz
 Author: Rambod Ghashghai
 Author-email: gh.rambod@gmail.com
 License: MIT
 Keywords: Mail,Server,smtp,send,email,tools,box
```

### Comparing `MailToolsBox-0.1.0.3/README.md` & `MailToolsBox-0.1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.3/setup.py` & `MailToolsBox-0.1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 
 setup(
     name='MailToolsBox',
     packages=['MailToolsBox'],
-    version='0.1.0.3',
+    version='0.1.0.4',
     license='MIT',
     # Give a short description about your library
     description='Mail tools simplify mail server and sender development for developers.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Rambod Ghashghai',                   # Type in your name
     author_email='gh.rambod@gmail.com',      # Type in your E-Mail
```

