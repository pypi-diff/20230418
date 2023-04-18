# Comparing `tmp/tpl.py-0.0.0.tar.gz` & `tmp/tpl.py-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpl.py-0.0.0.tar", last modified: Tue Apr 18 17:29:24 2023, max compression
+gzip compressed data, was "tpl.py-0.1.tar", last modified: Tue Apr 18 16:10:39 2023, max compression
```

## Comparing `tpl.py-0.0.0.tar` & `tpl.py-0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:29:24.422348 tpl.py-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 17:29:14.000000 tpl.py-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 17:29:14.000000 tpl.py-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 17:29:24.422348 tpl.py-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-18 17:29:14.000000 tpl.py-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 17:29:14.000000 tpl.py-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:29:24.422348 tpl.py-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 17:29:14.000000 tpl.py-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:29:24.418347 tpl.py-0.0.0/template_py/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 17:29:14.000000 tpl.py-0.0.0/template_py/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8027 2023-04-18 17:29:14.000000 tpl.py-0.0.0/template_py/template_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:29:24.422348 tpl.py-0.0.0/tpl.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 17:29:24.000000 tpl.py-0.0.0/tpl.py.egg-info/top_level.txt
+drwxr-xr-x   0 larskghf   (501) staff       (20)        0 2023-04-18 16:10:39.644949 tpl.py-0.1/
+-rw-r--r--   0 larskghf   (501) staff       (20)    11357 2023-04-17 21:25:27.000000 tpl.py-0.1/LICENSE
+-rw-r--r--   0 larskghf   (501) staff       (20)       50 2023-04-18 15:49:06.000000 tpl.py-0.1/MANIFEST.in
+-rw-r--r--   0 larskghf   (501) staff       (20)       70 2023-04-18 16:10:39.644816 tpl.py-0.1/PKG-INFO
+-rw-r--r--   0 larskghf   (501) staff       (20)     4666 2023-04-18 15:56:37.000000 tpl.py-0.1/README.md
+-rw-r--r--   0 larskghf   (501) staff       (20)       19 2023-04-17 21:25:27.000000 tpl.py-0.1/requirements.txt
+-rw-r--r--   0 larskghf   (501) staff       (20)       38 2023-04-18 16:10:39.644999 tpl.py-0.1/setup.cfg
+-rw-r--r--   0 larskghf   (501) staff       (20)      339 2023-04-18 16:10:36.000000 tpl.py-0.1/setup.py
+drwxr-xr-x   0 larskghf   (501) staff       (20)        0 2023-04-18 16:10:39.643856 tpl.py-0.1/template_py/
+-rw-r--r--   0 larskghf   (501) staff       (20)       29 2023-04-18 15:57:34.000000 tpl.py-0.1/template_py/__init__.py
+-rwxr-xr-x   0 larskghf   (501) staff       (20)     8027 2023-04-18 15:54:40.000000 tpl.py-0.1/template_py/template_py.py
+drwxr-xr-x   0 larskghf   (501) staff       (20)        0 2023-04-18 16:10:39.644520 tpl.py-0.1/tpl.py.egg-info/
+-rw-r--r--   0 larskghf   (501) staff       (20)       70 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/PKG-INFO
+-rw-r--r--   0 larskghf   (501) staff       (20)      288 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/SOURCES.txt
+-rw-r--r--   0 larskghf   (501) staff       (20)        1 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/dependency_links.txt
+-rw-r--r--   0 larskghf   (501) staff       (20)       75 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/entry_points.txt
+-rw-r--r--   0 larskghf   (501) staff       (20)       20 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/requires.txt
+-rw-r--r--   0 larskghf   (501) staff       (20)       12 2023-04-18 16:10:39.000000 tpl.py-0.1/tpl.py.egg-info/top_level.txt
```

### Comparing `tpl.py-0.0.0/LICENSE` & `tpl.py-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tpl.py-0.0.0/README.md` & `tpl.py-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 `template.py` is a simple python-based templating engine. It allows you to define templates for configuration files,
 which can be customized with values from environment variables or a variable file. Additionally, it provides the option
 to encrypt and decrypt the resulting files.
 
 ## 🚀 Usage
 
 ```bash
-template.py [-h] [-i DIR/FILE] [-o DIR/FILE] [-e ENC_KEY] [-d ENC_KEY] [--var-file VAR_FILE] [--create-encryption-key]
+py-template_py.py [-h] [-i DIR/FILE] [-o DIR/FILE] [-e ENC_KEY] [-d ENC_KEY] [--var-file VAR_FILE] [--create-encryption-key]
 ```
 
 ### Arguments
 
 * `-h, --help`: show help message and exit
 * `-i DIR/FILE, --input DIR/FILE`: set input directory or single file
 * `-o DIR/FILE, --output DIR/FILE`: set output directory or single file
