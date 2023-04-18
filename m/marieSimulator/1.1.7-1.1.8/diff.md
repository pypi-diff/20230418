# Comparing `tmp/marieSimulator-1.1.7.tar.gz` & `tmp/marieSimulator-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marieSimulator-1.1.7.tar", last modified: Sat Apr  8 02:13:18 2023, max compression
+gzip compressed data, was "marieSimulator-1.1.8.tar", last modified: Tue Apr 18 04:07:12 2023, max compression
```

## Comparing `marieSimulator-1.1.7.tar` & `marieSimulator-1.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-08 02:13:18.724865 marieSimulator-1.1.7/
--rw-r--r--   0 aaryandehade   (501) staff       (20)     1070 2023-03-31 14:38:41.000000 marieSimulator-1.1.7/LICENSE
--rw-r--r--   0 aaryandehade   (501) staff       (20)     1448 2023-04-08 02:13:18.724650 marieSimulator-1.1.7/PKG-INFO
--rw-r--r--   0 aaryandehade   (501) staff       (20)      886 2023-04-08 01:56:36.000000 marieSimulator-1.1.7/README.md
--rw-r--r--   0 aaryandehade   (501) staff       (20)      103 2023-03-31 14:33:58.000000 marieSimulator-1.1.7/pyproject.toml
--rw-r--r--   0 aaryandehade   (501) staff       (20)       38 2023-04-08 02:13:18.724938 marieSimulator-1.1.7/setup.cfg
--rw-r--r--   0 aaryandehade   (501) staff       (20)      861 2023-04-08 02:10:11.000000 marieSimulator-1.1.7/setup.py
-drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-08 02:13:18.720858 marieSimulator-1.1.7/src/
-drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-08 02:13:18.723430 marieSimulator-1.1.7/src/marieSimulator/
--rw-r--r--   0 aaryandehade   (501) staff       (20)     4023 2023-04-08 02:03:37.000000 marieSimulator-1.1.7/src/marieSimulator/Marie.py
--rw-r--r--   0 aaryandehade   (501) staff       (20)    10096 2023-04-08 02:06:14.000000 marieSimulator-1.1.7/src/marieSimulator/MarieGUI.py
--rw-r--r--   0 aaryandehade   (501) staff       (20)     2596 2023-04-07 21:40:43.000000 marieSimulator-1.1.7/src/marieSimulator/MarieReader.py
--rw-r--r--   0 aaryandehade   (501) staff       (20)       97 2023-04-08 02:09:46.000000 marieSimulator-1.1.7/src/marieSimulator/__init__.py
-drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-08 02:13:18.724342 marieSimulator-1.1.7/src/marieSimulator.egg-info/
--rw-r--r--   0 aaryandehade   (501) staff       (20)     1448 2023-04-08 02:13:18.000000 marieSimulator-1.1.7/src/marieSimulator.egg-info/PKG-INFO
--rw-r--r--   0 aaryandehade   (501) staff       (20)      333 2023-04-08 02:13:18.000000 marieSimulator-1.1.7/src/marieSimulator.egg-info/SOURCES.txt
--rw-r--r--   0 aaryandehade   (501) staff       (20)        1 2023-04-08 02:13:18.000000 marieSimulator-1.1.7/src/marieSimulator.egg-info/dependency_links.txt
--rw-r--r--   0 aaryandehade   (501) staff       (20)       15 2023-04-08 02:13:18.000000 marieSimulator-1.1.7/src/marieSimulator.egg-info/top_level.txt
+drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-18 04:07:12.162392 marieSimulator-1.1.8/
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     1070 2023-03-31 14:38:41.000000 marieSimulator-1.1.8/LICENSE
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     1659 2023-04-18 04:07:12.162158 marieSimulator-1.1.8/PKG-INFO
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     1096 2023-04-08 06:34:41.000000 marieSimulator-1.1.8/README.md
+-rw-r--r--   0 aaryandehade   (501) staff       (20)      103 2023-03-31 14:33:58.000000 marieSimulator-1.1.8/pyproject.toml
+-rw-r--r--   0 aaryandehade   (501) staff       (20)       38 2023-04-18 04:07:12.162468 marieSimulator-1.1.8/setup.cfg
+-rw-r--r--   0 aaryandehade   (501) staff       (20)      861 2023-04-18 04:06:43.000000 marieSimulator-1.1.8/setup.py
+drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-18 04:07:12.158237 marieSimulator-1.1.8/src/
+drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-18 04:07:12.160691 marieSimulator-1.1.8/src/marieSimulator/
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     4688 2023-04-18 02:51:10.000000 marieSimulator-1.1.8/src/marieSimulator/Marie.py
+-rw-r--r--   0 aaryandehade   (501) staff       (20)    11134 2023-04-18 04:06:20.000000 marieSimulator-1.1.8/src/marieSimulator/MarieGUI.py
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     2821 2023-04-18 01:32:16.000000 marieSimulator-1.1.8/src/marieSimulator/MarieReader.py
+-rw-r--r--   0 aaryandehade   (501) staff       (20)       97 2023-04-08 02:09:46.000000 marieSimulator-1.1.8/src/marieSimulator/__init__.py
+drwxr-xr-x   0 aaryandehade   (501) staff       (20)        0 2023-04-18 04:07:12.161814 marieSimulator-1.1.8/src/marieSimulator.egg-info/
+-rw-r--r--   0 aaryandehade   (501) staff       (20)     1659 2023-04-18 04:07:12.000000 marieSimulator-1.1.8/src/marieSimulator.egg-info/PKG-INFO
+-rw-r--r--   0 aaryandehade   (501) staff       (20)      333 2023-04-18 04:07:12.000000 marieSimulator-1.1.8/src/marieSimulator.egg-info/SOURCES.txt
+-rw-r--r--   0 aaryandehade   (501) staff       (20)        1 2023-04-18 04:07:12.000000 marieSimulator-1.1.8/src/marieSimulator.egg-info/dependency_links.txt
+-rw-r--r--   0 aaryandehade   (501) staff       (20)       15 2023-04-18 04:07:12.000000 marieSimulator-1.1.8/src/marieSimulator.egg-info/top_level.txt
```

### Comparing `marieSimulator-1.1.7/LICENSE` & `marieSimulator-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `marieSimulator-1.1.7/PKG-INFO` & `marieSimulator-1.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marieSimulator
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python Package to simulate a MARIE architecture on any computer
 Home-page: https://github.com/dehadeaaryan/MarieSimulator
 Author: Aaryan Dehade
 Author-email: dehadeaaryan@gmail.com
 Project-URL: Bug Tracker, https://github.com/dehadeaaryan/MarieSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -68,7 +68,12 @@
 10. Clear
 11. AddI X
 12. JumpI X
 13. LoadI X
 14. StoreI X
 15. JnS X
 16. HEX X
+
+---
+
+Download the GUI application [here](https://www.aaryandehade.live/Marie%20Simulator.dmg)
+Or copy: [https://www.aaryandehade.live/Marie%20Simulator.dmg](https://www.aaryandehade.live/Marie%20Simulator.dmg)
```

