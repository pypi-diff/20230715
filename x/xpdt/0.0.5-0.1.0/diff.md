# Comparing `tmp/xpdt-0.0.5.tar.gz` & `tmp/xpdt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpdt-0.0.5.tar", last modified: Thu Jan  6 08:42:16 2022, max compression
+gzip compressed data, was "xpdt-0.1.0.tar", last modified: Sat Jul 15 02:03:13 2023, max compression
```

## Comparing `xpdt-0.0.5.tar` & `xpdt-0.1.0.tar`

### file list

```diff
@@ -1,73 +1,57 @@
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.372918 xpdt-0.0.5/
--rw-r-----   0 scara     (1000) scara     (1000)      177 2021-12-21 02:35:25.000000 xpdt-0.0.5/.gitignore
--rw-r-----   0 scara     (1000) scara     (1000)    35147 2021-05-22 04:38:57.000000 xpdt-0.0.5/LICENSE.txt
--rw-r-----   0 scara     (1000) scara     (1000)       90 2021-05-22 04:38:57.000000 xpdt-0.0.5/MANIFEST.in
--rw-r-----   0 scara     (1000) scara     (1000)      462 2021-12-21 02:35:25.000000 xpdt-0.0.5/Makefile
--rw-r-----   0 scara     (1000) scara     (1000)     4168 2022-01-06 08:42:16.372918 xpdt-0.0.5/PKG-INFO
--rw-r-----   0 scara     (1000) scara     (1000)     3178 2021-12-21 02:35:25.000000 xpdt-0.0.5/README.md
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.367918 xpdt-0.0.5/benchmark/
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.0.5/benchmark/__init__.py
--rw-r-----   0 scara     (1000) scara     (1000)     1586 2021-05-22 04:38:57.000000 xpdt-0.0.5/benchmark/__main__.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.367918 xpdt-0.0.5/examples/
--rw-r-----   0 scara     (1000) scara     (1000)      291 2021-12-21 02:35:25.000000 xpdt-0.0.5/examples/example1.xpdt
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.366918 xpdt-0.0.5/include/
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.368918 xpdt-0.0.5/include/xpdt/
--rw-r-----   0 scara     (1000) scara     (1000)     1886 2021-12-21 02:36:10.000000 xpdt-0.0.5/include/xpdt/xbuf.h
--rw-r-----   0 scara     (1000) scara     (1000)     2314 2021-12-21 02:35:25.000000 xpdt-0.0.5/include/xpdt/xbuf_iter.h
--rw-r-----   0 scara     (1000) scara     (1000)     2687 2021-12-21 02:35:25.000000 xpdt-0.0.5/include/xpdt/xfilemap.h
--rw-r-----   0 scara     (1000) scara     (1000)     1988 2021-12-21 02:36:10.000000 xpdt-0.0.5/include/xpdt/xpdt.h
--rw-r-----   0 scara     (1000) scara     (1000)     1665 2021-12-21 02:35:25.000000 xpdt-0.0.5/include/xpdt/xu128.h
--rwxr-x---   0 scara     (1000) scara     (1000)      191 2021-05-26 05:19:37.000000 xpdt-0.0.5/pre-commit.sh
--rw-r-----   0 scara     (1000) scara     (1000)       79 2022-01-06 08:42:16.372918 xpdt-0.0.5/setup.cfg
--rwxr-x---   0 scara     (1000) scara     (1000)     1572 2021-12-22 03:35:14.000000 xpdt-0.0.5/setup.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.368918 xpdt-0.0.5/test/
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.0.5/test/__init__.py
--rw-r-----   0 scara     (1000) scara     (1000)     2024 2021-12-21 02:36:10.000000 xpdt-0.0.5/test/test_decode.py
--rw-r-----   0 scara     (1000) scara     (1000)     1167 2022-01-06 08:30:19.000000 xpdt-0.0.5/test/test_enums.py
--rw-r-----   0 scara     (1000) scara     (1000)     1273 2021-12-21 02:35:25.000000 xpdt-0.0.5/test/test_nested.py
--rw-r-----   0 scara     (1000) scara     (1000)     2266 2021-12-21 02:35:25.000000 xpdt-0.0.5/test/test_parser.py
--rw-r-----   0 scara     (1000) scara     (1000)     1597 2021-12-21 02:35:25.000000 xpdt-0.0.5/test/test_roundtrip.py
--rw-r-----   0 scara     (1000) scara     (1000)     2007 2021-12-21 02:35:25.000000 xpdt-0.0.5/test/test_stringy.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.370918 xpdt-0.0.5/xpdt/
--rw-r-----   0 scara     (1000) scara     (1000)      801 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/__init__.py
--rw-r-----   0 scara     (1000) scara     (1000)     3637 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/__main__.py
--rw-r-----   0 scara     (1000) scara     (1000)      282 2022-01-06 08:41:56.000000 xpdt-0.0.5/xpdt/__version__.py
--rw-r-----   0 scara     (1000) scara     (1000)     1477 2022-01-06 08:31:08.000000 xpdt-0.0.5/xpdt/basetypes.py
--rw-r-----   0 scara     (1000) scara     (1000)     1799 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/buftypes.py
--rw-r-----   0 scara     (1000) scara     (1000)      505 2021-05-22 04:38:57.000000 xpdt-0.0.5/xpdt/c.py
--rw-r-----   0 scara     (1000) scara     (1000)      587 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/decl.py
--rw-r-----   0 scara     (1000) scara     (1000)      222 2021-05-26 05:19:37.000000 xpdt-0.0.5/xpdt/dupes.py
--rw-r-----   0 scara     (1000) scara     (1000)     1107 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/integraltype.py
--rw-r-----   0 scara     (1000) scara     (1000)      799 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/intstack.py
--rw-r-----   0 scara     (1000) scara     (1000)     1586 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/jinja.py
--rw-r-----   0 scara     (1000) scara     (1000)     1507 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/lex.py
--rw-r-----   0 scara     (1000) scara     (1000)     1891 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/load.py
--rw-r-----   0 scara     (1000) scara     (1000)      726 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/member.py
--rw-r-----   0 scara     (1000) scara     (1000)     4642 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/namespace.py
--rw-r-----   0 scara     (1000) scara     (1000)     5165 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/parse.py
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.0.5/xpdt/py.typed
--rw-r-----   0 scara     (1000) scara     (1000)     2491 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/shiftreduce.py
--rw-r-----   0 scara     (1000) scara     (1000)     7269 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/struct.py
--rw-r-----   0 scara     (1000) scara     (1000)     3078 2021-12-21 02:35:25.000000 xpdt-0.0.5/xpdt/symbology.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.372918 xpdt-0.0.5/xpdt/templates/
--rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.0.5/xpdt/templates/__init__.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.372918 xpdt-0.0.5/xpdt/templates/__pycache__/
--rw-r-----   0 scara     (1000) scara     (1000)      140 2021-12-04 01:49:09.000000 xpdt-0.0.5/xpdt/templates/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 scara     (1000) scara     (1000)      138 2021-07-11 02:04:47.000000 xpdt-0.0.5/xpdt/templates/__pycache__/__init__.cpython-39.pyc
--rw-r-----   0 scara     (1000) scara     (1000)      919 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/api.c
--rw-r-----   0 scara     (1000) scara     (1000)      543 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/apihdr.c
--rw-r-----   0 scara     (1000) scara     (1000)     2151 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/fixed.pyt
--rw-r-----   0 scara     (1000) scara     (1000)    11792 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/macros.c
--rw-r-----   0 scara     (1000) scara     (1000)     4088 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/vbuf.pyt
--rw-r-----   0 scara     (1000) scara     (1000)     1765 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/templates/xpdt.c
--rw-r-----   0 scara     (1000) scara     (1000)     7750 2022-01-06 08:41:40.000000 xpdt-0.0.5/xpdt/templates/xpdt.pyt
--rw-r-----   0 scara     (1000) scara     (1000)     2434 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/type.py
--rw-r-----   0 scara     (1000) scara     (1000)      150 2021-05-22 04:38:57.000000 xpdt-0.0.5/xpdt/typedef.py
--rw-r-----   0 scara     (1000) scara     (1000)      511 2021-12-21 02:36:10.000000 xpdt-0.0.5/xpdt/uuidtype.py
-drwxr-x---   0 scara     (1000) scara     (1000)        0 2022-01-06 08:42:16.371918 xpdt-0.0.5/xpdt.egg-info/
--rw-r-----   0 scara     (1000) scara     (1000)     4168 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/PKG-INFO
--rw-r-----   0 scara     (1000) scara     (1000)     1230 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/SOURCES.txt
--rw-r-----   0 scara     (1000) scara     (1000)        1 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/dependency_links.txt
--rw-r-----   0 scara     (1000) scara     (1000)       45 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/entry_points.txt
--rw-r-----   0 scara     (1000) scara     (1000)       12 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/requires.txt
--rw-r-----   0 scara     (1000) scara     (1000)        5 2022-01-06 08:42:16.000000 xpdt-0.0.5/xpdt.egg-info/top_level.txt
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.487199 xpdt-0.1.0/
+-rw-r-----   0 scara     (1000) scara     (1000)    35147 2021-05-22 04:38:57.000000 xpdt-0.1.0/LICENSE.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       90 2021-05-22 04:38:57.000000 xpdt-0.1.0/MANIFEST.in
+-rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-15 02:03:13.487199 xpdt-0.1.0/PKG-INFO
+-rw-r-----   0 scara     (1000) scara     (1000)     3178 2023-07-09 09:54:10.000000 xpdt-0.1.0/README.md
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.482199 xpdt-0.1.0/examples/
+-rw-r-----   0 scara     (1000) scara     (1000)      291 2023-07-09 09:54:10.000000 xpdt-0.1.0/examples/example1.xpdt
+-rw-r-----   0 scara     (1000) scara     (1000)       79 2023-07-15 02:03:13.487199 xpdt-0.1.0/setup.cfg
+-rwxr-x---   0 scara     (1000) scara     (1000)     1600 2023-07-09 09:54:10.000000 xpdt-0.1.0/setup.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.484199 xpdt-0.1.0/test/
+-rw-r-----   0 scara     (1000) scara     (1000)     2024 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_decode.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1167 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_enums.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1273 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_nested.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2266 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_parser.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1597 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_roundtrip.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2007 2023-07-09 09:54:10.000000 xpdt-0.1.0/test/test_stringy.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.486199 xpdt-0.1.0/xpdt/
+-rw-r-----   0 scara     (1000) scara     (1000)      801 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/__init__.py
+-rw-r-----   0 scara     (1000) scara     (1000)     3720 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/__main__.py
+-rw-r-----   0 scara     (1000) scara     (1000)      282 2023-07-15 02:01:41.000000 xpdt-0.1.0/xpdt/__version__.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1477 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/basetypes.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1799 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/buftypes.py
+-rw-r-----   0 scara     (1000) scara     (1000)      505 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/c.py
+-rw-r-----   0 scara     (1000) scara     (1000)      587 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/decl.py
+-rw-r-----   0 scara     (1000) scara     (1000)      222 2021-05-26 05:19:37.000000 xpdt-0.1.0/xpdt/dupes.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1107 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/integraltype.py
+-rw-r-----   0 scara     (1000) scara     (1000)      799 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/intstack.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1586 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/jinja.py
+-rw-r-----   0 scara     (1000) scara     (1000)     1506 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/lex.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2091 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/load.py
+-rw-r-----   0 scara     (1000) scara     (1000)      726 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/member.py
+-rw-r-----   0 scara     (1000) scara     (1000)     4768 2023-07-09 10:14:27.000000 xpdt-0.1.0/xpdt/namespace.py
+-rw-r-----   0 scara     (1000) scara     (1000)     5165 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/parse.py
+-rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/py.typed
+-rw-r-----   0 scara     (1000) scara     (1000)     5013 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/registry.py
+-rw-r-----   0 scara     (1000) scara     (1000)     2583 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/shiftreduce.py
+-rw-r-----   0 scara     (1000) scara     (1000)     7269 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/struct.py
+-rw-r-----   0 scara     (1000) scara     (1000)     3078 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/symbology.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.487199 xpdt-0.1.0/xpdt/templates/
+-rw-r-----   0 scara     (1000) scara     (1000)        0 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/templates/__init__.py
+-rw-r-----   0 scara     (1000) scara     (1000)      664 2023-07-09 10:21:23.000000 xpdt-0.1.0/xpdt/templates/api.c
+-rw-r-----   0 scara     (1000) scara     (1000)      385 2023-07-09 09:56:13.000000 xpdt-0.1.0/xpdt/templates/apihdr.c
+-rw-r-----   0 scara     (1000) scara     (1000)     2151 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/fixed.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)    12735 2023-07-09 10:16:00.000000 xpdt-0.1.0/xpdt/templates/macros.c
+-rw-r-----   0 scara     (1000) scara     (1000)     4088 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/vbuf.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)     1765 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/xpdt.c
+-rw-r-----   0 scara     (1000) scara     (1000)     7750 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/templates/xpdt.pyt
+-rw-r-----   0 scara     (1000) scara     (1000)     2434 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/type.py
+-rw-r-----   0 scara     (1000) scara     (1000)      150 2021-05-22 04:38:57.000000 xpdt-0.1.0/xpdt/typedef.py
+-rw-r-----   0 scara     (1000) scara     (1000)      511 2023-07-09 09:54:10.000000 xpdt-0.1.0/xpdt/uuidtype.py
+drwxr-x---   0 scara     (1000) scara     (1000)        0 2023-07-15 02:03:13.486199 xpdt-0.1.0/xpdt.egg-info/
+-rw-r-----   0 scara     (1000) scara     (1000)     4166 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/PKG-INFO
+-rw-r-----   0 scara     (1000) scara     (1000)      939 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/SOURCES.txt
+-rw-r-----   0 scara     (1000) scara     (1000)        1 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/dependency_links.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       44 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/entry_points.txt
+-rw-r-----   0 scara     (1000) scara     (1000)       12 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/requires.txt
+-rw-r-----   0 scara     (1000) scara     (1000)        5 2023-07-15 02:03:13.000000 xpdt-0.1.0/xpdt.egg-info/top_level.txt
```

### Comparing `xpdt-0.0.5/LICENSE.txt` & `xpdt-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/PKG-INFO` & `xpdt-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpdt
-Version: 0.0.5
+Version: 0.1.0
 Summary: eXPeditious Data Transfer
 Home-page: https://github.com/giannitedesco/xpdt
 Author: Gianni Tedesco
 Author-email: gianni@scaramanga.co.uk
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -127,9 +127,7 @@
 
 # License
 The compiler is released under the GPLv3.
 
 The C support code/headers are released under the MIT license.
 
 The generated code is yours.
