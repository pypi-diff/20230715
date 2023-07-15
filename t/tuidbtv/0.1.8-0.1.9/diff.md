# Comparing `tmp/tuidbtv-0.1.8.tar.gz` & `tmp/tuidbtv-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.8.tar", max compression
+gzip compressed data, was "tuidbtv-0.1.9.tar", max compression
```

## Comparing `tuidbtv-0.1.8.tar` & `tuidbtv-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.8/LICENSE
--rw-r--r--   0        0        0      917 2023-07-07 21:53:09.681354 tuidbtv-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.8/tuidbtv/__init__.py
--rw-r--r--   0        0        0     4677 2023-07-07 21:38:37.857844 tuidbtv-0.1.8/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.8/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.8/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.8/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.8/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      472 2023-07-03 17:12:50.735465 tuidbtv-0.1.8/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2447 2023-07-03 17:12:50.736498 tuidbtv-0.1.8/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3303 2023-07-03 18:28:32.471479 tuidbtv-0.1.8/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1429 2023-07-03 17:12:50.740476 tuidbtv-0.1.8/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.8/tuidbtv/default.css
--rw-r--r--   0        0        0      276 2023-07-07 20:07:13.437708 tuidbtv-0.1.8/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.8/tuidbtv/suggesters/__init__.py
--rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.8/tuidbtv/suggesters/SuggesterDict.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.8/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.8/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.8/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.8/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.8/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.8/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5781 2023-07-07 21:46:01.271982 tuidbtv-0.1.8/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.8/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-03 17:12:50.721482 tuidbtv-0.1.9/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-15 19:46:44.454160 tuidbtv-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-07-03 17:12:50.723479 tuidbtv-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.728476 tuidbtv-0.1.9/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     5299 2023-07-15 19:52:15.173681 tuidbtv-0.1.9/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.732474 tuidbtv-0.1.9/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-07-03 17:12:50.731466 tuidbtv-0.1.9/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.742470 tuidbtv-0.1.9/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:12:50.733489 tuidbtv-0.1.9/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      497 2023-07-15 19:44:48.564736 tuidbtv-0.1.9/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2568 2023-07-15 19:44:48.566111 tuidbtv-0.1.9/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3450 2023-07-15 19:44:48.567113 tuidbtv-0.1.9/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1551 2023-07-15 19:44:48.568108 tuidbtv-0.1.9/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-07-03 17:12:50.744473 tuidbtv-0.1.9/tuidbtv/default.css
+-rw-r--r--   0        0        0      299 2023-07-15 19:52:15.177577 tuidbtv-0.1.9/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0      416 2023-07-15 19:44:48.569112 tuidbtv-0.1.9/tuidbtv/signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.747479 tuidbtv-0.1.9/tuidbtv/suggesters/__init__.py
+-rw-r--r--   0        0        0      838 2023-07-03 17:12:50.746488 tuidbtv-0.1.9/tuidbtv/suggesters/SuggesterDict.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.757487 tuidbtv-0.1.9/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:50.760465 tuidbtv-0.1.9/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-07-03 17:12:50.759464 tuidbtv-0.1.9/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-07-03 17:12:50.748488 tuidbtv-0.1.9/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-07-03 17:12:50.750478 tuidbtv-0.1.9/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0     1860 2023-07-15 19:44:48.569112 tuidbtv-0.1.9/tuidbtv/widgets/PreviewData.py
+-rw-r--r--   0        0        0      668 2023-07-03 17:12:50.751469 tuidbtv-0.1.9/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     5781 2023-07-07 21:46:01.271982 tuidbtv-0.1.9/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1902 2023-07-07 20:07:13.437708 tuidbtv-0.1.9/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.9/PKG-INFO
```

### Comparing `tuidbtv-0.1.8/LICENSE` & `tuidbtv-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/pyproject.toml` & `tuidbtv-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.8"
+version = "0.1.9"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.8/README.md` & `tuidbtv-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/__main__.py` & `tuidbtv-0.1.9/tuidbtv/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from textual import on
 from textual.app import App, ComposeResult
 from textual.containers import *
 from textual.widgets import Tree, DataTable, Footer, Header, TabbedContent, TabPane, Markdown, ContentSwitcher
