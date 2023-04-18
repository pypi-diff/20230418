# Comparing `tmp/tkdial-0.0.4.tar.gz` & `tmp/tkdial-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkdial-0.0.4.tar", last modified: Wed Nov 30 06:16:59 2022, max compression
+gzip compressed data, was "tkdial-0.0.5.tar", last modified: Tue Apr 18 10:35:28 2023, max compression
```

## Comparing `tkdial-0.0.4.tar` & `tkdial-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 06:16:59.888882 tkdial-0.0.4/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    13895 2022-11-30 06:16:59.888882 tkdial-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13295 2022-11-30 06:16:24.000000 tkdial-0.0.4/README.md
--rw-rw-rw-   0        0        0      598 2022-11-30 06:16:59.888882 tkdial-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1133 2022-11-29 06:47:23.000000 tkdial-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-30 06:16:59.856262 tkdial-0.0.4/tkdial/
--rw-rw-rw-   0        0        0      367 2022-11-29 06:46:49.000000 tkdial-0.0.4/tkdial/__init__.py
--rw-rw-rw-   0        0        0    13441 2022-11-30 05:32:41.000000 tkdial-0.0.4/tkdial/meter.py
--rw-rw-rw-   0        0        0     8386 2022-11-27 13:47:40.000000 tkdial-0.0.4/tkdial/scrollknob.py
--rw-rw-rw-   0        0        0    16011 2022-11-29 17:24:58.000000 tkdial-0.0.4/tkdial/tkdial.py
-drwxrwxrwx   0        0        0        0 2022-11-30 06:16:59.888882 tkdial-0.0.4/tkdial.egg-info/
--rw-rw-rw-   0        0        0    13895 2022-11-30 06:16:59.000000 tkdial-0.0.4/tkdial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2022-11-30 06:16:59.000000 tkdial-0.0.4/tkdial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2022-11-30 06:16:59.000000 tkdial-0.0.4/tkdial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-11-30 06:16:59.000000 tkdial-0.0.4/tkdial.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-30 06:16:59.000000 tkdial-0.0.4/tkdial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.326878 tkdial-0.0.5/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    16712 2023-04-18 10:35:28.326878 tkdial-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16112 2023-04-18 10:34:41.000000 tkdial-0.0.5/README.md
+-rw-rw-rw-   0        0        0      598 2023-04-18 10:35:28.342508 tkdial-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1133 2023-04-18 10:34:53.000000 tkdial-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.279989 tkdial-0.0.5/tkdial/
+-rw-rw-rw-   0        0        0      381 2023-04-18 08:26:58.000000 tkdial-0.0.5/tkdial/__init__.py
+-rw-rw-rw-   0        0        0    15120 2023-04-18 10:20:00.000000 tkdial-0.0.5/tkdial/jogwheel.py
+-rw-rw-rw-   0        0        0    14988 2023-04-18 09:34:10.000000 tkdial-0.0.5/tkdial/meter.py
+-rw-rw-rw-   0        0        0     9627 2023-04-18 09:33:53.000000 tkdial-0.0.5/tkdial/scrollknob.py
+-rw-rw-rw-   0        0        0    17769 2023-04-18 09:34:03.000000 tkdial-0.0.5/tkdial/tkdial.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:35:28.311248 tkdial-0.0.5/tkdial.egg-info/
+-rw-rw-rw-   0        0        0    16712 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       33 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 10:35:28.000000 tkdial-0.0.5/tkdial.egg-info/top_level.txt
```

### Comparing `tkdial-0.0.4/LICENSE` & `tkdial-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.4/PKG-INFO` & `tkdial-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkdial
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rotatory dial-knob widgets for Tkinter.
 Home-page: https://github.com/Akascape/TkDial
 Author: Akascape
 License: Creative Commons Zero v1.0 Universal
 Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -82,31 +82,31 @@
                 
 app.grid_columnconfigure((0,1), weight=1)
 app.grid_rowconfigure((0,1), weight=1)
 
 frame_1 = customtkinter.CTkFrame(master=app)
 frame_1.grid(padx=20, pady=20, sticky="nswe")
 
-dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"), bg="#2a2d2e",
+dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"),
              text_color="white", text="Current: ", unit_length=10, radius=50)
 dial1.grid(padx=20, pady=20)
 
-dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"), bg="#2a2d2e",
+dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"),
              text_color="white", text="Position: ", unit_length=10, radius=50)
 dial2.grid(padx=20, pady=20)
 
