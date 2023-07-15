# Comparing `tmp/sport-activities-features-gui-0.2.0.tar.gz` & `tmp/sport_activities_features_gui-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sport-activities-features-gui-0.2.0.tar", max compression
+gzip compressed data, was "sport_activities_features_gui-0.2.1.tar", max compression
```

## Comparing `sport-activities-features-gui-0.2.0.tar` & `sport_activities_features_gui-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-07-04 18:42:19.126948 sport-activities-features-gui-0.2.0/LICENSE
--rw-r--r--   0        0        0      600 2023-07-04 18:42:19.127948 sport-activities-features-gui-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/__init__.py
--rw-r--r--   0        0        0       88 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/globalVars.py
--rw-r--r--   0        0        0     5020 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/Graphs.py
--rw-r--r--   0        0        0     1647 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/ImportData.py
--rw-r--r--   0        0        0     1830 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/MultiThread.py
--rw-r--r--   0        0        0     1788 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/Transformations.py
--rw-r--r--   0        0        0      275 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/__init.py
--rw-r--r--   0        0        0      617 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/main.py
--rw-r--r--   0        0        0    12488 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/media/Icon.png
--rw-r--r--   0        0        0     1353 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/models/User.py
--rw-r--r--   0        0        0      103 2023-07-04 18:42:19.128949 sport-activities-features-gui-0.2.0/sport_activities_features_gui/models/__init__.py
--rw-r--r--   0        0        0     3019 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/CalendarWidget.py
--rw-r--r--   0        0        0     8358 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/GraphsWidget.py
--rw-r--r--   0        0        0     6900 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/ImportDataWidget.py
--rw-r--r--   0        0        0     5032 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/TransformationsWidget.py
--rw-r--r--   0        0        0      369 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/__init__.py
--rw-r--r--   0        0        0     1844 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/AddProfile.py
--rw-r--r--   0        0        0     6429 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/MainWindow.py
--rw-r--r--   0        0        0     5291 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/ProfilesWindow.py
--rw-r--r--   0        0        0     2285 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/ViewAttributesWindow.py
--rw-r--r--   0        0        0      399 2023-07-04 18:42:19.129948 sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/__init__.py
--rw-r--r--   0        0        0      993 2023-07-04 18:42:30.507183 sport-activities-features-gui-0.2.0/setup.py
--rw-r--r--   0        0        0      515 2023-07-04 18:42:30.507335 sport-activities-features-gui-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-15 15:19:59.653577 sport_activities_features_gui-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2205 2023-07-15 15:19:59.653577 sport_activities_features_gui-0.2.1/README.md
+-rw-r--r--   0        0        0      981 2023-07-15 15:19:59.656577 sport_activities_features_gui-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/globalVars.py
+-rw-r--r--   0        0        0     5020 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Graphs.py
+-rw-r--r--   0        0        0     1619 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/ImportData.py
+-rw-r--r--   0        0        0     1830 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/MultiThread.py
+-rw-r--r--   0        0        0     1788 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Transformations.py
+-rw-r--r--   0        0        0      255 2023-07-15 15:19:59.659577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/main.py
+-rw-r--r--   0        0        0    12488 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/media/Icon.png
+-rw-r--r--   0        0        0     1355 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/User.py
+-rw-r--r--   0        0        0       72 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/__init__.py
+-rw-r--r--   0        0        0     3066 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/CalendarWidget.py
+-rw-r--r--   0        0        0     8417 2023-07-15 15:19:59.660577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/GraphsWidget.py
+-rw-r--r--   0        0        0     6991 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/ImportDataWidget.py
+-rw-r--r--   0        0        0     5122 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/TransformationsWidget.py
+-rw-r--r--   0        0        0      341 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/__init__.py
+-rw-r--r--   0        0        0     1844 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/AddProfile.py
+-rw-r--r--   0        0        0     6580 2023-07-15 15:19:59.661577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/MainWindow.py
+-rw-r--r--   0        0        0     5383 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ProfilesWindow.py
+-rw-r--r--   0        0        0     2285 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ViewAttributesWindow.py
+-rw-r--r--   0        0        0      372 2023-07-15 15:19:59.662577 sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/__init__.py
+-rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.1/setup.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 sport_activities_features_gui-0.2.1/PKG-INFO
```

### Comparing `sport-activities-features-gui-0.2.0/LICENSE` & `sport_activities_features_gui-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/Graphs.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Graphs.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/MultiThread.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/MultiThread.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/logic/Transformations.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/logic/Transformations.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/main.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 from PyQt6 import QtWidgets
-from windows.ProfilesWindow import Ui_ProfilesWindow
-
+from sport_activities_features_gui.windows.ProfilesWindow import Ui_ProfilesWindow
 
 def main():
     app = QtWidgets.QApplication(sys.argv)
     app.setStyle('Fusion')
     profilesWindow = Ui_ProfilesWindow()
     profilesWindow.show()
     sys.exit(app.exec())
