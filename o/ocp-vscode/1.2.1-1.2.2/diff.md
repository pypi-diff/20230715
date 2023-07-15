# Comparing `tmp/ocp_vscode-1.2.1.tar.gz` & `tmp/ocp_vscode-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.2.1.tar", last modified: Sun Jul  2 18:27:51 2023, max compression
+gzip compressed data, was "ocp_vscode-1.2.2.tar", last modified: Sat Jul 15 12:19:34 2023, max compression
```

## Comparing `ocp_vscode-1.2.1.tar` & `ocp_vscode-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.992004 ocp_vscode-1.2.1/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.2.1/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 18:27:51.992058 ocp_vscode-1.2.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     9831 2023-07-02 18:26:46.000000 ocp_vscode-1.2.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.991124 ocp_vscode-1.2.1/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.2.1/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10270 2023-07-01 11:38:14.000000 ocp_vscode-1.2.1/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.2.1/ocp_vscode/finder.py
--rw-r--r--   0 bernhard   (501) staff       (20)    25004 2023-07-02 08:06:35.000000 ocp_vscode-1.2.1/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.991885 ocp_vscode-1.2.1/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-07-02 18:27:51.992310 ocp_vscode-1.2.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-07-02 18:26:46.000000 ocp_vscode-1.2.1/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-15 12:19:34.739901 ocp_vscode-1.2.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.2.2/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-15 12:19:34.739982 ocp_vscode-1.2.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     9939 2023-07-15 10:08:52.000000 ocp_vscode-1.2.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-15 12:19:34.739033 ocp_vscode-1.2.2/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.2.2/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.2.2/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.2.2/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.2.2/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12626 2023-07-15 09:09:46.000000 ocp_vscode-1.2.2/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4429 2023-07-13 06:08:05.000000 ocp_vscode-1.2.2/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    26526 2023-07-15 10:23:55.000000 ocp_vscode-1.2.2/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-15 12:19:34.739783 ocp_vscode-1.2.2/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-07-15 12:19:34.000000 ocp_vscode-1.2.2/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-07-15 12:19:34.740424 ocp_vscode-1.2.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-07-14 16:29:53.000000 ocp_vscode-1.2.2/setup.py
```

### Comparing `ocp_vscode-1.2.1/LICENSE` & `ocp_vscode-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.1/PKG-INFO` & `ocp_vscode-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 1.2.1
+Version: 1.2.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.2.1/README.md` & `ocp_vscode-1.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ### Breaking changes from v1.0.0
 
 -   IPython and the ipython extensions are not supported any more out of the box. Instead the Microsoft's Jupyter extension with ipykernel is supported. If you have the installation configs in your local VS Code settings.json file, you might want to remove the ipython installation commands.
 -   For the color maps, `CM` is replaced by `ColorMap` (to resolve the conflict with build123d `CM`)
 
 ### Installation
 
-1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.2.1_.
+1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.2.2_.
 
     Afterwards the OCP viewer is available in the VS Code sidebar:
 
     ![](screenshots/ocp_icon.png)
 
 2. Clicking on it shows the OCP CAD Viewer UI:
 
