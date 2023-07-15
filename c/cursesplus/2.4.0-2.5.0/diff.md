# Comparing `tmp/cursesplus-2.4.0.tar.gz` & `tmp/cursesplus-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.4.0.tar", last modified: Sat Jul 15 20:52:22 2023, max compression
+gzip compressed data, was "cursesplus-2.5.0.tar", last modified: Sat Jul 15 21:29:39 2023, max compression
```

## Comparing `cursesplus-2.4.0.tar` & `cursesplus-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.126721 cursesplus-2.4.0/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.4.0/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1225 2023-07-15 20:52:22.116721 cursesplus-2.4.0/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      622 2023-07-15 20:51:43.000000 cursesplus-2.4.0/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-07-15 20:49:09.000000 cursesplus-2.4.0/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-07-15 20:52:22.126721 cursesplus-2.4.0/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      452 2023-07-15 20:47:26.000000 cursesplus-2.4.0/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.4.0/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    17447 2023-07-15 20:41:49.000000 cursesplus-2.4.0/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-07-15 20:49:42.000000 cursesplus-2.4.0/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-07-15 20:50:21.000000 cursesplus-2.4.0/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1225 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.5.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1176 2023-07-15 21:29:39.116721 cursesplus-2.5.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      573 2023-07-15 21:27:06.000000 cursesplus-2.5.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-07-15 21:26:24.000000 cursesplus-2.5.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-07-15 21:29:39.116721 cursesplus-2.5.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.106721 cursesplus-2.5.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      545 2023-07-15 21:14:23.000000 cursesplus-2.5.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.5.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18822 2023-07-15 21:23:54.000000 cursesplus-2.5.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-07-15 20:49:42.000000 cursesplus-2.5.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-07-15 20:50:21.000000 cursesplus-2.5.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 21:29:39.116721 cursesplus-2.5.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1176 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-07-15 21:29:39.000000 cursesplus-2.5.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.4.0/LICENSE` & `cursesplus-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.4.0/pyproject.toml` & `cursesplus-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.4.0"
+version = "2.5.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.4.0/src/cursesplus/__init__.py` & `cursesplus-2.5.0/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.4.0/src/cursesplus/cp.py` & `cursesplus-2.5.0/src/cursesplus/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import curses#Depends on windows-curses on win32
 from curses.textpad import rectangle, Textbox
 import os
 from time import sleep
 import random
 from datetime import datetime
+import threading
 
 #DEFINE SOME CONSTANTS
 BLACK = curses.COLOR_BLACK
 WHITE = curses.COLOR_WHITE
 RED = curses.COLOR_RED
 YELLOW = curses.COLOR_YELLOW
 GREEN = curses.COLOR_GREEN
@@ -356,14 +357,55 @@
     """Hide Cursor. Can only be called in an active curses window"""
     curses.curs_set(0)
 
 def showcursor():
     """Show cursor. Can only be called in an active curses window"""
     curses.curs_set(1)
 
+class PleaseWaitScreen:
+    def __init__(self,stdscr,message=["Please Wait"]):
+        self.message = message + [""]
+        self.screen = stdscr
+        self.tick = 0
+        self.stopped = False
+    def _update(self):
+        message = self.message
+        self.screen.clear()
+        #self.screen.refresh()
+        self.tick += 1
+        if self.tick == 4:
+            self.tick = 0
+        x,y = os.get_terminal_size()
+        ox = 0
+        for o in message:
+            ox += 1
+            if "\n" in o:
+                message.insert(ox,o.split("\n")[1])
+        message = [m[0:x-5].split("\n")[0] for m in message]#Limiting characters
+        message[-2] += self.tick*"."
+        maxs = max([len(s) for s in message])
+        rectangle(self.screen,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+2, x//2+(maxs//2+1)+1)
+        mi = -(len(message)/2)
+        
+        for msgl in message[0:-1]:
+            mi += 1
+            self.screen.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl)
+        
+        self.screen.refresh()
+    def _tst(self):
+        while not self.stopped:
+            self._update()
+            sleep(0.3)
+    def start(self):
+        threading.Thread(target=self._tst).start()
+    def stop(self):
+        self.stopped = True
+    def destroy(self):
+        del self
+
 class ProgressBarTypes:
     FullScreenProgressBar: int = 0
     SmallProgressBar: int = 1
 class ProgressBarLocations:
     TOP = 0
     CENTER = 1
     BOTTOM = 2
```

### Comparing `cursesplus-2.4.0/src/cursesplus/filedialog.py` & `cursesplus-2.5.0/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.4.0/src/cursesplus/messagebox.py` & `cursesplus-2.5.0/src/cursesplus/messagebox.py`

 * *Files identical despite different names*

