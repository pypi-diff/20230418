# Comparing `tmp/codeframe-0.1.9.tar.gz` & `tmp/codeframe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.1.9.tar", last modified: Tue Jan 10 15:05:17 2023, max compression
+gzip compressed data, was "codeframe-0.2.1.tar", last modified: Tue Apr 18 14:28:37 2023, max compression
```

## Comparing `codeframe-0.1.9.tar` & `codeframe-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2023-01-10 15:05:17.837070 codeframe-0.1.9/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1858 2023-01-10 15:05:15.000000 codeframe-0.1.9/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.833070 codeframe-0.1.9/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30022 2023-01-10 15:04:48.000000 codeframe-0.1.9/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2021-10-05 12:11:35.000000 codeframe-0.1.9/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2022-05-11 14:51:32.000000 codeframe-0.1.9/codeframe/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2021-10-05 12:11:35.000000 codeframe-0.1.9/codeframe/prj_utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/codeframe.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-01-10 15:05:17.837070 codeframe-0.1.9/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2021-10-05 12:11:35.000000 codeframe-0.1.9/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:28:37.959415 codeframe-0.2.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1916 2023-04-14 15:32:36.000000 codeframe-0.2.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    37245 2023-04-18 14:28:21.000000 codeframe-0.2.1/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2023-04-14 15:32:36.000000 codeframe-0.2.1/codeframe/prj_utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-18 14:28:37.959415 codeframe-0.2.1/codeframe.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2219 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-18 14:28:37.000000 codeframe-0.2.1/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-18 14:28:37.959415 codeframe-0.2.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2023-04-14 15:32:36.000000 codeframe-0.2.1/setup.py
```

### Comparing `codeframe-0.1.9/PKG-INFO` & `codeframe-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,75 @@
-Metadata-Version: 2.1
-Name: codeframe
-Version: 0.1.9
-Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
-Home-page: http://gitlab.com/jaromrax/codeframe
-Author: jaromrax
-Author-email: jaromrax@gmail.com
-License: GPL2
-Description: Project codeframe
-        =================
-        
-        *Creates a simple package structure, Fire, git, PyPI, bumpversion,
-        pytest and configfile ready*
-        
-        Introduction
-        ------------
-        
-        To create a new python project is a bit tedious task, especially if one
-        doesn\'t know how to.
-        
-        This purpose of this package is to make a simple, but still functional
-        project structure.
-        
-        Installation
-        ------------
-        
-        `pip3 install codeframe`
-        
-        Usage
-        -----
-        
-        Try just:
-        
-        `codeframe myproject myunit`
-        
-        This will create:
-        
-        -   subdirectory named `myproject` and inside:
-        -   **hardlink** to `bin/myproject` named `bin_myproject`,
-        -   unit `myunit`, that is soft-linked as `test_myunit`, so it works
-            with `pytest`,
-        -   `version.py`, that works with `bumpversion`
-        -   subsubdirectory `myproject`, that contains softlinks to `../` so
-            that the package structure works
-        -   `setup.py` file, where you need to fill the requirements list and
-            other things
-        -   `README.org`, that will generate `README.md` when `./distcheck` is
-            run
-        -   with `config` module it **creates** a new config DIR
-            `~/.config/myproject`
-        -   and some less important stuff
-        
-        Highlights:
-        -----------
-        
-        1.  The modules should be callable in `jupyter` that is opened in the
-            `myproj` directory.
-        2.  The hardlink `bin_myproject` make the script inside `bin/` callable
-            (but git pull from elsewhere looses the hardlink!)
-        3.  Installable on local system with the usual command
-            `pip3 install -e .`
-        4.  `config` module can be both - used at a new project and imported
-            from any project `from codeframe import config`
-        
-        ./distcheck
-        -----------
-        
-        -   generates `README.md`
-        -   creates git commit
-        -   bumpversion release
-        -   pushes to PyPI
-        
-        Idea for development
-        --------------------
-        
-        Thanks to `Fire`, each module can be developed separately and CLI can be
-        finally tuned in `bin/myproject` (hard-linked to `bin_myproject`) file.
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Project codeframe
+=================
+
+*Creates a simple package structure, Fire, git, PyPI, bumpversion,
+pytest and configfile ready*
+
+Introduction
+------------
+
+To create a new python project is a bit tedious task, especially if one
+doesn\'t know how to.
+
+This purpose of this package is to make a simple, but still functional
+project structure.
+
+Installation
+------------
+
+`pip3 install codeframe`
+
+Usage
+-----
+
+Try just:
+
+`codeframe myproject myunit`
+
+This will create:
+
+-   subdirectory named `myproject` and inside:
+-   **hardlink** to `bin/myproject` named `bin_myproject`,
+-   unit `myunit`, that is soft-linked as `test_myunit`, so it works
+    with `pytest`,
+-   `version.py`, that works with `bumpversion`
+-   subsubdirectory `myproject`, that contains softlinks to `../` so
+    that the package structure works
+-   `setup.py` file, where you need to fill the requirements list and
+    other things
+-   `README.org`, that will generate `README.md` when `./distcheck` is
+    run
+-   with `config` module it **creates** a new config DIR
+    `~/.config/myproject`
+-   and some less important stuff
+
+Highlights:
+-----------
+
+1.  The modules should be callable in `jupyter` that is opened in the
+    `myproj` directory.
+2.  The hardlink `bin_myproject` make the script inside `bin/` callable
+    (but git pull from elsewhere looses the hardlink!)
+3.  Installable on local system with the usual command
+    `pip3 install -e .`
+4.  `config` module can be both - used at a new project and imported
+    from any project `from codeframe import config`
+
+./distcheck
+-----------
+
+-   generates `README.md`
+-   creates git commit
+-   bumpversion release
+-   pushes to PyPI
+
+Notes for development
+---------------------
+
+Thanks to `Fire`, each module can be developed separately and CLI can be
+finally tuned in `bin/myproject` (hard-linked to `bin_myproject`) file.
+
+TODO
+====
+
+-   topbar from gregory
+-   key~enter~ \'\'
```

### Comparing `codeframe-0.1.9/README.md` & `codeframe-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: codeframe
+Version: 0.2.1
+Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
+Home-page: http://gitlab.com/jaromrax/codeframe
+Author: jaromrax
+Author-email: jaromrax@gmail.com
+License: GPL2
+Description-Content-Type: text/markdown
+
 Project codeframe
 =================
 
 *Creates a simple package structure, Fire, git, PyPI, bumpversion,
 pytest and configfile ready*
 
 Introduction