@@ -162,38 +162,28 @@
 
         show_all()
         # %%
         ```
 
         ![named contexts](./screenshots/context_vars.png)
 
+-   **Keep camera orientation** of an object with `reset_camera`
+
+    Sometimes it is helpful to keep the orientation of an object across code changes. This is what `reset_camera` does:
+
+    -   `reset_camera=Camera.Center` will keep position and rotation, but ignore panning. This means the new object will be repositioned to the center (most robust approach)
+    -   `reset_camera=Camera.KEEP` will keep position, rotation and panning. However, panning can be problematic. When the next object to be shown is much larger or smaller and the object before was panned, it can happen that nothing is visible (the new object at the pan location is outside of the viewer frustum). OCP CAD Viewer checks whether the bounding box of an object is 2x smaller or larger than the one of the last shown object. If so, it falls back to `Camera.CENTER`. A notification is written to the OCP CAD Viewer output panel.
+    -   `reset_camera=Camera.RESET` will ensure that position, rotation and panning will be reset to the initial default
+
 ## Changes
 
-v1.2.1
+v1.2.2
+
+-   Replace the boolean values for `reset_camera` with the `Camera` enum; `reset_camera` now supports `Camera.RESET` (works like `True` before), `Camera.CENTER` (works like `False` before) and `Camera.KEEP` (additionally keeps the pan location). See best practices for details.
+-   Replace the values for `collapse` with the `Collapse` enum: `Collapse.ALL` (was `"C"`), `Collapse.None` (was `"E"`), `Collapse.LEAVES` (was `"1"` or `1`) and `Collapse.Root` (was `"R"`)
+-   Added a button to toggle the output panel for OCP CAD Viewer
+-   Visual debug is on by default now (workspace setting `WatchByDefault` to `true`)
+-   Changed behavior of ` show` during debug session: `show` will be executed, however, visual debug step omitted
+-   Do not show Jupyter variables `_`, `__`, `_1`, `_2`, ... in `show_all`
+-   Fix an error where the orientation marker was partly or fully moved outside its view due to panning of the object ([vscode-ocp-cad-viewer issue #22](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/22))
 
--   XYZ labels for orientation marker ([vscode-ocp-cad-viewer issue #13](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/13))
--   Support for metalness and roughness ([three-cad-viewer issue #9](https://github.com/bernhard-42/three-cad-viewer/issues/9))
--   New "Material" configurator tab in the viewer UI
--   Fix: OCP_Part can be shown now ([vscode-ocp-cad-viewer issue #20](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/20))
--   Fix: reset_camera respects panning ([vscode-ocp-cad-viewer issue #19](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/19))
--   Fix: `collapse="C"` also collapses single item trees ([vscode-ocp-cad-viewer issue #18](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/18))
--   Fix: Show_all supports having a sketch that uses face as a workplane ([vscode-ocp-cad-viewer issue #17](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/17))
--   Fix: `_config==undefined` is handled properly ([vscode-ocp-cad-viewer issue #12](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/12))
-
-v1.1.3
-
--   Fix racing conditions that prevented having more than one viewer window
--   No need to add port for next viewer any more. The default port 3939 will be incremented until a free port is found
--   Use ocp-tessellate 1.1.1 (fixes axis helper scale)
-
-v1.1.2
-
--   Added Visual debugging (including a toggle switch in the status bar)
--   Added function `show_all` and `show_clear` for the visual debugging
--   New (opinonated) Quickstart modes to install ever for build123d or CadQury with one click
--   Websocket communication between Python and the VS Code extension
--   Remove IPython support and introduce Jupyter / ipykernel support
--   Rename ColorMap to BaseColorMap and CM to ColorMap
--   Check versions of the viewer and the Pyhton module ocp_vscode are the same at OCP Viewer start
--   Support OCCT Shells
--   Bump three-cad-viewer 1.7.12
--   Fix two race conditions at viewer start (missing awaits)
+full change log see [Changes.md](./Changes.md)
```

### Comparing `ocp_vscode-1.2.1/ocp_vscode/__init__.py` & `ocp_vscode-1.2.2/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.1/ocp_vscode/animation.py` & `ocp_vscode-1.2.2/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.1/ocp_vscode/colors.py` & `ocp_vscode-1.2.2/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.1/ocp_vscode/comms.py` & `ocp_vscode-1.2.2/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.1/ocp_vscode/config.py` & `ocp_vscode-1.2.2/ocp_vscode/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,27 +10,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from enum import Enum
+
 from .comms import send_command, send_data, get_port
 
 __all__ = [
     "workspace_config",
     "combined_config",
     "set_viewer_config",
     "set_defaults",
     "reset_defaults",
     "get_default",
     "get_defaults",
     "status",
+    "Camera",
+    "Collapse",
+    "check_deprecated",
 ]
 