@@ -13,10 +12,11 @@
 def icon_loader_for_win32(): # Windows needs this to display the icon in the taskbar
     if sys.platform == "win32":
         import ctypes
         myappid = 'firefly-cpp.sport-activities-features.gui'
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 
 
+
 if __name__ == '__main__':
     icon_loader_for_win32()
     main()
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/media/Icon.png` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/media/Icon.png`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/models/User.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/models/User.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle
 import pandas as pd
 import os
-from globalVars import *
+from ..globalVars import *
 
 
 def initGlobalUser(userName, settings):
     global user
     user = User(userName, settings)
     return user
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/CalendarWidget.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/CalendarWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from PyQt6.QtWidgets import QWidget, QApplication, QCalendarWidget
 
 from PyQt6.QtGui import QPalette, QTextCharFormat
 from PyQt6.QtCore import Qt
 from datetime import datetime
 import numpy as np
 
-import User
+from sport_activities_features_gui.models.User import User
 
 
 class Ui_CalendarWidget(QWidget):
     globalUser: User
 
     def __init__(self):
         super().__init__()
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/GraphsWidget.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/GraphsWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from PyQt6 import QtCore, QtGui, QtWidgets
 from PyQt6.QtWidgets import QWidget, QMessageBox
-from logic.Graphs import Graphs
-from windows.ViewAttributesWindow import Ui_ViewAttributesWindow
-
-
 class Ui_GraphsWidget(QWidget):
     exampleGraphs = ["All biking distances ridden",
                      "Sum of biking duration for competitor",
                      "Altitude vs calories",
                      "Calories by activity type",
                      "Heart rate by activities"]
     graphFn = None
@@ -163,7 +159,11 @@
     def on_combobox_changed(self, value):
         if (value == "Bar" or value == "Line"):
             self.xAxisInput.setEnabled(False)
             self.btnViewAttributesX.setEnabled(False)
         else:
             self.xAxisInput.setEnabled(True)
             self.btnViewAttributesX.setEnabled(True)
+
+
+from sport_activities_features_gui.logic.Graphs import Graphs
+from sport_activities_features_gui.windows.ViewAttributesWindow import Ui_ViewAttributesWindow
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/ImportDataWidget.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/ImportDataWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 from PyQt6.QtWidgets import QWidget, QFileDialog
 
