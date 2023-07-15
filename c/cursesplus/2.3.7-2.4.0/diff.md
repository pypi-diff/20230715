# Comparing `tmp/cursesplus-2.3.7.tar.gz` & `tmp/cursesplus-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.3.7.tar", last modified: Fri Jun 30 18:59:43 2023, max compression
+gzip compressed data, was "cursesplus-2.4.0.tar", last modified: Sat Jul 15 20:52:22 2023, max compression
```

## Comparing `cursesplus-2.3.7.tar` & `cursesplus-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.3.7/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1457 2023-06-30 18:59:43.587034 cursesplus-2.3.7/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      854 2023-06-30 18:59:24.000000 cursesplus-2.3.7/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-06-30 18:59:12.000000 cursesplus-2.3.7/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-06-30 18:59:43.597034 cursesplus-2.3.7/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      357 2023-06-30 18:52:19.000000 cursesplus-2.3.7/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.3.7/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    17144 2023-06-30 18:58:46.000000 cursesplus-2.3.7/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-05-18 14:43:10.000000 cursesplus-2.3.7/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.3.7/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-06-30 18:59:43.587034 cursesplus-2.3.7/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1457 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-06-30 18:59:43.000000 cursesplus-2.3.7/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.126721 cursesplus-2.4.0/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.4.0/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1225 2023-07-15 20:52:22.116721 cursesplus-2.4.0/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      622 2023-07-15 20:51:43.000000 cursesplus-2.4.0/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-07-15 20:49:09.000000 cursesplus-2.4.0/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-07-15 20:52:22.126721 cursesplus-2.4.0/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      452 2023-07-15 20:47:26.000000 cursesplus-2.4.0/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.4.0/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    17447 2023-07-15 20:41:49.000000 cursesplus-2.4.0/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    18476 2023-07-15 20:49:42.000000 cursesplus-2.4.0/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     9323 2023-07-15 20:50:21.000000 cursesplus-2.4.0/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-07-15 20:52:22.116721 cursesplus-2.4.0/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1225 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-07-15 20:52:22.000000 cursesplus-2.4.0/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.3.7/LICENSE` & `cursesplus-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.7/pyproject.toml` & `cursesplus-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.3.7"
+version = "2.4.0"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.3.7/src/cursesplus/__init__.py` & `cursesplus-2.4.0/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.7/src/cursesplus/cp.py` & `cursesplus-2.4.0/src/cursesplus/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,21 @@
                 ERROR = " You have reached the top of the text "
                 curses.beep()
         else:
             if len(chn) > 1:
                 #Special char
                 if chn == b"^D":
                     stdscr.erase()
-                    return "\n".join([lx for lx in ["".join(t) for t in text] if lx != ""])
+                    if retremptylines:
+                        fretr = "\n".join([lx for lx in ["".join(t) for t in text]])
+                        if len(fretr.splitlines()) < len(text):
+                            fretr += "\n"
+                        return fretr
+                    else:
+                        return "\n".join([lx for lx in ["".join(t) for t in text] if lx != ""])
                 elif chn == b"^K":
                     text = [[] for _ in range(lines)]#Delete
                     ln = 0
                     col = 0
                     stdscr.erase()
             else:
                 #append
```

### Comparing `cursesplus-2.3.7/src/cursesplus/filedialog.py` & `cursesplus-2.4.0/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.3.7/src/cursesplus/messagebox.py` & `cursesplus-2.4.0/src/cursesplus/messagebox.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,14 +37,85 @@
         if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
             selected = not selected
         elif ch == 121 or ch == 110:
             return ch == 121
         elif ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return selected
 
+def askokcancel(stdscr,message: list = [],colour=False) -> bool:
+    """Display a messagebox that asks a user a question OK or canel  Returns TRUE on OK and FALSE on Cancel. Colour is green"""
+    selected = True
+    x,y = os.get_terminal_size()
+    ox = 0
+    if colour:
+        BGCL = cp.GREEN
+    else:
+        BGCL = cp.BLACK
+    for o in message:
+        ox += 1
+        if "\n" in o:
+            message.insert(ox,o.split("\n")[1])
+    message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
+    maxs = max([len(s) for s in message])
+    while True:
+        for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
+            for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
+        rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
+        mi = -(len(message)/2)
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",[cp.set_colour(cp.WHITE,cp.BLACK) if selected else cp.set_colour(cp.BLACK,cp.WHITE)][0])
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[Cancel]",[cp.set_colour(cp.BLACK,cp.WHITE) if selected else cp.set_colour(cp.WHITE,cp.BLACK)][0])   
+        for msgl in message:
+            mi += 1
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
+    
+        stdscr.refresh()
+        
+        ch = stdscr.getch()
+        if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
+            selected = not selected
+        elif ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
+            return selected
+        
+def askretrycancel(stdscr,message: list = [],colour=False) -> bool:
+    """Display a messagebox that asks a user a question OK or canel  Returns TRUE on OK and FALSE on Cancel. Colour is green"""
+    selected = True
+    x,y = os.get_terminal_size()
+    ox = 0
+    if colour:
+        BGCL = cp.GREEN
+    else:
+        BGCL = cp.BLACK
+    for o in message:
+        ox += 1
+        if "\n" in o:
+            message.insert(ox,o.split("\n")[1])
+    message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
+    maxs = max([len(s) for s in message])
+    while True:
+        for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
+            for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
+        rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
+        mi = -(len(message)/2)
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[Retry]",[cp.set_colour(cp.WHITE,cp.BLACK) if selected else cp.set_colour(cp.BLACK,cp.WHITE)][0])
+        stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[Cancel]",[cp.set_colour(cp.BLACK,cp.WHITE) if selected else cp.set_colour(cp.WHITE,cp.BLACK)][0])   
+        for msgl in message:
+            mi += 1
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
+    
+        stdscr.refresh()
+        
+        ch = stdscr.getch()
+        if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
+            selected = not selected
+        elif ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
+            return selected
+    
+
 def showinfo(stdscr,message: list = [],title:str="Info",colour=False) -> None:
     """Display a messagebox that shows info to a user. Background BLUE"""
     selected = True
     if colour:
         BGCL = cp.BLUE
     else:
         BGCL = cp.BLACK
@@ -103,15 +174,15 @@
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
-def showerror(stdscr,message: list = [],title:str="Warning",colour=False) -> None:
+def showerror(stdscr,message: list = [],title:str="Error",colour=False) -> None:
     """Display a message to a user that shows an error. background red."""
     selected = True
     x,y = os.get_terminal_size()
     ox = 0
     if colour:
         BGCL = cp.RED
     else:
```