+
+class Camera(Enum):
+    RESET = "reset"
+    CENTER = "center"
+    KEEP = "keep"
+
+
+class Collapse(Enum):
+    NONE = 0
+    LEAVES = 1
+    ALL = 2
+    ROOT = 3
+
+
 CONFIG_UI_KEYS = [
     "axes",
     "axes0",
     "black_edges",
     "grid",
     "ortho",
     "transparent",
@@ -101,29 +120,28 @@
     "ambient_intensity",
     "direct_intensity",
     "metalness",
     "roughness",
     "zoom_speed",
     "pan_speed",
     "rotate_speed",
-    "reset_camera",
     "glass",
     "tools",
     "tree_width",
     "collapse",
 ]
 
 DEFAULTS = {
     "render_edges": True,
     "render_normals": False,
     "render_mates": False,
     "render_joints": False,
     "helper_scale": 1.0,
     "timeit": False,
-    "reset_camera": True,
+    "reset_camera": Camera.RESET,
     "debug": False,
 }
 
 
 def set_viewer_config(
     axes=None,
     axes0=None,
@@ -219,26 +237,31 @@
         axes0:             Show axes at (0,0,0) (default=False)
         grid:              Show grid (default=False)
         ortho:             Use orthographic projections (default=True)
         transparent:       Show objects transparent (default=False)
         default_opacity:   Opacity value for transparent objects (default=0.5)
         black_edges:       Show edges in black color (default=False)
         orbit_control:     Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:          1: collapse all single leaf nodes, R: expand root only,
-                           C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:          Collapse.LEAVES: collapse all single leaf nodes,
+                           Collapse.ROOT: expand root only,
+                           Collapse.ALL: collapse all nodes,
+                           Collapse.NONE: expand all nodes
+                           (default=Collapse.LEAVES)
         ticks:             Hint for the number of ticks in both directions (default=10)
         up:                Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
         explode:           Turn on explode mode (default=False)
 
         zoom:              Zoom factor of view (default=1.0)
         position:          Camera position
         quaternion:        Camera orientation as quaternion
         target:            Camera look at target
-        reset_camera:      Reset camera position, rotation and zoom to default (default=True)
-
+        reset_camera:      Camera.RESET: Reset camera position, rotation, toom and target
+                           Camera.CENTER: Keep camera position, rotation, toom, but look at center
+                           Camera.KEEP: Keep camera position, rotation, toom, and target
+                           (default=Camera.RESET)
         pan_speed:         Speed of mouse panning (default=1)
         rotate_speed:      Speed of mouse rotate (default=1)
         zoom_speed:        Speed of mouse zoom (default=1)
 
     - Renderer
         deviation:         Shapes: Deviation from linear deflection value (default=0.1)
         angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
@@ -260,18 +283,15 @@
     - Debug
         debug:             Show debug statements to the VS Code browser console (default=False)
         timeit:            Show timing information from level 0-3 (default=False)
     """
 
     kwargs = {k: v for k, v in locals().items() if v is not None}
 
-    if kwargs.get("mate_scale") is not None:
-        print("\nmate_scale is deprecated, use helper_scale instead\n")
-        kwargs["helper_scale"] = kwargs["mate_scale"]
-        del kwargs["mate_scale"]
+    kwargs = check_deprecated(kwargs)
 
     global DEFAULTS
     for key, value in kwargs.items():
         if key in CONFIG_KEYS:
             DEFAULTS[key] = value
         else:
             print(f"'{key}' is an unkown config, ignored!")
@@ -303,15 +323,27 @@
         )
 
 
 def workspace_config(port=None):
     if port is None:
         port = get_port()
     try:
-        return send_command("config", port=port)
+        conf = send_command("config", port=port)
+        mapping = {
+            "none": Collapse.NONE,
+            "leaves": Collapse.LEAVES,
+            "all": Collapse.ALL,
+            "root": Collapse.ROOT,
+            "E": Collapse.NONE,
+            "1": Collapse.LEAVES,
+            "C": Collapse.ALL,
+            "R": Collapse.ROOT,
+        }
+        conf["collapse"] = mapping[conf["collapse"]]
+        return conf
 
     except Exception as ex:
         raise RuntimeError(
             "Cannot access viewer config. Is the viewer running?\n" + str(ex.args)
         )
 
 
@@ -339,39 +371,85 @@
 
     wspace_config.update(DEFAULTS)
     if use_status:
         wspace_config.update(ui_filter(wspace_status))
     return wspace_config
 
 
-def get_changed_config(key):
+def get_changed_config(key=None):
     wspace_config = workspace_config()
     wspace_config.update(DEFAULTS)
-    return wspace_config.get(key)
+    if key is None:
+        return wspace_config
+    else:
+        return wspace_config.get(key)
 
 
 def reset_defaults():
     """Reset defaults not given in workspace config"""
     global DEFAULTS
 
     config = {
         key: value
         for key, value in workspace_config().items()
         if key in CONFIG_SET_KEYS
     }
-    config["reset_camera"] = True
+    config["reset_camera"] = Camera.RESET
 
     set_viewer_config(**config)
 
     if config.get("transparent") is not None:
         set_viewer_config(transparent=config["transparent"])
 
     DEFAULTS = {
         "render_edges": True,
         "render_normals": False,
         "render_mates": False,
         "render_joints": False,
         "helper_scale": 1.0,
         "timeit": False,
-        "reset_camera": True,
+        "reset_camera": Camera.RESET,
         "debug": False,
     }
+
+
+def check_deprecated(kwargs):
+    if kwargs.get("mate_scale") is not None:
+        print("\nmate_scale is deprecated, use helper_scale instead\n")
+        kwargs["helper_scale"] = kwargs["mate_scale"]
+        del kwargs["mate_scale"]
+
+    if kwargs.get("reset_camera") == True:
+        print(
+            "\n'reset_camera=True' is deprecated, use 'reset_camera=Camera.RESET' instead\n"
+        )
+        kwargs["reset_camera"] = Camera.RESET
+
+    if kwargs.get("reset_camera") == False:
+        print(
+            "\n'reset_camera=False' is deprecated, use 'reset_camera=Camera.CENTER' instead\n"
+        )
+        kwargs["reset_camera"] = Camera.CENTER
+
+    if kwargs.get("collapse") == "C":
+        print("\n'collapse=\"C\"' is deprecated, use 'collapse=Collapse.ALL' instead\n")
+        kwargs["collapse"] = Collapse.ALL
+
+    if kwargs.get("collapse") == "1" or kwargs.get("collapse") == 1:
+        print(
+            "\n'collapse=\"1\"' is deprecated, use 'collapse=Collapse.LEAVES' instead\n"
+        )
+        kwargs["collapse"] = Collapse.LEAVES
+
+    if kwargs.get("collapse") == "R":
+        print(
+            "\n'collapse=\"R\"' is deprecated, use 'collapse=Collapse.ROOT' instead\n"
+        )
+        kwargs["collapse"] = Collapse.ROOT
+
+    if kwargs.get("collapse") == "E":
+        print(
+            "\n'collapse=\"E\"' is deprecated, use 'collapse=Collapse.NONE' instead\n"
+        )
+        kwargs["collapse"] = Collapse.NONE
+
+    return kwargs
```

### Comparing `ocp_vscode-1.2.1/ocp_vscode/finder.py` & `ocp_vscode-1.2.2/ocp_vscode/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from build123d import *
 from ocp_vscode import *
 
 
 class Finder:
     def __init__(self, obj, colormap=CM.tab20()):
         self.obj = obj
@@ -50,15 +51,15 @@
         faces = self.obj.faces().group_by(axis)
         show(
             *faces,
             names=[str(i) for i in range(len(faces))],
             colors=self.colormap,
             default_opacity=0.9,
             progress="",
-            collapse="C",
+            collapse=Collapse.ALL,
             show_parent=False,
         )
         while True:
             try:
                 time.sleep(0.5)
                 new_pick = status()["lastPick"]
                 if pick["name"] != new_pick["name"]:
@@ -86,16 +87,15 @@
             if edge in face.edges():
                 result.append(face)
         show(*result, edge)
         return edge, result
 
 
 # %%
-if __name__ =0 "__main__":
-
+if __name__ == "__main__":
     a = 55 / 2
     c100 = Circle(100).edges()[0]
     c85 = Circle(85).edges()[0]
 
     lines = []
     vertices = []
     for sign in (1, -1):
```

### Comparing `ocp_vscode-1.2.1/ocp_vscode/show.py` & `ocp_vscode-1.2.2/ocp_vscode/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import re
 import sys
 from ocp_tessellate import PartGroup
 from ocp_tessellate.convert import (
     tessellate_group,
     get_normal_len,
     combined_bb,
     to_assembly,
@@ -52,30 +53,47 @@
     preset,
     get_changed_config,
     workspace_config,
     combined_config,
     get_default,
     status,
     set_viewer_config,
+    Camera,
+    Collapse,
+    check_deprecated,
 )
 from .comms import send_data, MessageType
 from .colors import *
 
 __all__ = ["show", "show_object", "reset_show", "show_all", "show_clear"]
 
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
+FIRST_CALL = True
+LAST_CALL = "other"
+
 
 def _tessellate(
     *cad_objs, names=None, colors=None, alphas=None, progress=None, **kwargs
 ):
+    global FIRST_CALL
+
     if workspace_config().get("_splash"):
         conf = combined_config(use_status=False)
     else:
         conf = combined_config(use_status=True)
+        if FIRST_CALL:
+            conf["reset_camera"] = Camera.RESET.value
+            FIRST_CALL = False
+        else:
+            reset_camera = conf.get("reset_camera", Camera.RESET)
+            conf["reset_camera"] = reset_camera.value
+
+    collapse = conf.get("collapse", Collapse.LEAVES)
+    conf["collapse"] = collapse.value
 
     if kwargs.get("default_facecolor") is not None:
         oc.FACE_COLOR = Color(kwargs["default_facecolor"]).percentage
         del kwargs["default_facecolor"]
     else:
         oc.FACE_COLOR = Color(conf["default_facecolor"]).percentage
 
@@ -96,28 +114,29 @@
     if timeit is None:
         timeit = False
 
     if progress is None:
         progress = Progress([c for c in "-+c"])
 
     with Timer(timeit, "", "to_assembly", 1):
+        changed_config = get_changed_config()
         part_group = to_assembly(
             *cad_objs,
             names=names,
             colors=colors,
             alphas=alphas,
-            render_mates=kwargs.get("render_mates", get_changed_config("render_mates")),
+            render_mates=kwargs.get("render_mates", changed_config.get("render_mates")),
             render_joints=kwargs.get(
-                "render_joints", get_changed_config("render_joints")
+                "render_joints", changed_config.get("render_joints")
             ),
-            helper_scale=kwargs.get("helper_scale", get_changed_config("helper_scale")),
+            helper_scale=kwargs.get("helper_scale", changed_config.get("helper_scale")),
             default_color=kwargs.get(
-                "default_color", get_changed_config("default_color")
+                "default_color", changed_config.get("default_color")
             ),
-            show_parent=kwargs.get("show_parent", get_changed_config("show_parent")),
+            show_parent=kwargs.get("show_parent", changed_config.get("show_parent")),
             progress=progress,
         )
 
         if len(part_group.objects) == 1 and isinstance(
             part_group.objects[0], PartGroup
         ):
             part_group = part_group.objects[0]
@@ -206,17 +225,14 @@
         progress=progress,
         **kwargs,
     )
     if config.get("dark") is not None:
         config["theme"] = "dark"
     elif config.get("orbit_control") is not None:
         config["control"] = "orbit" if config["control"] else "trackball"
-    elif config.get("collapse") is not None:
-        mapping = {"1": 1, "E": 0, "C": 2, "R": 3}
-        config["collapse"] = mapping.get(config["collapse"], 1)
 
     if config.get("debug") is not None and config["debug"]:
         print("\nconfig:\n", config)
 
     if kwargs.get("explode") is not None:
         config["explode"] = kwargs["explode"]
 
@@ -335,25 +351,31 @@
         axes0:                   Show axes at (0,0,0) (default=False)
         grid:                    Show grid (default=False)
         ortho:                   Use orthographic projections (default=True)
         transparent:             Show objects transparent (default=False)
         default_opacity:         Opacity value for transparent objects (default=0.5)
         black_edges:             Show edges in black color (default=False)
         orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:                1: collapse all single leaf nodes, R: expand root only,
-                                 C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:                Collapse.LEAVES: collapse all single leaf nodes,
+                                 Collapse.ROOT: expand root only,
+                                 Collapse.ALL: collapse all nodes,
+                                 Collapse.NONE: expand all nodes
+                                 (default=Collapse.LEAVES)
         ticks:                   Hint for the number of ticks in both directions (default=10)
         up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
         explode:                 Turn on explode mode (default=False)
 
         zoom:                    Zoom factor of view (default=1.0)
         position:                Camera position
         quaternion:              Camera orientation as quaternion
         target:                  Camera look at target
-        reset_camera:            Reset camera position, rotation and zoom to default (default=True)
+        reset_camera:            Camera.RESET: Reset camera position, rotation, toom and target
+                                 Camera.CENTER: Keep camera position, rotation, toom, but look at center
+                                 Camera.KEEP: Keep camera position, rotation, toom, and target
+                                 (default=Camera.RESET)
 
         pan_speed:               Speed of mouse panning (default=1)
         rotate_speed:            Speed of mouse rotate (default=1)
         zoom_speed:              Speed of mouse zoom (default=1)
 
     - Renderer
         deviation:               Shapes: Deviation from linear deflection value (default=0.1)
@@ -378,37 +400,37 @@
         show_parent:             Render parent of faces, edges or vertices as wireframe
         helper_scale:              Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:                   Show debug statements to the VS Code browser console (default=False)
         timeit:                  Show timing information from level 0-3 (default=False)
     """
-    if sys.gettrace() is not None and not _force_in_debug:
-        print("\nshow and show_object are ignored in debugging sessions\n")
-        return
+    global LAST_CALL
+
+    # if sys.gettrace() is not None and not _force_in_debug:
+    #     print("\nshow and show_object are ignored in debugging sessions\n")
+    #     return
 
     kwargs = {
         k: v
         for k, v in locals().items()
         if v is not None
         and k
         not in [
             "cad_objs",
             "names",
             "colors",
             "alphas",
             "port",
             "progress",
+            "LAST_CALL",
         ]
     }
 
-    if kwargs.get("mate_scale") is not None:
-        print("\nmate_scale is deprecated, use helper_scale instead\n")
-        kwargs["helper_scale"] = kwargs["mate_scale"]
-        del kwargs["mate_scale"]
+    kwargs = check_deprecated(kwargs)
 
     timeit = preset("timeit", timeit)
 
     names = align_attrs(names, len(cad_objs), None, "names", explode=False)
 
     # Handle colormaps
 
@@ -447,14 +469,19 @@
             names=names,
             colors=colors,
             alphas=alphas,
             progress=progress,
             **kwargs,
         )
 
