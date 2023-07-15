# Comparing `tmp/rastermap-0.1.3.tar.gz` & `tmp/rastermap-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rastermap-0.1.3.tar", last modified: Thu Jan 16 19:08:23 2020, max compression
+gzip compressed data, was "rastermap-0.9.0.tar", last modified: Sat Jul 15 12:01:36 2023, max compression
```

## Comparing `rastermap-0.1.3.tar` & `rastermap-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,59 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-01-16 19:08:23.000000 rastermap-0.1.3/
--rwxrwxrwx   0 root         (0) root         (0)    35147 2018-08-21 14:01:32.000000 rastermap-0.1.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       72 2018-08-21 14:01:32.000000 rastermap-0.1.3/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     9572 2020-01-16 19:08:23.000000 rastermap-0.1.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7939 2020-01-16 18:58:00.000000 rastermap-0.1.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap/
--rwxrwxrwx   0 root         (0) root         (0)       63 2018-11-12 15:23:37.000000 rastermap-0.1.3/rastermap/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2332 2019-08-16 13:57:22.000000 rastermap-0.1.3/rastermap/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    13405 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/filtermap.py
--rwxrwxrwx   0 root         (0) root         (0)    41698 2020-01-16 19:06:24.000000 rastermap-0.1.3/rastermap/gui.py
--rwxrwxrwx   0 root         (0) root         (0)    15776 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/isorec.py
--rwxrwxrwx   0 root         (0) root         (0)    30756 2019-08-05 14:02:45.000000 rastermap-0.1.3/rastermap/mapping.py
--rwxrwxrwx   0 root         (0) root         (0)     4973 2018-11-12 15:23:37.000000 rastermap-0.1.3/rastermap/mapping2.py
--rwxrwxrwx   0 root         (0) root         (0)    18780 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/mapping_copy.py
--rwxrwxrwx   0 root         (0) root         (0)    19976 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/mapping_inc.py
--rwxrwxrwx   0 root         (0) root         (0)    21089 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/mapping_new.py
--rwxrwxrwx   0 root         (0) root         (0)    16729 2019-06-07 15:42:35.000000 rastermap-0.1.3/rastermap/mapping_old.py
--rwxrwxrwx   0 root         (0) root         (0)    14219 2018-12-18 15:13:24.000000 rastermap-0.1.3/rastermap/rasterPCA.py
--rwxrwxrwx   0 root         (0) root         (0)     7053 2020-01-16 19:06:24.000000 rastermap-0.1.3/rastermap/roi.py
--rwxrwxrwx   0 root         (0) root         (0)     7216 2019-08-16 14:05:57.000000 rastermap-0.1.3/rastermap/run.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     9572 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      507 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       68 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2020-01-16 19:08:23.000000 rastermap-0.1.3/rastermap.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2020-01-16 19:08:23.000000 rastermap-0.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      828 2020-01-16 19:06:35.000000 rastermap-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.151928 rastermap-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.135928 rastermap-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.139928 rastermap-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 12:01:21.000000 rastermap-0.9.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-15 12:01:21.000000 rastermap-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-15 12:01:21.000000 rastermap-0.9.0/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-15 12:01:21.000000 rastermap-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-15 12:01:36.151928 rastermap-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-15 12:01:21.000000 rastermap-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-15 12:01:21.000000 rastermap-0.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.143928 rastermap-0.9.0/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21082 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/splitting.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:01:36.151928 rastermap-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-15 12:01:21.000000 rastermap-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.151928 rastermap-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-15 12:01:21.000000 rastermap-0.9.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-15 12:01:21.000000 rastermap-0.9.0/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 12:01:21.000000 rastermap-0.9.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rastermap-0.1.3/LICENSE` & `rastermap-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.1.3/rastermap/run.py` & `rastermap-0.9.0/rastermap/gui/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,95 @@
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
 import numpy as np
 import os
 from PyQt5 import QtGui, QtCore
