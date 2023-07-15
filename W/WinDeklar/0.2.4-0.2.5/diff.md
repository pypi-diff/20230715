# Comparing `tmp/windeklar-0.2.4.tar.gz` & `tmp/windeklar-0.2.5.tar.gz`

## Comparing `windeklar-0.2.4.tar` & `windeklar-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.4/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.4/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/__init__.py
--rwxr-xr-x   0        0        0    16073 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.4/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.4/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.4/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.5/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/__init__.py
+-rwxr-xr-x   0        0        0    16215 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    45955 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.5/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 windeklar-0.2.5/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 windeklar-0.2.5/PKG-INFO
```

### Comparing `windeklar-0.2.4/.github/workflows/python-publish.yml` & `windeklar-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/QTAux.py` & `windeklar-0.2.5/src/WinDeklar/QTAux.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,19 @@
         self.ename = new_ename
 
     def set_fixed_width(self, width):
         _, widget = self.get_widget()
         if widget is not None:
             widget.setFixedWidth(width)
 
+    def set_visible(self, is_visible):
+        valid, widget = self.get_widget()
+        if valid:
+            widget.setVisible(is_visible)
+
 
 class EnumCombo(ScreenControl):
     def __init__(self, name, title, bound, enum, action, layout, tooltip=None):
     
         self.enum  = enum
         self.combo = QtWidgets.QComboBox(None)
         for member in self.enum:
```

### Comparing `windeklar-0.2.4/src/WinDeklar/WindowForm.py` & `windeklar-0.2.5/src/WinDeklar/WindowForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,16 +562,15 @@
             return None
         return self.main_window.get_control_by_name(name)
 
     def get_control_value(self, name):
         if name in self.state:
             return self.state[name]
         else:
-            value = self.calculated_value(name)
-            return value if value is not None else 0
+            return self.calculated_value(name)
 
     def control_has_value(self, name):
         return name in self.state
 
     def controls_def(self):
         # abstract method
         return []
@@ -725,16 +724,21 @@
     def on_mouse_move(self, event, ax):
         # abstract method
         # print('%s click: button=%d, x=%d, y=%d, xdata=%f, ydata=%f' %
         #      ('double' if event.dblclick else 'single', event.button, event.x, event.y, event.xdata, event.ydata))
         return False
 
     def calculated_value(self, name):
+        """
+        Abstract method, used to return a value that is a formula of other values
+        :param name:
+        :return:
+        """
         # abstract method
-        return None
+        return 0.0
 
     def save_cycle(self):
         """
         Save the info of a given cycle
         Note: it is directly called from an event in the UI (as defined in a yaml config file)
         :return:
         """
```

### Comparing `windeklar-0.2.4/src/WinDeklar/graph_aux.py` & `windeklar-0.2.5/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/points_box.py` & `windeklar-0.2.5/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/record.py` & `windeklar-0.2.5/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/signal_aux.py` & `windeklar-0.2.5/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/test_animation.py` & `windeklar-0.2.5/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.5/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/view_animation.py` & `windeklar-0.2.5/src/WinDeklar/view_animation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import WinDeklar.QTAux as QTAux
 import WinDeklar.WindowForm as WinForm
 import WinDeklar.graph_aux as ga
 
 
 class ExampleHost(WinForm.HostModel):
     """
-    Shows tentacles
+    Shows a two animated graphs
     """
 
     def __init__(self, function1=np.sin, function2=np.cos, color='Blue', y_bounds=(-1.2, 1.2)):
         # keys (names used in the yaml definition file)
         self.start_stop_key        = 'start_stop'
         self.start_stop_action_key = 'start_stop_action'
         self.graph1_key = 'graph1'
```

### Comparing `windeklar-0.2.4/src/WinDeklar/view_animation.yaml` & `windeklar-0.2.5/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/view_example.py` & `windeklar-0.2.5/src/WinDeklar/view_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         * Toolbar
         * Many kinds of controls (Slider, Combo, Check, Button, etc.)
         * Mouse move
     """
 
     def __init__(self, default_directory='/tmp', file_extension='yaml'):
         # keys (names used in the yaml definition file)
-        self.check1_key = 'check1'
         self.points_key = 'points'
         self.axis_key   = 'show_axis'
         self.type_key   = 'graph_type'
         self.action_key = 'action'
         self.width_key  = 'line_width'
         self.graph1_key = 'graph1'
         self.graph2_key = 'graph2'
@@ -78,14 +77,23 @@
     def redraw(self):
         """
         Event defined in the yaml file to be called when button redraw is pressed
         :return:
         """
         self.refresh()
 
+    def initialize(self):
+        """
+        Code to run when initializing the form
+        In this case it is shown how to set visible (or not) a control
+        :return:
+        """
+        control = self.get_control_by_name('just_text')
+        control.set_visible(True)
+
     # actions
     def event_open_file(self):
         """
         Event defined in the yaml file to be called when File/Open is clicked
         :return:
         """
         file_name = self.get_file_name(title='Open an YAML', file_filter=self.file_filter, directory=self.directory)
```

### Comparing `windeklar-0.2.4/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.5/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.5/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/LICENSE` & `windeklar-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.4/README.md` & `windeklar-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+Metadata-Version: 2.1
+Name: WinDeklar
+Version: 0.2.5
+Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
+Project-URL: Homepage, https://github.com/njodal/WinDeklar
+Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
+Author-email: Nicolas Jodal <jnj@genexus.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Description
 A simple, declarative oriented framework to create WinForms in Python.
 
 While it can be used for all kinds of forms, it was created with the purpose of being applied in Robotics, where the need to visualize complex algorithms and, above all, observe the effect of parameter changes is very common.
 
 The forms are defined in a declarative way in an YAML (layouts, controls, toolbar, menus, etc.) and used in a Python program with just a few lines of code.
 
 # How to use it
-The best way to learn how to use it is just take a look at the code.
+To create a WinForm it is necessary to create two files:
+* a declaration file (*.yaml) that define the WinForm (menu bar, toolbar, layouts, controls, etc.)
+* a python file (with the same name) that handles all the WinForm logic (events, drawing, etc.)
 
 For a complete form see `view_example.yaml` to understand how the form is defined and `view_example.py` how it is used.
 
 If you run `python view_example.py` the form is: 
 
 <img width="997" alt="winform_example" src="https://github.com/njodal/WIndow_form/assets/28706901/ab02ce1f-9409-454d-8d95-e130fe6d77ed">
 
 In case a simple graph is needed look at `view_simple_graph.py`.
 # Examples
 
-## Form used to tune a PID controller for control a model car
-
-<img width="1003" alt="PID tuning" src="https://github.com/njodal/WIndow_form/assets/28706901/c978edfc-808b-47d4-993c-22d00b7fd154">
-
+## Form used to visualize a PID controller for control the speed of a car
 
+<img width="999" alt="Screen Shot 2023-07-12 at 6 22 05 PM" src="https://github.com/njodal/WinDeklar/assets/28706901/93859f05-f9b6-4333-a451-34f5c302f8c1">
```

### Comparing `windeklar-0.2.4/pyproject.toml` & `windeklar-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

