# Comparing `tmp/qvsed-1.5.9.tar.gz` & `tmp/qvsed-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.9.tar", last modified: Fri Jul 14 21:20:16 2023, max compression
+gzip compressed data, was "qvsed-1.6.0.tar", last modified: Fri Jul 14 22:31:14 2023, max compression
```

## Comparing `qvsed-1.5.9.tar` & `qvsed-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.071239 qvsed-1.5.9/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.9/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-14 21:20:16.071239 qvsed-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.041498 qvsed-1.5.9/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.9/qvsed/__init__.py
--rw-rw-rw-   0        0        0      787 2023-07-14 16:23:39.000000 qvsed-1.5.9/qvsed/config_default.py
--rw-rw-rw-   0        0        0    28046 2023-07-14 21:19:41.000000 qvsed-1.5.9/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.9/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.9/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.071239 qvsed-1.5.9/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 21:20:16.071239 qvsed-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-14 21:19:57.000000 qvsed-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.309876 qvsed-1.6.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.6.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-14 22:31:14.309876 qvsed-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.283219 qvsed-1.6.0/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.6.0/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-07-14 22:10:14.000000 qvsed-1.6.0/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    30654 2023-07-14 22:30:09.000000 qvsed-1.6.0/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7852 2023-07-14 22:26:54.000000 qvsed-1.6.0/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.6.0/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-14 22:31:14.307667 qvsed-1.6.0/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 22:31:14.000000 qvsed-1.6.0/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 22:31:14.309876 qvsed-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-14 22:30:56.000000 qvsed-1.6.0/setup.py
```

### Comparing `qvsed-1.5.9/LICENSE.txt` & `qvsed-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.9/PKG-INFO` & `qvsed-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.9
+Version: 1.6.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.9/README.md` & `qvsed-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.9/qvsed/qvsed.py` & `qvsed-1.6.0/qvsed/qvsed.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,27 +61,38 @@
         self.load_ui_file()
         self.focus_text_area()
         self.install_event_filter()
         self.set_text_area_encoding("UTF-8")
         self.set_up_text_area_handlers()
         self.set_up_action_deck()
         self.load_config()
-        self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
+        if self.echoArea.text() == "":
+            self.echo_area_update(f"Welcome to QVSED v{self.get_qvsed_version()}!")
         self.set_up_fonts()
         if self.check_if_file_parameter():
             self.load_from_file(sys.argv[1])
 
-    def apply_style_sheet(self, text_color, background_color, button_color, button_text_color,
-                            button_hover_color, button_pressed_color, text_area_color,
-                            text_area_text_color, echo_area_color, echo_area_text_color,
-                            scroll_bar_color, scroll_bar_background_color, scroll_bar_hover_color,
-                            scroll_bar_pressed_color):
+    def apply_style_sheet(self, colours):
         """
         Generate and apply a style sheet based on the config.py file.
         """
+        text_color = colours['text_color']
+        background_color = colours['background_color']
+        button_color = colours['button_color']
+        button_text_color = colours['button_text_color']
+        button_hover_color = colours['button_hover_color']
+        button_pressed_color = colours['button_pressed_color']
+        text_area_color = colours['text_area_color']
+        text_area_text_color = colours['text_area_text_color']
+        echo_area_color = colours['echo_area_color']
+        echo_area_text_color = colours['echo_area_text_color']
+        scroll_bar_color = colours['scroll_bar_color']
+        scroll_bar_background_color = colours['scroll_bar_background_color']
+        scroll_bar_hover_color = colours['scroll_bar_hover_color']
+        scroll_bar_pressed_color = colours['scroll_bar_pressed_color']
 
         stylesheet = f"""
 QMainWindow, QDialog {{
     color: {text_color};
     background: {background_color};
 }}
 
@@ -302,17 +313,17 @@
 
         Used to handle incorrect key combinations.
         """
         text_area = self.textArea
         self.keyPressFilter = KeyPressFilter(self)
         text_area.installEventFilter(self.keyPressFilter)
 
-    def load_config(self):
+    def load_config_file(self):
         """
-        Load the configuration for QVSED.
+        Load the configuration file for QVSED.
         """
         if os.name == "nt":  # Windows
             user_config_dir = os.path.join(os.environ["APPDATA"], "QVSED")
         else:  # *nix
             user_config_dir = os.path.expanduser("~") + "/.config/QVSED"
 
         user_config_file = os.path.join(user_config_dir, "config.py")
@@ -320,47 +331,102 @@
         if not os.path.isfile(user_config_file):
             self.generate_config()
 
         spec = importlib.util.spec_from_file_location("qvsed_config", user_config_file)
         qvsed_config = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(qvsed_config)
 