+    if not _force_in_debug:
+        LAST_CALL = "show"
+    else:
+        LAST_CALL = "other"
+
     with Timer(timeit, "", "send"):
         return send_data(data, port=port, timeit=timeit)
 
 
 def reset_show():
     global OBJECTS
 
@@ -541,24 +568,30 @@
         axes0:                   Show axes at (0,0,0) (default=False)
         grid:                    Show grid (default=False)
         ortho:                   Use orthographic projections (default=True)
         transparent:             Show objects transparent (default=False)
         default_opacity:         Opacity value for transparent objects (default=0.5)
         black_edges:             Show edges in black color (default=False)
         orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:                1: collapse all single leaf nodes, R: expand root only,
-                                 C: collapse all nodes, E: expand all nodes (default=1)
+        collapse:                Collapse.LEAVES: collapse all single leaf nodes,
+                                 Collapse.ROOT: expand root only,
+                                 Collapse.ALL: collapse all nodes,
+                                 Collapse.NONE: expand all nodes
+                                 (default=Collapse.LEAVES)
         ticks:                   Hint for the number of ticks in both directions (default=10)
         up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
 
         zoom:                    Zoom factor of view (default=1.0)
         position:                Camera position
         quaternion:              Camera orientation as quaternion
         target:                  Camera look at target