+from PyQt5.QtWidgets import QMainWindow, QApplication, QSizePolicy, QDialog, QWidget, QScrollBar, QSlider, QComboBox, QGridLayout, QPushButton, QFrame, QCheckBox, QLabel, QProgressBar, QLineEdit, QMessageBox, QGroupBox, QButtonGroup, QRadioButton, QStatusBar, QTextEdit
+from . import io
+
+
+### custom QDialog which allows user to fill in ops and run rastermap
+class RunWindow(QDialog):
 
-### custom QDialog which allows user to fill in ops and run suite2p!
-class RunWindow(QtGui.QDialog):
     def __init__(self, parent=None):
         super(RunWindow, self).__init__(parent)
-        self.setGeometry(50,50,600,600)
-        self.setWindowTitle('Choose rastermap run options')
-        self.win = QtGui.QWidget(self)
-        self.layout = QtGui.QGridLayout()
+        self.setGeometry(50, 50, 600, 600)
+        self.setWindowTitle("Choose rastermap run options")
+        self.win = QWidget(self)
+        self.layout = QGridLayout()
         self.layout.setHorizontalSpacing(25)
         self.win.setLayout(self.layout)
 
+        print(
+            ">>> importing rastermap functions (will be slow if you haven't run rastermap before) <<<"
+        )
+        from rastermap import default_settings, settings_info, Rastermap
         # default ops
-        self.ops = {'n_components': 2, 'n_X': 40, 'alpha': 1., 'K': 1.,
-                    'nPC': 200, 'constraints': 2, 'annealing': True, 'init': 'pca',
-                    'start_time': 0, 'end_time': -1}
-
-        keys = ['n_components','n_X','alpha','constraints','K','nPC','annealing','init','start_time','end_time']
-        tooltips = ['dimensionality of low-D space (1 or 2)',
-                    'number of nodes in low-D space (rasterization)',
-                    'decay of power-law 1/(K + n^alpha)',
-                    'decay of power-law 1/(K + n^alpha)',
-                    'number of PCs used to compute embedding',
-                    '0=no constraints, 1=smoothing only, 2=power-law',
-                    'whether to anneal at the end (otherwise each neuron is kept at assigned node)',
-                    "initialization - 'pca' for PCs, 'random' for random",
-                    "start time for training set",
-                    "end time for training set (if -1, use all points for training)"]
-
+        self.ops = default_settings()
+        info = settings_info()
+        keys = [
+            "n_clusters", "n_PCs", "time_lag_window", "locality", "grid_upsample",
+            "time_bin", "n_splits", "run_scaled_kmeans"
+        ]
+        tooltips = [info[key] for key in keys]
         bigfont = QtGui.QFont("Arial", 10, QtGui.QFont.Bold)
-        l=0
+        l = 0
         self.keylist = []
         self.editlist = []
-        k=0
+        k = 0
         for key in keys:
-            qedit = LineEdit(k,key,self)
-            qlabel = QtGui.QLabel(key)
+            qedit = LineEdit(k, key, self)
+            qlabel = QLabel(key)
             qlabel.setToolTip(tooltips[k])
             qedit.set_text(self.ops)
             qedit.setFixedWidth(90)
-            self.layout.addWidget(qlabel,k,0,1,1)
-            self.layout.addWidget(qedit,k,1,1,1)
+            self.layout.addWidget(qlabel, k, 0, 1, 1)
+            self.layout.addWidget(qedit, k, 1, 1, 1)
             self.keylist.append(key)
             self.editlist.append(qedit)
-            k+=1
+            k += 1
 
-        self.layout.addWidget(QtGui.QLabel("."),19,4,1,1)
-        self.layout.addWidget(QtGui.QLabel("."),19,5,1,1)
-        self.layout.addWidget(QtGui.QLabel("."),19,6,1,1)
-        self.layout.addWidget(QtGui.QLabel("."),19,7,1,1)
-        self.layout.addWidget(QtGui.QLabel("."),19,8,1,1)
+        #for j in range(10):
+        #    self.layout.addWidget(QLabel("."),19,4+j,1,1)
 