@@ -58,12 +68,18 @@
 -----------
 
 -   generates `README.md`
 -   creates git commit
 -   bumpversion release
 -   pushes to PyPI
 
-Idea for development
---------------------
+Notes for development
+---------------------
 
 Thanks to `Fire`, each module can be developed separately and CLI can be
 finally tuned in `bin/myproject` (hard-linked to `bin_myproject`) file.
+
+TODO
+====
+
+-   topbar from gregory
+-   key~enter~ \'\'
```

### Comparing `codeframe-0.1.9/bin/codeframe` & `codeframe-0.2.1/bin/codeframe`

 * *Files 15% similar despite different names*

```diff
@@ -132,14 +132,343 @@
     with cd(proj):
         with cd(proj):
             os.symlink("../"+NAME, NAME)
     print("             [OK]")
 
 
 
+def create_unit_topbar(proj):
+    result = """#!/usr/bin/env python3
+
+# from {proj}.version import __version__
+from fire import Fire
+import time
+
+import pytermgui
+from pytermgui import print_to, report_cursor, bold, inverse, underline, italic, save_cursor, restore_cursor, terminal, cursor_up, move_cursor
+
+import threading # for key input
+
+from console import fg, bg, fx
+import datetime as dt
+
+theight= terminal.height
+twidth= terminal.width
+
+global_mode = " "
+
+
+class Topbar:
+    def __init__(self, pos=1, bgcolor=bg.blue ):
+        self.pos = pos
+        self.positions = {}
+        self.t2 = None
+        if pos==1:
+            self.BCOL = bgcolor #bg.blue
+        elif pos==2:
+            self.BCOL = bgcolor # bg.white
+        #self.t = threading.currentThread()
+
+        try:
+            #print("report_cursor to appear")
+            print( "i... topbar: pos/cursor",pos, report_cursor() )
+            #print("report done")
+        except:
+            print("X... problem with report_cursor")
+
+        #print("i... topbar bar started")
+
+
+    def add(self,two=2, bgcolor=bg.blue ):
+        if two==2:
+            self.t2 = Topbar(two ,bgcolor = bgcolor)
+        else:
+            print("X... nobody wanted more than two......  NOT OK")
+        return self.t2
+
+
+    def print_to(self, tup, s):
+        if type(tup) is tuple:
+            x,y = tup[0],tup[1]
+            print("X.......... TUPLE in the TOPBAR  IS SUPRESSED")
+        elif type(tup) is int:
+            x=tup
+            y=1
+        else:
+            print("X... NOBODY WANTED something else than tuple or int in the TOPBAR  position")
+        self.positions[ x ] = s
+
+
+    def place(self):
+        '''
+        Place he BAR on screen
+        '''
+        curs =(-1,-1)
+        if self.pos==1:
+            save_cursor()
+        print_to( (1,self.pos),  f"{self.BCOL}"+" "*twidth+bg.default )
+        print_to( (1,self.pos+1), " "*twidth )
+
+        ###### self.positions[ twidth] = f"{fx.default}{fg.default}{bg.default}"
+
+        for k in self.positions.keys():
+            print_to( (k,self.pos), f"{self.BCOL}{self.positions[k]}{bg.default}{fx.default}{fg.default}" )
+
+
+
+        if self.t2 is not None:
+            self.t2.place()
+
+        if self.pos==1:
+            restore_cursor()
+            print("", end="\\r") # this make GOOD thing in printing
+
+
+
+def main():
+    #print()
+    t = Topbar(1)
+    for i in range(100):
+        #
+        # DO whatever stuff and PLACE PRINTTO SLEEP
+        #
+        t.place()
+        t.print_to( (1,1), f"{fg.white} {str(dt.datetime.now())[:-4]} {fg.default}" )
+        time.sleep(0.1)
+
+if __name__=="__main__":
+    Fire(main)
+"""
+    unit = "topbar"
+    print(f"i...    creating  {unit}", end="")
+    NAME = f"{unit}.py"
+    UNIT1 = proj + "/" + NAME
+    with open(UNIT1, "w") as f:
+        f.write(result)
+    os.chmod(UNIT1, 0o775)
+    with cd(proj):
+        with cd(proj):
+            os.symlink("../"+NAME, NAME)
+    # --- link to test_unit.py
+    with cd(proj):
+        os.symlink(NAME, "test_"+NAME)
+    print("             [OK]")
+
+
+
+
+
+def create_unit_keyb(proj):
+    result="""#!/usr/bin/env python3
+
+# from {proj}.version import __version__
+from fire import Fire
+import threading
+import time
+from console import fg,bg,fx
+
+#import readchar
+from sshkeyboard import listen_keyboard, stop_listening
+
+global_key = ""
+
+def get_global_key():
+    global global_key
+    a = global_key
+    #global_key = ""
+    return a
+
+# https://sshkeyboard.readthedocs.io/en/latest/reference.html#sshkeyboard.listen_keyboard_manual
+# https://github.com/ollipal/sshkeyboard
+
+
+class KeyboardThreadSsh(threading.Thread):
+    def __init__(self,  name='keyboard-input-thread', ending=None):
+        '''
+        Restart itself as thread
+        '''
+        self.block = False
+        self.ending = ending
+        self.cursor = 0
+        super(KeyboardThreadSsh, self).__init__(name=name)
+        self.start()
+
+
+    def text_split(self):
+        '''
+        operates on global_key and cursor, returns 3 parts
+        0 is before 1.st letter
+        '''
+        global global_key
+        a,b,c="","",""
+        lel = len(global_key)
+
+        cursor = self.cursor
+
+        if  cursor>lel:
+            cursor=lel
+        if cursor<0:
+            cursor=0
+
+        if lel==0:
+            return a,b
+
+        #  a b c
+        # 0 1 2 3
+        if cursor==lel:
+            a=global_key
+            return a,b
+
+        if cursor == 0:
+            b = global_key
+            return a,b
+
+        if cursor == 1:
+            a = global_key[0]
+            b = global_key[1:]
+            return a,b
+        else:
+            a=global_key[:cursor]
+            b=global_key[cursor:]
+        return a,b
+
+
+    def press(self,key):
+        '''
+        the callback - uses the global_key to remember
+        '''
+        global global_key
+        #print("D...", f"'{key}' pressed")
+        #print("D...", f"{global_key} , cu=={self.cursor} :", self.text_split() )
+
+
+        # the tricks: space up down
+        if key=="space":
+            key=" "
+            self.cursor+=1
+        elif key=="delete":
+            if self.cursor<=len(global_key):
+                global_key =  global_key[:self.cursor]+global_key[self.cursor+1:]
+            key=""
+        elif key=="backspace":
+            global_key =  global_key[:self.cursor-1]+global_key[self.cursor:]
+            self.cursor-=1
+            key=""
+        elif key=="end":
+            self.cursor = len(global_key)
+            key=""
+        elif key=="home":
+            self.cursor = 0
+            key=""
+        elif key=="left":
+            self.cursor-=1
+            key=""
+        elif key=="right":
+            self.cursor+=1
+            key=""
+        elif key=="enter":
+            key="\\n"
+            self.cursor=len(global_key)
+        elif key=="up":
+            key=""
+        elif key=="down":
+            key=""
+        elif key=="tab":
+            key=""
+        #else:
+        #    self.cursor+=1
+
+        # print("D...  ..........",self.cursor, "after press /    limit",len(global_key)+1)
+
+        #### global_key = f"{global_key[:self.cursor+1]}{key}{global_key[self.cursor+1:]}" # KEEP IT GLOBAL !!!!!
+        a,b = self.text_split()
+        # print(f"i... joining {a} {key} {b}")
+        global_key = f"{a}{key}{b}" # KEEP IT GLOBAL !!!!!
+        if len(key)>0:
+            self.cursor+=1
+
+        # correct cursor if  it went too far
+        if self.cursor>len(global_key)+1:self.cursor=len(global_key)+1
+        if self.cursor<0:self.cursor=0
+
+        #print("D...",f"RESULT: '{global_key}' , cu=={self.cursor} :", self.text_split() )
+        #print("D...")
+        #self.cursor+=1
+
+        if key=="\\n":
+            stop_listening()
+
+
+
+    def get_global_key(self):
+        '''
+        use to read the situation and reset on enter from the main program, True when ENTER
+        '''
+        global global_key
+        if global_key.find("\\n")>=0:
+            a = global_key
+            global_key = ""
+            return a, True, self.text_split()
+        return global_key, False, self.text_split()
+
+
+    def run(self):
+        '''
+        this is a mandatory for Thread child
+        '''
+        global global_key
+        self.t = threading.current_thread()
+        while True:
+            #print("!...  ........................keyboard listen START")
+            listen_keyboard(on_press=self.press,
+                            sequential=True) # syncio
+            #print("!...  ........................keyboard listen STOP")
+            #print("D...",f"/{global_key}/")
+            if global_key.strip() == self.ending:
+                #print("!...  ........................keyboard listen BREAK")
+                break
+        print("!...  ........................keyboard THREAD  ENDED")
+
+
+
+
+#--------https://stackoverflow.com/questions/2408560/python-nonblocking-console-input
+# ON ENTER
+# CALL WITH CALLBACK FUNCTION AS A PARAMETER
+#class KeyboardThread(threading.Thread):
+
+
+
+
+def main():
+    print()
+
+if __name__=="__main__":
+    Fire(main)
+
+"""
+
+    unit = "key_enter"
+    print(f"i...    creating  {unit}", end="")
+    NAME = f"{unit}.py"
+    UNIT1 = proj + "/" + NAME
+    with open(UNIT1, "w") as f:
+        f.write(result)
+    os.chmod(UNIT1, 0o775)
+    with cd(proj):
+        with cd(proj):
+            os.symlink("../"+NAME, NAME)
+    # --- link to test_unit.py
+    with cd(proj):
+        os.symlink(NAME, "test_"+NAME)
+    print("             [OK]")
+
+
+
+
 def create_unit(proj, unit):
     result=f"""#!/usr/bin/env python3
 '''
 We create a unit, that will be the test_ unit by ln -s simoultaneously. Runs with 'pytest'
 '''
 from {proj}.version import __version__
 from fire import Fire
@@ -488,31 +817,14 @@
 
 import pkg_resources  # to be able to read data in package
 from fire import Fire
 import sys
 import builtins as __builtin__
 
 
-# THIS I DONT SEE A POINT..... always returns the same
-#par = pkg_resources.Requirement.parse('pandas')
-#print("parse://".format(par))
-# adds '--' to the package PATH
-#print( pkg_resources.resource_filename( 'pandas', '--') )
-
-class Bcolors:
-    HEADER = '\\033[95m'
-    OKBLUE = '\\033[94m'
-    OKGREEN = '\\033[92m'
-    WARNING = '\\033[93m'
-    FAIL = '\\033[91m'
-    ENDC = '\\033[0m'
-    BOLD = '\\033[1m'
-    UNDERLINE = '\\033[4m'
-
-
 def fail(t):
     print("")
     print(t)
     sys.exit()
 
 def get_file_path(filename):
 
@@ -520,43 +832,14 @@
 
     ret = pkg_resources.resource_filename('{proj}',
                                         'data/'+filename )
     return ret
 
 
 
-def super_print(debug=True):
-    """ filename is the file where output will be written"""
-    def wrap(func):
-        """ func is the function you are "overriding", i.e. wrapping"""
-        def wrapped_func(*args,**kwargs):
-            """  *args and **kwargs are the arguments supplied
-             to the overridden function"""
-
-            #use with statement to open, write to, and close the file safely
-            #with open(filename,'a') as outputfile:
-            #    outputfile.write(*args,**kwargs)
-            #now original function executed with its arguments as normal
-
-            if len(args)>0:
-                #print(type(args[0]), args[0])
-                if (isinstance(args[0], str)) and (args[0].find("D...")>=0):
-                    if not debug:
-                        return
-            if 'file' in kwargs:
-                __builtin__.print(*args, **kwargs )
-            else:
-                __builtin__.print(*args, **kwargs, file=sys.stderr)
-            return #func(*args,**kwargs)
-        return wrapped_func
-    return wrap
-
-#USE AS print = super_print(debug)(print)
-#     print = super_print('output.txt')(print) ... original post
-
 if __name__=="__main__":
     Fire(get_file_path)
 '''
 
     print("i...    running  prj_utils.py - helper unit creation", end="")
     NAME = "prj_utils.py"
 
@@ -623,14 +906,28 @@
 
 #==============================================
 
 def create_distcheck(proj):
     result=f"""#/bin/bash
 
 rm dist/*
+
+pip3 freeze  | grep twine
+if [ "$0" != "0" ]; then
+  echo X... pip3 install twine
+  exit 1
+fi
+
+pip3 freeze  | grep -e "bumpversion="
+if [ "$0" != "0" ]; then
+  echo X... pip3 install bumpversion
+  exit 1
+fi
+
+
 python3 setup.py sdist
 twine check dist/*
 echo "                                 ok? passed?  ENTER then"
 echo "                                 ok? passed?  ENTER then"
 echo " - check  correctness of download/url and email"
 echo " - AND        !!!  I WILL CONVERT README.org to README.md"
 echo "                                 ok? passed?  ENTER then"
@@ -674,15 +971,15 @@
 echo "          real PyPI UPLOAD (after bumpversion release):"
 echo "          real PyPI UPLOAD (after bumpversion release):"
 echo "twine upload dist/*"
 echo " ... "
 twine upload  dist/*
 
 echo "i... pushing newly created tags to GITREPO"
-git push origin master --tags
+git push origin main --tags
 """
     print("i...    creating  distcheck", end="")
     NAME = "distcheck"
     FIPY = proj+"/"+ NAME
     with open(FIPY, "w") as f:
         f.write(result)
     os.chmod(FIPY, 0o775)
@@ -724,14 +1021,16 @@
 six==1.12.0
 tqdm==4.31.1
 twine==1.13.0
 urllib3==1.24.1
 webencodings==0.5.1
 fire==0.2.1
 pytest==5.3.4
+console
+sshkeyboard
 """
     print("i...    creating  requirements", end="")
     NAME = "requirements.txt"
     FIPY = proj+"/"+ NAME
     with open(FIPY, "w") as f:
         f.write(result)
     print("             [OK]")
@@ -740,80 +1039,99 @@
 
 
 
 
 #==============================================
 
 def create_binary(proj, unit):
-    result=f"""#!/usr/bin/env python3
+    result1=f"""#!/usr/bin/env python3
 
 # to override print <= can be a big problem with exceptions
 from __future__ import print_function # must be 1st
 import builtins
 
 import sys
 
 from fire import Fire
 
 from {proj}.version import __version__
 from {proj} import {unit}
 from {proj} import config
 
 
-class Bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
+from {proj}  import topbar
+from {proj}  import key_enter
+import time
+import datetime as dt
+from console import fg,bg,fx
 
 def main(cmd = "usage", debug=False):
     ''' Main function of the project
     '''
-    if not debug:
-        _print = print # keep a local copy of the original print
-        builtins.print =lambda *args, **kwargs:  None  if (isinstance(args[0], str)) and (args[0].find("D...")==0) else  _print( *args, **kwargs) if ('file' in kwargs) else _print( "{{}}".format(Bcolors.FAIL   if ((isinstance(args[0], str)) and (args[0].find("X...")>=0)) else Bcolors.ENDC) , *args, Bcolors.ENDC, **kwargs, file=sys.stderr)
-    else:
-        # debug - show all + colors
-        _print = print # keep a local copy of the original print
-        builtins.print =lambda *args, **kwargs:   _print( *args, **kwargs) if ('file' in kwargs) else _print( "{{}}".format(Bcolors.FAIL   if ((isinstance(args[0], str)) and (args[0].find("X...")>=0)) else Bcolors.OKGREEN if  ((isinstance(args[0], str)) and (args[0].find("i...")>=0)) else Bcolors.ENDC  ), *args, Bcolors.ENDC, **kwargs, file=sys.stderr)
 
     #======== DEFINE THE CONFIG FILE HERE ========
 
     config.CONFIG['filename'] = "~/.config/{proj}/cfg.json"
     # config.load_config()
     # config.save_config()
 
-    print("D... bbb script; version:",__version__)
-    print("i... testing info  message",1,2)
-    print("D... testing debug message",3,4)
-    print("X... testing alert message",5,6)
-    print(7,8)
     if cmd == "usage":
         print(''' ... usage:
         	 _
         ''')
-        sys.exit(0)
+        #sys.exit(0)
     else:
         {unit}.func()
+"""
+    result2="""
+    # ===================== top bar and keyboard ==========
+
+    top = topbar.Topbar( bgcolor = bg.blue)
+    top2 = top.add( bgcolor = bg.black)
+    kthread = key_enter.KeyboardThreadSsh(ending="q")
+
+
+
+    while True: # ================================= LOOP
+        time.sleep(0.05)
+        top.print_to(  10, f" {fg.white}{fx.bold}{dt.datetime.now()}{fx.default}{fg.default} ")
+
+        key,enter,abc = kthread.get_global_key()
+        (a,b) = abc # unpack tuple
+
+        if enter:
+            #print("--------------------------------------ENTER")
+            if key.strip()=="q":
+                break
+            cmd = key.strip()
+            print(f"----------------------- {cmd} --------------------- ***")
+        else:
+            cmd = ""
+        arg = ""
+
+        if len(key)==0:
+            top2.print_to( 0, f"{fg.cyan}{bg.black}{' '*80}{bg.black}")
+        else:
+            top2.print_to( 0, f"{fg.white}{bg.red} > {fx.bold}{a}{fg.yellow}_{fg.white}{b}{fx.default}{fg.default}{bg.default} ")
+        top.place()
+
+#====================================================================
 
 if __name__=="__main__":
     Fire(main)
 
 
 """
     print("i...    creating  bin script", end="")
     NAME = proj
     FIPY = proj+"/bin/"+ NAME
     with open(FIPY, "w") as f:
-        f.write(result)
+        f.write(result1)
+        f.write("\n")
+        f.write(result2)
     os.chmod(FIPY, 0o775)
     print("             [OK]")
     print("i...    creating hardlink", end="")
     NAME = proj
     FIPY = proj+"/bin/"+ NAME
     os.link(FIPY, proj+"/bin_"+proj+".py")
     print("             [OK]")
@@ -881,23 +1199,24 @@
     else:
         raise RuntimeError("Unable to find version string.")
 
 setup(
     name="{proj}",
     description="Automatically created environment for python package",
     author="me",
+    url="http://gitlab.com/me/{proj}",
     author_email="mail@gmail.com",
     license="GPL2",
     version=get_version("{proj}/version.py"),
     packages=['{proj}'],
     package_data={{'{proj}': ['data/*']}},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/{proj}'],
-    install_requires = ['fire'],
+    install_requires = ['fire','console','sshkeyboard'],
 )
 """
     print("i...    creating  setup", end="")
     NAME = "setup.py"
     FIPY = proj+"/"+ NAME
     with open(FIPY, "w") as f:
         f.write(result)
@@ -997,19 +1316,21 @@
         f.write(result)
     print("             [OK]")
 
 
 #==============================================
 
 def init_git(proj):
+    print("D... INITGIT")
     print("i...    running  init git", end="")
 
     with cd(proj):
         CMD="git init ."
         s.check_output(CMD.split())
+        print("------------------add")
         CMD="git add ."
         s.check_output(CMD.split())
         CMD='git commit -a -m "First_Automatic_Commit"'
         s.check_output(CMD.split())
         CMD='bumpversion patch'
         s.check_output(CMD.split())
     print("             [OK]")
@@ -1096,14 +1417,17 @@
     os.mkdir(proj+"/data")
     os.mkdir(proj+"/"+proj)
     #os.mkdir(proj+"")
     #os.mkdir(proj+"")
     #--- version; unit; __init__ ==> ./unit1.py should work=====
     create_version(proj)
     create_unit(proj, unit)
+    create_unit_keyb(proj)
+    create_unit_topbar(proj)
+
     create_config(proj )
     #create_prj_utils(proj) # I dont use anymore
     create_init(proj)
     create_binary(proj, unit)
     #--- now - it should be possible to run ./unit1.py==========
     # AUXILIARY FILES.....
     create_readme(proj, unit)
@@ -1116,15 +1440,16 @@
     #install_requirements(proj)
     usage_bumpversion(proj)
     usage_developmentcycle(proj)
     create_gitignore(proj)
     if not create_only:
         init_git(proj)
         init_test(proj)
-        print(f"X... HIGHLY PROBABLY I CREATED ~/.config/{proj}/cfg.conf - with pytest")
+        print(f"i... HIGHLY PROBABLY I CREATED ~/.config/{proj}/cfg.conf - during pytest")
+
 
     print("______________________________")
     print(f"cd {proj}; ./bin_{proj}.py test; echo __; ./bin_{proj}.py test -d; cd ..")
     print("______________________________")
```

### Comparing `codeframe-0.1.9/codeframe/config.py` & `codeframe-0.2.1/codeframe/config.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.1.9/codeframe/prj_utils.py` & `codeframe-0.2.1/codeframe/prj_utils.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.1.9/codeframe.egg-info/PKG-INFO` & `codeframe-0.2.1/codeframe.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,85 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.1.9
+Version: 0.2.1
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
-Description: Project codeframe
-        =================
-        
-        *Creates a simple package structure, Fire, git, PyPI, bumpversion,
-        pytest and configfile ready*
-        
-        Introduction
-        ------------
-        
-        To create a new python project is a bit tedious task, especially if one
-        doesn\'t know how to.
-        
-        This purpose of this package is to make a simple, but still functional
-        project structure.
-        
-        Installation
-        ------------
-        
-        `pip3 install codeframe`
-        
-        Usage
-        -----
-        
-        Try just:
-        
-        `codeframe myproject myunit`
-        
-        This will create:
-        
-        -   subdirectory named `myproject` and inside:
-        -   **hardlink** to `bin/myproject` named `bin_myproject`,
-        -   unit `myunit`, that is soft-linked as `test_myunit`, so it works
-            with `pytest`,
-        -   `version.py`, that works with `bumpversion`
-        -   subsubdirectory `myproject`, that contains softlinks to `../` so
-            that the package structure works
-        -   `setup.py` file, where you need to fill the requirements list and
-            other things
-        -   `README.org`, that will generate `README.md` when `./distcheck` is
-            run
-        -   with `config` module it **creates** a new config DIR
-            `~/.config/myproject`
-        -   and some less important stuff
-        
-        Highlights:
-        -----------
-        
-        1.  The modules should be callable in `jupyter` that is opened in the
-            `myproj` directory.
-        2.  The hardlink `bin_myproject` make the script inside `bin/` callable
-            (but git pull from elsewhere looses the hardlink!)
-        3.  Installable on local system with the usual command
-            `pip3 install -e .`
-        4.  `config` module can be both - used at a new project and imported
-            from any project `from codeframe import config`
-        
-        ./distcheck
-        -----------
-        
-        -   generates `README.md`
-        -   creates git commit
-        -   bumpversion release
-        -   pushes to PyPI
-        
-        Idea for development
-        --------------------
-        
-        Thanks to `Fire`, each module can be developed separately and CLI can be
-        finally tuned in `bin/myproject` (hard-linked to `bin_myproject`) file.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+Project codeframe
+=================
+
+*Creates a simple package structure, Fire, git, PyPI, bumpversion,
+pytest and configfile ready*
+
+Introduction
+------------
+
+To create a new python project is a bit tedious task, especially if one
+doesn\'t know how to.
+
+This purpose of this package is to make a simple, but still functional
+project structure.
+
+Installation
+------------
+
+`pip3 install codeframe`
+
+Usage
+-----
+
+Try just:
+
+`codeframe myproject myunit`
+
+This will create:
+
+-   subdirectory named `myproject` and inside:
+-   **hardlink** to `bin/myproject` named `bin_myproject`,
+-   unit `myunit`, that is soft-linked as `test_myunit`, so it works
+    with `pytest`,
+-   `version.py`, that works with `bumpversion`
+-   subsubdirectory `myproject`, that contains softlinks to `../` so
+    that the package structure works
+-   `setup.py` file, where you need to fill the requirements list and
+    other things
+-   `README.org`, that will generate `README.md` when `./distcheck` is
+    run
+-   with `config` module it **creates** a new config DIR
+    `~/.config/myproject`
+-   and some less important stuff
+
+Highlights:
+-----------
+
+1.  The modules should be callable in `jupyter` that is opened in the
+    `myproj` directory.
+2.  The hardlink `bin_myproject` make the script inside `bin/` callable
+    (but git pull from elsewhere looses the hardlink!)
+3.  Installable on local system with the usual command
+    `pip3 install -e .`
+4.  `config` module can be both - used at a new project and imported
+    from any project `from codeframe import config`
+
+./distcheck
+-----------
+
+-   generates `README.md`
+-   creates git commit
+-   bumpversion release
+-   pushes to PyPI
+
+Notes for development
+---------------------
+
+Thanks to `Fire`, each module can be developed separately and CLI can be
+finally tuned in `bin/myproject` (hard-linked to `bin_myproject`) file.
+
+TODO
+====
+
+-   topbar from gregory
+-   key~enter~ \'\'
```

### Comparing `codeframe-0.1.9/setup.py` & `codeframe-0.2.1/setup.py`

 * *Files identical despite different names*