### Comparing `marieSimulator-1.1.7/setup.py` & `marieSimulator-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="marieSimulator",
-    version="1.1.7",
+    version="1.1.8",
     author="Aaryan Dehade",
     author_email="dehadeaaryan@gmail.com",
     description="A Python Package to simulate a MARIE architecture on any computer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dehadeaaryan/MarieSimulator",
     project_urls={
```

### Comparing `marieSimulator-1.1.7/src/marieSimulator/Marie.py` & `marieSimulator-1.1.8/src/marieSimulator/Marie.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,163 +6,185 @@
         self.MBR = 0x0000
         self.IR = 0x0000
         self.InReg = 0x00
         self.OutReg = 0x00
 
         self.GUI = False
 
-        self.M = []
+        self.M = [0 for i in range(4096)]
 
         self.operation = None
         self.running = True
+        self.canStep = True
 
         if mr != None:
             self.parse(mr)
     
     def parse(self, mr):
         self.M = mr.M
+        self.M += [0] * (16**3 - len(mr.M))
         self.symbolTable = mr.symbolTable
 
     def show(self):
         output = "\n"
 
         for item in self.M:
             output += hex(item) + " | "
         output = output[:-3] + "\n"
 
         print(output)
     
     def run(self):
         while self.running:
-            self.fetch()
-            self.next()
-            self.decode()
-            self.getOperand()
-            self.execute()
+            self.__fetch()
+            self.__incrementPC()
+            self.__decode()
+            self.__getOperand()
+            self.__execute()
+    
+    def step(self):
+        if self.canStep:
+            previousM = self.M.copy()
+            self.__fetch()
+            self.__incrementPC()
+            self.__decode()
+            self.__getOperand()
+            self.__execute()
+        
+            output = []
+
+            for i in range(len(self.M)):
+                if self.M[i] != previousM[i]:
+                    output.append(i)
+            
+            return output
+        else:
+            return None
+
+
 
-    def fetch(self):
+    def __fetch(self):
         self.MAR = self.PC
         self.MBR = self.M[self.MAR]
         self.IR = self.MBR
     
-    def next(self):
+    def __incrementPC(self):
         self.PC += 1
     
-    def decode(self):
+    def __decode(self):
         self.MAR = (self.IR & 0x0FFF)
         self.operation = (self.IR & 0xF000) >> 12
 
-    def getOperand(self):
+    def __getOperand(self):
         if self.operation not in [0x5, 0x6, 0x7, 0x8, 0xA, 0xB, 0xC, 0xD, 0xE, 0xF]:
             self.MBR = self.M[self.MAR]
 
-    def execute(self):
+    def __execute(self):
         if self.operation == 0x0:
-            pass
+            self.__jnS()
         elif self.operation == 0x1:
-            self.load()
+            self.__load()
         elif self.operation == 0x2:
-            self.store()
+            self.__store()
         elif self.operation == 0x3:
-            self.add()
+            self.__add()
         elif self.operation == 0x4:
-            self.subt()
+            self.__subt()
         elif self.operation == 0x5:
-            self.input()
+            self.__input()
         elif self.operation == 0x6:
-            self.output()
+            self.__output()
         elif self.operation == 0x7:
-            self.halt()
+            self.__halt()
         elif self.operation == 0x8:
-            self.skipcond()
+            self.__skipcond()
         elif self.operation == 0x9:
-            self.jump()
+            self.__jump()
         elif self.operation == 0xA:
-            self.clear()
+            self.__clear()
         elif self.operation == 0xB:
-            self.addI()
+            self.__addI()
         elif self.operation == 0xC:
-            self.jumpI()
+            self.__jumpI()
         elif self.operation == 0xD:
-            self.loadI()
+            self.__loadI()
         elif self.operation == 0xE:
-            self.storeI()
-        elif self.operation == 0xF:
-            self.jnS()
+            self.__storeI()
         
 
 
-    def jnS(self):
+    def __jnS(self):
         self.MBR = self.PC
         self.M[self.MAR] = self.MBR
         self.MBR = (self.IR & 0x0FFF)
         self.AC = 0x1
         self.AC = self.AC + self.MBR
         self.PC = self.AC
 
-    def load(self):
+    def __load(self):
         self.AC = self.MBR
 
-    def store(self):
+    def __store(self):
         self.MBR = self.AC
         self.M[self.MAR] = self.MBR
 
-    def add(self):
+    def __add(self):
         self.AC = self.AC + self.MBR
 
-    def subt(self):
+    def __subt(self):
         self.AC = self.AC - self.MBR
 
-    def input(self):
+    def __input(self):
         if self.GUI:
             self.InReg = None
             while self.InReg == None:
                 self.InReg = self.InReg
         else:
             self.InReg = int(input("Input (HEX): "), 16)
         self.AC = self.InReg
 
-    def output(self):
+    def __output(self):
         self.OutReg = self.AC
         if not self.GUI:
             print("Output (HEX): " + hex(self.OutReg))
 
 
-    def halt(self):
+    def __halt(self):
         self.running = False
+        self.canStep = False
 
-    def skipcond(self):
+    def __skipcond(self):
         skipBits = (self.IR & 0b0000110000000000) >> 8
         if skipBits == 0b0000:
             if self.AC < 0:
-                self.next()
+                self.__incrementPC()
         elif skipBits == 0b0100:
             if self.AC == 0:
-                self.next()
+                self.__incrementPC()
         elif skipBits == 0b1000:
             if self.AC > 0:
-                self.next()
+                self.__incrementPC()
 
-    def jump(self):
+    def __jump(self):
         self.PC = (self.IR & 0x0FFF)
     
-    def clear(self):
+    def __clear(self):
         self.AC = 0x0
     
-    def addI(self):
+    def __addI(self):
         self.MAR = self.MBR
         self.MBR = self.M[self.MAR]
         self.AC = self.AC + self.MBR
 
-    def jumpI(self):
+    def __jumpI(self):
         self.PC = self.MBR
     
-    def loadI(self):
+    def __loadI(self):
         self.MAR = self.MBR
         self.MBR = self.M[self.MAR]
         self.AC = self.MBR
     
-    def storeI(self):
+    def __storeI(self):
         self.MAR = self.MBR
         self.MBR = self.AC
         self.M[self.MAR] = self.MBR
```

### Comparing `marieSimulator-1.1.7/src/marieSimulator/MarieGUI.py` & `marieSimulator-1.1.8/src/marieSimulator/MarieGUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from PySide6 import QtCore
 from PySide6.QtWidgets import QApplication, QMainWindow, QGridLayout, QWidget, QToolBar, QPushButton, QStatusBar, QFileDialog, QTableWidgetItem, QTableWidget, QAbstractItemView, QHeaderView
-from PySide6.QtGui import QAction, QDesktopServices
+from PySide6.QtGui import QAction, QDesktopServices, QColor, QPalette
 
 from .Marie import Marie
 from .MarieReader import MarieReader
 
 app = QApplication(sys.argv)
 
 class MarieGUI(QMainWindow):
@@ -77,16 +77,16 @@
         statusbar = QStatusBar(self)
         menu = self.menuBar()
 
         runButton = QPushButton("Run", self)
         stepButton = QPushButton("Step", self)
         resetButton = QPushButton("Reset", self)
         runButton.setStatusTip("Run the program")
-        stepButton.setStatusTip("Step through the program - Disabled")
-        resetButton.setStatusTip("Reset the Registers and Keeps the Memory")
+        stepButton.setStatusTip("Step through the program")
+        resetButton.setStatusTip("Reset the Registers and keep the Memory")
         runButton.clicked.connect(self.guiRun)
         stepButton.clicked.connect(self.guiStep)
         resetButton.clicked.connect(self.guiReset)
         toolbar.addWidget(runButton)
         toolbar.addWidget(stepButton)
         toolbar.addWidget(resetButton)
 
@@ -212,45 +212,69 @@
     def updateMemoryTableWidget(self):
         self.memoryTableWidget.setRowCount(16**2)
         self.memoryTableWidget.setColumnCount(16)
         self.memoryTableWidget.setVerticalHeaderLabels([(hex(i)[2:].zfill(2) + "0").upper() for i in range(16**2)])
         self.memoryTableWidget.setHorizontalHeaderLabels([("+" + hex(i)[2:].zfill(1)).upper() for i in range(16)])
         self.memoryTableWidget.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.memoryTableWidget.horizontalHeader().setSectionResizeMode(QHeaderView.Stretch)
-        self.memoryTableWidget.setAlternatingRowColors(True)
-        self.M = self.marie.M if self.marie != None else self.M
-        self.M += [0] * (16**3 - len(self.M))
+        self.M = self.marie.M if self.marie != None else [0] * (16**3)
         for i in range(16**2):
             for j in range(16):
                 self.memoryTableWidget.setItem(i, j, QTableWidgetItem(hex(self.M[i*16+j])[2:].zfill(4).upper()))
 
 
 
     def guiRun(self):
+
+        
+
         self.AC = self.marie.AC
         self.PC = self.marie.PC
         self.MAR = self.marie.MAR
         self.MBR = self.marie.MBR
         self.IR = self.marie.IR
         self.InReg = self.marie.InReg
         self.OutReg =  self.marie.OutReg
         self.M = self.marie.M[:]
         self.marie.run()
         self.updateRegisterTableWidget()
 
     def guiStep(self):
-        pass
+        self.AC = self.marie.AC
+        self.PC = self.marie.PC
+        self.MAR = self.marie.MAR
+        self.MBR = self.marie.MBR
+        self.IR = self.marie.IR
+        self.InReg = self.marie.InReg
+        self.OutReg =  self.marie.OutReg
+        self.M = self.marie.M[:]
+        changed = self.marie.step()
+        self.updateRegisterTableWidget()
+        for i in range(self.programTableWidget.rowCount()):
+            self.setColortoRow(self.programTableWidget, i, QColor(1, 0, 0, 0))
+        self.setColortoRow(self.programTableWidget, self.marie.PC - 1, QColor(51, 102, 153))
+        for element in changed:
+            row = element / 16
+            col = element % 16
+            for i in range(self.memoryTableWidget.rowCount()):
+                self.setColortoRow(self.memoryTableWidget, i, QColor(1, 0, 0, 0))
+            self.memoryTableWidget.item(row, col).setBackground(QColor(51, 102, 153))
+
     
     def guiReset(self):
         self.marie = None
+        for i in range(self.programTableWidget.rowCount()):
+            self.setColortoRow(self.programTableWidget, i, QColor(1, 0, 0, 0))
         self.updateRegisterTableWidget()
-        self.updateMemoryTableWidget()
         self.marie = Marie(self.marieReader)
+
+    def setColortoRow(self, table, rowIndex, color):
+        for j in range(table.columnCount()):
+            table.item(rowIndex, j).setBackground(color)
         
 
 if __name__ == "__main__":
-    app = QApplication(sys.argv)
 
     window = MarieGUI()
     window.show()
 
     sys.exit(app.exec())
```

### Comparing `marieSimulator-1.1.7/src/marieSimulator/MarieReader.py` & `marieSimulator-1.1.8/src/marieSimulator/MarieReader.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,28 @@
         self.symbolTable = {}
 
         self.read(filename)
     
     def read(self, filename):
         with open(filename, 'r') as file:
             for line in file:
+                if len(self.input) == 4096:
+                    print("Error: Memory Limit Exceeded")
+                    exit()
                 self.input.append(line)
                 if line != '\n':
                     self.M.append(0)
         
-        self.interpret()
+        self.__interpret()
         for item in self.M:
             if item & 0b100000000000 == 0b100000000000:
-                self.interpret()
+                self.__interpret()
                 break
 
-    def interpret(self):
+    def __interpret(self):
         ctr = 0
         for line in self.input:
             if line[-1] == '\n':
                 line = line[:-1]
 
             line = " ".join(line.strip().split())
             
@@ -33,15 +36,15 @@
                 self.symbolTable[tokens[0][:-1]] = ctr
                 tokens = tokens[1:]
 
             opcode = None
 
             instruction = (tokens[0]).upper()
             if instruction == 'JNS':
-                opcode = 0xF
+                opcode = 0x0
             elif instruction == 'LOAD':
                 opcode = 0x1
             elif instruction == 'STORE':
                 opcode = 0x2
             elif instruction == 'ADD':
                 opcode = 0x3
             elif instruction == 'SUBT':
@@ -67,25 +70,28 @@
             elif instruction == 'JUMPI':
                 opcode = 0xC
             elif instruction == 'LOADI':
                 opcode = 0xD
             elif instruction == 'STOREI':
                 opcode = 0xE
             else:
-                opcode = 0x0
+                opcode = 0xF
 
             address = tokens[1]
             try:
                 address = int(address, 16)
             except:
                 if address in self.symbolTable:
                     address = self.symbolTable[address]
                 else:
                     address = -1
             
-            self.M[ctr] = (opcode << 12) | address
+            if opcode != 0xF:
+                self.M[ctr] = (opcode << 12) | address
+            else:
+                self.M[ctr] = address
 
             ctr += 1
```

### Comparing `marieSimulator-1.1.7/src/marieSimulator.egg-info/PKG-INFO` & `marieSimulator-1.1.8/src/marieSimulator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marieSimulator
-Version: 1.1.7
+Version: 1.1.8
 Summary: A Python Package to simulate a MARIE architecture on any computer
 Home-page: https://github.com/dehadeaaryan/MarieSimulator
 Author: Aaryan Dehade
 Author-email: dehadeaaryan@gmail.com
 Project-URL: Bug Tracker, https://github.com/dehadeaaryan/MarieSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -68,7 +68,12 @@
 10. Clear
 11. AddI X
 12. JumpI X
 13. LoadI X
 14. StoreI X
 15. JnS X
 16. HEX X
+
+---
+
+Download the GUI application [here](https://www.aaryandehade.live/Marie%20Simulator.dmg)
+Or copy: [https://www.aaryandehade.live/Marie%20Simulator.dmg](https://www.aaryandehade.live/Marie%20Simulator.dmg)
```