-        self.layout.setColumnStretch(4,10)
-        self.runButton = QtGui.QPushButton('RUN')
+        self.layout.setColumnStretch(4, 10)
+        self.runButton = QPushButton("RUN")
         self.runButton.clicked.connect(lambda: self.run_RMAP(parent))
-        self.layout.addWidget(self.runButton,19,0,1,1)
+        self.layout.addWidget(self.runButton, 19, 0, 1, 1)
         #self.runButton.setEnabled(False)
-        self.textEdit = QtGui.QTextEdit()
-        self.textEdit.setSizePolicy(QtGui.QSizePolicy.Expanding, QtGui.QSizePolicy.Expanding)
-        self.layout.addWidget(self.textEdit, 20,0,30,9)
+        self.textEdit = QTextEdit()
+        self.textEdit.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
+        self.layout.addWidget(self.textEdit, 20, 0, 30, 14)
         self.process = QtCore.QProcess(self)
         self.process.readyReadStandardOutput.connect(self.stdout_write)
         self.process.readyReadStandardError.connect(self.stderr_write)
         # disable the button when running the s2p process
         self.process.started.connect(self.started)
         self.process.finished.connect(lambda: self.finished(parent))
         # stop process
-        self.stopButton = QtGui.QPushButton('STOP')
+        self.stopButton = QPushButton("STOP")
         self.stopButton.setEnabled(False)
-        self.layout.addWidget(self.stopButton, 19,1,1,1)
+        self.layout.addWidget(self.stopButton, 19, 1, 1, 1)
         self.stopButton.clicked.connect(self.stop)
 
+        self.show()
+
     def run_RMAP(self, parent):
         del parent.sp
         self.finish = True
         self.error = False
         self.save_text()
-        np.save('ops.npy', self.ops)
-        print('Running rastermap!')
-        print('starting process')
+        np.save("rmap_ops.npy", self.ops)
+        print("Running rastermap with command:")
+        cmd = f"python -u -W ignore -m rastermap --ops rmap_ops.npy --S {parent.filebase} "
         if parent.file_iscell is not None:
-            self.process.start('python -u -W ignore -m rastermap --ops ops.npy --S %s --iscell %s'%(parent.filebase, parent.file_iscell))
-        else:
-            self.process.start('python -u -W ignore -m rastermap --ops ops.npy --S %s'%parent.filebase)
+            cmd += f"--iscell {parent.file_iscell}"
+        print(cmd)
+        self.process.start(cmd)
 
     def stop(self):
         self.finish = False
         self.process.kill()
 
     def started(self):
         self.runButton.setEnabled(False)
@@ -96,78 +97,81 @@
 
     def finished(self, parent):
         self.runButton.setEnabled(True)
         self.stopButton.setEnabled(False)
         if self.finish and not self.error:
             cursor = self.textEdit.textCursor()
             cursor.movePosition(cursor.End)
-            cursor.insertText('Opening in GUI (can close this window)\n')
-            basename,fname = os.path.split(parent.fname)
-            if os.path.isfile(os.path.join(basename, 'embedding.npy')):
-                parent.fname = os.path.join(basename, 'embedding.npy')
+            cursor.insertText("Opening in GUI (can close this window)\n")
+            basename, fname = os.path.split(parent.fname)
+            fname = os.path.splitext(fname)[0]
+            if os.path.isfile(os.path.join(basename, f"{fname}_embedding.npy")):
+                parent.fname = os.path.join(basename, f"{fname}_embedding.npy")
             else:
-                parent.fname = 'embedding.npy'
-            parent.load_proc(parent.fname)
+                parent.fname = f"{fname}_embedding.npy"
+            io.load_proc(parent, name=parent.fname)
         elif not self.error:
             cursor = self.textEdit.textCursor()
             cursor.movePosition(cursor.End)
-            cursor.insertText('Interrupted by user (not finished)\n')
+            cursor.insertText("Interrupted by user (not finished)\n")
         else:
             cursor = self.textEdit.textCursor()
             cursor.movePosition(cursor.End)
