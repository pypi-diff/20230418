# Comparing `tmp/ExpdFtpService-0.6.0.tar.gz` & `tmp/ExpdFtpService-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdFtpService-0.6.0.tar", last modified: Thu Apr 13 01:57:24 2023, max compression
+gzip compressed data, was "dist\ExpdFtpService-0.7.0.tar", last modified: Tue Apr 18 05:36:32 2023, max compression
```

## Comparing `ExpdFtpService-0.6.0.tar` & `ExpdFtpService-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/
--rw-rw-rw-   0        0        0      305 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-04-07 09:01:05.000000 ExpdFtpService-0.6.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-04-13 01:56:30.000000 ExpdFtpService-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService/
--rw-rw-rw-   0        0        0     4348 2023-04-13 01:57:14.000000 ExpdFtpService-0.6.0/src/ExpdFtpService/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 01:57:24.000000 ExpdFtpService-0.6.0/src/ExpdFtpService.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/
+-rw-rw-rw-   0        0        0      305 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-04-07 09:01:05.000000 ExpdFtpService-0.7.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-04-18 04:32:03.000000 ExpdFtpService-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService/
+-rw-rw-rw-   0        0        0     4339 2023-04-18 05:35:54.000000 ExpdFtpService-0.7.0/src/ExpdFtpService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:36:32.000000 ExpdFtpService-0.7.0/src/ExpdFtpService.egg-info/top_level.txt
```

### Comparing `ExpdFtpService-0.6.0/README.md` & `ExpdFtpService-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ExpdFtpService-0.6.0/src/ExpdFtpService/__init__.py` & `ExpdFtpService-0.7.0/src/ExpdFtpService/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     """
     The ConnFtpServer class is used for connecting to a FTP Server. The constructor accepts the following parameters with the indicated types:
         hostname (str): The hostname of the FTP server.
         username (str): The username to login to the FTP server.
         password (str): The password to login to the FTP server.
     """    
     def __init__(self, hostname, username, password):
+        self.servercode = str(hostname).split("-")[0].upper()
         self.ftp = FTP()
         self.ftp.connect(host=hostname, port=21)
         self.ftp.sendcmd('OPTS UTF8 ON')
         self.ftp.set_pasv(True)
         self.ftp.login(user=username, passwd=password)
 
 
@@ -33,35 +34,34 @@
         self.ftp.cwd(self.destfolder)
         if self.fstartwith is not None:
             files = [x for x in self.ftp.nlst() if x.startswith(self.fstartwith)]
         elif self.filendwith is not None:
             files = [x for x in self.ftp.nlst() if x.endswith(self.filendwith)]
         else:
             files = [x for x in self.ftp.nlst() if str(x).lower() != 'history']
-            logger.debug(f"server total files: [{len(files)}]")
+        logger.debug(f"server total files: [{len(files)}]")
         return files
     
     def archive(self, from_file, to_path, to_file):
         history = self.ftp.nlst(to_path)
         if to_file not in history:
             self.ftp.rename(f"{from_file}", f"{to_path}\{to_file}")
-            # logger.debug(f"server file [ {from_file} ] archived to history folder successfully.")
         else:
             logger.warning(f"file exist in history folder, delete: {from_file}")
             self.ftp.delete(from_file)
 
     @logger.catch(reraise=True)
     def download(self, numbers):
         try:
             for count, file in enumerate(self.files, 1):
                 if count <= numbers:
                     with open(path.join(self.savefolder, f"{file}"), 'wb') as rd:
                         self.ftp.retrbinary('RETR %s' % file, rd.write)
                     self.archive(file, "History", file)
-                    logger.debug(f"NO.{count}: file {file} download & archived successfully")
+                    logger.debug(f"NO.{count}: file {file} download from {self.servercode} successfully")
         finally:
             self.ftp.quit()
     
 
 class ExpdUploadFtpServerFile(ConnFtpServer):
     """Class is used for connecting to a FTP Server and upload files.
         The constructor accepts the following parameters with the indicated types:
@@ -84,15 +84,15 @@
     
     @logger.catch(reraise=True)
     def upload_file_to_server(self, local_file):
         try:
             with open(local_file,'rb') as f:  
                 self.ftp.cwd(self.destfolder)          
                 self.ftp.storbinary(f'STOR {path.basename(local_file)}', f)
-                logger.debug(f"{local_file} uploaded successfully")
+                logger.debug(f"{local_file} uploaded to {self.servercode} successfully")
         finally:
             self.ftp.quit()
     
 
 if __name__ == '__main__':
     ExpdUploadFtpServerFile(
         hostname="xxx",
```

