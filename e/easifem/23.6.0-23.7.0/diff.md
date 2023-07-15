# Comparing `tmp/easifem-23.6.0.tar.gz` & `tmp/easifem-23.7.0.tar.gz`

## Comparing `easifem-23.6.0.tar` & `easifem-23.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/clean.py
--rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/cmake.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/components.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/console.py
--rwxr-xr-x   0        0        0     3711 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/easifem.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/install.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/parsers.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/run.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/setenv.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/test.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/uninstall.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_clean.py
--rw-r--r--   0        0        0    32343 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_install.py
--rw-r--r--   0        0        0    10907 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_run.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_setenv.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 easifem-23.6.0/src/easifem/utils_uninstall.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/hello.F90
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/hello.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/test2.F90
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 easifem-23.6.0/tests/test2.md
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easifem-23.6.0/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 easifem-23.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 easifem-23.6.0/README.md
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 easifem-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 easifem-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/clean.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/cmake.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/components.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/console.py
+-rwxr-xr-x   0        0        0     3711 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/easifem.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/install.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/parsers.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/run.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/setenv.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/test.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/uninstall.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/utils_clean.py
+-rw-r--r--   0        0        0    32378 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/utils_install.py
+-rw-r--r--   0        0        0    10907 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/utils_run.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/utils_setenv.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 easifem-23.7.0/src/easifem/utils_uninstall.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easifem-23.7.0/tests/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 easifem-23.7.0/tests/hello.F90
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 easifem-23.7.0/tests/hello.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 easifem-23.7.0/tests/test2.F90
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 easifem-23.7.0/tests/test2.md
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easifem-23.7.0/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 easifem-23.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 easifem-23.7.0/README.md
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 easifem-23.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 easifem-23.7.0/PKG-INFO
```

### Comparing `easifem-23.6.0/src/easifem/clean.py` & `easifem-23.7.0/src/easifem/clean.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/cmake.py` & `easifem-23.7.0/src/easifem/cmake.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/easifem.py` & `easifem-23.7.0/src/easifem/easifem.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/install.py` & `easifem-23.7.0/src/easifem/install.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/run.py` & `easifem-23.7.0/src/easifem/run.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/setenv.py` & `easifem-23.7.0/src/easifem/setenv.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/test.py` & `easifem-23.7.0/src/easifem/test.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/uninstall.py` & `easifem-23.7.0/src/easifem/uninstall.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/utils_clean.py` & `easifem-23.7.0/src/easifem/utils_clean.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/utils_install.py` & `easifem-23.7.0/src/easifem/utils_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
+import platform
 
 # import sys
 import shutil
 import subprocess
 from easifem.console import console
 from rich.panel import Panel
 from rich.text import Text
+from distutils.ccompiler import new_compiler
+from distutils.sysconfig import customize_compiler
 
 # _easifem = "easifem"
 
 _extpkgs = ["openblas", "lapack95", "sparsekit", "fftw", "superlu", "arpack", "lis"]
 
 _components = ["extpkgs", "base", "classes", "materials", "kernels"] + _extpkgs
 
@@ -464,20 +467,35 @@
         os.chdir(pkg_with_path)
 
     os.makedirs(EASIFEM_EXTPKGS, exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_EXTPKGS, "include"), exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_EXTPKGS, "lib"), exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_EXTPKGS, "bin"), exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_EXTPKGS, "share"), exist_ok=True)
-    cargs = [
-        os.path.join(pkg_with_path, "configure"),
-        "--prefix",
-        EASIFEM_EXTPKGS,
-        "--enable-openmp",
-    ]
+    ccompiler = new_compiler()
+    customize_compiler(ccompiler)
+    print("platform.system = ", platform.system())
+    print("c compiler: = ", ccompiler.compiler[0] )
+    check_darwin = platform.system() == "Darwin" and  ccompiler.compiler[0] == "clang"
+
+    if(check_darwin):
+        cargs = [
+            os.path.join(pkg_with_path, "configure"),
+            "--prefix",
+            EASIFEM_EXTPKGS, 
+            "--disable-openmp"
+        ]
+    else:
+        cargs = [
+            os.path.join(pkg_with_path, "configure"),
+            "--prefix",
+            EASIFEM_EXTPKGS,
+            "--enable-openmp",
+        ]
+
     runCommand(cargs=cargs, quite=quite)
     cargs = [
         "make",
     ]
     runCommand(cargs=cargs, quite=quite)
 
     cargs = [
@@ -722,16 +740,16 @@
     url = "https://github.com/anishida/" + pkg_name + ".git"
     cmake_def = []
     cmake_def.append(f"--prefix={EASIFEM_EXTPKGS}")
     cmake_def.append("--enable-omp")
     cmake_def.append("--enable-f90")
     cmake_def.append("--enable-shared")
     cmake_def.append("--enable-saamg")
-    cmake_def.append("FC=gfortran")
-    cmake_def.append("CC=gcc")
+    ##cmake_def.append("FC=gfortran")
+    # cmake_def.append("CC=gcc")
 
     cwd = os.getcwd()
 
     if os.path.exists(pkg_with_path):
         os.chdir(pkg_with_path)
         cargs = ["git", "pull"]
         runCommand(cargs=cargs, quite=quite)
@@ -823,28 +841,29 @@
     cmake_def.append("-D USE_ARPACK:BOOL=ON")
     cmake_def.append("-D USE_PARPACK:BOOL=OFF")
     cmake_def.append("-D USE_METIS:BOOL=OFF")
     cmake_def.append("-D USE_SUPERLU:BOOL=ON")
     cmake_def.append("-D USE_LIS:BOOL=ON")
     cmake_def.append("-D USE_Int32:BOOL=ON")
     cmake_def.append("-D USE_Real64:BOOL=ON")
+    cmake_def.append("-D COLOR_DISP:BOOL=OFF")
 
     build_dir = os.path.join(build, "easifem", pkg_name, "build")
 
     cwd = os.getcwd()
 
     if os.path.exists(pkg_with_path):
         os.chdir(pkg_with_path)
         cargs = ["git", "pull"]
         runCommand(cargs=cargs, quite=quite)
     else:
         console.print(f"Path {pkg_with_path} does not exist.")
         console.print(f"Creating {pkg_with_path}")
-        # cargs = ["git", "clone", f"{url}", f"{pkg_with_path}"]
-        cargs = ["gh", "repo", "clone", "vickysharma0812/easifem-base", pkg_with_path]
+        cargs = ["git", "clone", url, pkg_with_path]
+        # cargs = ["gh", "repo", "clone", "vickysharma0812/easifem-base", pkg_with_path]
         runCommand(cargs=cargs, quite=quite)
         os.chdir(pkg_with_path)
 
     os.makedirs(build_dir, exist_ok=True)
     os.makedirs(EASIFEM_BASE, exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_BASE, "include"), exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_BASE, "lib"), exist_ok=True)