-            cursor.insertText('Interrupted by error (not finished)\n')
+            cursor.insertText("Interrupted by error (not finished)\n")
 
     def save_text(self):
         for k in range(len(self.editlist)):
             key = self.keylist[k]
             self.ops[key] = self.editlist[k].get_text(self.ops[key])
 
     def stdout_write(self):
         cursor = self.textEdit.textCursor()
         cursor.movePosition(cursor.End)
-        cursor.insertText(str(self.process.readAllStandardOutput(), 'utf-8'))
+        cursor.insertText(str(self.process.readAllStandardOutput(), "utf-8"))
         self.textEdit.ensureCursorVisible()
 
     def stderr_write(self):
         cursor = self.textEdit.textCursor()
         cursor.movePosition(cursor.End)
-        cursor.insertText('>>>ERROR<<<\n')
-        cursor.insertText(str(self.process.readAllStandardError(), 'utf-8'))
+        cursor.insertText(">>>ERROR<<<\n")
+        cursor.insertText(str(self.process.readAllStandardError(), "utf-8"))
         self.textEdit.ensureCursorVisible()
         self.error = True
 
-class LineEdit(QtGui.QLineEdit):
-    def __init__(self,k,key,parent=None):
-        super(LineEdit,self).__init__(parent)
+
+class LineEdit(QLineEdit):
+
+    def __init__(self, k, key, parent=None):
+        super(LineEdit, self).__init__(parent)
         self.key = key
         #self.textEdited.connect(lambda: self.edit_changed(parent.ops, k))
 
-    def get_text(self,okey):
+    def get_text(self, okey):
         key = self.key
-        if key=='diameter' or key=='block_size':
-            diams = self.text().replace(' ','').split(',')
-            if len(diams)>1:
+        if key == "diameter" or key == "block_size":
+            diams = self.text().replace(" ", "").split(",")
+            if len(diams) > 1:
                 okey = [int(diams[0]), int(diams[1])]
             else:
                 okey = int(diams[0])
         else:
             if type(okey) is float:
                 okey = float(self.text())
             elif type(okey) is str:
                 okey = self.text()
             elif type(okey) is int or bool:
                 okey = int(self.text())
 
         return okey
 
-    def set_text(self,ops):
+    def set_text(self, ops):
         key = self.key
-        if key=='diameter' or key=='block_size':
-            if (type(ops[key]) is not int) and (len(ops[key])>1):
-                dstr = str(int(ops[key][0])) + ', ' + str(int(ops[key][1]))
+        if key == "diameter" or key == "block_size":
+            if (type(ops[key]) is not int) and (len(ops[key]) > 1):
+                dstr = str(int(ops[key][0])) + ", " + str(int(ops[key][1]))
             else:
                 dstr = str(int(ops[key]))
         else:
             if type(ops[key]) is bool:
                 dstr = str(int(ops[key]))
             elif type(ops[key]) is str:
                 dstr = ops[key]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rastermap-0.1.3/setup.py` & `rastermap-0.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,46 @@
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
 import setuptools
 
+install_deps = [
+        "numpy>=1.24.0", 
+        "scipy", 
+        "scikit-learn", 
+        "numba>=0.57.0",
+        "natsort",
+        "tqdm"
+        ]
+
+gui_deps = [
+        "pyqtgraph>=0.11.0rc0", 
+        "pyqt5", 
+        "pyqt5.sip",
+        "superqt",
+        ]
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rastermap",
-    version="0.1.3",
+    use_scm_version=True,
     author="Marius Pachitariu and Carsen Stringer",
     author_email="carsen.stringer@gmail.com",
-    description="Unsupervised clustering algorithm for 2D data",
+    description="Unsupervised clustering algorithm for 2D data (neurons by time)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MouseLand/rastermap",
     packages=setuptools.find_packages(),
-	install_requires = ['numpy>=1.13.0', 'scipy','scikit-learn', 'pyqtgraph', 'matplotlib','numba','natsort'],
+	install_requires = install_deps,
+    extras_require = {
+      "gui": gui_deps
+    },
+    tests_require = ["pytest"],
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ),
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

