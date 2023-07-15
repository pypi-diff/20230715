# Comparing `tmp/morphoaap-0.0.3.tar.gz` & `tmp/morphoaap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphoaap-0.0.3.tar", last modified: Sat Jul 15 17:01:16 2023, max compression
+gzip compressed data, was "morphoaap-0.0.4.tar", last modified: Sat Jul 15 17:25:50 2023, max compression
```

## Comparing `morphoaap-0.0.3.tar` & `morphoaap-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:01:16.339725 morphoaap-0.0.3/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1165 2023-07-14 16:12:06.000000 morphoaap-0.0.3/CMakeLists.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)    35149 2023-07-13 11:33:07.000000 morphoaap-0.0.3/LICENSE
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      111 2023-07-14 16:12:23.000000 morphoaap-0.0.3/MANIFEST.in
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      507 2023-07-15 17:01:16.339353 morphoaap-0.0.3/PKG-INFO
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       33 2023-07-13 13:11:59.000000 morphoaap-0.0.3/README.md
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:01:16.333530 morphoaap-0.0.3/morphoaap/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     3074 2023-07-15 16:11:57.000000 morphoaap-0.0.3/morphoaap/CMakeLists.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       67 2023-07-14 16:57:27.000000 morphoaap-0.0.3/morphoaap/__init__.py
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     2455 2023-07-14 16:20:27.000000 morphoaap-0.0.3/morphoaap/aap.cpp
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:01:16.336957 morphoaap-0.0.3/morphoaap/include/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1707 2023-07-14 16:10:54.000000 morphoaap-0.0.3/morphoaap/include/AttributeComputedIncrementally.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     4432 2023-07-14 16:10:59.000000 morphoaap-0.0.3/morphoaap/include/AttributeFilters.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      574 2023-07-14 16:11:02.000000 morphoaap-0.0.3/morphoaap/include/AttributeProfile.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1020 2023-07-14 16:11:06.000000 morphoaap-0.0.3/morphoaap/include/ComponentTree.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      731 2023-07-14 16:11:10.000000 morphoaap-0.0.3/morphoaap/include/ComputerMSER.hpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      479 2023-07-11 21:03:13.000000 morphoaap-0.0.3/morphoaap/include/NodeCT.hpp
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:01:16.338906 morphoaap-0.0.3/morphoaap/src/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      569 2023-07-14 16:11:20.000000 morphoaap-0.0.3/morphoaap/src/AttributeComputedIncrementally.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     1784 2023-07-14 16:11:23.000000 morphoaap-0.0.3/morphoaap/src/AttributeFilters.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     2980 2023-07-14 16:11:26.000000 morphoaap-0.0.3/morphoaap/src/AttributeProfile.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     5370 2023-07-14 16:11:30.000000 morphoaap-0.0.3/morphoaap/src/ComponentTree.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     4239 2023-07-14 16:11:33.000000 morphoaap-0.0.3/morphoaap/src/ComputerMSER.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      709 2023-07-14 16:11:37.000000 morphoaap-0.0.3/morphoaap/src/NodeCT.cpp
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      874 2023-07-14 16:19:49.000000 morphoaap-0.0.3/morphoaap/test.py
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       21 2023-07-14 11:33:58.000000 morphoaap-0.0.3/morphoaap/version.py
-drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:01:16.334885 morphoaap-0.0.3/morphoaap.egg-info/
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      507 2023-07-15 17:01:16.000000 morphoaap-0.0.3/morphoaap.egg-info/PKG-INFO
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      742 2023-07-15 17:01:16.000000 morphoaap-0.0.3/morphoaap.egg-info/SOURCES.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-07-15 17:01:16.000000 morphoaap-0.0.3/morphoaap.egg-info/dependency_links.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       10 2023-07-15 17:01:16.000000 morphoaap-0.0.3/morphoaap.egg-info/top_level.txt
--rw-r--r--   0 wonderalexandre   (501) staff       (20)      338 2023-07-14 11:21:09.000000 morphoaap-0.0.3/pybind11.cmake
--rw-r--r--   0 wonderalexandre   (501) staff       (20)       38 2023-07-15 17:01:16.339849 morphoaap-0.0.3/setup.cfg
--rw-r--r--   0 wonderalexandre   (501) staff       (20)     2658 2023-07-15 17:00:49.000000 morphoaap-0.0.3/setup.py
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:25:50.533213 morphoaap-0.0.4/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1165 2023-07-14 16:12:06.000000 morphoaap-0.0.4/CMakeLists.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)    35149 2023-07-13 11:33:07.000000 morphoaap-0.0.4/LICENSE
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      111 2023-07-14 16:12:23.000000 morphoaap-0.0.4/MANIFEST.in
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      507 2023-07-15 17:25:50.532783 morphoaap-0.0.4/PKG-INFO
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       33 2023-07-13 13:11:59.000000 morphoaap-0.0.4/README.md
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:25:50.525388 morphoaap-0.0.4/morphoaap/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     3074 2023-07-15 16:11:57.000000 morphoaap-0.0.4/morphoaap/CMakeLists.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       96 2023-07-15 17:08:14.000000 morphoaap-0.0.4/morphoaap/__init__.py
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     2455 2023-07-14 16:20:27.000000 morphoaap-0.0.4/morphoaap/aap.cpp
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:25:50.529624 morphoaap-0.0.4/morphoaap/include/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1707 2023-07-14 16:10:54.000000 morphoaap-0.0.4/morphoaap/include/AttributeComputedIncrementally.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     4432 2023-07-14 16:10:59.000000 morphoaap-0.0.4/morphoaap/include/AttributeFilters.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      574 2023-07-14 16:11:02.000000 morphoaap-0.0.4/morphoaap/include/AttributeProfile.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1020 2023-07-14 16:11:06.000000 morphoaap-0.0.4/morphoaap/include/ComponentTree.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      731 2023-07-14 16:11:10.000000 morphoaap-0.0.4/morphoaap/include/ComputerMSER.hpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      479 2023-07-11 21:03:13.000000 morphoaap-0.0.4/morphoaap/include/NodeCT.hpp
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:25:50.532134 morphoaap-0.0.4/morphoaap/src/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      569 2023-07-14 16:11:20.000000 morphoaap-0.0.4/morphoaap/src/AttributeComputedIncrementally.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     1784 2023-07-14 16:11:23.000000 morphoaap-0.0.4/morphoaap/src/AttributeFilters.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     2980 2023-07-14 16:11:26.000000 morphoaap-0.0.4/morphoaap/src/AttributeProfile.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     5370 2023-07-14 16:11:30.000000 morphoaap-0.0.4/morphoaap/src/ComponentTree.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     4239 2023-07-14 16:11:33.000000 morphoaap-0.0.4/morphoaap/src/ComputerMSER.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      709 2023-07-14 16:11:37.000000 morphoaap-0.0.4/morphoaap/src/NodeCT.cpp
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      874 2023-07-14 16:19:49.000000 morphoaap-0.0.4/morphoaap/test.py
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       21 2023-07-14 11:33:58.000000 morphoaap-0.0.4/morphoaap/version.py
+drwxr-xr-x   0 wonderalexandre   (501) staff       (20)        0 2023-07-15 17:25:50.526777 morphoaap-0.0.4/morphoaap.egg-info/
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      507 2023-07-15 17:25:49.000000 morphoaap-0.0.4/morphoaap.egg-info/PKG-INFO
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      742 2023-07-15 17:25:50.000000 morphoaap-0.0.4/morphoaap.egg-info/SOURCES.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)        1 2023-07-15 17:25:49.000000 morphoaap-0.0.4/morphoaap.egg-info/dependency_links.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       10 2023-07-15 17:25:49.000000 morphoaap-0.0.4/morphoaap.egg-info/top_level.txt
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)      338 2023-07-14 11:21:09.000000 morphoaap-0.0.4/pybind11.cmake
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)       38 2023-07-15 17:25:50.533326 morphoaap-0.0.4/setup.cfg
+-rw-r--r--   0 wonderalexandre   (501) staff       (20)     2659 2023-07-15 17:25:42.000000 morphoaap-0.0.4/setup.py
```

### Comparing `morphoaap-0.0.3/CMakeLists.txt` & `morphoaap-0.0.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/LICENSE` & `morphoaap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/CMakeLists.txt` & `morphoaap-0.0.4/morphoaap/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/aap.cpp` & `morphoaap-0.0.4/morphoaap/aap.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/include/AttributeComputedIncrementally.hpp` & `morphoaap-0.0.4/morphoaap/include/AttributeComputedIncrementally.hpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/include/AttributeFilters.hpp` & `morphoaap-0.0.4/morphoaap/include/AttributeFilters.hpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/include/AttributeProfile.hpp` & `morphoaap-0.0.4/morphoaap/include/AttributeProfile.hpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/include/ComponentTree.hpp` & `morphoaap-0.0.4/morphoaap/include/ComponentTree.hpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/include/ComputerMSER.hpp` & `morphoaap-0.0.4/morphoaap/include/ComputerMSER.hpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/AttributeComputedIncrementally.cpp` & `morphoaap-0.0.4/morphoaap/src/AttributeComputedIncrementally.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/AttributeFilters.cpp` & `morphoaap-0.0.4/morphoaap/src/AttributeFilters.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/AttributeProfile.cpp` & `morphoaap-0.0.4/morphoaap/src/AttributeProfile.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/ComponentTree.cpp` & `morphoaap-0.0.4/morphoaap/src/ComponentTree.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/ComputerMSER.cpp` & `morphoaap-0.0.4/morphoaap/src/ComputerMSER.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/src/NodeCT.cpp` & `morphoaap-0.0.4/morphoaap/src/NodeCT.cpp`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap/test.py` & `morphoaap-0.0.4/morphoaap/test.py`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/morphoaap.egg-info/SOURCES.txt` & `morphoaap-0.0.4/morphoaap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphoaap-0.0.3/setup.py` & `morphoaap-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             try:
                 cmake_configure_command = [
                     'cmake',
                     '-H{0}'.format(_source_dir),
                     '-B{0}'.format(_build_dir),
                     '-DCMAKE_INSTALL_PREFIX={0}'.format(_prefix),
                    # '-DTYPE_EXECUTABLE={0}'.format(sys.executable),
-                    '-DPYTHON_LIBRARY_DIR={0}'.format(_prefix),
+                    #'-DPYTHON_LIBRARY_DIR={0}'.format(_prefix),
                 ]
                 _generator = os.getenv('CMAKE_GENERATOR')
                 if _generator is not None:
                     cmake_configure_command.append('-G{0}'.format(_generator))
                 spawn.spawn(cmake_configure_command)
                 spawn.spawn(
                     ['cmake', '--build', _build_dir, '--target', 'install'])
@@ -54,15 +54,15 @@
 
 version = {}
 with open(os.path.join(_here, _this_package, 'version.py')) as f:
     exec(f.read(), version)
 
 setup(
     name="morphoaap",
-    version="0.0.3",
+    version="0.0.4",
     description='A simple library for adative attribute profiles',
     long_description="",
     author='Wonder Alexandre Luz Alves',
     author_email='wonderalexandre@gmail.com',
     license='GPL-3.0',
     url = 'https://github.com/wonderalexandre/aap',
     packages=[_this_package],
```

