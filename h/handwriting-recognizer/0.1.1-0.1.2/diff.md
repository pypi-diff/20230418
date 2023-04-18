# Comparing `tmp/handwriting_recognizer-0.1.1.tar.gz` & `tmp/handwriting_recognizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handwriting_recognizer-0.1.1.tar", max compression
+gzip compressed data, was "handwriting_recognizer-0.1.2.tar", max compression
```

## Comparing `handwriting_recognizer-0.1.1.tar` & `handwriting_recognizer-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-18 06:42:53.995961 handwriting_recognizer-0.1.1/handwriting_recognizer/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-18 07:33:09.289424 handwriting_recognizer-0.1.1/handwriting_recognizer/main.py
--rw-r--r--   0        0        0      553 2023-04-18 07:35:27.100751 handwriting_recognizer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-18 06:42:53.995961 handwriting_recognizer-0.1.1/README.md
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 handwriting_recognizer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 06:42:53.995961 handwriting_recognizer-0.1.2/handwriting_recognizer/__init__.py
+-rw-r--r--   0        0        0     5456 2023-04-18 07:49:13.197589 handwriting_recognizer-0.1.2/handwriting_recognizer/main.py
+-rw-r--r--   0        0        0      592 2023-04-18 07:49:16.312710 handwriting_recognizer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 06:42:53.995961 handwriting_recognizer-0.1.2/README.md
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 handwriting_recognizer-0.1.2/PKG-INFO
```

### Comparing `handwriting_recognizer-0.1.1/handwriting_recognizer/main.py` & `handwriting_recognizer-0.1.2/handwriting_recognizer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import tkinter as tk
 from tkinter import *
 from tkinter import messagebox
 
 window = tk.Tk()
 window.title("Handwritten digit recognition")
 
-l1 = tk.Label(window, text="Digit", font=('Algerian', 20))
+l1 = tk.Label(window, text="Digit", font=('Algerian', 12))
 l1.place(x=5, y=0)
 
 t1 = tk.Entry(window, width=20, border=5)
 t1.place(x=150, y=0)
 
 
 def screen_capture():
     import pyscreenshot as ImageGrab
     import time
     import os
     os.startfile(
         "C:/ProgramData/Microsoft/Windows/Start Menu/Programs/Accessories/Paint")
     s1 = t1.get()
     print("S1: "+s1)
+    if not os.path.exists("captured_images/"+s1):
+        os.makedirs("captured_images/"+s1)  
     os.chdir(t2.get() + "/captured_images")
     os.chdir(t2.get())
 
     # "C:/Users/adiun/Github/Handwriting_Recognizer"
 
     images_folder = "captured_images/"+s1+"/"
     time.sleep(15)
@@ -31,15 +33,15 @@
         time.sleep(8)
         im = ImageGrab.grab(bbox=(60, 150, 400, 550))  # x1,y1,x2,y2
         print("saved......", i)
         im.save(images_folder+str(i)+'.png')
         print("clear screen now and redraw now........")
     messagebox.showinfo("Result", "Capturing screen is completed!!")
 
-l2 = tk.Label(window, text="Enter folder path", font=('Algerian', 20))
+l2 = tk.Label(window, text="Enter folder path", font=('Algerian', 12))
 l2.place(x=5, y= 10)
 
 t2 = tk.Entry(window, width=20, border=5)
 t2.place(x=150, y=30)
 b1 = tk.Button(window, text="1. Open paint and capture the screen", font=(
     'Algerian', 15), bg="orange", fg="black", command=screen_capture)
 b1.place(x=5, y=50)
```

### Comparing `handwriting_recognizer-0.1.1/pyproject.toml` & `handwriting_recognizer-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "handwriting-recognizer"
-version = "0.1.1"
+version = "0.1.2"
 description = "handwriting project recognizer using paint"
 authors = ["Aditya Unnikrishnan <adiunni@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "handwriting_recognizer"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.7"
 pyscreenshot = "^3.1"
 opencv-python = "^4.7.0.72"
 pillow = "^9.5.0"
+scikit-learn = "^1.2.2"
+tk = "^0.1.0"
 
 [tool.poetry.scripts]
 handwriting_recognizer = "handwriting_recognizer.main:main"
 
 
 [build-system]
 requires = ["poetry-core"]
```