-        reset_camera:            Reset camera position, rotation and zoom to default (default=True)
+        reset_camera:            Camera.RESET: Reset camera position, rotation, toom and target
+                                 Camera.CENTER: Keep camera position, rotation, toom, but look at center
+                                 Camera.KEEP: Keep camera position, rotation, toom, and target
+                                 (default=Camera.RESET)
 
         pan_speed:               Speed of mouse panning (default=1)
         rotate_speed:            Speed of mouse rotate (default=1)
         zoom_speed:              Speed of mouse zoom (default=1)
 
     - Renderer
         deviation:               Shapes: Deviation from linear deflection value (default=0.1)
@@ -630,41 +663,47 @@
         alphas=OBJECTS["alphas"],
         port=port,
         progress=progress,
         **kwargs,
     )
 
 
-first_call = True
-
-
 def show_clear():
     data = {
         "type": "clear",
     }
     send_data(data)
 
 
 def show_all(variables=None, exclude=None, **kwargs):
     import inspect
 
-    global first_call
+    global FIRST_CALL, LAST_CALL
+
+    if LAST_CALL == "show":
+        LAST_CALL = "other"
+        print("\nSkip visual debug step after a show() command")
+        return
 
     if variables is None:
         cf = inspect.currentframe()
         variables = cf.f_back.f_locals
 
     if exclude is None:
         exclude = []
 
     objects = []
     names = []
     for name, obj in variables.items():