@@ -914,51 +933,38 @@
 def _install_classes(quite, install, build, source):
     pkg_dir = os.path.join(source, "easifem")
     pkg_name = "classes"
     pkg_with_path = os.path.join(pkg_dir, pkg_name)
     url = "https://github.com/vickysharma0812/easifem-classes.git"
 
     cmake_def = []
-    cmake_def.append("-D USE_OpenMP:BOOL=ON")
     cmake_def.append(f"-D CMAKE_INSTALL_PREFIX:PATH={EASIFEM_CLASSES}")
     cmake_def.append("-D CMAKE_BUILD_TYPE:STRING=Release")
     cmake_def.append("-D BUILD_SHARED_LIBS:BOOL=ON")
-    cmake_def.append("-D USE_PLPLOT:BOOL=ON")
-    cmake_def.append("-D USE_BLAS95:BOOL=ON")
-    cmake_def.append("-D USE_LAPACK95:BOOL=ON")
-    cmake_def.append("-D USE_FFTW:BOOL=ON")
-    cmake_def.append("-D USE_ARPACK:BOOL=ON")
-    cmake_def.append("-D USE_SUPERLU:BOOL=ON")
-    cmake_def.append("-D USE_LIS:BOOL=ON")
-    cmake_def.append("-D USE_Int32:BOOL=ON")
-    cmake_def.append("-D USE_Real64:BOOL=ON")
-    cmake_def.append("-D USE_PARPACK:BOOL=OFF")
-    cmake_def.append("-D USE_METIS:BOOL=OFF")
     cmake_def.append("-D USE_GMSH_SDK:BOOL=OFF")
-    cmake_def.append("-D USE_GTK:BOOL=OFF")
 
     build_dir = os.path.join(build, "easifem", pkg_name, "build")
 
     cwd = os.getcwd()
 
     if os.path.exists(pkg_with_path):
         os.chdir(pkg_with_path)
         cargs = ["git", "pull"]
         runCommand(cargs=cargs, quite=quite)
     else:
         console.print(f"Path {pkg_with_path} does not exist.")
         console.print(f"Creating {pkg_with_path}")
-        # cargs = ["git", "clone", f"{url}", f"{pkg_with_path}"]
-        cargs = [
-            "gh",
-            "repo",
-            "clone",
-            "vickysharma0812/easifem-classes",
-            pkg_with_path,
-        ]
+        cargs = ["git", "clone", url, pkg_with_path]
+        # cargs = [
+        #     "gh",
+        #     "repo",
+        #     "clone",
+        #     "vickysharma0812/easifem-classes",
+        #     pkg_with_path,
+        # ]
         runCommand(cargs=cargs, quite=quite)
         os.chdir(pkg_with_path)
 
     os.makedirs(build_dir, exist_ok=True)
     os.makedirs(EASIFEM_CLASSES, exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_CLASSES, "include"), exist_ok=True)
     os.makedirs(os.path.join(EASIFEM_CLASSES, "lib"), exist_ok=True)
@@ -974,15 +980,15 @@
         f"{build_dir}",
     ] + cmake_def
 
     runCommand(cargs=cargs, quite=quite)
     cargs = [
         "cmake",
         "--build",
-        f"{build_dir}",
+        build_dir,
         "--target",
         "install",
     ]
     runCommand(cargs=cargs, quite=quite)
 
     text = Text()
     text.append(
```

### Comparing `easifem-23.6.0/src/easifem/utils_run.py` & `easifem-23.7.0/src/easifem/utils_run.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/utils_setenv.py` & `easifem-23.7.0/src/easifem/utils_setenv.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/src/easifem/utils_uninstall.py` & `easifem-23.7.0/src/easifem/utils_uninstall.py`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/.gitignore` & `easifem-23.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/LICENSE.txt` & `easifem-23.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/README.md` & `easifem-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/pyproject.toml` & `easifem-23.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easifem-23.6.0/PKG-INFO` & `easifem-23.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easifem
-Version: 23.6.0
+Version: 23.7.0
 Summary: easifem is a command line interface for using EASIFEM library. Expandable And Scalable Infrastructure for Finite Element Methods, EASIFEM, is Modern Fortran framework for solving partial differential equations (PDEs) using finite element methods.
 Project-URL: Documentation, https://github.com/vickysharma0812/easifem#readme
 Project-URL: Issues, https://github.com/vickysharma0812/easifem/issues
 Project-URL: Source, https://github.com/vickysharma0812/easifem
 Author-email: Vikas Sharma <Vickysharma0812@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