-import widgets
-from logic.ImportData import ImportData
-from models.User import User
+from sport_activities_features_gui.models import User
+from sport_activities_features_gui.logic.ImportData import ImportData
+
 from PyQt6 import sip
 from PyQt6.QtCore import Qt
 # Rest of the code
 
 class PandasModel(QtCore.QAbstractTableModel):
     """
     Class to populate a table view with a pandas dataframe
@@ -98,18 +98,20 @@
         self.lbl_Output.setText(_translate("ImportData", "Output:"))
         self.lbl_ExportRawData.setText(_translate("ImportData", "Export Raw Data:"))
         self.btn_Csv.setText(_translate("ImportData", "CSV"))
         self.btn_Json.setText(_translate("ImportData", "JSON"))
         self.btn_Pickle.setText(_translate("ImportData", "Pickle"))
     
     def readFiles(self):
-        self.importDataFn.openFileDialog(self)
+        df = self.importDataFn.openFileDialog()
+        if(df is not None):
+            self.OutputExistingData(df)
+            self.refreshCalendarWidget()
         # Refresh calendar widget
-        self.refreshCalendarWidget()
-        
+
     def saveFileDialog(self, defaultFileName, fileFormat):
         fd = QFileDialog()
         fd.setOption(QFileDialog.Option.DontUseNativeDialog, True)
         fileName, _ = fd.getSaveFileName(self,"QFileDialog.getSaveFileName()",defaultFileName, fileFormat)
         return fileName
     
     def exportCSV(self):
@@ -145,10 +147,10 @@
             model = PandasModel(df2)
             self.pte_Output.setModel(model)
         
     def refreshCalendarWidget(self):
         self.refMainWindow.mainLayout_4.removeWidget(self.refMainWindow.calendarUi)
         sip.delete(self.refMainWindow.calendarUi)
         self.refMainWindow.calendarUi = None
-        self.refMainWindow.calendarUi = widgets.Ui_ImportDataWidget()
+        self.refMainWindow.calendarUi = Ui_ImportDataWidget()
         self.refMainWindow.mainLayout_4.addWidget(self.refMainWindow.calendarUi)
         self.refMainWindow.calendarUi.importGlobalUser(self.globalUser)
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/widgets/TransformationsWidget.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/widgets/TransformationsWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt6 import QtCore, QtGui, QtWidgets
 from PyQt6.QtWidgets import QMainWindow, QApplication, QMessageBox, QWidget
 from PyQt6.QtGui import QAction
-from logic.ImportData import ImportData
-from logic.Transformations import Transformations
-from models.User import User
+from sport_activities_features_gui.logic.ImportData import ImportData
+from sport_activities_features_gui.logic.Transformations import Transformations
+from sport_activities_features_gui.models.User import User
 import pandas as pd
 
 class Ui_TransformationsWidget(QWidget):
     globalUser: User
     importDataFn: ImportData
     transformations: Transformations
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/AddProfile.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/AddProfile.py`

 * *Files identical despite different names*

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/MainWindow.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/MainWindow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from PyQt6.QtWidgets import QMainWindow
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from widgets.ImportDataWidget import Ui_ImportDataWidget
-from widgets.GraphsWidget import Ui_GraphsWidget
-from widgets.CalendarWidget import Ui_CalendarWidget
-from widgets.TransformationsWidget import Ui_TransformationsWidget
-from models.User import User
+from sport_activities_features_gui.widgets.GraphsWidget import Ui_GraphsWidget
+from sport_activities_features_gui.widgets.CalendarWidget import Ui_CalendarWidget
+from sport_activities_features_gui.widgets.TransformationsWidget import Ui_TransformationsWidget
+from sport_activities_features_gui.widgets.ImportDataWidget import Ui_ImportDataWidget
+
+from sport_activities_features_gui.models.User import User
 
 
 class Ui_MainWindow(QMainWindow):
     globalUser: User
     importDataUi: Ui_ImportDataWidget
     graphsUi = Ui_GraphsWidget
     calendarUi = Ui_CalendarWidget
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/ProfilesWindow.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ProfilesWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shutil
 from PyQt6 import QtCore, QtWidgets, QtGui
 from PyQt6.QtWidgets import QMainWindow, QMessageBox
-from models.User import initGlobalUser, User
-from windows.AddProfile import Ui_AddProfileWindow
-from windows.MainWindow import Ui_MainWindow
+from sport_activities_features_gui.models.User import initGlobalUser, User
+from sport_activities_features_gui.windows.AddProfile import Ui_AddProfileWindow
+from sport_activities_features_gui.windows.MainWindow import Ui_MainWindow
 import os
-from globalVars import *
+from ..globalVars import *
 
 
 class Ui_ProfilesWindow(QMainWindow):
     currentProfile = None
     profileList = []
 
     def __init__(self):
```

### Comparing `sport-activities-features-gui-0.2.0/sport_activities_features_gui/windows/ViewAttributesWindow.py` & `sport_activities_features_gui-0.2.1/sport_activities_features_gui/windows/ViewAttributesWindow.py`

 * *Files identical despite different names*