-        if isinstance(obj, type):
-            continue  # ignore classes
+        if (
+            isinstance(obj, type)
+            or name in ["_", "__", "___"]
+            or re.search("_\d+", name) is not None
+        ):
+            continue  # ignore classes and jupyter variables
 
         if name not in exclude:
             if hasattr(obj, "_obj") and obj._obj is None:
                 continue
 
             if hasattr(obj, "locations") and hasattr(obj, "local_locations"):
                 obj = obj.locations
@@ -703,14 +742,21 @@
 
             elif is_cadquery_sketch(obj):
                 pg = to_assembly([obj], names=[name])
                 pg.name = name
                 objects.append(pg)
                 names.append(name)
 
-    kwargs["reset_camera"] = first_call
+    if FIRST_CALL:
+        kwargs["reset_camera"] = Camera.RESET
 
     if len(objects) > 0:
-        show(*objects, names=names, collapse="R", _force_in_debug=True, **kwargs)
-        first_call = False
+        show(
+            *objects,
+            names=names,
+            collapse=Collapse.ROOT,
+            _force_in_debug=True,
+            **kwargs,
+        )
+        FIRST_CALL = False
     else:
         show_clear()
```

### Comparing `ocp_vscode-1.2.1/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.2.2/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 1.2.1
+Version: 1.2.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.2.1/setup.cfg` & `ocp_vscode-1.2.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.1
+current_version = 1.2.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.2.1/setup.py` & `ocp_vscode-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.2.1",
+    "version": "1.2.2",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
-        "ocp-tessellate>=1.1.2,<1.2.1",
+        "ocp-tessellate>=1.1.2,<1.2.2",
         "requests",
         "ipykernel",
         "orjson",
         "websockets>=11.0,<11.1",
     ],
     "packages": find_packages(),
     "zip_safe": False,
```