-dial3 = Dial(master=frame_1, color_gradient=("white", "pink"), bg="#2a2d2e",
+dial3 = Dial(master=frame_1, color_gradient=("white", "pink"),
              text_color="white", text=" ", unit_length=10, radius=50)
 dial3.grid(row=0, column=1, padx=20, pady=20)
 
-dial4 = Dial(master=frame_1, color_gradient=("green", "green"), bg="#2a2d2e",
+dial4 = Dial(master=frame_1, color_gradient=("green", "green"),
              text_color="white", text="", unit_width=15, radius=50)
 dial4.grid(row=1, column=1, padx=20, pady=20)
 
-app.mainloop()                  
+app.mainloop()                
 ```
 ![Screenshot 3](https://user-images.githubusercontent.com/89206401/202906638-a1c863b7-54b0-4e7a-9619-415e28b3ab51.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -161,37 +161,37 @@
 ```python
 import customtkinter
 from tkdial import ScrollKnob
 
 app = customtkinter.CTk()
 app.geometry("500x500")
 
-knob1 = ScrollKnob(app, bg="#212325", radius=250, progress_color="#87ceeb", steps=10,
+knob1 = ScrollKnob(app, radius=250, progress_color="#87ceeb", steps=10,
                  border_width=40, start_angle=90, inner_width=1, outer_width=1,
                  text_font="calibri 20", text_color="#87ceeb", bar_color="black")
 knob1.grid(row=0, column=0)
 
-knob2 = ScrollKnob(app, bg="#212325", radius=200, progress_color="#7eff00",
+knob2 = ScrollKnob(app, radius=200, progress_color="#7eff00",
                  border_width=40, start_angle=90, inner_width=1, outer_width=0,
                  text_font="calibri 20", text_color="#7eff00", integer=True,
                  fg="#212325")
 knob2.grid(row=1, column=0)
 
-knob3 = ScrollKnob(app, bg="#212325", text=" ", radius=250, progress_color="white",
+knob3 = ScrollKnob(app, text=" ", radius=250, progress_color="white",
                    bar_color="#2937a6", border_width=30, start_angle=0, inner_width=5,
                    outer_width=0, text_font="calibri 20", steps=1, text_color="white", fg="#303ba1")
 knob3.grid(row=0, column=1)
 
-knob4 = ScrollKnob(app, bg="#212325", text=" ", steps=10, radius=200, bar_color="#212325", 
+knob4 = ScrollKnob(app, text=" ", steps=10, radius=200, bar_color="#242424", 
                    progress_color="yellow", outer_color="yellow", outer_length=10, 
                    border_width=30, start_angle=270, inner_width=0, outer_width=5, text_font="calibri 20", 
                    text_color="white", fg="#212325")
 knob4.grid(row=1, column=1)
                 
-app.mainloop()      
+app.mainloop() 
 ```
 ![Complex example](https://user-images.githubusercontent.com/89206401/204139428-c3c3c313-539f-4867-9d50-8876a19432ee.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -246,40 +246,38 @@
 ```python
 import customtkinter
 from tkdial import Meter
 
 app = customtkinter.CTk()
 app.geometry("950x350")
 
-meter1 = Meter(app, bg="#212325", radius=300, start=0, end=160, border_width=0,
+meter1 = Meter(app, radius=300, start=0, end=160, border_width=0,
                fg="black", text_color="white", start_angle=270, end_angle=-270,
                text_font="DS-Digital 30", scale_color="white", needle_color="red")
 meter1.set_mark(140, 160) # set red marking from 140 to 160
 meter1.grid(row=0, column=1, padx=20, pady=30)
 
-meter2 = Meter(app, bg="#212325", radius=260, start=0, end=200, border_width=5,
+meter2 = Meter(app, radius=260, start=0, end=200, border_width=5,
                fg="black", text_color="white", start_angle=270, end_angle=-360,
                text_font="DS-Digital 30", scale_color="black", axis_color="white",
                needle_color="white")
 meter2.set_mark(1, 100, "#92d050")
 meter2.set_mark(105, 150, "yellow")
 meter2.set_mark(155, 196, "red")
 meter2.set(80) # set value
 meter2.grid(row=0, column=0, padx=20, pady=30)
 
-meter3 = Meter(app, bg="#212325", fg="#212325", radius=300, start=0, end=50,
+meter3 = Meter(app, fg="#242424", radius=300, start=0, end=50,
                major_divisions=10, border_width=0, text_color="white",
                start_angle=0, end_angle=-360, scale_color="white", axis_color="cyan",
                needle_color="white",  scroll_steps=0.2)
 meter3.set(15)
 meter3.grid(row=0, column=2, pady=30)
 
 app.mainloop()
-                    
-# Font used: https://www.dafont.com/ds-digital.font
 ```
 ![styles_meter](https://user-images.githubusercontent.com/89206401/204718389-d3195b3b-0f7a-41c3-85b8-ffc1d961db70.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -309,14 +307,94 @@
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the meter |
   | _.set()_ | set the value of the meter |
+  | _.configure()_ | configure parameters of the meter| 
+  | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
+  
+# JogWheel
+
+## Usage
+
+```python
+import tkinter
+from tkdial import Jogwheel
+
+app = tkinter.Tk()
+
+knob = Jogwheel(app)
+knob.grid()
+
+app.mainloop()
+```
+![Jogwheel](https://user-images.githubusercontent.com/89206401/232750598-37f4f863-0aba-48c8-9a69-4cb1e15e1457.png)
+
+### Styles: 
+```python
+import customtkinter
+from tkdial import Jogwheel
+
+app = customtkinter.CTk()
+
+wheel_1 = Jogwheel(app, radius=200, fg="#045252", scale_color="white",
+                text=None, button_radius=10)
+wheel_1.set_mark(0,100, "green")
+
+wheel_1.grid()
+
+wheel_2 = Jogwheel(app, radius=200, fg="#045252", scale_color="white", start_angle=0,
+                   end_angle=360, start=0, end=200, text="Volume: ", button_radius=10)
+wheel_2.set_mark(0,50, "blue")
+wheel_2.set_mark(50, 90, "green")
+wheel_2.set_mark(90, 150, "orange")
+wheel_2.set_mark(150, 200, "red")
+wheel_2.grid()
+
+app.mainloop()
+```
+![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the meter widget |
+  | _fg_ | Specify the color of the wheel face |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _start_angle_ | Determines the starting angle of the arc |
+  | _end_angle_ | Determines the final angle of the arc |
+  | _radius_ | Determines the radius for the widget |
+  | _divisions_ | Determines the number of scale lines in the scale |
+  | _division_height_ | Determines the height of scale lines |
+  | _scale_color_ |  Specify the color of the knob scale |
+  | _border_width_ | Define the width of the border case (default=1) |
+  | _border_color_ |  Specify the color of the border case |
+  | _button_color_ | Specify the color of the knob |
+  | _button_radius_ | Specify the radius the knob |
+  | _text_ | A string that will be displayed |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the meter |
+  | _.set()_ | set the value of the meter |
   | _.configure()_ | configure parameters of the meter| 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
 ## Conclusion
 This library is focused to create some circular widgets that can be used with Tkinter easily.
 I hope it will be helpful for UI development in python.
```

### Comparing `tkdial-0.0.4/README.md` & `tkdial-0.0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -67,31 +67,31 @@
                 
 app.grid_columnconfigure((0,1), weight=1)
 app.grid_rowconfigure((0,1), weight=1)
 
 frame_1 = customtkinter.CTkFrame(master=app)
 frame_1.grid(padx=20, pady=20, sticky="nswe")
 
-dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"), bg="#2a2d2e",
+dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"),
              text_color="white", text="Current: ", unit_length=10, radius=50)
 dial1.grid(padx=20, pady=20)
 
-dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"), bg="#2a2d2e",
+dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"),
              text_color="white", text="Position: ", unit_length=10, radius=50)
 dial2.grid(padx=20, pady=20)
 
-dial3 = Dial(master=frame_1, color_gradient=("white", "pink"), bg="#2a2d2e",
+dial3 = Dial(master=frame_1, color_gradient=("white", "pink"),
              text_color="white", text=" ", unit_length=10, radius=50)
 dial3.grid(row=0, column=1, padx=20, pady=20)
 
-dial4 = Dial(master=frame_1, color_gradient=("green", "green"), bg="#2a2d2e",
+dial4 = Dial(master=frame_1, color_gradient=("green", "green"),
              text_color="white", text="", unit_width=15, radius=50)
 dial4.grid(row=1, column=1, padx=20, pady=20)
 
-app.mainloop()                  
+app.mainloop()                
 ```
 ![Screenshot 3](https://user-images.githubusercontent.com/89206401/202906638-a1c863b7-54b0-4e7a-9619-415e28b3ab51.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -146,37 +146,37 @@
 ```python
 import customtkinter
 from tkdial import ScrollKnob
 
 app = customtkinter.CTk()
 app.geometry("500x500")
 
-knob1 = ScrollKnob(app, bg="#212325", radius=250, progress_color="#87ceeb", steps=10,
+knob1 = ScrollKnob(app, radius=250, progress_color="#87ceeb", steps=10,
                  border_width=40, start_angle=90, inner_width=1, outer_width=1,
                  text_font="calibri 20", text_color="#87ceeb", bar_color="black")
 knob1.grid(row=0, column=0)
 
-knob2 = ScrollKnob(app, bg="#212325", radius=200, progress_color="#7eff00",
+knob2 = ScrollKnob(app, radius=200, progress_color="#7eff00",
                  border_width=40, start_angle=90, inner_width=1, outer_width=0,
                  text_font="calibri 20", text_color="#7eff00", integer=True,
                  fg="#212325")
 knob2.grid(row=1, column=0)
 
-knob3 = ScrollKnob(app, bg="#212325", text=" ", radius=250, progress_color="white",
+knob3 = ScrollKnob(app, text=" ", radius=250, progress_color="white",
                    bar_color="#2937a6", border_width=30, start_angle=0, inner_width=5,
                    outer_width=0, text_font="calibri 20", steps=1, text_color="white", fg="#303ba1")
 knob3.grid(row=0, column=1)
 
-knob4 = ScrollKnob(app, bg="#212325", text=" ", steps=10, radius=200, bar_color="#212325", 
+knob4 = ScrollKnob(app, text=" ", steps=10, radius=200, bar_color="#242424", 
                    progress_color="yellow", outer_color="yellow", outer_length=10, 
                    border_width=30, start_angle=270, inner_width=0, outer_width=5, text_font="calibri 20", 
                    text_color="white", fg="#212325")
 knob4.grid(row=1, column=1)
                 
-app.mainloop()      
+app.mainloop() 
 ```
 ![Complex example](https://user-images.githubusercontent.com/89206401/204139428-c3c3c313-539f-4867-9d50-8876a19432ee.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -231,40 +231,38 @@
 ```python
 import customtkinter
 from tkdial import Meter
 
 app = customtkinter.CTk()
 app.geometry("950x350")
 
-meter1 = Meter(app, bg="#212325", radius=300, start=0, end=160, border_width=0,
+meter1 = Meter(app, radius=300, start=0, end=160, border_width=0,
                fg="black", text_color="white", start_angle=270, end_angle=-270,
                text_font="DS-Digital 30", scale_color="white", needle_color="red")
 meter1.set_mark(140, 160) # set red marking from 140 to 160
 meter1.grid(row=0, column=1, padx=20, pady=30)
 
-meter2 = Meter(app, bg="#212325", radius=260, start=0, end=200, border_width=5,
+meter2 = Meter(app, radius=260, start=0, end=200, border_width=5,
                fg="black", text_color="white", start_angle=270, end_angle=-360,
                text_font="DS-Digital 30", scale_color="black", axis_color="white",
                needle_color="white")
 meter2.set_mark(1, 100, "#92d050")
 meter2.set_mark(105, 150, "yellow")
 meter2.set_mark(155, 196, "red")
 meter2.set(80) # set value
 meter2.grid(row=0, column=0, padx=20, pady=30)
 
-meter3 = Meter(app, bg="#212325", fg="#212325", radius=300, start=0, end=50,
+meter3 = Meter(app, fg="#242424", radius=300, start=0, end=50,
                major_divisions=10, border_width=0, text_color="white",
                start_angle=0, end_angle=-360, scale_color="white", axis_color="cyan",
                needle_color="white",  scroll_steps=0.2)
 meter3.set(15)
 meter3.grid(row=0, column=2, pady=30)
 
 app.mainloop()
-                    
-# Font used: https://www.dafont.com/ds-digital.font
 ```
 ![styles_meter](https://user-images.githubusercontent.com/89206401/204718389-d3195b3b-0f7a-41c3-85b8-ffc1d961db70.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -294,14 +292,94 @@
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the meter |
   | _.set()_ | set the value of the meter |
+  | _.configure()_ | configure parameters of the meter| 
+  | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
+  
+# JogWheel
+
+## Usage
+
+```python
+import tkinter
+from tkdial import Jogwheel
+
+app = tkinter.Tk()
+
+knob = Jogwheel(app)
+knob.grid()
+
+app.mainloop()
+```
+![Jogwheel](https://user-images.githubusercontent.com/89206401/232750598-37f4f863-0aba-48c8-9a69-4cb1e15e1457.png)
+
+### Styles: 
+```python
+import customtkinter
+from tkdial import Jogwheel
+
+app = customtkinter.CTk()
+
+wheel_1 = Jogwheel(app, radius=200, fg="#045252", scale_color="white",
+                text=None, button_radius=10)
+wheel_1.set_mark(0,100, "green")
+
+wheel_1.grid()
+
+wheel_2 = Jogwheel(app, radius=200, fg="#045252", scale_color="white", start_angle=0,
+                   end_angle=360, start=0, end=200, text="Volume: ", button_radius=10)
+wheel_2.set_mark(0,50, "blue")
+wheel_2.set_mark(50, 90, "green")
+wheel_2.set_mark(90, 150, "orange")
+wheel_2.set_mark(150, 200, "red")
+wheel_2.grid()
+
+app.mainloop()
+```
+![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the meter widget |
+  | _fg_ | Specify the color of the wheel face |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _start_angle_ | Determines the starting angle of the arc |
+  | _end_angle_ | Determines the final angle of the arc |
+  | _radius_ | Determines the radius for the widget |
+  | _divisions_ | Determines the number of scale lines in the scale |
+  | _division_height_ | Determines the height of scale lines |
+  | _scale_color_ |  Specify the color of the knob scale |
+  | _border_width_ | Define the width of the border case (default=1) |
+  | _border_color_ |  Specify the color of the border case |
+  | _button_color_ | Specify the color of the knob |
+  | _button_radius_ | Specify the radius the knob |
+  | _text_ | A string that will be displayed |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the meter |
+  | _.set()_ | set the value of the meter |
   | _.configure()_ | configure parameters of the meter| 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
 ## Conclusion
 This library is focused to create some circular widgets that can be used with Tkinter easily.
 I hope it will be helpful for UI development in python.
```

### Comparing `tkdial-0.0.4/setup.cfg` & `tkdial-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b64 6961 6c0d 0a76 6572 7369   = tkdial..versi
-00000020: 6f6e 203d 2030 2e30 2e34 0d0a 6465 7363  on = 0.0.4..desc
+00000020: 6f6e 203d 2030 2e30 2e35 0d0a 6465 7363  on = 0.0.5..desc
 00000030: 7269 7074 696f 6e20 3d20 546b 696e 7465  ription = Tkinte
 00000040: 7220 4469 616c 2061 6e64 204b 6e6f 6220  r Dial and Knob 
 00000050: 5769 6467 6574 730d 0a6c 6f6e 675f 6465  Widgets..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `tkdial-0.0.4/setup.py` & `tkdial-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tkdial',
-    version = '0.0.4',
+    version = '0.0.5',
     description = "Rotatory dial-knob widgets for Tkinter.",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akascape',
     url = "https://github.com/Akascape/TkDial",
```

### Comparing `tkdial-0.0.4/tkdial/meter.py` & `tkdial-0.0.5/tkdial/jogwheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,85 @@
-###################--------------TkDial-Meter--------------###################
+###################--------------TkDial-Jogwheel--------------###################
 
 import tkinter as tk
 import tkinter.font as tkFont
-import math, cmath
+import math
+
+class Jogwheel(tk.Canvas):
 
-class Meter(tk.Canvas):
-    
     def __init__(self,
                  master,
                  start: float = 0,
                  end: float = 100,
                  radius: int = 250,
                  width: int = None,
                  height: int = None,
                  text: str = " ",
                  text_color: str = "black",
                  text_font: str = None,
-                 border_width: int = 1,
-                 border_color: int = "grey40",
-                 major_divisions: int = 10,
-                 minor_divisions: int = 1,
+                 border_width: int = 3,
+                 border_color: str = "black",
+                 divisions: int = 10,
+                 division_height: int = 10,
                  start_angle: int = 240,
                  end_angle: int = -295,
-                 axis_color: str = "grey80",
+                 button_color: str = "grey80",
+                 button_radius: int = 20,
+                 scale_color: str = "grey60",
                  bg: str = None,
                  fg: str = "white",
                  scroll: bool = True,
                  scroll_steps: float = 1,
-                 scale_color: str = "black",
-                 needle_color: str = "grey30",
                  integer: bool = False,
                  state: str = "normal",
+                 progress: bool = True,
                  command=None):
         
         self.bg = bg
         self.fg = fg
-        self.major_div = major_divisions
-        self.min_div = minor_divisions
+        self.major_div = divisions
         self.radius = radius  
         self.border_width = border_width
         self.text = text
         self.start_angle = start_angle 
         self.end_angle = end_angle
         self.start = start
         self.max = end
-        self.axis_color = axis_color
+        self.div_width = division_height
         self.end = self.start_angle + self.end_angle
+        self.border_color = border_color
         self.scale_color = scale_color
-        self.bd_color = border_color
         self.bound = True
         self.integer = integer
-        self.needle_color = needle_color
         self.text_color = text_color
         self.value = self.start  
         self.text_font = text_font
         self.scroll = scroll
         self.scroll_steps = scroll_steps
+        self.bt_radius = button_radius
         self.command = command
+        self.button_color = button_color
         self.state = state
         self.__x = radius/2
         self.__y = radius/2
-        
+        self.progress = progress
+
+        if not self.bg:
+            try:
+                if master.winfo_name()=="!ctkframe":
+                    # get bg_color of customtkinter frames
+                    self.bg = master._apply_appearance_mode(master.cget("fg_color"))
+                else:
+                    self.bg = master.cget("bg")
+            except:  
+                self.bg = "white"
+                
+        if self.end_angle==360:
+            self.end_angle = 358
+            
         if self.start > self.max:
             self.direction = -1
         else:
             self.direction = 1
             
         if width is None:
             self.width = self.radius + self.border_width
@@ -74,28 +89,32 @@
         if height is None:
             self.height = self.radius + self.border_width
         else:
             self.height = height
         
         super().__init__(master, width=self.width, height=self.height, bg=self.bg, borderwidth=0, highlightthickness=0)
         
-        self.create_oval(self.border_width, self.border_width, self.radius, self.radius,
-                         width=self.border_width, fill=self.fg, outline=self.bd_color, tags="face")
-        
         self.create_divisions()
         self.create_needle()
         
         if self.scroll==True:
             super().bind('<MouseWheel>', self.scroll_command)
-        
+            super().bind("<Button-4>", lambda e: self.scroll_command(-1))
+            super().bind("<Button-5>", lambda e: self.scroll_command(1))
+            
     def scroll_command(self, event):
         """
         This function is used to change the value of the dial with mouse scroll
         """
-        if event.delta > 0:        
+        if type(event) is int:
+            event_delta = event
+        else:
+            event_delta = event.delta
+            
+        if event_delta > 0:        
             if self.value < self.max:
                 self.set(self.value+self.scroll_steps)
             elif  self.value==self.max:
                 self.set(self.max)
             else:
                 self.set(self.value-self.scroll_steps)
         else:
@@ -107,71 +126,78 @@
                 self.set(self.value+self.scroll_steps)
                 
     def create_divisions(self):
         """
         This function creates the division lines.
         """
         
-        self.xn = self.yn = (self.radius + self.border_width) / 2
-        self.radians = (self.radius - self.border_width) / 2  
+        self.xn = self.yn = (self.radius) / 2
+        self.radians = (self.radius) / 2
         self.absolute = abs(self.max - self.start)
-        self.arc_pos = self.radians / 3
+        self.arc_pos = (self.radians) / 4
+        
+        # major scale 
 
-        # minor scale
-        if self.min_div != 0:
-            lines = int(self.absolute / self.min_div) + 1
-            angles = (self.start_angle + n * self.end_angle * self.min_div / self.absolute for n in range(lines))
-            for angle in angles:
-                x1 = self.xn + (self.radians - self.arc_pos) * math.cos(math.radians(angle))
-                y1 = self.yn - (self.radians - self.arc_pos) * math.sin(math.radians(angle))
-                x2 = x1 + self.arc_pos / 5 * math.cos(math.radians(angle))
-                y2 = y1 - self.arc_pos / 5 * math.sin(math.radians(angle))
-                self.create_line(x1, y1, x2, y2, fill=self.scale_color, tags='min_scale')
+        lines = int(self.absolute) + 1
+        angles = (self.start_angle + n * self.end_angle / self.absolute for n in range(lines))
 
-        # major scale 
+        for angle in angles:
+            x1 = self.xn + (self.radians - self.arc_pos) * math.cos(math.radians(angle))
+            y1 = self.yn - (self.radians - self.arc_pos) * math.sin(math.radians(angle))
+            x2 = x1 + (self.arc_pos + self.div_width) / 3 * math.cos(math.radians(angle))
+            y2 = y1 - (self.arc_pos + self.div_width)/ 3 * math.sin(math.radians(angle))
+            self.create_line(x1, y1, x2, y2, fill=self.scale_color, width=5, tags='min_scale')
+
+        if self.progress:
+            x5 = self.radius - self.arc_pos + (self.arc_pos + self.div_width)/ 6
+            x6 = self.arc_pos - (self.arc_pos + self.div_width)/ 6
+            
+            self.arc_id = self.create_arc(x6, x6, x5, x5, extent=0, tag="progress",
+                                            start=self.start_angle+self.end_angle, outline=self.scale_color,
+                                            width=(self.arc_pos + self.div_width)/ 3, style='arc')
+        
         lines = int(self.absolute / self.major_div) + int(abs(self.end_angle) != 360)
         angles = (self.start_angle + n * self.end_angle * self.major_div / self.absolute for n in range(lines))
         textvals = (self.start + n * self.major_div * self.direction for n in range(lines))
-        textpos = self.arc_pos / 2.5
-        self.scalefont = tkFont.Font(size=int(self.arc_pos / 5), weight='bold')
+        
         for angle, textval in zip(angles, textvals):
             x1 = self.xn + (self.radians - self.arc_pos) * math.cos(math.radians(angle))
             y1 = self.yn - (self.radians - self.arc_pos) * math.sin(math.radians(angle))
-            x2 = x1 + self.arc_pos / 3 * math.cos(math.radians(angle))
-            y2 = y1 - self.arc_pos / 3 * math.sin(math.radians(angle))
-            self.create_line(x1, y1, x2, y2, width=3, tags='major_scale', fill=self.scale_color)
-            x1 = self.xn + (self.radians - textpos) * math.cos(math.radians(angle))
-            y1 = self.yn - (self.radians - textpos) * math.sin(math.radians(angle))
-            self.create_text(x1, y1, text=textval, font=self.scalefont, fill=self.scale_color, tags='scale_text')
-
+            x2 = x1 + (self.arc_pos + self.div_width)/ 3 * math.cos(math.radians(angle))
+            y2 = y1 - (self.arc_pos + self.div_width)/ 3 * math.sin(math.radians(angle))
+            self.create_line(x1, y1, x2, y2, width=self.border_width, tags='major_scale', fill=self.border_color)
+                        
         # scale arc
-        x1 = y1 = self.arc_pos + self.border_width
-        x2 = y2 = self.radius - self.arc_pos
+        x1 = y1 = self.arc_pos
+        x2 = y2 = self.radius - self.arc_pos 
+        x3 = y3 = self.radius - self.arc_pos + (self.arc_pos + self.div_width)/ 3
+        x4 = y4 = self.arc_pos - (self.arc_pos + self.div_width)/3
+
+        self.create_oval(x1, y1, x2, y2, width=2, tags='arc', outline=self.border_color, fill=self.fg)
+        
         if abs(self.end_angle) != 360:
-            self.create_arc(x1, y1, x2, y2, start=self.start_angle, extent=self.end_angle, width=2,
-                            outline=self.scale_color, style='arc', tags='arc')
+            self.create_arc(x3, y3, x4, y4, start=self.start_angle, extent=self.end_angle, width=self.border_width-1,
+                            outline=self.border_color, style='arc', tags='arc')
         else:
-            self.create_oval(x1, y1, x2, y2, width=2, tags='arc')
+            self.create_oval(x3, y3, x4, y4, width=self.border_width-1, tags='arc', outline=self.border_color)
             
     def create_needle(self):
         """
         This function creates the needle and axis that can rotate.
         """
         x1 = self.xn
         y1 = self.yn + self.arc_pos * 4 / 3
+        if self.text:
+            self.create_text(x1, y1, font=self.text_font, tags='text')
+
+        x1 = y1 = self.arc_pos+(self.arc_pos/2)
+        x2 = y2 = self.arc_pos*2.5
+        
+        self.knob = self.create_oval(x1,y1,x2,y2, width=self.border_width-1, tags='needle', fill=self.button_color, outline=self.border_color)
         
-        self.create_text(x1, y1, font=self.text_font, tags='text')
-        self.axis_rad = self.radius / 25
-        xy1 = (self.xn + 2.5 * self.arc_pos, self.yn)
-        xy2 = (self.xn, self.yn + 0.75 * self.axis_rad)
-        xy3 = (self.xn, self.yn - 0.75 * self.axis_rad)
-        self.needle_coords = [xy1, xy2, xy3]
-        self.needle = self.create_polygon(self.needle_coords, tags='needle', fill=self.needle_color)    
-        self.create_oval(self.xn - self.axis_rad, self.yn - self.axis_rad, self.xn + self.axis_rad, self.yn + self.axis_rad,
-                         outline=self.bd_color, fill=self.axis_color, tags='axis')
         self.needle_state()
         self.set(self.value)
         
     def needle_state(self):
         """
         This function binds/unbinds the mouse button with the needle
         """
@@ -203,75 +229,100 @@
             
         self.previous_angle = 0
         
     def rotate_needle(self, event):
         
         angle = math.degrees(math.atan2(self.__y - event.y, event.x - self.__x))
         if self.previous_angle>angle:
-            self.set(self.value+self.scroll_steps)
+            if self.max>self.start and self.start_angle>self.end_angle:
+                self.set(self.value+self.scroll_steps)
+            elif self.max<self.start and self.start_angle<self.end_angle:
+                self.set(self.value+self.scroll_steps)
+            else:
+                self.set(self.value-self.scroll_steps)
         else:
-            self.set(self.value-self.scroll_steps)
-        self.previous_angle=angle
+            if self.max>self.start and self.start_angle>self.end_angle:
+                self.set(self.value-self.scroll_steps)
+            elif self.max<self.start and self.start_angle<self.end_angle:
+                self.set(self.value-self.scroll_steps)
+            else:
+               self.set(self.value+self.scroll_steps)
+                
+        self.previous_angle = angle         
+
+
+    def line_coordinates(self, r1: float, r2: float, angle: float) -> tuple:
         
+        return (
+            self.xn + r2 * math.cos(math.radians(angle)) -self.bt_radius,
+            self.yn - r2 * math.sin(math.radians(angle)) -self.bt_radius,
+            self.xn + r2 * math.cos(math.radians(angle)) +self.bt_radius,
+            self.yn - r2 * math.sin(math.radians(angle)) +self.bt_radius
+        )
+    
     def set(self, value):
         """
         This function is used to set the position of the needle
         """
         
         self.value = value
         angle = (value - self.start) * (self.end - self.start_angle) / (self.max - self.start) + self.start_angle
 
         if self.start < self.max:  
             if value < self.start:
-                angle = self.start_angle
                 self.value = self.start
                 value = self.start
             elif value > self.max:
-                angle = self.end
                 self.value = self.max
                 value = self.max
         else:
             if value > self.start:
-                angle = self.start_angle
                 self.value = self.start
                 value = self.start
             elif value < self.max:
-                angle = self.end
                 self.value = self.max
                 value = self.max
-                
-        xy_pos = []
-        offset = complex(self.xn, self.yn)
-        for x, y in self.needle_coords:
-            exp = cmath.exp(math.radians(-angle) * 1j) * (complex(x, y) - offset) + offset
-            xy_pos.append(exp.real)
-            xy_pos.append(exp.imag)
-        self.coords(self.needle, *xy_pos)
 
+        if self.progress:
+            extend_angle = angle-(self.start_angle+self.end_angle)
+            self.itemconfigure(self.arc_id, extent=extend_angle)
+            
+        self.coords(
+            self.knob,
+            self.line_coordinates(
+                r1=0,
+                r2= self.radius/2 - self.arc_pos - self.bt_radius,
+                angle=angle
+            )
+        )
+        
         if self.integer==False:
             value = round(value, 2)
         else:
             value = int(value)
-        self.itemconfig(tagOrId='text', text=str(value)+self.text, fill=self.text_color)
+            
+        if self.text:
+            self.itemconfig(tagOrId='text', text=self.text+str(value), fill=self.text_color)
         
         if self.previous_angle!=0:
             if self.command is not None:
                 self.command()
-            
+        
     def get(self):
         """
         This function returns the current value of the meter
         :return: float
         """
         return self.value
     
     def set_mark(self, from_, to, color="red"):
+        if from_==0: from_=1
         colored_lines = self.find_withtag('min_scale')[from_:to]
         for line in colored_lines:
-            self.itemconfig(line, fill=color, width=6)
+            self.itemconfig(line, fill=color, width=10)
             
     def configure(self, **kwargs):
         """
         This function contains some configurable options
         """
         
         if "text" in kwargs:
@@ -294,53 +345,49 @@
         if "height" in kwargs:
             super().configure(height=kwargs.pop("height"))
             
         if "scale_color" in kwargs:
             self.itemconfigure(tagOrId="min_scale",
                     fill=kwargs['scale_color'])
             self.itemconfigure(
-                tagOrId="major_scale",
-                fill=kwargs['scale_color'])
-            self.itemconfigure(
-                tagOrId="arc",
-                outline=kwargs.pop('scale_color'))
+                tagOrId="progress",
+                outline=kwargs.pop("scale_color"))
             
         if "fg" in kwargs:
             self.itemconfigure(
                 tagOrId="face",
                 fill=kwargs.pop('fg'))
             
         if "text_color" in kwargs:
             self.itemconfigure(
                 tagOrId="text",
                 fill=kwargs.pop("text_color"))
             
-        if "needle_color" in kwargs:
+        if "button_color" in kwargs:
             self.itemconfigure(
                 tagOrId="needle",
-                fill=kwargs.pop("needle_color"))
+                fill=kwargs.pop("button_color"))
             
         if "border_color" in kwargs:
             self.itemconfigure(
                 tagOrId="face",
                 outline=kwargs.pop("border_color"))
             
-        if "axis_color" in kwargs:
-            self.itemconfigure(
-                tagOrId="axis",
-                fill=kwargs.pop("axis_color"))
-            
         if "scroll_steps" in kwargs:
             self.scroll_steps = kwargs.pop("scroll_steps")
             
         if "scroll" in kwargs:
             if kwargs["scroll"]==False:
                 super().unbind('<MouseWheel>')
+                super().unbind('<Button-4>')
+                super().unbind('<Button-5>')
             else:
                 super().bind('<MouseWheel>', self.scroll_command)
+                super().bind("<Button-4>", lambda e: self.scroll_command(-1))
+                super().bind("<Button-5>", lambda e: self.scroll_command(1))
             kwargs.pop("scroll")
             
         if "integer" in kwargs:
             self.set(self.value)
             self.integer = kwargs.pop("integer")
             
         if "state" in kwargs:
```

### Comparing `tkdial-0.0.4/tkdial/scrollknob.py` & `tkdial-0.0.5/tkdial/scrollknob.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  text_font: str = None,
                  progress_color: str = "grey60",
                  inner_color: str = "grey80",
                  outer_color: str = "grey80",
                  inner_width: int = 10,
                  outer_width: int = 10,
                  outer_length: int = 0,
-                 bg: str = "#f0f0f0",
+                 bg: str = None,
                  fg: str = "#f0f0f0",
                  bar_color: str = "#f0f0f0",
                  integer: bool = False,
                  steps: int = 5,
                  state: str = "normal",
                  command = None
                  ):
@@ -60,57 +60,83 @@
         self.outer = outer_width
         self.incolor = inner_color
         self.outcolor = outer_color
         self.text = text
         self.text_color = text_color
         self.text_font = text_font
         self.start_ang, self.full_extent = start_angle, 360
-        self.steps = (steps/self.start-self.end)*360
+        self.steps = (steps/abs(self.start-self.end))*360
         self.progress_color = progress_color
         self.delta = 0
         w2 = self.width / 2
         self.value = self.start
         self.state = state
         self.integer = integer
         self.command = command
         
+        if not self.bg:
+            try:
+                if master.winfo_name()=="!ctkframe":
+                    # get bg_color of customtkinter frames
+                    self.bg = master._apply_appearance_mode(master.cget("fg_color"))
+                else:
+                    self.bg = master.cget("bg")
+            except:  
+                self.bg = "white"
+                
         super().__init__(self.__master, bg=self.bg, width=width, height=height, bd=0, highlightthickness=0)
         
         if self.inner > self.x0:
             self.inner = self.x0
         if self.outer > self.y0:
             self.outer = self.y0
         if text=="":
-            self.disable_text = True          
-        if self.steps > (self.start-self.end):
-            self.steps = self.start - self.end
-            
+            self.disable_text = True
+
+        if self.steps<0:
+            self.steps = - self.steps
+
+        if self.steps > abs(self.start-self.end):
+            if self.start>self.end:
+                self.steps = self.start - self.end
+            else:
+                self.steps = self.end - self.start
+                
         self.arc_back = self.create_arc(self.x0, self.y0, self.x1, self.y1, extent=359,
                                              start=self.start_ang, outline=self.bar_color,
                                              width=self.width, style='arc')
         
         self.arc_id = self.create_arc(self.x0, self.y0, self.x1, self.y1, extent=0,
                                         start=self.start_ang, outline=self.progress_color,
                                         width=self.width, style='arc')
         
-        self.oval_id1 = self.create_oval(self.x0-w2-self.outer_length, self.y0-w2-self.outer_length, self.x1+w2+self.outer_length, self.y1+w2+self.outer_length, outline=self.outcolor,width=self.outer)
+        self.oval_id1 = self.create_oval(self.x0-w2-self.outer_length, self.y0-w2-self.outer_length, self.x1+w2+self.outer_length,
+                                         self.y1+w2+self.outer_length, outline=self.outcolor,width=self.outer)
         
         self.oval_id2 = self.create_oval(self.x0+w2, self.y0+w2, self.x1-w2, self.y1-w2, width=self.inner, outline=self.incolor, fill=self.fg)
-        
-        self.label_id = self.create_text(self.tx, self.ty, fill=self.text_color, font=self.text_font)        
+     
+        if self.text:
+            self.label_id = self.create_text(self.tx, self.ty, fill=self.text_color, font=self.text_font)        
         self.set_text()
         
         if state=="normal":
             self.bind('<MouseWheel>', self.scroll_command)
-        
+            self.bind("<Button-4>", lambda e: self.scroll_command(-1))
+            self.bind("<Button-5>", lambda e: self.scroll_command(1))
+            
     def scroll_command(self, event):
         """
         This function is used to change the value of the knob with mouse scroll
         """
-        if event.delta > 0:
+        if type(event) is int:
+            event_delta = event
+        else:
+            event_delta = event.delta
+       
+        if event_delta > 0:
             if self.delta>=(360-self.steps):
                 self.itemconfigure(self.arc_id, extent=359)
                 self.delta=360
             else:
                 self.delta+=self.steps
                 self.itemconfigure(self.arc_id, extent=self.delta)
         else:
@@ -126,14 +152,16 @@
         if self.command is not None:
             self.command()
             
     def set_text(self):
         """
         This function is to set text for the knob
         """
+        if not self.text:
+            return
         if self.disable_text==False:
             if self.integer==True:
                 self.value = int(round((self.end - self.start) / 360 * (360 - self.delta) + self.start, 2))
             else:
                 self.value = round((self.end - self.start) / 360 * (360 - self.delta) + self.start, 2)
             self.itemconfigure(self.label_id, text=str(self.value) + self.text)
         else:
@@ -153,30 +181,35 @@
         
         if value<self.end:
             value = self.end
             
         if value>=self.start:
             value = self.start
 
-        self.delta = 360-(360/(self.end - self.start))*(value - self.start)
+        self.delta = 360-(360/abs(self.end - self.start))*(value - self.start)
         self.itemconfigure(self.arc_id, extent=self.delta)
         self.set_text()
         
         if self.command is not None:
             self.command()
             
     def configure(self, **kwargs):
         """
         This function contains some configurable options
         """
         if "state" in kwargs:
-            if kwargs["scroll"]!="normal":
+            if kwargs["state"]!="normal":
                 super().unbind('<MouseWheel>')
+                super().unbind('<Button-4>')
+                super().unbind('<Button-5>')
             else:
                 super().bind('<MouseWheel>', self.scroll_command)
+                super().bind("<Button-4>", lambda e: self.scroll_command(-1))
+                super().bind("<Button-5>", lambda e: self.scroll_command(1))
+            kwargs.pop("state")
             
         if "text" in kwargs:
              self.itemconfigure(self.label_id,
                 text=kwargs.pop("text"))
              
         if "start" in kwargs:
             self.end = kwargs.pop("start")
```

### Comparing `tkdial-0.0.4/tkdial/tkdial.py` & `tkdial-0.0.5/tkdial/tkdial.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             width: int = None,
             height: int = None,
             x: int = None,
             y: int = None,
             unit_length: float = 10,
             unit_width: float = 5,
             radius: float = 50.0,
-            bg: str = "#f0f0f0",
+            bg: str = None,
             text: str = "Value: ",
             unit_color: str = "grey",
             text_color: str = "black",
             text_font: str = None,
             needle_color: str = "grey",
             color_gradient: tuple = None,
             integer: bool = False,
@@ -127,38 +127,66 @@
             ("red", "red"):(255, 0, 0, True),
             ("green", "green"): (0, 255, 0, False),
             ("blue", "blue"): (0, 0, 255, False),
             ("cyan", "cyan"):(0, 255, 255, True),
             ("pink", "pink"): (255, 0, 255, False),
             ("yellow", "yellow"): (255, 255, 0, False)
         }
-        
+        if not self.__bg:
+            try:
+                if master.winfo_name()=="!ctkframe":
+                    # get bg_color of customtkinter frames
+                    self.__bg = master._apply_appearance_mode(master.cget("fg_color"))
+                else:
+                    self.__bg = master.cget("bg")
+            except:  
+                self.__bg = "white"
+                
         super().__init__(self.__master, bg=self.__bg, width=self.__width, height=self.__height, bd=0, highlightthickness=0)
         self.__palette = self.__create_palette()
         self.__create_needle()
         self.__create_units()
-        self.__create_text()
+        if self.__text_title:
+            self.__create_text()
         
         if scroll==True:
             super().bind('<MouseWheel>', self.scroll_command)
-        
+            super().bind("<Button-4>", lambda e: self.scroll_command(-1))
+            super().bind("<Button-5>", lambda e: self.scroll_command(1))
+            
     def scroll_command(self, event):
         """
         This function is used to change the value of the dial with mouse scroll
         """
-        if event.delta > 0:        
-            if self.value < self.__end:
-                self.set(self.value+self.__scroll_steps)
-        else:
-            if self.value > self.__start:
-                self.set(self.value-self.__scroll_steps)
-            elif  self.value==self.__start:
-                self.set(self.__start+0.1)
-                self.set(self.__start)
-                
+        if type(event) is int:
+            event_delta = event
+        else:
+            event_delta = event.delta
+            
+        if event_delta > 0:
+            if self.__end>self.__start:
+                if self.value < self.__end:
+                    self.set(self.value+self.__scroll_steps)
+            else:
+                if self.value > self.__end:
+                    self.set(self.value-self.__scroll_steps)
+        else:
+            if self.__end>self.__start:
+                if self.value > self.__start:
+                    self.set(self.value-self.__scroll_steps)
+                elif self.value==self.__start:
+                    self.set(self.__start+0.1)
+                    self.set(self.__start)
+            else:
+                if self.value > self.__end:
+                    self.set(self.value+self.__scroll_steps)
+                elif self.value==self.__end:
+                    self.set(self.__start+0.1)
+                    self.set(self.__start)
+
     def __line_coordinates(self, r1: float, r2: float, angle: float) -> tuple:
         """
         This function is used for placing the lines around a circle.
         :return: A tuple that contains 4 coordinates
         """
         return (
             self.__x + r1 * cos(radians(angle)),
@@ -352,24 +380,25 @@
         self.__colorize(angle=angle, start=int(angle), end=360)
         self.__colorize(
             angle=angle,
             start=0,
             end=int(angle),
             color=self.__unit_color
         )
-        if self.__integer==False:
-            self.itemconfigure(
-                tagOrId="value",
-                text=f"{self.__text_title}{self.value}"
-            )
-        else:
-            self.itemconfigure(
-                tagOrId="value",
-                text=f"{self.__text_title}{int(self.value)}"
-            )
+        if self.__text_title:
+            if self.__integer==False:
+                self.itemconfigure(
+                    tagOrId="value",
+                    text=f"{self.__text_title}{self.value}"
+                )
+            else:
+                self.itemconfigure(
+                    tagOrId="value",
+                    text=f"{self.__text_title}{int(self.value)}"
+                )
         if self.__command is not None:
             self.__command()
             
     def __create_text(self) -> None:
         """
         A function that creates a text object to show what
         the value of the position of needle is.
@@ -389,21 +418,29 @@
         """
         return self.value
     
     def set(self, value):
         """
         This function is used to set the position of the needle
         """
-        if value<self.__start:
-            value = self.__start
-            
-        if value>=self.__end:
-            value = self.__end
-            self.__rotate_needle(self, angle=-350)
-            
+        if self.__start<self.__end:
+            if value<self.__start:
+                value = self.__start
+                
+            if value>=self.__end:
+                value = self.__end
+                self.__rotate_needle(self, angle=-350)
+        else:
+            if value>self.__start:
+                value = self.__start
+                
+            if value<=self.__end:
+                value = self.__end
+                self.__rotate_needle(self, angle=-350)
+                
         angle = float(-(360/(self.__end - self.__start))*(value - self.__start))
         self.__rotate_needle(self, angle=angle)
 
     def configure(self, **kwargs):
         """
         This function contains some configurable options
         """
@@ -454,16 +491,20 @@
             
         if "scroll_steps" in kwargs:
             self.__scroll_steps = kwargs.pop("scroll_steps")
             
         if "scroll" in kwargs:
             if kwargs["scroll"]==False:
                 super().unbind('<MouseWheel>')
+                super().unbind('<Button-4>')
+                super().unbind('<Button-5>')
             else:
                 super().bind('<MouseWheel>', self.scroll_command)
+                super().bind("<Button-4>", lambda e: self.scroll_command(-1))
+                super().bind("<Button-5>", lambda e: self.scroll_command(1))
             kwargs.pop("scroll")
             
         if "integer" in kwargs:
             self.set(self.value)
             self.__integer = kwargs.pop("integer")
             
         if len(kwargs)>0:
```

### Comparing `tkdial-0.0.4/tkdial.egg-info/PKG-INFO` & `tkdial-0.0.5/tkdial.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkdial
-Version: 0.0.4
+Version: 0.0.5
 Summary: Rotatory dial-knob widgets for Tkinter.
 Home-page: https://github.com/Akascape/TkDial
 Author: Akascape
 License: Creative Commons Zero v1.0 Universal
 Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -82,31 +82,31 @@
                 
 app.grid_columnconfigure((0,1), weight=1)
 app.grid_rowconfigure((0,1), weight=1)
 
 frame_1 = customtkinter.CTkFrame(master=app)
 frame_1.grid(padx=20, pady=20, sticky="nswe")
 
-dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"), bg="#2a2d2e",
+dial1 = Dial(master=frame_1, color_gradient=("green", "cyan"),
              text_color="white", text="Current: ", unit_length=10, radius=50)
 dial1.grid(padx=20, pady=20)
 
-dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"), bg="#2a2d2e",
+dial2 = Dial(master=frame_1, color_gradient=("yellow", "white"),
              text_color="white", text="Position: ", unit_length=10, radius=50)
 dial2.grid(padx=20, pady=20)
 
-dial3 = Dial(master=frame_1, color_gradient=("white", "pink"), bg="#2a2d2e",
+dial3 = Dial(master=frame_1, color_gradient=("white", "pink"),
              text_color="white", text=" ", unit_length=10, radius=50)
 dial3.grid(row=0, column=1, padx=20, pady=20)
 
-dial4 = Dial(master=frame_1, color_gradient=("green", "green"), bg="#2a2d2e",
+dial4 = Dial(master=frame_1, color_gradient=("green", "green"),
              text_color="white", text="", unit_width=15, radius=50)
 dial4.grid(row=1, column=1, padx=20, pady=20)
 
-app.mainloop()                  
+app.mainloop()                
 ```
 ![Screenshot 3](https://user-images.githubusercontent.com/89206401/202906638-a1c863b7-54b0-4e7a-9619-415e28b3ab51.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -161,37 +161,37 @@
 ```python
 import customtkinter
 from tkdial import ScrollKnob
 
 app = customtkinter.CTk()
 app.geometry("500x500")
 
-knob1 = ScrollKnob(app, bg="#212325", radius=250, progress_color="#87ceeb", steps=10,
+knob1 = ScrollKnob(app, radius=250, progress_color="#87ceeb", steps=10,
                  border_width=40, start_angle=90, inner_width=1, outer_width=1,
                  text_font="calibri 20", text_color="#87ceeb", bar_color="black")
 knob1.grid(row=0, column=0)
 
-knob2 = ScrollKnob(app, bg="#212325", radius=200, progress_color="#7eff00",
+knob2 = ScrollKnob(app, radius=200, progress_color="#7eff00",
                  border_width=40, start_angle=90, inner_width=1, outer_width=0,
                  text_font="calibri 20", text_color="#7eff00", integer=True,
                  fg="#212325")
 knob2.grid(row=1, column=0)
 
-knob3 = ScrollKnob(app, bg="#212325", text=" ", radius=250, progress_color="white",
+knob3 = ScrollKnob(app, text=" ", radius=250, progress_color="white",
                    bar_color="#2937a6", border_width=30, start_angle=0, inner_width=5,
                    outer_width=0, text_font="calibri 20", steps=1, text_color="white", fg="#303ba1")
 knob3.grid(row=0, column=1)
 
-knob4 = ScrollKnob(app, bg="#212325", text=" ", steps=10, radius=200, bar_color="#212325", 
+knob4 = ScrollKnob(app, text=" ", steps=10, radius=200, bar_color="#242424", 
                    progress_color="yellow", outer_color="yellow", outer_length=10, 
                    border_width=30, start_angle=270, inner_width=0, outer_width=5, text_font="calibri 20", 
                    text_color="white", fg="#212325")
 knob4.grid(row=1, column=1)
                 
-app.mainloop()      
+app.mainloop() 
 ```
 ![Complex example](https://user-images.githubusercontent.com/89206401/204139428-c3c3c313-539f-4867-9d50-8876a19432ee.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -246,40 +246,38 @@
 ```python
 import customtkinter
 from tkdial import Meter
 
 app = customtkinter.CTk()
 app.geometry("950x350")
 
-meter1 = Meter(app, bg="#212325", radius=300, start=0, end=160, border_width=0,
+meter1 = Meter(app, radius=300, start=0, end=160, border_width=0,
                fg="black", text_color="white", start_angle=270, end_angle=-270,
                text_font="DS-Digital 30", scale_color="white", needle_color="red")
 meter1.set_mark(140, 160) # set red marking from 140 to 160
 meter1.grid(row=0, column=1, padx=20, pady=30)
 
-meter2 = Meter(app, bg="#212325", radius=260, start=0, end=200, border_width=5,
+meter2 = Meter(app, radius=260, start=0, end=200, border_width=5,
                fg="black", text_color="white", start_angle=270, end_angle=-360,
                text_font="DS-Digital 30", scale_color="black", axis_color="white",
                needle_color="white")
 meter2.set_mark(1, 100, "#92d050")
 meter2.set_mark(105, 150, "yellow")
 meter2.set_mark(155, 196, "red")
 meter2.set(80) # set value
 meter2.grid(row=0, column=0, padx=20, pady=30)
 
-meter3 = Meter(app, bg="#212325", fg="#212325", radius=300, start=0, end=50,
+meter3 = Meter(app, fg="#242424", radius=300, start=0, end=50,
                major_divisions=10, border_width=0, text_color="white",
                start_angle=0, end_angle=-360, scale_color="white", axis_color="cyan",
                needle_color="white",  scroll_steps=0.2)
 meter3.set(15)
 meter3.grid(row=0, column=2, pady=30)
 
 app.mainloop()
-                    
-# Font used: https://www.dafont.com/ds-digital.font
 ```
 ![styles_meter](https://user-images.githubusercontent.com/89206401/204718389-d3195b3b-0f7a-41c3-85b8-ffc1d961db70.png)
 
 ## Arguments:
   | Parameters  | Description |
   | -------- | ----------- |
   | _master_ | The master parameter is the parent widget |
@@ -309,14 +307,94 @@
   | _command_ | Call a function whenever the needle is rotated |
   
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the meter |
   | _.set()_ | set the value of the meter |
+  | _.configure()_ | configure parameters of the meter| 
+  | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
+  
+# JogWheel
+
+## Usage
+
+```python
+import tkinter
+from tkdial import Jogwheel
+
+app = tkinter.Tk()
+
+knob = Jogwheel(app)
+knob.grid()
+
+app.mainloop()
+```
+![Jogwheel](https://user-images.githubusercontent.com/89206401/232750598-37f4f863-0aba-48c8-9a69-4cb1e15e1457.png)
+
+### Styles: 
+```python
+import customtkinter
+from tkdial import Jogwheel
+
+app = customtkinter.CTk()
+
+wheel_1 = Jogwheel(app, radius=200, fg="#045252", scale_color="white",
+                text=None, button_radius=10)
+wheel_1.set_mark(0,100, "green")
+
+wheel_1.grid()
+
+wheel_2 = Jogwheel(app, radius=200, fg="#045252", scale_color="white", start_angle=0,
+                   end_angle=360, start=0, end=200, text="Volume: ", button_radius=10)
+wheel_2.set_mark(0,50, "blue")
+wheel_2.set_mark(50, 90, "green")
+wheel_2.set_mark(90, 150, "orange")
+wheel_2.set_mark(150, 200, "red")
+wheel_2.grid()
+
+app.mainloop()
+```
+![Jogwheel styles](https://user-images.githubusercontent.com/89206401/232751129-72d29a4e-d0ea-49b4-9051-e65cabd5fb55.png)
+
+
+## Arguments:
+  | Parameters  | Description |
+  | -------- | ----------- |
+  | _master_ | The master parameter is the parent widget |
+  | _bg_  | The default background color of the meter widget |
+  | _fg_ | Specify the color of the wheel face |
+  | _width_ | Define width of the widget manually (optional) |
+  | _height_ | Define height of the widget manually (optional) |
+  | _start_ |  The start point of the range from where the knob will rotate |
+  | _end_ |  The end point of the range |
+  | _start_angle_ | Determines the starting angle of the arc |
+  | _end_angle_ | Determines the final angle of the arc |
+  | _radius_ | Determines the radius for the widget |
+  | _divisions_ | Determines the number of scale lines in the scale |
+  | _division_height_ | Determines the height of scale lines |
+  | _scale_color_ |  Specify the color of the knob scale |
+  | _border_width_ | Define the width of the border case (default=1) |
+  | _border_color_ |  Specify the color of the border case |
+  | _button_color_ | Specify the color of the knob |
+  | _button_radius_ | Specify the radius the knob |
+  | _text_ | A string that will be displayed |
+  | _text_color_ | Specify the color of the text that will be displayed |
+  | _text_font_ | Specify the font of the text that will be displayed |
+  | _integer_ | A boolean (True/False), displays only the integer value in text if True (default=False) |
+  | _scroll_ | A boolean (True/False), enables mouse scroll (default=True) |
+  | _scroll_steps_ | Number of steps per scroll |
+  | _state_ | Unbind/Bind the mouse movement with the widget |
+  | _command_ | Call a function whenever the needle is rotated |
+  
+### Methods:
+  | Methods   | Description |
+  |-----------|-------------|
+  | _.get()_ | get the current value of the meter |
+  | _.set()_ | set the value of the meter |
   | _.configure()_ | configure parameters of the meter| 
   | _.set_mark()_ | set markings for the scale. Eg: **meter.set_mark(from, to, color)** | 
   
 ## Conclusion
 This library is focused to create some circular widgets that can be used with Tkinter easily.
 I hope it will be helpful for UI development in python.
```