+        return qvsed_config
+
+    def extract_color_values(self, qvsed_config):
+        """
+        Extract the colour values from the configuration file.
+        """
+        colors = getattr(qvsed_config, 'colors', None)
+
+        if colors is not None:
+            # New-style config file
+            text_color = colors['window']['text']
+            background_color = colors['window']['background']
+
+            button_text_color = colors['button']['text']
+            button_color = colors['button']['background']
+            button_hover_color = colors['button']['hover']
+            button_pressed_color = colors['button']['pressed']
+
+            text_area_text_color = colors['text_area']['text']
+            text_area_color = colors['text_area']['background']
+
+            echo_area_text_color = colors['echo_area']['text']
+            echo_area_color = colors['echo_area']['background']
+
+            scroll_bar_color = colors['scroll_bar']['text']
+            scroll_bar_background_color = colors['scroll_bar']['background']
+            scroll_bar_hover_color = colors['scroll_bar']['hover']
+            scroll_bar_pressed_color = colors['scroll_bar']['pressed']
+        else:
+            # Old-style config file
+            self.echo_area_update("Warning: config.py is using old-style colour definitions")
+
+            text_color = getattr(qvsed_config, 'text_color', None)
+            background_color = getattr(qvsed_config, 'background_color', None)
+
+            button_text_color = getattr(qvsed_config, 'button_text_color', text_color)
+            button_color = getattr(qvsed_config, 'button_color', None)
+            button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
+            button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
+
+            text_area_text_color = getattr(qvsed_config, 'text_area_text_color', text_color)
+            text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
+
+            echo_area_text_color = getattr(qvsed_config, 'echo_area_text_color', text_color)
+            echo_area_color = getattr(qvsed_config, 'echo_area_color', text_area_color)
+
+            scroll_bar_color = getattr(qvsed_config, 'scroll_bar_color', button_color)
+            scroll_bar_background_color = getattr(qvsed_config, 'scroll_bar_background_color', button_hover_color)
+            scroll_bar_hover_color = getattr(qvsed_config, 'scroll_bar_hover_color', button_pressed_color)
+            scroll_bar_pressed_color = getattr(qvsed_config, 'scroll_bar_pressed_color', button_pressed_color)
+
+        colours = {
+                'text_color': text_color,
+                'background_color': background_color,
+                'button_color': button_color,
+                'button_text_color': button_text_color,
+                'button_hover_color': button_hover_color,
+                'button_pressed_color': button_pressed_color,
+                'text_area_color': text_area_color,
+                'text_area_text_color': text_area_text_color,
+                'echo_area_color': echo_area_color,
+                'echo_area_text_color': echo_area_text_color,
+                'scroll_bar_color': scroll_bar_color,
+                'scroll_bar_background_color': scroll_bar_background_color,
+                'scroll_bar_hover_color': scroll_bar_hover_color,
+                'scroll_bar_pressed_color': scroll_bar_pressed_color
+        }
+
+        return colours
+
+    def load_config(self):
+        """
+        Load the configuration for QVSED.
+        """
+        self.echo_area_timeout = 3000
+        qvsed_config = self.load_config_file()
+
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
         self.tab_stop_width = getattr(qvsed_config, 'tab_stop_width', 4)
-
         self.echo_area_timeout = getattr(qvsed_config, 'echo_area_timeout', 3000)
 
         # Load the colour scheme settings from the config file
-        # We use the shorter American spellings because it's standard, I guess
-        text_color = getattr(qvsed_config, 'text_color', None)
-        background_color = getattr(qvsed_config, 'background_color', None)
-
-        button_color = getattr(qvsed_config, 'button_color', None)
-        button_text_color = getattr(qvsed_config, 'button_text_color', text_color)
-        button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
-        button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
-
-        text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
-        text_area_text_color = getattr(qvsed_config, 'text_area_text_color', text_color)
-        echo_area_color = getattr(qvsed_config, 'echo_area_color', text_area_color)
-        echo_area_text_color = getattr(qvsed_config, 'echo_area_text_color', text_color)
-
-        scroll_bar_color = getattr(qvsed_config, 'scroll_bar_color', button_color)
-        scroll_bar_background_color = getattr(qvsed_config, 'scroll_bar_background_color', button_hover_color)
-        scroll_bar_hover_color = getattr(qvsed_config, 'scroll_bar_hover_color', button_pressed_color)
-        scroll_bar_pressed_color = getattr(qvsed_config, 'scroll_bar_pressed_color', button_pressed_color)
-
-        self.apply_style_sheet(text_color, background_color, button_color, button_text_color,
-                               button_hover_color, button_pressed_color, text_area_color,
-                               text_area_text_color, echo_area_color, echo_area_text_color,
-                               scroll_bar_color, scroll_bar_background_color, scroll_bar_hover_color,
-                               scroll_bar_pressed_color)
+        colours = self.extract_color_values(qvsed_config)
+
+        self.apply_style_sheet(colours)
 
-        if None in (text_color, background_color, button_color, button_hover_color):
+        if None in (colours['text_color'], colours['background_color'], colours['button_color'], colours['button_hover_color']):
             self.echo_area_update("config.py appears to be broken, generating a new one.")
             self.generate_config()
 
     def load_from_file(self, file_path=None):
         """
         Open a file dialog, and load the contents of a file into the Text Area.
         """
```

### Comparing `qvsed-1.5.9/qvsed/qvsed.ui` & `qvsed-1.6.0/qvsed/qvsed.ui`

 * *Files 0% similar despite different names*

#### Comparing `qvsed-1.5.9/qvsed/qvsed.ui` & `qvsed-1.6.0/qvsed/qvsed.ui`

```diff
@@ -249,17 +249,14 @@
             <item>
               <widget class="QLineEdit" name="echoArea">
                 <property name="font">
                   <font>
                     <pointsize>11</pointsize>
                   </font>
                 </property>
-                <property name="text">
-                  <string>Welcome to QVSED!</string>
-                </property>
                 <property name="cursorPosition">
                   <number>0</number>
                 </property>
                 <property name="readOnly">
                   <bool>true</bool>
                 </property>
               </widget>
```

### Comparing `qvsed-1.5.9/qvsed/qvsed_dialog.ui` & `qvsed-1.6.0/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.9/qvsed.egg-info/PKG-INFO` & `qvsed-1.6.0/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.9
+Version: 1.6.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.9/setup.py` & `qvsed-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.9',
+    version='1.6.0',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