-
-
```

### Comparing `xpdt-0.0.5/README.md` & `xpdt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/benchmark/__main__.py` & `xpdt-0.1.0/test/test_roundtrip.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-from timeit import default_timer as timer
-from pathlib import Path
+import unittest
 
 from xpdt import NameSpace, StructDef, MemberDef, BaseType
 
-
-def main():
-    cls = NameSpace(
-        structs=(
-            StructDef(
-                name='SomeStruct',
-                members=(
-                    MemberDef('a', BaseType.u64),
-                    MemberDef('b', BaseType.u64),
-                    MemberDef('c', BaseType.u64),
-                    MemberDef('d', BaseType.u64),
-                    MemberDef('e', BaseType.u64),
-                    MemberDef('f', BaseType.u64),
-                    MemberDef('g', BaseType.u64),
-                    MemberDef('h', BaseType.u64),
-                    MemberDef('i', BaseType.u64),
-                    MemberDef('j', BaseType.u64),
-                    MemberDef('k', BaseType.u64),
-                    MemberDef('l', BaseType.u64),
-                    MemberDef('m', BaseType.u64),
-                    MemberDef('n', BaseType.u64),
-                    MemberDef('o', BaseType.u64),
-                    MemberDef('p', BaseType.u64),
+class Test_RoundTrips(unittest.TestCase):
+    def setUp(self):
+        self.code = NameSpace(
+            structs=(
+                StructDef(
+                    name='Point',
+                    members=(
+                        MemberDef('x', BaseType.i32),
+                        MemberDef('y', BaseType.i32),
+                        MemberDef('z', BaseType.i32),
+                        MemberDef('_pad0', BaseType.i32),
+                        MemberDef('_pad1', BaseType.bytes),
+                    ),
+                ),
+                StructDef(
+                    name='Item',
+                    members=(
+                        MemberDef('uuid', BaseType.uuid),
+                        MemberDef('id', BaseType.u32),
+                        MemberDef('first_name', BaseType.utf8),
+                        MemberDef('surname', BaseType.utf8),
+                        MemberDef('data', BaseType.bytes),
+                        MemberDef('_pad0', BaseType.i32),
+                        MemberDef('_pad1', BaseType.bytes),
+                    ),
                 ),
             ),
-        ),
-    ).gen_dynamic_python().SomeStruct
-
-    sz = cls._bin_size
+            name=None,
+        ).gen_dynamic_python()
 
-    with Path('/dev/zero').open('rb') as f:
-        iters = 1000000
-        start = timer()
-        for i in range(iters):
-            buf = f.read(sz)
-            obj = cls._frombytes(buf)
-        end = timer()
-        elapsed = end - start
-        per_iter = elapsed / iters
-        print(f'{elapsed:.2f} sec elapsed')
-        print(f'{per_iter*1e9:.0f} nsec per record')
+    def test_point(self):
+        orig = self.code.Point(1, -2, 3)
+        b = bytes(orig)
+        clone = orig._frombytes(b)
+        self.assertEqual(orig, clone)
 
 
-if __name__ == '__main__':
-    main()
+    def test_item(self):
+        orig = self.code.Item(b'\x00' * 16, 0xdeadbeef, 'Malkovich', '', b'\x12\x34')
+        b = bytes(orig)
+        clone = orig._frombytes(b)
+        self.assertEqual(orig, clone)
```

### Comparing `xpdt-0.0.5/setup.py` & `xpdt-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     long_description=Path('README.md').read_text(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     license=v['__license__'],
     platforms='any',
     packages=[
         pkg,
+        f'{pkg}.templates',
     ],
     url=v['__url__'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: POSIX',
```

### Comparing `xpdt-0.0.5/test/test_decode.py` & `xpdt-0.1.0/test/test_decode.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/test/test_enums.py` & `xpdt-0.1.0/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/test/test_nested.py` & `xpdt-0.1.0/test/test_nested.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/test/test_parser.py` & `xpdt-0.1.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/test/test_stringy.py` & `xpdt-0.1.0/test/test_stringy.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/__init__.py` & `xpdt-0.1.0/xpdt/__init__.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/__main__.py` & `xpdt-0.1.0/xpdt/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from xpdt import NameSpace, load
 
 _fmt = logging.Formatter('%(message)s')
 _stdio_handler = logging.StreamHandler(stream=stdout)
 _stdio_handler.setFormatter(_fmt)
-_log = logging.getLogger('xpdt')
+_log = logging.getLogger(__package__)
 _log.addHandler(_stdio_handler)
 
 
 class BackendDef:
     suffix: ClassVar[str]
 
     __slots__ = (
@@ -74,14 +74,24 @@
     suffix = '.py'
     __slots__ = ()
 
     def _gen(self, f: TextIO) -> None:
         self._ns.gen_python(f)
 
 
+_c_lang = (OutputC, OutputCAPI, OutputCHdr)
+_py_lang = (OutputPy,)
+
+backends = {
+    'c': _c_lang,
+    'python': _py_lang,
+    'py': _py_lang,
+}
+
+
 def main() -> None:
     opts = ArgumentParser(description='xpdt: eXPeditious Data Transfer')
     opts.add_argument('--verbose', '-v',
                       action='count',
                       default=0,
                       help='Be more talkative')
     opts.add_argument('--registry', '-r',
@@ -91,15 +101,15 @@
     opts.add_argument('--module-name', '-n',
                       default=None,
                       type=str,
                       help='Name of module (output file)')
     opts.add_argument('--language', '-l',
                       default='c',
                       type=str,
-                      help='Output language')
+                      help='Output language: %s' % ', '.join(backends.keys()))
     opts.add_argument('--out', '-o',
                       default=Path(),
                       type=Path,
                       help='Output dir')
     opts.add_argument('-I',
                       dest='inc_prefix',
                       help='Include path (for C headers)')
@@ -119,28 +129,21 @@
         registry=args.registry,
         module_name=args.module_name,
     )
 
     if ns.name is None:
         ns.name = 'xpdt'
 
-    backends = {
-        'c': OutputC,
-        'capi': OutputCAPI,
-        'chdr': OutputCHdr,
-        'py': OutputPy,
-        'python': OutputPy,
-    }
-
     try:
-        cls = backends[args.language]
+        file_generators = backends[args.language]
     except KeyError:
         print(f'Unknown language: "{args.language}"')
         raise SystemExit(1)
 
     args.out.mkdir(exist_ok=True)
-    backend = cls(ns, args.out, args.inc_prefix)
-    backend.gen()
+    for cls in file_generators:
+        backend = cls(ns, args.out, args.inc_prefix)
+        backend.gen()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `xpdt-0.0.5/xpdt/basetypes.py` & `xpdt-0.1.0/xpdt/basetypes.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/buftypes.py` & `xpdt-0.1.0/xpdt/buftypes.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/decl.py` & `xpdt-0.1.0/xpdt/decl.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/integraltype.py` & `xpdt-0.1.0/xpdt/integraltype.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/intstack.py` & `xpdt-0.1.0/xpdt/intstack.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/jinja.py` & `xpdt-0.1.0/xpdt/jinja.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/lex.py` & `xpdt-0.1.0/xpdt/lex.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         m = _dfa.match(s, pos)
         if not m:
             break
         grp = m.lastgroup
         begin, end = m.span()
         pos = end
         if grp not in _ignored:
-            assert(grp is not None)
+            assert grp is not None
             yield Lexeme(grp, s[begin:end], file, line)
         elif grp == 'newline':
             line += 1
 
     if pos < len(s):
         bad = s[pos:]
         if len(bad) > 32:
```

### Comparing `xpdt-0.0.5/xpdt/member.py` & `xpdt-0.1.0/xpdt/member.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/namespace.py` & `xpdt-0.1.0/xpdt/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
         self._name = name
 
         # TODO: Allow sub-structs
         self._structs = {s.name: s for s in structs}
 
     @property
+    def needs_discr_enum(self) -> bool:
+        return any(s.has_discriminant for s in self._structs.values())
+
+    @property
     def name(self) -> Optional[str]:
         return self._name
 
     @name.setter
     def name(self, name: Optional[str]) -> None:
         self._name = name
```

### Comparing `xpdt-0.0.5/xpdt/parse.py` & `xpdt-0.1.0/xpdt/parse.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/shiftreduce.py` & `xpdt-0.1.0/xpdt/shiftreduce.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,17 +48,22 @@
 
 _T = TypeVar('_T')
 
 
 class State(Generic[_T]):
     __slots__ = ()
 
-    def on(self: _T, *args: str) -> Callable[..., StateFunc[_T]]: ...
-    def default(self: _T) -> Callable[..., StateFunc[_T]]: ...
-    def __call__(self: _T, tok: Token) -> NextState[_T]: ...
+    def on(self: _T, *args: str) -> Callable[..., StateFunc[_T]]:
+        raise NotImplementedError
+
+    def default(self: _T) -> Callable[..., StateFunc[_T]]:
+        raise NotImplementedError
+
+    def __call__(self: _T, tok: Token) -> NextState[_T]:
+        raise NotImplementedError
 
 
 NextState = Optional[State[_T]]
 StateFunc = Callable[[_T, Token], NextState[_T]]
 
 
 def state(func: Callable[[_T], None]) -> State[_T]:
```

### Comparing `xpdt-0.0.5/xpdt/struct.py` & `xpdt-0.1.0/xpdt/struct.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/symbology.py` & `xpdt-0.1.0/xpdt/symbology.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/templates/fixed.pyt` & `xpdt-0.1.0/xpdt/templates/fixed.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/templates/macros.c` & `xpdt-0.1.0/xpdt/templates/macros.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 /*#- macro init_macro_name(struct) -#*/
 /*{struct.name.upper()}*/_INIT
 /*#- endmacro #*/
 
 
+/*#- macro struct_enum_entry(namespace, struct) -#*/
+/*{namespace.name.upper()}*/_/*{struct.name.upper()}*/
+/*#- endmacro #*/
+
+
 /*#- macro ctor(struct) -#*/
 /*{struct.name}*/__new
 /*#- endmacro -#*/
 
 
 /*#- macro fixed_ctor(struct) -#*/
 /*{struct.name}*/__fixed
@@ -159,14 +164,49 @@
 // for member in struct
 	/*{member.cdecl}*/;
 // endfor
 }/*{naturally_packed(struct)}*/;
 /*#- endmacro -#*/
 
 
+/*#- macro entry_name(namespace, struct) -#*/
+/*{namespace.name}*/_/*{struct.name}*/
+/*#- endmacro #*/
+
+
+/*#- macro cdecls(struct) -#*/
+/*{struct.non_reserved_members
+	| map(attribute="const_cdecl")
+	| join(",\n\t\t")}*/
+/*#- endmacro -#*/
+
+
+/*#- macro stream(namespace) -#*/
+/*{namespace.name}*/_xostream
+/*#- endmacro #*/
+
+
+################################################################################
+/*# macro discr_enum(namespace) #*/
+/*# if namespace.needs_discr_enum #*/
+
+typedef enum /*{namespace.name}*/_discr_e
+#if __GNUC__ >= 13
+: xpdt_discriminant_t
+#endif
+{
+/*# for struct in namespace #*/
+/*# if struct.has_discriminant #*/
+	/*{struct_enum_entry(namespace, struct)}*/ = 0x/*{struct.discriminant|hex32}*/,
+/*# endif #*/
+/*# endfor #*/
+} /*{namespace.name}*/_discr_t;
+/*# endif #*/
+/*# endmacro #*/
+
 ################################################################################
 /*# macro fixed_struct_decl(struct) #*/
 
 /*{fixed(struct)}*/ {
 // for member in struct
 // if member.needs_vbuf
 // if member.is_scalar
@@ -513,15 +553,15 @@
 /*{struct.ctype}*/
 /*{construct(struct)}*/(const /*{struct_fixed(struct)}*/ *rec, const /*{ptrs_struct(struct)}*/ *ptrs)
 {
 	return (/*{struct.ctype}*/){
 // for member in struct.non_reserved_members
 // if member.needs_vbuf
 // if member.is_scalar
-		./*{member.name}*/ = xbuf(rec->/*{member.name}*/, ptrs->/*{member.name}*/),
+		./*{member.name}*/ = xbuf(ptrs->/*{member.name}*/, rec->/*{member.name}*/),
 // else
 		./*{member.name}*/ = /*{member.type.struct.name}*/_construct(&rec->/*{member.name}*/, &ptrs->/*{member.name}*/),
 // endif
 // else
 		./*{member.name}*/ = rec->/*{member.name}*/,
 // endif
 // endfor
```

### Comparing `xpdt-0.0.5/xpdt/templates/vbuf.pyt` & `xpdt-0.1.0/xpdt/templates/vbuf.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/templates/xpdt.c` & `xpdt-0.1.0/xpdt/templates/xpdt.c`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/templates/xpdt.pyt` & `xpdt-0.1.0/xpdt/templates/xpdt.pyt`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt/type.py` & `xpdt-0.1.0/xpdt/type.py`

 * *Files identical despite different names*

### Comparing `xpdt-0.0.5/xpdt.egg-info/PKG-INFO` & `xpdt-0.1.0/xpdt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpdt
-Version: 0.0.5
+Version: 0.1.0
 Summary: eXPeditious Data Transfer
 Home-page: https://github.com/giannitedesco/xpdt
 Author: Gianni Tedesco
 Author-email: gianni@scaramanga.co.uk
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -127,9 +127,7 @@
 
 # License
 The compiler is released under the GPLv3.
 
 The C support code/headers are released under the MIT license.
 
 The generated code is yours.
-
-
```

### Comparing `xpdt-0.0.5/xpdt.egg-info/SOURCES.txt` & `xpdt-0.1.0/xpdt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-.gitignore
 LICENSE.txt
 MANIFEST.in
-Makefile
 README.md
-pre-commit.sh
 setup.cfg
 setup.py
-benchmark/__init__.py
-benchmark/__main__.py
 examples/example1.xpdt
-include/xpdt/xbuf.h
-include/xpdt/xbuf_iter.h
-include/xpdt/xfilemap.h
-include/xpdt/xpdt.h
-include/xpdt/xu128.h
-test/__init__.py
 test/test_decode.py
 test/test_enums.py
 test/test_nested.py
 test/test_parser.py
 test/test_roundtrip.py
 test/test_stringy.py
 xpdt/__init__.py
@@ -34,14 +23,15 @@
 xpdt/jinja.py
 xpdt/lex.py
 xpdt/load.py
 xpdt/member.py
 xpdt/namespace.py
 xpdt/parse.py
 xpdt/py.typed
+xpdt/registry.py
 xpdt/shiftreduce.py
 xpdt/struct.py
 xpdt/symbology.py
 xpdt/type.py
 xpdt/typedef.py
 xpdt/uuidtype.py
 xpdt.egg-info/PKG-INFO
@@ -53,10 +43,8 @@
 xpdt/templates/__init__.py
 xpdt/templates/api.c
 xpdt/templates/apihdr.c
 xpdt/templates/fixed.pyt
 xpdt/templates/macros.c
 xpdt/templates/vbuf.pyt
 xpdt/templates/xpdt.c
-xpdt/templates/xpdt.pyt
-xpdt/templates/__pycache__/__init__.cpython-310.pyc
-xpdt/templates/__pycache__/__init__.cpython-39.pyc
+xpdt/templates/xpdt.pyt
```