+from textual.widgets._header import HeaderTitle
 
+from tuidbtv.enums_and_variables import APP_VERSION
+from tuidbtv.signals import PreviewNeed
+from tuidbtv.widgets.PreviewData import PreviewData
 from tuidbtv.widgets.QuitScreen import QuitScreen
 from tuidbtv.widgets.SQLEditor import SQLEditor
 from tuidbtv.widgets.SelectConnection import SelectConnection
 
 '''
 TODO:
 - add more connection types
@@ -24,35 +28,37 @@
 
     BINDINGS = [
         ("q", "quit_window()", "Quit"),
         ("s", "select_connection_window()", "Select connection"),
         ("r", "quit_window()", "Refresh"),
         ("a", "add_new_tab()", "Add tab"),
         ("d", "remove_current_tab()", "Delete current tab"),
+        ("m", "toggle_dark", "Toggle dark mode"),
     ]
 
     def __init__(self):
         super().__init__()
         self.tabs_count = 0
         self.suggestions = []
+        self.dbController = None
 
     def compose(self) -> ComposeResult:
-        yield Header()
+        yield Header(name="tuidbtv 0.1.9")
         with Horizontal():
             yield Tree("schemas")
             with TabbedContent():
                 with TabPane("preview", id="preview_tab"):
-                    yield DataTable(id="preview_data_table")
+                    yield PreviewData()
                 with TabPane("editor", id="editor_tab"):
                     yield SQLEditor()
                 with TabPane(" + ", id="add_new_tab_pane"):
                     yield Markdown()
         yield Footer()
 
-    def openConnectionSelectScreen(self, _firstRun = False):
+    def openConnectionSelectScreen(self, _firstRun=False):
         def select_connection(db_controller):
             self.dbController = db_controller
             tree = self.query_one(Tree)
             tree.clear()
             tree.root.expand()
             self.suggestions = []
             for schemaName in self.dbController.getSchemaNames():
@@ -65,24 +71,35 @@
             for editor in self.query(SQLEditor).nodes:
                 editor.clean_completions()
                 editor.add_completions(self.suggestions)
 
         self.push_screen(SelectConnection(firstRun=_firstRun), select_connection)
 
     def on_mount(self) -> None:
+        header = self.query_one(HeaderTitle)
+        header.text = f"tuidbtv {APP_VERSION}"
         self.openConnectionSelectScreen(_firstRun=True)
 
-    def on_tree_node_selected(self, event: Tree.NodeSelected):
-        if not event.node.allow_expand:
-            table = self.query_one("#preview_data_table")
-            table.clear(columns=True)
-            tableData = self.dbController.getTablePreview(event.node.parent.label, event.node.label)
-            table.add_columns(*tableData[0])
-            table.zebra_stripes = True
-            table.add_rows(tableData[1:])
+
+    def action_toggle_dark(self) -> None:
+        self.dark = not self.dark
+
+    @on(Tree.NodeSelected)
+    def refresh_preview_data(self, event: Tree.NodeSelected):
+        preview = self.query(PreviewData).first()
+        preview.refresh_table_data(event)
+
+    @on(PreviewNeed)
+    def update_preview_data(self, event: PreviewNeed):
+        preview = self.query_one(PreviewData)
+        data = self.dbController.getTablePreview(event.schema,
+                                                 event.table,
+                                                 event.column,
+                                                 event.desc)
+        preview.populate_data(data)
 
     def action_quit_window(self):
         self.push_screen(QuitScreen())
 
     def action_select_connection_window(self):
         self.openConnectionSelectScreen()
```

### Comparing `tuidbtv-0.1.8/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.1.9/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.1.9/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.1.9/tuidbtv/controllers/MySQLController.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 
     def getSchemaNames(self):
         return self.executeQuery("SHOW DATABASES")
 
     def getTableNamesBySchema(self, schemaName: str):
         return self.executeQuery(f"SHOW TABLES FROM `{schemaName}`")
 
-    def getTablePreview(self, schemaName: str, tableName: str):
-        return self.executeQueryWithHeaders(f"SELECT * FROM {schemaName}.{tableName} limit 100")
+    def getTablePreview(self, schemaName: str, tableName: str, order_by="", desc=False):
+        order = f"order by {order_by} {'desc' if desc else  'asc'}" if order_by else ''
+        return self.executeQueryWithHeaders(f"SELECT * FROM {schemaName}.{tableName} {order} limit 50")
 
     def executeQuery(self, query_text: str):
         try:
             cursor = self.connection.cursor()
             cursor.execute(query_text)
             data = cursor.fetchall()
             return data
```

### Comparing `tuidbtv-0.1.8/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.1.9/tuidbtv/controllers/PostgresController.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,19 @@
     def getTableNamesBySchema(self, schemaName):
         data = self.executeQuery(f"SELECT table_name FROM information_schema.tables WHERE table_schema='{schemaName}'")
         try:
             return sorted(data)
         except:
             return data
 
-    def getTablePreview(self, schemaName, tableName):
-        data = self.executeQuery(f"SELECT * FROM {schemaName}.{tableName} limit 100")
+    def getTablePreview(self, schemaName, tableName, order_by="", desc=False):
+        order = f"order by {order_by} {'desc' if desc else  'asc'}" if order_by else ''
+        data = self.executeQuery(
+            f"SELECT * FROM {schemaName}.{tableName} {order} limit 50"
+        )
         cutted_data = []
         for row in data:
             cutted_data.append(
                 tuple(
                     str(cell)[:50] for cell in row
                 )
             )
@@ -78,8 +81,8 @@
             Label("Hostname/IP"),
             Input(placeholder="localhost", id="hostName", classes=CONNECTION_FIELD_CLASS),
             Label("Port"),
             Input(placeholder="5432", id="port", validators=[Number()], classes=CONNECTION_FIELD_CLASS),
             Label("Database"),
             Input(placeholder="public", id="database", classes=CONNECTION_FIELD_CLASS),
             id="connection_form"
-        )
+        )
```

### Comparing `tuidbtv-0.1.8/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.1.9/tuidbtv/controllers/SQLLiteController.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 
     def getSchemaNames(self) -> list[str]:
         return [['tables']]
 
     def getTableNamesBySchema(self, schemaName: str) -> list[str]:
         return self.executeQuery("SELECT name FROM sqlite_master WHERE type='table';")
 
-    def getTablePreview(self, schemaName: str, tableName: str) -> list[dict]:
-        return self.executeQueryWithHeaders(f"select * from {tableName} limit 50;")
+    def getTablePreview(self, schemaName: str, tableName: str, order_by="", desc=False) -> list[dict]:
+        order = f"order by {order_by} {'desc' if desc else  'asc'}" if order_by else ''
+        return self.executeQueryWithHeaders(f"select * from {tableName} {order} limit 50;")
 
     def executeQuery(self, queryText: str) -> list[str]:
         cursor = self.connection.cursor()
         cursor.execute(queryText)
         return cursor.fetchall()
 
     def executeQueryWithHeaders(self, queryText: str):
```

### Comparing `tuidbtv-0.1.8/tuidbtv/default.css` & `tuidbtv-0.1.9/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/suggesters/SuggesterDict.py` & `tuidbtv-0.1.9/tuidbtv/suggesters/SuggesterDict.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.1.9/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.1.9/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.1.9/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.1.9/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.1.9/tuidbtv/widgets/SelectConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.1.9/tuidbtv/widgets/SQLEditor.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.8/PKG-INFO` & `tuidbtv-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.8
+Version: 0.1.9
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