@@ -19,74 +19,74 @@
 * `-d ENC_KEY, --decrypt ENC_KEY`: set mode to decrypt an encrypted file (parameter: encryption key)
 * `--var-file VAR_FILE`: provide variable file instead of using environment variables
 * `--create-encryption-key`: generate new encryption key and print to console
 
 ### Examples
 
 ```bash
-template.py -i <Input> -o <Output>
+py-template_py.py -i <Input> -o <Output>
 ```
 
 ```bash
-template.py -e <encryption_key> -i <Input> -o <Output>
+py-template_py.py -e <encryption_key> -i <Input> -o <Output>
 ```
 
 ```bash
-template.py -d <encryption_key> -i <Input> -o <Output>
+py-template_py.py -d <encryption_key> -i <Input> -o <Output>
 ```
 
 ## :whale: Using `template.py` with Docker
 
 `template.py` is also available as a Docker image. This allows you to use the tool without having to install it on your
 local machine.
 
 To use `template.py` with Docker, you can pull the latest image from Docker Hub:
 
 ```bash
-docker pull larskghf/template.py:latest
+docker pull larskghf/py-template_py.py:latest
 ```
 
 You can then run the image using the `docker run` command. For example, to use `template.py` to render a template file
 and write the output to a file on your local machine, you can use the following command:
 
 ```bash
-docker run --rm -v /path/to/input:/input -v /path/to/output:/output larskghf/template.py:latest -i /input/template.tpl -o /output/output.txt
+docker run --rm -v /path/to/input:/input -v /path/to/output:/output larskghf/py-template_py.py:latest -i /input/template_py.tpl -o /output/output.txt
 ```
 
 This command mounts two volumes (`/path/to/input` and `/path/to/output`) to the Docker container, which
 allows `template.py` to access the input and output files on your local machine.
 
 Note that the `--rm` flag removes the container after it has finished running, which helps to keep your Docker
 environment clean.
 
 You can also pass other command-line arguments to `template.py` as part of the `docker run` command. For example, to
 encrypt the output file using an encryption key, you can use the following command:
 
 ```bash
-docker run --rm -v /path/to/input:/input -v /path/to/output:/output larskghf/template.py:latest -i /input/template.tpl -o /output/output.txt -e <encryption_key>
+docker run --rm -v /path/to/input:/input -v /path/to/output:/output larskghf/py-template_py.py:latest -i /input/template_py.tpl -o /output/output.txt -e <encryption_key>
 ```
 
 Again, make sure to replace `/path/to/input`, `/path/to/output`, and `<encryption_key>` with the appropriate values for
 your environment.
 
 ## 🔑 How to create a new encryption key
 
 `template.py` provides an option to create a new encryption key. This is useful if you want to encrypt the resulting
 files and you don't have a key yet. To create a new encryption key, run `template.py` with the `--create-encryption-key`
 argument:
 
 ```bash
-template.py --create-encryption-key
+py-template_py.py --create-encryption-key
 ```
 
 This will generate a new encryption key and print it to the console. You can then copy the key and use it to encrypt
 your files by running `template.py` with the `-e` argument followed by the key:
 
 ```bash
-template.py -e <encryption_key> -i <Input> -o <Output>
+py-template_py.py -e <encryption_key> -i <Input> -o <Output>
 ```
 
 Note that the encryption key should be kept secret and not shared with anyone who should not have access to the
 encrypted files.
 
 ## 🔧 How it works
```

### Comparing `tpl.py-0.0.0/template_py/template_py.py` & `tpl.py-0.1/template_py/template_py.py`

 * *Files identical despite different names*

