# Comparing `tmp/MailToolsBox-0.1.0.2.tar.gz` & `tmp/MailToolsBox-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailToolsBox-0.1.0.2.tar", last modified: Tue Apr 18 07:15:12 2023, max compression
+gzip compressed data, was "MailToolsBox-0.1.0.3.tar", last modified: Tue Apr 18 11:46:51 2023, max compression
```

## Comparing `MailToolsBox-0.1.0.2.tar` & `MailToolsBox-0.1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/
--rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.112032 MailToolsBox-0.1.0.2/MailToolsBox/
--rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.2/MailToolsBox/__init__.py
--rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.2/MailToolsBox/imapClient.py
--rw-rw-rw-   0        0        0     3853 2023-04-17 09:46:24.000000 MailToolsBox-0.1.0.2/MailToolsBox/mailSender.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:15:12.138023 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3496 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-18 07:15:12.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 07:15:11.000000 MailToolsBox-0.1.0.2/MailToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3496 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2723 2023-04-17 11:23:42.000000 MailToolsBox-0.1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 07:15:12.140023 MailToolsBox-0.1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1388 2023-04-18 07:08:46.000000 MailToolsBox-0.1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.702589 MailToolsBox-0.1.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.662353 MailToolsBox-0.1.0.3/MailToolsBox/
+-rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.3/MailToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.3/MailToolsBox/imapClient.py
+-rw-rw-rw-   0        0        0     4341 2023-04-18 11:43:35.000000 MailToolsBox-0.1.0.3/MailToolsBox/mailSender.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:46:51.699590 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     6059 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 11:46:51.000000 MailToolsBox-0.1.0.3/MailToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6059 2023-04-18 11:46:51.701589 MailToolsBox-0.1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5232 2023-04-18 11:39:35.000000 MailToolsBox-0.1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 11:46:51.703589 MailToolsBox-0.1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-04-18 11:45:35.000000 MailToolsBox-0.1.0.3/setup.py
```

### Comparing `MailToolsBox-0.1.0.2/LICENSE.txt` & `MailToolsBox-0.1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.2/MailToolsBox/imapClient.py` & `MailToolsBox-0.1.0.3/MailToolsBox/imapClient.py`

 * *Files identical despite different names*

### Comparing `MailToolsBox-0.1.0.2/MailToolsBox/mailSender.py` & `MailToolsBox-0.1.0.3/MailToolsBox/mailSender.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,28 @@
         self.user_email_password = user_email_password
         self.server_smtp_address = server_smtp_address
         self.port = port
         self.msg = MIMEMultipart()
         self.msg['From'] = self.user_email
         self.server = smtplib.SMTP(self.server_smtp_address, self.port)
 
-    def send_mail(self, recipient_email: str, subject: str, message_body: str, cc: Optional[List[str]] = None,
-                  attachments: Optional[List[str]] = None, tls: bool = True, server_quit: bool = False) -> None:
+    def send_mail(self, recipient_email: Optional[List[str]], subject: str, message_body: str, cc: Optional[List[str]] = None,
+                  bcc: Optional[List[str]] = None, attachments: Optional[List[str]] = None, tls: bool = True, server_quit: bool = False) -> None:
         try:
             self.msg['Subject'] = subject
-            self.msg['To'] = recipient_email
+            # self.msg['To'] = recipient_email
+            self.msg['To'] = COMMASPACE.join(recipient_email) if not isinstance(
+                recipient_email, str) else recipient_email
             if cc:
-                self.msg['Cc'] = COMMASPACE.join(cc)
+                # self.msg['Cc'] = COMMASPACE.join(cc)
+                self.msg['Cc'] = COMMASPACE.join(
+                    cc) if not isinstance(cc, str) else cc
+            if bcc:
+                self.msg['Bcc'] = COMMASPACE.join(
+                    bcc) if not isinstance(bcc, str) else bcc
             if tls:
                 self.server.starttls()
             self.server.login(self.user_email, self.user_email_password)
 
             body = MIMEText(message_body, 'html')
             self.msg.attach(body)
 
@@ -40,15 +47,16 @@
                         attachment_data = attachment_file.read()
                     attachment_part = MIMEApplication(
                         attachment_data, Name=os.path.basename(attachment))
                     attachment_part[
                         'Content-Disposition'] = f'attachment; filename="{os.path.basename(attachment)}"'
                     self.msg.attach(attachment_part)
 
-            recipients = [recipient_email] + cc if cc else [recipient_email]
+            # recipients = [recipient_email] + cc if cc else [recipient_email]
+            recipients = [recipient_email]
             self.server.sendmail(
                 self.user_email, recipients, self.msg.as_string())
 
         except (smtplib.SMTPException, FileNotFoundError) as e:
             print(f"An error occurred while sending the email: {e}")
         finally:
             if server_quit:
```

### Comparing `MailToolsBox-0.1.0.2/setup.py` & `MailToolsBox-0.1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 
 setup(
     name='MailToolsBox',
     packages=['MailToolsBox'],
-    version='0.1.0.2',
+    version='0.1.0.3',
     license='MIT',
     # Give a short description about your library
     description='Mail tools simplify mail server and sender development for developers.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Rambod Ghashghai',                   # Type in your name
     author_email='gh.rambod@gmail.com',      # Type in your E-Mail
```

