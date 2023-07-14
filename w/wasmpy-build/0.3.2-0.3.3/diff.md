# Comparing `tmp/wasmpy-build-0.3.2.tar.gz` & `tmp/wasmpy-build-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.3.2.tar", last modified: Fri Jul 14 11:04:08 2023, max compression
+gzip compressed data, was "wasmpy-build-0.3.3.tar", last modified: Fri Jul 14 23:44:30 2023, max compression
```

## Comparing `wasmpy-build-0.3.2.tar` & `wasmpy-build-0.3.3.tar`

### file list

```diff
@@ -1,682 +1,682 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.904367 wasmpy-build-0.3.2/
--rw-rw-rw-   0        0        0     1068 2023-07-13 12:38:30.000000 wasmpy-build-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1686 2023-07-14 11:04:08.903367 wasmpy-build-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      940 2023-07-14 10:51:14.000000 wasmpy-build-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-14 11:04:08.904367 wasmpy-build-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-07-14 10:55:36.000000 wasmpy-build-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.626880 wasmpy-build-0.3.2/wasmpy_build/
--rw-rw-rw-   0        0        0     2221 2023-07-14 10:38:29.000000 wasmpy-build-0.3.2/wasmpy_build/__init__.py
--rw-rw-rw-   0        0        0       61 2023-07-13 12:38:42.000000 wasmpy-build-0.3.2/wasmpy_build/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.618784 wasmpy-build-0.3.2/wasmpy_build/include/
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.792421 wasmpy-build-0.3.2/wasmpy_build/include/cp310/
--rw-rw-rw-   0        0        0    13936 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/LICENSE
--rw-rw-rw-   0        0        0     3224 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/Python.h
--rw-rw-rw-   0        0        0      344 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/README.rst
--rw-rw-rw-   0        0        0    31405 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/abstract.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bltinmodule.h
--rw-rw-rw-   0        0        0     1224 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytearrayobject.h
--rw-rw-rw-   0        0        0     2593 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytesobject.h
--rw-rw-rw-   0        0        0      720 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cellobject.h
--rw-rw-rw-   0        0        0     5703 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/classobject.h
--rw-rw-rw-   0        0        0      318 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/code.h
--rw-rw-rw-   0        0        0     7071 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/codecs.h
--rw-rw-rw-   0        0        0      520 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/compile.h
--rw-rw-rw-   0        0        0     1806 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/context.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.843496 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/
--rw-rw-rw-   0        0        0    14054 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4119 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1468 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/ceval.h
--rw-rw-rw-   0        0        0     7570 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/compile.h
--rw-rw-rw-   0        0        0     3734 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/dictobject.h
--rw-rw-rw-   0        0        0      723 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4267 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3152 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1630 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/import.h
--rw-rw-rw-   0        0        0     7597 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/initconfig.h
--rw-rw-rw-   0        0        0      387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1243 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19613 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/object.h
--rw-rw-rw-   0        0        0     3356 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     1387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pydebug.h
--rw-rw-rw-   0        0        0     5476 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyfpe.h
--rw-rw-rw-   0        0        0     2095 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pymem.h
--rw-rw-rw-   0        0        0    11914 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     9196 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pytime.h
--rw-rw-rw-   0        0        0      506 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      404 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/traceback.h
--rw-rw-rw-   0        0        0      975 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    44284 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9635 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/datetime.h
--rw-rw-rw-   0        0        0     3002 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/descrobject.h
--rw-rw-rw-   0        0        0     3853 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/errcode.h
--rw-rw-rw-   0        0        0      831 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/eval.h
--rw-rw-rw-   0        0        0     1098 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/exports.h
--rw-rw-rw-   0        0        0     1571 2023-07-13 10:35:26.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileobject.h
--rw-rw-rw-   0        0        0      508 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/frameobject.h
--rw-rw-rw-   0        0        0     4257 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/genericaliasobject.h
--rw-rw-rw-   0        0        0     3347 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/genobject.h
--rw-rw-rw-   0        0        0     3026 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/import.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.917967 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/
--rw-rw-rw-   0        0        0      479 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     2971 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    28828 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6457 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16979 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     5271 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0      870 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3484 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      696 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2809 2023-07-13 10:35:26.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      822 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1704 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      480 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_format.h
--rw-rw-rw-   0        0        0     6859 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      346 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5625 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     9289 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      350 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_list.h
--rw-rw-rw-   0        0        0     2589 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1047 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0     5989 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_object.h
--rw-rw-rw-   0        0        0      626 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_parser.h
--rw-rw-rw-   0        0        0     1981 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2314 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     4940 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3211 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3938 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4902 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      386 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5578 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      548 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     2970 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      425 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0      898 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0      629 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      633 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/interpreteridobject.h
--rw-rw-rw-   0        0        0      772 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/longintrepr.h
--rw-rw-rw-   0        0        0     8606 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/longobject.h
--rw-rw-rw-   0        0        0      803 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/memoryobject.h
--rw-rw-rw-   0        0        0     4147 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/methodobject.h
--rw-rw-rw-   0        0        0    10333 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/modsupport.h
--rw-rw-rw-   0        0        0     2458 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/namespaceobject.h
--rw-rw-rw-   0        0        0    28344 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/object.h
--rw-rw-rw-   0        0        0     8445 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/objimpl.h
--rw-rw-rw-   0        0        0     5509 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/osmodule.h
--rw-rw-rw-   0        0        0     1302 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/patchlevel.h
--rw-rw-rw-   0        0        0     2474 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/py_curses.h
--rw-rw-rw-   0        0        0     1725 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pycapsule.h
--rw-rw-rw-   0        0        0    48758 2023-07-13 12:23:44.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyconfig.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.h
--rw-rw-rw-   0        0        0    12426 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyexpat.h
--rw-rw-rw-   0        0        0      466 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyframe.h
--rw-rw-rw-   0        0        0     4223 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyhash.h
--rw-rw-rw-   0        0        0     2080 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacro.h
--rw-rw-rw-   0        0        0     8313 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymath.h
--rw-rw-rw-   0        0        0     3891 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymem.h
--rw-rw-rw-   0        0        0    31684 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrtod.h
--rw-rw-rw-   0        0        0     1110 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythread.h
--rw-rw-rw-   0        0        0      628 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/rangeobject.h
--rw-rw-rw-   0        0        0     3381 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/sliceobject.h
--rw-rw-rw-   0        0        0     2074 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/structseq.h
--rw-rw-rw-   0        0        0     1242 2023-07-13 10:35:28.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/token.h
--rw-rw-rw-   0        0        0      584 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/tupleobject.h
--rw-rw-rw-   0        0        0     2460 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/typeslots.h
--rw-rw-rw-   0        0        0    36148 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-07-13 10:35:28.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.023154 wasmpy-build-0.3.2/wasmpy_build/include/cp311/
--rw-rw-rw-   0        0        0    13936 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/LICENSE
--rw-rw-rw-   0        0        0     2854 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/Python.h
--rw-rw-rw-   0        0        0      344 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/README.rst
--rw-rw-rw-   0        0        0    31404 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/abstract.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bltinmodule.h
--rw-rw-rw-   0        0        0     1212 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/boolobject.h
--rw-rw-rw-   0        0        0     1462 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytearrayobject.h
--rw-rw-rw-   0        0        0     2617 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytesobject.h
--rw-rw-rw-   0        0        0     6255 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/ceval.h
--rw-rw-rw-   0        0        0     7071 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/codecs.h
--rw-rw-rw-   0        0        0      520 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/compile.h
--rw-rw-rw-   0        0        0      724 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/complexobject.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.098708 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/
--rw-rw-rw-   0        0        0     8229 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/abstract.h
--rw-rw-rw-   0        0        0     1305 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4568 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytesobject.h
--rw-rw-rw-   0        0        0      723 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/cellobject.h
--rw-rw-rw-   0        0        0     1239 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/ceval.h
--rw-rw-rw-   0        0        0     1656 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/classobject.h
--rw-rw-rw-   0        0        0    11484 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/compile.h
--rw-rw-rw-   0        0        0     1248 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/complexobject.h
--rw-rw-rw-   0        0        0     1959 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/context.h
--rw-rw-rw-   0        0        0     1642 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/descrobject.h
--rw-rw-rw-   0        0        0     3324 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/dictobject.h
--rw-rw-rw-   0        0        0      818 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileobject.h
--rw-rw-rw-   0        0        0      232 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileutils.h
--rw-rw-rw-   0        0        0      702 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/floatobject.h
--rw-rw-rw-   0        0        0     1108 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/frameobject.h
--rw-rw-rw-   0        0        0     4424 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/funcobject.h
--rw-rw-rw-   0        0        0     3279 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/genobject.h
--rw-rw-rw-   0        0        0     1526 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/import.h
--rw-rw-rw-   0        0        0     7817 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/initconfig.h
--rw-rw-rw-   0        0        0     1769 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/listobject.h
--rw-rw-rw-   0        0        0     3817 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longintrepr.h
--rw-rw-rw-   0        0        0     4532 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longobject.h
--rw-rw-rw-   0        0        0     2556 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/methodobject.h
--rw-rw-rw-   0        0        0     4234 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/modsupport.h
--rw-rw-rw-   0        0        0    18305 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/object.h
--rw-rw-rw-   0        0        0     2998 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     3505 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h
--rw-rw-rw-   0        0        0     1387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1073 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pydebug.h
--rw-rw-rw-   0        0        0     4522 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyfpe.h
--rw-rw-rw-   0        0        0      582 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyframe.h
--rw-rw-rw-   0        0        0     2099 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pymem.h
--rw-rw-rw-   0        0        0    14351 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     1426 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythread.h
--rw-rw-rw-   0        0        0    12158 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pytime.h
--rw-rw-rw-   0        0        0     1997 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/setobject.h
--rw-rw-rw-   0        0        0      489 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      444 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/traceback.h
--rw-rw-rw-   0        0        0     1513 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    41910 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0      560 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/warnings.h
--rw-rw-rw-   0        0        0     2103 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/weakrefobject.h
--rw-rw-rw-   0        0        0     9635 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/datetime.h
--rw-rw-rw-   0        0        0     1256 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/descrobject.h
--rw-rw-rw-   0        0        0     3852 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/errcode.h
--rw-rw-rw-   0        0        0     1098 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/exports.h
--rw-rw-rw-   0        0        0     1570 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileobject.h
--rw-rw-rw-   0        0        0      507 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileutils.h
--rw-rw-rw-   0        0        0     1530 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/floatobject.h
--rw-rw-rw-   0        0        0      336 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/frameobject.h
--rw-rw-rw-   0        0        0      334 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/genericaliasobject.h
--rw-rw-rw-   0        0        0     3025 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/import.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.286358 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/
--rw-rw-rw-   0        0        0      611 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     3031 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    29315 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6535 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16979 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     6062 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     1424 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
--rw-rw-rw-   0        0        0     3475 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_call.h
--rw-rw-rw-   0        0        0     4409 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0    15930 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2839 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0     1239 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_context.h
--rw-rw-rw-   0        0        0     5684 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dict.h
--rw-rw-rw-   0        0        0      704 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0      562 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
--rw-rw-rw-   0        0        0      842 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h
--rw-rw-rw-   0        0        0     7313 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     1307 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h
--rw-rw-rw-   0        0        0      480 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_format.h
--rw-rw-rw-   0        0        0     7567 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_frame.h
--rw-rw-rw-   0        0        0      413 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_function.h
--rw-rw-rw-   0        0        0     6895 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gc.h
--rw-rw-rw-   0        0        0     1164 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_genobject.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     1436 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h
--rw-rw-rw-   0        0        0    12980 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h
--rw-rw-rw-   0        0        0     3696 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      743 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5800 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     6671 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      562 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
--rw-rw-rw-   0        0        0     1352 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_list.h
--rw-rw-rw-   0        0        0     3516 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1040 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0      392 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_namespace.h
--rw-rw-rw-   0        0        0    10037 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_object.h
--rw-rw-rw-   0        0        0    18986 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_opcode.h
--rw-rw-rw-   0        0        0      626 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_parser.h
--rw-rw-rw-   0        0        0      606 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2494 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3507 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     9435 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymath.h
--rw-rw-rw-   0        0        0     3708 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     4107 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     5988 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0    49092 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
--rw-rw-rw-   0        0        0      937 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_signal.h
--rw-rw-rw-   0        0        0      336 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
--rw-rw-rw-   0        0        0      937 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_strhex.h
--rw-rw-rw-   0        0        0      580 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5638 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      605 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3501 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0     2089 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0     1158 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h
--rw-rw-rw-   0        0        0      898 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0     1716 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
--rw-rw-rw-   0        0        0      678 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      740 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      772 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/iterobject.h
--rw-rw-rw-   0        0        0     1780 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/listobject.h
--rw-rw-rw-   0        0        0     3272 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/longobject.h
--rw-rw-rw-   0        0        0      827 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/marshal.h
--rw-rw-rw-   0        0        0     2810 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/memoryobject.h
--rw-rw-rw-   0        0        0     5072 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/methodobject.h
--rw-rw-rw-   0        0        0     6448 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/modsupport.h
--rw-rw-rw-   0        0        0     2374 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/moduleobject.h
--rw-rw-rw-   0        0        0    29800 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/object.h
--rw-rw-rw-   0        0        0     8428 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/objimpl.h
--rw-rw-rw-   0        0        0    11187 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/osmodule.h
--rw-rw-rw-   0        0        0     1300 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/patchlevel.h
--rw-rw-rw-   0        0        0     2471 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/py_curses.h
--rw-rw-rw-   0        0        0     5115 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pybuffer.h
--rw-rw-rw-   0        0        0     1725 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pycapsule.h
--rw-rw-rw-   0        0        0    53001 2023-07-13 12:29:25.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyconfig.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.h
--rw-rw-rw-   0        0        0    12782 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyexpat.h
--rw-rw-rw-   0        0        0      551 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyframe.h
--rw-rw-rw-   0        0        0     4154 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyhash.h
--rw-rw-rw-   0        0        0     2249 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacconfig.h
--rw-rw-rw-   0        0        0     6064 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacro.h
--rw-rw-rw-   0        0        0     1979 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymath.h
--rw-rw-rw-   0        0        0     3890 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymem.h
--rw-rw-rw-   0        0        0    24528 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyport.h
--rw-rw-rw-   0        0        0     4635 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrcmp.h
--rw-rw-rw-   0        0        0     1557 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrtod.h
--rw-rw-rw-   0        0        0     1189 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythonrun.h
--rw-rw-rw-   0        0        0     4833 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythread.h
--rw-rw-rw-   0        0        0      851 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pytypedefs.h
--rw-rw-rw-   0        0        0      628 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/rangeobject.h
--rw-rw-rw-   0        0        0     1543 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/sliceobject.h
--rw-rw-rw-   0        0        0     2040 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/structmember.h
--rw-rw-rw-   0        0        0     1388 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/structseq.h
--rw-rw-rw-   0        0        0     1381 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/token.h
--rw-rw-rw-   0        0        0      583 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/tracemalloc.h
--rw-rw-rw-   0        0        0     1613 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/tupleobject.h
--rw-rw-rw-   0        0        0     2342 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/typeslots.h
--rw-rw-rw-   0        0        0    36032 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/unicodeobject.h
--rw-rw-rw-   0        0        0     1129 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/warnings.h
--rw-rw-rw-   0        0        0     1226 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.483929 wasmpy-build-0.3.2/wasmpy_build/include/cp38/
--rw-rw-rw-   0        0        0    13937 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/LICENSE
--rw-rw-rw-   0        0        0    26491 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python-ast.h
--rw-rw-rw-   0        0        0     3615 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python.h
--rw-rw-rw-   0        0        0    30286 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/abstract.h
--rw-rw-rw-   0        0        0     1229 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/asdl.h
--rw-rw-rw-   0        0        0      948 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ast.h
--rw-rw-rw-   0        0        0      468 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bitset.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bltinmodule.h
--rw-rw-rw-   0        0        0      886 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/boolobject.h
--rw-rw-rw-   0        0        0     2114 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytearrayobject.h
--rw-rw-rw-   0        0        0     3301 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytes_methods.h
--rw-rw-rw-   0        0        0     8493 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytesobject.h
--rw-rw-rw-   0        0        0      713 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cellobject.h
--rw-rw-rw-   0        0        0     8366 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ceval.h
--rw-rw-rw-   0        0        0     1710 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/classobject.h
--rw-rw-rw-   0        0        0     7178 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/code.h
--rw-rw-rw-   0        0        0     6793 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/codecs.h
--rw-rw-rw-   0        0        0     3582 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/compile.h
--rw-rw-rw-   0        0        0     1807 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/complexobject.h
--rw-rw-rw-   0        0        0     2014 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/context.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.522810 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/
--rw-rw-rw-   0        0        0    12294 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/abstract.h
--rw-rw-rw-   0        0        0     3845 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/fileobject.h
--rw-rw-rw-   0        0        0    16028 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0    15691 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/object.h
--rw-rw-rw-   0        0        0     3600 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/objimpl.h
--rw-rw-rw-   0        0        0     4717 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2263 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pymem.h
--rw-rw-rw-   0        0        0     9810 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pystate.h
--rw-rw-rw-   0        0        0      547 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46308 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9260 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/descrobject.h
--rw-rw-rw-   0        0        0     3716 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dictobject.h
--rw-rw-rw-   0        0        0      458 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dtoa.h
--rw-rw-rw-   0        0        0    22469 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/enumobject.h
--rw-rw-rw-   0        0        0     1695 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/eval.h
--rw-rw-rw-   0        0        0     1571 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileobject.h
--rw-rw-rw-   0        0        0     4352 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileutils.h
--rw-rw-rw-   0        0        0     4794 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/floatobject.h
--rw-rw-rw-   0        0        0     3317 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/frameobject.h
--rw-rw-rw-   0        0        0     4200 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/funcobject.h
--rw-rw-rw-   0        0        0     3720 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/grammar.h
--rw-rw-rw-   0        0        0     4926 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/import.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.576544 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/
--rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16944 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0      966 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      542 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      779 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_context.h
--rw-rw-rw-   0        0        0     1254 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1520 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3698 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     5218 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     1548 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_long.h
--rw-rw-rw-   0        0        0     2896 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_object.h
--rw-rw-rw-   0        0        0     2037 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     1329 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3815 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     8217 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     9588 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     3076 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      418 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      591 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/intrcheck.h
--rw-rw-rw-   0        0        0      567 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/iterobject.h
--rw-rw-rw-   0        0        0     2927 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/longintrepr.h
--rw-rw-rw-   0        0        0     9520 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/longobject.h
--rw-rw-rw-   0        0        0      803 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/marshal.h
--rw-rw-rw-   0        0        0     2765 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/memoryobject.h
--rw-rw-rw-   0        0        0     4406 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/methodobject.h
--rw-rw-rw-   0        0        0     9591 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/modsupport.h
--rw-rw-rw-   0        0        0     2362 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/namespaceobject.h
--rw-rw-rw-   0        0        0     1328 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/node.h
--rw-rw-rw-   0        0        0    29599 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/object.h
--rw-rw-rw-   0        0        0    10537 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/objimpl.h
--rw-rw-rw-   0        0        0     1300 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/odictobject.h
--rw-rw-rw-   0        0        0     5164 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/patchlevel.h
--rw-rw-rw-   0        0        0      847 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/picklebufobject.h
--rw-rw-rw-   0        0        0     2477 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyarena.h
--rw-rw-rw-   0        0        0     1726 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pycapsule.h
--rw-rw-rw-   0        0        0    47623 2023-07-13 11:28:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyconfig.h
--rw-rw-rw-   0        0        0     1387 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyctype.h
--rw-rw-rw-   0        0        0     1214 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.h
--rw-rw-rw-   0        0        0    12786 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyexpat.h
--rw-rw-rw-   0        0        0      341 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyfpe.h
--rw-rw-rw-   0        0        0     4140 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyhash.h
--rw-rw-rw-   0        0        0     2081 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacconfig.h
--rw-rw-rw-   0        0        0     3778 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacro.h
--rw-rw-rw-   0        0        0     8312 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymath.h
--rw-rw-rw-   0        0        0     5406 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymem.h
--rw-rw-rw-   0        0        0    30221 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyport.h
--rw-rw-rw-   0        0        0     4686 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrtod.h
--rw-rw-rw-   0        0        0     7645 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythonrun.h
--rw-rw-rw-   0        0        0     5660 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythread.h
--rw-rw-rw-   0        0        0     8926 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pytime.h
--rw-rw-rw-   0        0        0      629 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/rangeobject.h
--rw-rw-rw-   0        0        0     3362 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/setobject.h
--rw-rw-rw-   0        0        0     2517 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/structmember.h
--rw-rw-rw-   0        0        0     1377 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/structseq.h
--rw-rw-rw-   0        0        0     5308 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/sysmodule.h
--rw-rw-rw-   0        0        0     2429 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/token.h
--rw-rw-rw-   0        0        0      601 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/tracemalloc.h
--rw-rw-rw-   0        0        0     1661 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/tupleobject.h
--rw-rw-rw-   0        0        0     2253 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ucnhash.h
--rw-rw-rw-   0        0        0    35732 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/warnings.h
--rw-rw-rw-   0        0        0     2866 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.785138 wasmpy-build-0.3.2/wasmpy_build/include/cp39/
--rw-rw-rw-   0        0        0    13937 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/LICENSE
--rw-rw-rw-   0        0        0    26193 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python-ast.h
--rw-rw-rw-   0        0        0     3532 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python.h
--rw-rw-rw-   0        0        0    30476 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/abstract.h
--rw-rw-rw-   0        0        0     1224 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/asdl.h
--rw-rw-rw-   0        0        0      947 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ast.h
--rw-rw-rw-   0        0        0      468 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bitset.h
--rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bltinmodule.h
--rw-rw-rw-   0        0        0      885 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytearrayobject.h
--rw-rw-rw-   0        0        0     3048 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytesobject.h
--rw-rw-rw-   0        0        0      712 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cellobject.h
--rw-rw-rw-   0        0        0     5954 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/classobject.h
--rw-rw-rw-   0        0        0      318 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/code.h
--rw-rw-rw-   0        0        0     6793 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/codecs.h
--rw-rw-rw-   0        0        0     3778 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/compile.h
--rw-rw-rw-   0        0        0     1806 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/context.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.832657 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/
--rw-rw-rw-   0        0        0    14200 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4114 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1537 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/ceval.h
--rw-rw-rw-   0        0        0     6989 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/code.h
--rw-rw-rw-   0        0        0     3797 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4004 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3059 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1473 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/import.h
--rw-rw-rw-   0        0        0    16979 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1364 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19358 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/object.h
--rw-rw-rw-   0        0        0     4456 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/objimpl.h
--rw-rw-rw-   0        0        0     5101 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2096 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pymem.h
--rw-rw-rw-   0        0        0    10134 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pystate.h
--rw-rw-rw-   0        0        0      575 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46154 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9255 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/descrobject.h
--rw-rw-rw-   0        0        0     3715 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/dictobject.h
--rw-rw-rw-   0        0        0    22469 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/enumobject.h
--rw-rw-rw-   0        0        0     1624 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/eval.h
--rw-rw-rw-   0        0        0     1098 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/exports.h
--rw-rw-rw-   0        0        0     1571 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileobject.h
--rw-rw-rw-   0        0        0      597 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/frameobject.h
--rw-rw-rw-   0        0        0     4057 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/genericaliasobject.h
--rw-rw-rw-   0        0        0     3525 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/grammar.h
--rw-rw-rw-   0        0        0     3026 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/import.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.901366 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/
--rw-rw-rw-   0        0        0      953 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pegen_interface.h
--rw-rw-rw-   0        0        0      479 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16977 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     3384 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     2620 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h
--rw-rw-rw-   0        0        0      870 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3403 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      541 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      800 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1541 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     6647 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      473 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5233 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     5299 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_interp.h
--rw-rw-rw-   0        0        0     1548 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_long.h
--rw-rw-rw-   0        0        0     4157 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_object.h
--rw-rw-rw-   0        0        0     1936 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2032 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3741 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3363 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3583 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4452 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      548 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3056 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      442 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      633 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/intrcheck.h
--rw-rw-rw-   0        0        0      521 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/longintrepr.h
--rw-rw-rw-   0        0        0     9513 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/longobject.h
--rw-rw-rw-   0        0        0      803 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/memoryobject.h
--rw-rw-rw-   0        0        0     3775 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/methodobject.h
--rw-rw-rw-   0        0        0     9959 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/modsupport.h
--rw-rw-rw-   0        0        0     2361 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/namespaceobject.h
--rw-rw-rw-   0        0        0     1281 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/node.h
--rw-rw-rw-   0        0        0    24628 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/object.h
--rw-rw-rw-   0        0        0     8423 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/odictobject.h
--rw-rw-rw-   0        0        0     4900 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/opcode.h
--rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/patchlevel.h
--rw-rw-rw-   0        0        0      846 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/picklebufobject.h
--rw-rw-rw-   0        0        0     2474 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyarena.h
--rw-rw-rw-   0        0        0     1725 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pycapsule.h
--rw-rw-rw-   0        0        0    48109 2023-07-13 11:35:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyconfig.h
--rw-rw-rw-   0        0        0     1387 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.h
--rw-rw-rw-   0        0        0    12427 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyexpat.h
--rw-rw-rw-   0        0        0      444 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyfpe.h
--rw-rw-rw-   0        0        0      466 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyframe.h
--rw-rw-rw-   0        0        0     4263 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyhash.h
--rw-rw-rw-   0        0        0     2136 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacro.h
--rw-rw-rw-   0        0        0     8580 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymath.h
--rw-rw-rw-   0        0        0     4406 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymem.h
--rw-rw-rw-   0        0        0    31273 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystate.h
--rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrtod.h
--rw-rw-rw-   0        0        0     7673 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythread.h
--rw-rw-rw-   0        0        0     8928 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pytime.h
--rw-rw-rw-   0        0        0      628 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/rangeobject.h
--rw-rw-rw-   0        0        0     3324 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/structseq.h
--rw-rw-rw-   0        0        0     5307 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/sysmodule.h
--rw-rw-rw-   0        0        0     2642 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/token.h
--rw-rw-rw-   0        0        0      584 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/tupleobject.h
--rw-rw-rw-   0        0        0     2350 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ucnhash.h
--rw-rw-rw-   0        0        0    35426 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.652953 wasmpy-build-0.3.2/wasmpy_build.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    28923 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.850117 wasmpy-build-0.3.3/
+-rw-rw-rw-   0        0        0     1068 2023-07-13 12:38:30.000000 wasmpy-build-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1686 2023-07-14 23:44:30.849118 wasmpy-build-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2023-07-14 10:51:14.000000 wasmpy-build-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 23:44:30.850117 wasmpy-build-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-07-14 23:41:23.000000 wasmpy-build-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:28.507834 wasmpy-build-0.3.3/wasmpy_build/
+-rw-rw-rw-   0        0        0     2221 2023-07-14 21:36:07.000000 wasmpy-build-0.3.3/wasmpy_build/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 12:38:42.000000 wasmpy-build-0.3.3/wasmpy_build/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:28.498430 wasmpy-build-0.3.3/wasmpy_build/include/
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:28.740467 wasmpy-build-0.3.3/wasmpy_build/include/cp310/
+-rw-rw-rw-   0        0        0    13936 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/LICENSE
+-rw-rw-rw-   0        0        0     3224 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/README.rst
+-rw-rw-rw-   0        0        0    31405 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/bltinmodule.h
+-rw-rw-rw-   0        0        0     1224 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2593 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/bytesobject.h
+-rw-rw-rw-   0        0        0      720 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cellobject.h
+-rw-rw-rw-   0        0        0     5703 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/code.h
+-rw-rw-rw-   0        0        0     7071 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:28.916706 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/
+-rw-rw-rw-   0        0        0    14054 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4119 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1468 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/ceval.h
+-rw-rw-rw-   0        0        0     7570 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/compile.h
+-rw-rw-rw-   0        0        0     3734 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4267 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3152 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1630 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/import.h
+-rw-rw-rw-   0        0        0     7597 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      387 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1243 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-14 18:53:36.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19613 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/object.h
+-rw-rw-rw-   0        0        0     3356 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     1387 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     5476 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0     2095 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pymem.h
+-rw-rw-rw-   0        0        0    11914 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     9196 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pytime.h
+-rw-rw-rw-   0        0        0      506 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      404 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/traceback.h
+-rw-rw-rw-   0        0        0      975 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    44284 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/datetime.h
+-rw-rw-rw-   0        0        0     3002 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/descrobject.h
+-rw-rw-rw-   0        0        0     3853 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/errcode.h
+-rw-rw-rw-   0        0        0      831 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-07-14 18:48:58.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/fileobject.h
+-rw-rw-rw-   0        0        0      508 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/frameobject.h
+-rw-rw-rw-   0        0        0     4257 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3347 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/genobject.h
+-rw-rw-rw-   0        0        0     3026 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:29.152767 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/
+-rw-rw-rw-   0        0        0      479 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     2971 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    28828 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6457 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     5271 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0      870 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3484 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      696 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2809 2023-07-14 18:48:59.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      822 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1704 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      480 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     6859 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      346 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5625 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     9289 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      350 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     2589 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1047 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0     5989 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_object.h
+-rw-rw-rw-   0        0        0      626 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0     1981 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2314 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     4940 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3211 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3938 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4902 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      386 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5578 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      548 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     2970 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      425 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0      898 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0      629 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 18:48:59.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/interpreteridobject.h
+-rw-rw-rw-   0        0        0      772 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-14 18:48:59.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/longintrepr.h
+-rw-rw-rw-   0        0        0     8606 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-14 18:48:59.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/memoryobject.h
+-rw-rw-rw-   0        0        0     4147 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/methodobject.h
+-rw-rw-rw-   0        0        0    10333 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/modsupport.h
+-rw-rw-rw-   0        0        0     2458 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-14 18:49:00.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/namespaceobject.h
+-rw-rw-rw-   0        0        0    28344 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/object.h
+-rw-rw-rw-   0        0        0     8445 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/objimpl.h
+-rw-rw-rw-   0        0        0     5509 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/osmodule.h
+-rw-rw-rw-   0        0        0     1302 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/patchlevel.h
+-rw-rw-rw-   0        0        0     2474 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/py_curses.h
+-rw-rw-rw-   0        0        0     1725 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pydtrace.h
+-rw-rw-rw-   0        0        0    12426 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyexpat.h
+-rw-rw-rw-   0        0        0      466 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyframe.h
+-rw-rw-rw-   0        0        0     4223 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyhash.h
+-rw-rw-rw-   0        0        0     2080 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymacro.h
+-rw-rw-rw-   0        0        0     8313 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymath.h
+-rw-rw-rw-   0        0        0     3891 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymem.h
+-rw-rw-rw-   0        0        0    31804 2023-07-14 23:35:14.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-14 18:49:00.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-14 18:49:00.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystrtod.h
+-rw-rw-rw-   0        0        0     1110 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/pythread.h
+-rw-rw-rw-   0        0        0      628 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/rangeobject.h
+-rw-rw-rw-   0        0        0     3381 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/sliceobject.h
+-rw-rw-rw-   0        0        0     2074 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/structseq.h
+-rw-rw-rw-   0        0        0     1242 2023-07-14 18:49:00.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/tupleobject.h
+-rw-rw-rw-   0        0        0     2460 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/typeslots.h
+-rw-rw-rw-   0        0        0    36148 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-14 18:49:01.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp310/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:29.437968 wasmpy-build-0.3.3/wasmpy_build/include/cp311/
+-rw-rw-rw-   0        0        0    13936 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/LICENSE
+-rw-rw-rw-   0        0        0     2854 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/README.rst
+-rw-rw-rw-   0        0        0    31404 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/bltinmodule.h
+-rw-rw-rw-   0        0        0     1212 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/boolobject.h
+-rw-rw-rw-   0        0        0     1462 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2617 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/bytesobject.h
+-rw-rw-rw-   0        0        0     6255 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/ceval.h
+-rw-rw-rw-   0        0        0     7071 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/compile.h
+-rw-rw-rw-   0        0        0      724 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/complexobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:29.594673 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/
+-rw-rw-rw-   0        0        0     8229 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/abstract.h
+-rw-rw-rw-   0        0        0     1305 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4568 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/cellobject.h
+-rw-rw-rw-   0        0        0     1239 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/ceval.h
+-rw-rw-rw-   0        0        0     1656 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/classobject.h
+-rw-rw-rw-   0        0        0    11484 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/compile.h
+-rw-rw-rw-   0        0        0     1248 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/complexobject.h
+-rw-rw-rw-   0        0        0     1959 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/context.h
+-rw-rw-rw-   0        0        0     1642 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/descrobject.h
+-rw-rw-rw-   0        0        0     3324 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      818 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/fileobject.h
+-rw-rw-rw-   0        0        0      232 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/fileutils.h
+-rw-rw-rw-   0        0        0      702 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/floatobject.h
+-rw-rw-rw-   0        0        0     1108 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     4424 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/funcobject.h
+-rw-rw-rw-   0        0        0     3279 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/genobject.h
+-rw-rw-rw-   0        0        0     1526 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/import.h
+-rw-rw-rw-   0        0        0     7817 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/initconfig.h
+-rw-rw-rw-   0        0        0     1769 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/listobject.h
+-rw-rw-rw-   0        0        0     3817 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/longintrepr.h
+-rw-rw-rw-   0        0        0     4532 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/longobject.h
+-rw-rw-rw-   0        0        0     2556 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/methodobject.h
+-rw-rw-rw-   0        0        0     4234 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/modsupport.h
+-rw-rw-rw-   0        0        0    18305 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/object.h
+-rw-rw-rw-   0        0        0     2998 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     3505 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pthread_stubs.h
+-rw-rw-rw-   0        0        0     1387 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1073 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     4522 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0      582 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyframe.h
+-rw-rw-rw-   0        0        0     2099 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-14 23:35:08.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pymem.h
+-rw-rw-rw-   0        0        0    14351 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     1426 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pythread.h
+-rw-rw-rw-   0        0        0    12158 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pytime.h
+-rw-rw-rw-   0        0        0     1997 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/setobject.h
+-rw-rw-rw-   0        0        0      489 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      444 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1513 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    41910 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0      560 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/warnings.h
+-rw-rw-rw-   0        0        0     2103 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/weakrefobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/datetime.h
+-rw-rw-rw-   0        0        0     1256 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/descrobject.h
+-rw-rw-rw-   0        0        0     3852 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/errcode.h
+-rw-rw-rw-   0        0        0     1098 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/exports.h
+-rw-rw-rw-   0        0        0     1570 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/fileobject.h
+-rw-rw-rw-   0        0        0      507 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/fileutils.h
+-rw-rw-rw-   0        0        0     1530 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/floatobject.h
+-rw-rw-rw-   0        0        0      336 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/frameobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3025 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:29.828000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/
+-rw-rw-rw-   0        0        0      611 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     3031 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    29315 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6535 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     6062 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     1424 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
+-rw-rw-rw-   0        0        0     3475 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     4409 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0    15930 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2839 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0     1239 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     5684 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_dict.h
+-rw-rw-rw-   0        0        0      704 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0      562 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
+-rw-rw-rw-   0        0        0      842 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_exceptions.h
+-rw-rw-rw-   0        0        0     7313 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     1307 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_floatobject.h
+-rw-rw-rw-   0        0        0      480 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     7567 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_frame.h
+-rw-rw-rw-   0        0        0      413 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_function.h
+-rw-rw-rw-   0        0        0     6895 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0     1164 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_genobject.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     1436 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_global_objects.h
+-rw-rw-rw-   0        0        0    12980 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_global_strings.h
+-rw-rw-rw-   0        0        0     3696 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-14 18:53:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      743 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5800 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     6671 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      562 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
+-rw-rw-rw-   0        0        0     1352 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     3516 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1040 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0      392 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_namespace.h
+-rw-rw-rw-   0        0        0    10037 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_object.h
+-rw-rw-rw-   0        0        0    18986 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_opcode.h
+-rw-rw-rw-   0        0        0      626 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0      606 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2494 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3507 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     9435 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pymath.h
+-rw-rw-rw-   0        0        0     3708 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     4107 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     5988 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0    49092 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
+-rw-rw-rw-   0        0        0      937 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_signal.h
+-rw-rw-rw-   0        0        0      336 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
+-rw-rw-rw-   0        0        0      937 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_strhex.h
+-rw-rw-rw-   0        0        0      580 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5638 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      605 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3501 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0     2089 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0     1158 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_typeobject.h
+-rw-rw-rw-   0        0        0      898 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0     1716 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
+-rw-rw-rw-   0        0        0      678 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      740 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      772 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/iterobject.h
+-rw-rw-rw-   0        0        0     1780 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/listobject.h
+-rw-rw-rw-   0        0        0     3272 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/longobject.h
+-rw-rw-rw-   0        0        0      827 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/marshal.h
+-rw-rw-rw-   0        0        0     2810 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/memoryobject.h
+-rw-rw-rw-   0        0        0     5072 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/methodobject.h
+-rw-rw-rw-   0        0        0     6448 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/modsupport.h
+-rw-rw-rw-   0        0        0     2374 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/moduleobject.h
+-rw-rw-rw-   0        0        0    29800 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/object.h
+-rw-rw-rw-   0        0        0     8428 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/objimpl.h
+-rw-rw-rw-   0        0        0    11187 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/osmodule.h
+-rw-rw-rw-   0        0        0     1300 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/patchlevel.h
+-rw-rw-rw-   0        0        0     2471 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/py_curses.h
+-rw-rw-rw-   0        0        0     5115 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pybuffer.h
+-rw-rw-rw-   0        0        0     1725 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pydtrace.h
+-rw-rw-rw-   0        0        0    12782 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyexpat.h
+-rw-rw-rw-   0        0        0      551 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyframe.h
+-rw-rw-rw-   0        0        0     4154 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyhash.h
+-rw-rw-rw-   0        0        0     2249 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymacconfig.h
+-rw-rw-rw-   0        0        0     6064 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymacro.h
+-rw-rw-rw-   0        0        0     1979 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymath.h
+-rw-rw-rw-   0        0        0     3890 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymem.h
+-rw-rw-rw-   0        0        0    24648 2023-07-14 23:35:20.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyport.h
+-rw-rw-rw-   0        0        0     4635 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pystrcmp.h
+-rw-rw-rw-   0        0        0     1557 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pystrtod.h
+-rw-rw-rw-   0        0        0     1189 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pythonrun.h
+-rw-rw-rw-   0        0        0     4833 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pythread.h
+-rw-rw-rw-   0        0        0      851 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/pytypedefs.h
+-rw-rw-rw-   0        0        0      628 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/rangeobject.h
+-rw-rw-rw-   0        0        0     1543 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-14 18:53:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/sliceobject.h
+-rw-rw-rw-   0        0        0     2040 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/structmember.h
+-rw-rw-rw-   0        0        0     1388 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/structseq.h
+-rw-rw-rw-   0        0        0     1381 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-14 23:35:09.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/token.h
+-rw-rw-rw-   0        0        0      583 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/tracemalloc.h
+-rw-rw-rw-   0        0        0     1613 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/tupleobject.h
+-rw-rw-rw-   0        0        0     2342 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/typeslots.h
+-rw-rw-rw-   0        0        0    36032 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/unicodeobject.h
+-rw-rw-rw-   0        0        0     1129 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/warnings.h
+-rw-rw-rw-   0        0        0     1226 2023-07-14 23:35:16.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp311/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.166279 wasmpy-build-0.3.3/wasmpy_build/include/cp38/
+-rw-rw-rw-   0        0        0    13937 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/LICENSE
+-rw-rw-rw-   0        0        0    26491 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/Python-ast.h
+-rw-rw-rw-   0        0        0     3615 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/Python.h
+-rw-rw-rw-   0        0        0    30286 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/abstract.h
+-rw-rw-rw-   0        0        0     1229 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/asdl.h
+-rw-rw-rw-   0        0        0      948 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/bltinmodule.h
+-rw-rw-rw-   0        0        0      886 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/boolobject.h
+-rw-rw-rw-   0        0        0     2114 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3301 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytes_methods.h
+-rw-rw-rw-   0        0        0     8493 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytesobject.h
+-rw-rw-rw-   0        0        0      713 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cellobject.h
+-rw-rw-rw-   0        0        0     8366 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/ceval.h
+-rw-rw-rw-   0        0        0     1710 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/classobject.h
+-rw-rw-rw-   0        0        0     7178 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/code.h
+-rw-rw-rw-   0        0        0     6793 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/codecs.h
+-rw-rw-rw-   0        0        0     3582 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/compile.h
+-rw-rw-rw-   0        0        0     1807 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/complexobject.h
+-rw-rw-rw-   0        0        0     2014 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.236287 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/
+-rw-rw-rw-   0        0        0    12294 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/abstract.h
+-rw-rw-rw-   0        0        0     3845 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/fileobject.h
+-rw-rw-rw-   0        0        0    16028 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0    15691 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/object.h
+-rw-rw-rw-   0        0        0     3600 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     4717 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2263 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pymem.h
+-rw-rw-rw-   0        0        0     9810 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pystate.h
+-rw-rw-rw-   0        0        0      547 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46308 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9260 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/descrobject.h
+-rw-rw-rw-   0        0        0     3716 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/dictobject.h
+-rw-rw-rw-   0        0        0      458 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/dtoa.h
+-rw-rw-rw-   0        0        0    22469 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/enumobject.h
+-rw-rw-rw-   0        0        0     1695 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/eval.h
+-rw-rw-rw-   0        0        0     1571 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/fileobject.h
+-rw-rw-rw-   0        0        0     4352 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/fileutils.h
+-rw-rw-rw-   0        0        0     4794 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/floatobject.h
+-rw-rw-rw-   0        0        0     3317 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/frameobject.h
+-rw-rw-rw-   0        0        0     4200 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/funcobject.h
+-rw-rw-rw-   0        0        0     3720 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/grammar.h
+-rw-rw-rw-   0        0        0     4926 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.328799 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16944 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0      966 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      542 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      779 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     1254 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1520 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3698 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     5218 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     1548 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     2896 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     2037 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     1329 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3815 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     8217 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     9588 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     3076 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      418 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      591 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/intrcheck.h
+-rw-rw-rw-   0        0        0      567 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/iterobject.h
+-rw-rw-rw-   0        0        0     2927 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/longintrepr.h
+-rw-rw-rw-   0        0        0     9520 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/marshal.h
+-rw-rw-rw-   0        0        0     2765 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/memoryobject.h
+-rw-rw-rw-   0        0        0     4406 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/methodobject.h
+-rw-rw-rw-   0        0        0     9591 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/modsupport.h
+-rw-rw-rw-   0        0        0     2362 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/namespaceobject.h
+-rw-rw-rw-   0        0        0     1328 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/node.h
+-rw-rw-rw-   0        0        0    29599 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/object.h
+-rw-rw-rw-   0        0        0    10537 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/objimpl.h
+-rw-rw-rw-   0        0        0     1300 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/odictobject.h
+-rw-rw-rw-   0        0        0     5164 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/patchlevel.h
+-rw-rw-rw-   0        0        0      847 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/picklebufobject.h
+-rw-rw-rw-   0        0        0     2477 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyarena.h
+-rw-rw-rw-   0        0        0     1726 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyctype.h
+-rw-rw-rw-   0        0        0     1214 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydtrace.h
+-rw-rw-rw-   0        0        0    12786 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyexpat.h
+-rw-rw-rw-   0        0        0      341 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyfpe.h
+-rw-rw-rw-   0        0        0     4140 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyhash.h
+-rw-rw-rw-   0        0        0     2081 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymacconfig.h
+-rw-rw-rw-   0        0        0     3778 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymacro.h
+-rw-rw-rw-   0        0        0     8312 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymath.h
+-rw-rw-rw-   0        0        0     5406 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymem.h
+-rw-rw-rw-   0        0        0    30369 2023-07-14 23:35:27.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyport.h
+-rw-rw-rw-   0        0        0     4686 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystrtod.h
+-rw-rw-rw-   0        0        0     7645 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pythonrun.h
+-rw-rw-rw-   0        0        0     5660 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pythread.h
+-rw-rw-rw-   0        0        0     8926 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/pytime.h
+-rw-rw-rw-   0        0        0      629 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/rangeobject.h
+-rw-rw-rw-   0        0        0     3362 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/setobject.h
+-rw-rw-rw-   0        0        0     2517 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/structmember.h
+-rw-rw-rw-   0        0        0     1377 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/structseq.h
+-rw-rw-rw-   0        0        0     5308 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/sysmodule.h
+-rw-rw-rw-   0        0        0     2429 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/token.h
+-rw-rw-rw-   0        0        0      601 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/tracemalloc.h
+-rw-rw-rw-   0        0        0     1661 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/tupleobject.h
+-rw-rw-rw-   0        0        0     2253 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/ucnhash.h
+-rw-rw-rw-   0        0        0    35732 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/warnings.h
+-rw-rw-rw-   0        0        0     2866 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp38/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.663030 wasmpy-build-0.3.3/wasmpy_build/include/cp39/
+-rw-rw-rw-   0        0        0    13937 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/LICENSE
+-rw-rw-rw-   0        0        0    26193 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/Python-ast.h
+-rw-rw-rw-   0        0        0     3532 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/Python.h
+-rw-rw-rw-   0        0        0    30476 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/abstract.h
+-rw-rw-rw-   0        0        0     1224 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/asdl.h
+-rw-rw-rw-   0        0        0      947 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/bltinmodule.h
+-rw-rw-rw-   0        0        0      885 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3048 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/bytesobject.h
+-rw-rw-rw-   0        0        0      712 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cellobject.h
+-rw-rw-rw-   0        0        0     5954 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/code.h
+-rw-rw-rw-   0        0        0     6793 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/codecs.h
+-rw-rw-rw-   0        0        0     3778 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.723806 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/
+-rw-rw-rw-   0        0        0    14200 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4114 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1537 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/ceval.h
+-rw-rw-rw-   0        0        0     6989 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/code.h
+-rw-rw-rw-   0        0        0     3797 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4004 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3059 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1473 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/import.h
+-rw-rw-rw-   0        0        0    16979 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1364 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19358 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/object.h
+-rw-rw-rw-   0        0        0     4456 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     5101 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2096 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pymem.h
+-rw-rw-rw-   0        0        0    10134 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pystate.h
+-rw-rw-rw-   0        0        0      575 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46154 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9255 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/descrobject.h
+-rw-rw-rw-   0        0        0     3715 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/dictobject.h
+-rw-rw-rw-   0        0        0    22469 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/enumobject.h
+-rw-rw-rw-   0        0        0     1624 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/fileobject.h
+-rw-rw-rw-   0        0        0      597 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/frameobject.h
+-rw-rw-rw-   0        0        0     4057 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3525 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/grammar.h
+-rw-rw-rw-   0        0        0     3026 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:30.845932 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/
+-rw-rw-rw-   0        0        0      953 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pegen_interface.h
+-rw-rw-rw-   0        0        0      479 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16977 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     3384 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     2620 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_byteswap.h
+-rw-rw-rw-   0        0        0      870 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3403 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      541 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      800 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1541 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     6647 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      473 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5233 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     5299 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0     1548 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     4157 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     1936 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2032 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3741 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3363 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3583 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4452 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      548 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3056 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      442 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/intrcheck.h
+-rw-rw-rw-   0        0        0      521 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/longintrepr.h
+-rw-rw-rw-   0        0        0     9513 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/memoryobject.h
+-rw-rw-rw-   0        0        0     3775 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/methodobject.h
+-rw-rw-rw-   0        0        0     9959 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/modsupport.h
+-rw-rw-rw-   0        0        0     2361 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/namespaceobject.h
+-rw-rw-rw-   0        0        0     1281 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/node.h
+-rw-rw-rw-   0        0        0    24628 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/object.h
+-rw-rw-rw-   0        0        0     8423 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/odictobject.h
+-rw-rw-rw-   0        0        0     4900 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/patchlevel.h
+-rw-rw-rw-   0        0        0      846 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/picklebufobject.h
+-rw-rw-rw-   0        0        0     2474 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyarena.h
+-rw-rw-rw-   0        0        0     1725 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pycapsule.h
+-rw-rw-rw-   0        0        0    48603 2023-07-14 23:28:18.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydtrace.h
+-rw-rw-rw-   0        0        0    12427 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyexpat.h
+-rw-rw-rw-   0        0        0      444 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyfpe.h
+-rw-rw-rw-   0        0        0      466 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyframe.h
+-rw-rw-rw-   0        0        0     4263 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyhash.h
+-rw-rw-rw-   0        0        0     2136 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymacro.h
+-rw-rw-rw-   0        0        0     8580 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymath.h
+-rw-rw-rw-   0        0        0     4406 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymem.h
+-rw-rw-rw-   0        0        0    31393 2023-07-14 23:35:33.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystrtod.h
+-rw-rw-rw-   0        0        0     7673 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pythread.h
+-rw-rw-rw-   0        0        0     8928 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/pytime.h
+-rw-rw-rw-   0        0        0      628 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/rangeobject.h
+-rw-rw-rw-   0        0        0     3324 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/structseq.h
+-rw-rw-rw-   0        0        0     5307 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/sysmodule.h
+-rw-rw-rw-   0        0        0     2642 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/tupleobject.h
+-rw-rw-rw-   0        0        0     2350 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/ucnhash.h
+-rw-rw-rw-   0        0        0    35426 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-14 23:35:22.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-07-14 23:35:28.000000 wasmpy-build-0.3.3/wasmpy_build/include/cp39/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 23:44:28.547552 wasmpy-build-0.3.3/wasmpy_build.egg-info/
+-rw-rw-rw-   0        0        0     1686 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28923 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 23:44:28.000000 wasmpy-build-0.3.3/wasmpy_build.egg-info/top_level.txt
```

### Comparing `wasmpy-build-0.3.2/LICENSE` & `wasmpy-build-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/PKG-INFO` & `wasmpy-build-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.3.2
+Version: 0.3.3
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wasmpy-build-0.3.2/README.md` & `wasmpy-build-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/setup.py` & `wasmpy-build-0.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             paths.append(os.path.join("..", path, file))
 
     return paths
 
 
 setuptools.setup(
     name="wasmpy-build",
-    version="0.3.2",
+    version="0.3.3",
     author="Olivia Ryan",
     author_email="olivia.r.dev@gmail.com",
     description="WebAssembly build tool for CPython C extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/olivi-r/wasmpy-build",
     packages=["wasmpy_build"],
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/__init__.py` & `wasmpy-build-0.3.3/wasmpy_build/__init__.py`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/LICENSE` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/Python.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/boolobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cellobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/classobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/codecs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/complexobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/frameobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/odictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/picklebufobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyctype.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pydebug.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pytime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/datetime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/descrobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/dynamic_annotations.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/errcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/eval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/exports.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/funcobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/genobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_accu.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_asdl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_call.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_condvar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gil.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hamt.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_interp.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_long.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_parser.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_runtime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_symtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/intrcheck.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/iterobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/longintrepr.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/longobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/marshal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/memoryobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/modsupport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/opcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/osdefs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/patchlevel.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/py_curses.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pycapsule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyconfig.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,14 @@
    build system. */
 /* #undef AIX_BUILDDATE */
 
 /* Define for AIX if your compiler is a genuine IBM xlC/xlC_r and you want
    support for AIX C++ shared extension modules. */
 /* #undef AIX_GENUINE_CPLUSPLUS */
 
-/* The normal alignment of `long', in bytes. */
-#define ALIGNOF_LONG 8
-
-/* The normal alignment of `size_t', in bytes. */
-#define ALIGNOF_SIZE_T 8
-
 /* Alternative SOABI used in debug build to load C extensions built in release
    mode */
 /* #undef ALT_SOABI */
 
 /* The Android API level. */
 /* #undef ANDROID_API_LEVEL */
 
@@ -37,18 +31,15 @@
 /* #undef DOUBLE_IS_BIG_ENDIAN_IEEE754 */
 
 /* Define if C doubles are 64-bit IEEE 754 binary format, stored with the
    least significant byte first */
 #define DOUBLE_IS_LITTLE_ENDIAN_IEEE754 1
 
 /* Define if --enable-ipv6 is specified */
-#define ENABLE_IPV6 1
-
-/* Better isolate subinterpreters, experimental build mode. */
-/* #undef EXPERIMENTAL_ISOLATED_SUBINTERPRETERS */
+/* #undef ENABLE_IPV6 */
 
 /* Define to 1 if your system stores words within floats with the most
    significant word first */
 /* #undef FLOAT_WORDS_BIGENDIAN */
 
 /* Define if flock needs to be linked with bsd library. */
 /* #undef FLOCK_NEEDS_LIBBSD */
@@ -59,15 +50,15 @@
 /* Define to 1 if you have the `accept4' function. */
 #define HAVE_ACCEPT4 1
 
 /* Define to 1 if you have the `acosh' function. */
 #define HAVE_ACOSH 1
 
 /* struct addrinfo (netdb.h) */
-#define HAVE_ADDRINFO 1
+/* #undef HAVE_ADDRINFO */
 
 /* Define to 1 if you have the `alarm' function. */
 #define HAVE_ALARM 1
 
 /* Define if aligned memory access is required */
 /* #undef HAVE_ALIGNED_REQUIRED */
 
@@ -77,15 +68,15 @@
 /* Define this if your time.h defines altzone. */
 /* #undef HAVE_ALTZONE */
 
 /* Define to 1 if you have the `asinh' function. */
 #define HAVE_ASINH 1
 
 /* Define to 1 if you have the <asm/types.h> header file. */
-#define HAVE_ASM_TYPES_H 1
+/* #undef HAVE_ASM_TYPES_H */
 
 /* Define to 1 if you have the `atanh' function. */
 #define HAVE_ATANH 1
 
 /* Define to 1 if you have the `bind_textdomain_codeset' function. */
 #define HAVE_BIND_TEXTDOMAIN_CODESET 1
 
@@ -116,15 +107,15 @@
 
 /* define to 1 if your sem_getvalue is broken. */
 /* #undef HAVE_BROKEN_SEM_GETVALUE */
 
 /* Define if `unsetenv` does not return an int. */
 /* #undef HAVE_BROKEN_UNSETENV */
 
-/* Has builtin __atomic_load_n() and __atomic_store_n() functions */
+/* Has builtin atomics */
 #define HAVE_BUILTIN_ATOMIC 1
 
 /* Define to 1 if you have the 'chflags' function. */
 /* #undef HAVE_CHFLAGS */
 
 /* Define to 1 if you have the `chown' function. */
 #define HAVE_CHOWN 1
@@ -140,17 +131,14 @@
 
 /* Define to 1 if you have the `clock_gettime' function. */
 #define HAVE_CLOCK_GETTIME 1
 
 /* Define to 1 if you have the `clock_settime' function. */
 #define HAVE_CLOCK_SETTIME 1
 
-/* Define to 1 if you have the `close_range' function. */
-#define HAVE_CLOSE_RANGE 1
-
 /* Define if the C compiler supports computed gotos. */
 #define HAVE_COMPUTED_GOTOS 1
 
 /* Define to 1 if you have the `confstr' function. */
 #define HAVE_CONFSTR 1
 
 /* Define to 1 if you have the <conio.h> header file. */
@@ -220,56 +208,56 @@
 
 /* Define to 1 if you have the declaration of `isnan', and to 0 if you don't.
  */
 #define HAVE_DECL_ISNAN 1
 
 /* Define to 1 if you have the declaration of `RTLD_DEEPBIND', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_DEEPBIND 1
+/* #undef HAVE_DECL_RTLD_DEEPBIND */
 
 /* Define to 1 if you have the declaration of `RTLD_GLOBAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_GLOBAL 1
+/* #undef HAVE_DECL_RTLD_GLOBAL */
 
 /* Define to 1 if you have the declaration of `RTLD_LAZY', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LAZY 1
+/* #undef HAVE_DECL_RTLD_LAZY */
 
 /* Define to 1 if you have the declaration of `RTLD_LOCAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LOCAL 1
+/* #undef HAVE_DECL_RTLD_LOCAL */
 
 /* Define to 1 if you have the declaration of `RTLD_MEMBER', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_MEMBER 0
+/* #undef HAVE_DECL_RTLD_MEMBER */
 
 /* Define to 1 if you have the declaration of `RTLD_NODELETE', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NODELETE 1
+/* #undef HAVE_DECL_RTLD_NODELETE */
 
 /* Define to 1 if you have the declaration of `RTLD_NOLOAD', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOLOAD 1
+/* #undef HAVE_DECL_RTLD_NOLOAD */
 
 /* Define to 1 if you have the declaration of `RTLD_NOW', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOW 1
+/* #undef HAVE_DECL_RTLD_NOW */
 
 /* Define to 1 if you have the declaration of `tzname', and to 0 if you don't.
  */
 /* #undef HAVE_DECL_TZNAME */
 
 /* Define to 1 if you have the device macros. */
-#define HAVE_DEVICE_MACROS 1
+/* #undef HAVE_DEVICE_MACROS */
 
 /* Define to 1 if you have the /dev/ptc device file. */
 /* #undef HAVE_DEV_PTC */
 
 /* Define to 1 if you have the /dev/ptmx device file. */
-#define HAVE_DEV_PTMX 1
+/* #undef HAVE_DEV_PTMX */
 
 /* Define to 1 if you have the <direct.h> header file. */
 /* #undef HAVE_DIRECT_H */
 
 /* Define to 1 if the dirent structure has a d_type field */
 #define HAVE_DIRENT_D_TYPE 1
 
@@ -277,108 +265,105 @@
  */
 #define HAVE_DIRENT_H 1
 
 /* Define if you have the 'dirfd' function or macro. */
 #define HAVE_DIRFD 1
 
 /* Define to 1 if you have the <dlfcn.h> header file. */
-#define HAVE_DLFCN_H 1
+/* #undef HAVE_DLFCN_H */
 
 /* Define to 1 if you have the `dlopen' function. */
-#define HAVE_DLOPEN 1
+/* #undef HAVE_DLOPEN */
 
 /* Define to 1 if you have the `dup2' function. */
-#define HAVE_DUP2 1
+/* #undef HAVE_DUP2 */
 
 /* Define to 1 if you have the `dup3' function. */
-#define HAVE_DUP3 1
+/* #undef HAVE_DUP3 */
 
 /* Define if you have the '_dyld_shared_cache_contains_path' function. */
 /* #undef HAVE_DYLD_SHARED_CACHE_CONTAINS_PATH */
 
 /* Defined when any dynamic module loading is enabled. */
 #define HAVE_DYNAMIC_LOADING 1
 
 /* Define to 1 if you have the <endian.h> header file. */
 #define HAVE_ENDIAN_H 1
 
 /* Define if you have the 'epoll' functions. */
-#define HAVE_EPOLL 1
+/* #undef HAVE_EPOLL */
 
 /* Define if you have the 'epoll_create1' function. */
-#define HAVE_EPOLL_CREATE1 1
+/* #undef HAVE_EPOLL_CREATE1 */
 
 /* Define to 1 if you have the `erf' function. */
 #define HAVE_ERF 1
 
 /* Define to 1 if you have the `erfc' function. */
 #define HAVE_ERFC 1
 
 /* Define to 1 if you have the <errno.h> header file. */
 #define HAVE_ERRNO_H 1
 
-/* Define if you have the 'eventfd' function. */
-#define HAVE_EVENTFD 1
-
 /* Define to 1 if you have the `execv' function. */
-#define HAVE_EXECV 1
+/* #undef HAVE_EXECV */
 
 /* Define to 1 if you have the `explicit_bzero' function. */
 #define HAVE_EXPLICIT_BZERO 1
 
 /* Define to 1 if you have the `explicit_memset' function. */
 /* #undef HAVE_EXPLICIT_MEMSET */
 
 /* Define to 1 if you have the `expm1' function. */
 #define HAVE_EXPM1 1
 
 /* Define to 1 if you have the `faccessat' function. */
 #define HAVE_FACCESSAT 1
 
 /* Define if you have the 'fchdir' function. */
-#define HAVE_FCHDIR 1
+/* #undef HAVE_FCHDIR */
 
 /* Define to 1 if you have the `fchmod' function. */
-#define HAVE_FCHMOD 1
+/* #undef HAVE_FCHMOD */
 
 /* Define to 1 if you have the `fchmodat' function. */
-#define HAVE_FCHMODAT 1
+/* #undef HAVE_FCHMODAT */
 
 /* Define to 1 if you have the `fchown' function. */
-#define HAVE_FCHOWN 1
+/* #undef HAVE_FCHOWN */
 
 /* Define to 1 if you have the `fchownat' function. */
-#define HAVE_FCHOWNAT 1
+/* #undef HAVE_FCHOWNAT */
 
 /* Define to 1 if you have the <fcntl.h> header file. */
 #define HAVE_FCNTL_H 1
 
 /* Define if you have the 'fdatasync' function. */
 #define HAVE_FDATASYNC 1
 
 /* Define to 1 if you have the `fdopendir' function. */
 #define HAVE_FDOPENDIR 1
 
 /* Define to 1 if you have the `fdwalk' function. */
 /* #undef HAVE_FDWALK */
 
 /* Define to 1 if you have the `fexecve' function. */
-#define HAVE_FEXECVE 1
+/* #undef HAVE_FEXECVE */
 
 /* Define to 1 if you have the `finite' function. */
 #define HAVE_FINITE 1
 
 /* Define to 1 if you have the `flock' function. */
-#define HAVE_FLOCK 1
+/* #undef HAVE_FLOCK */
 
 /* Define to 1 if you have the `fork' function. */
-#define HAVE_FORK 1
+/* #undef HAVE_FORK */
 
 /* Define to 1 if you have the `forkpty' function. */
-#define HAVE_FORKPTY 1
+/* #undef HAVE_FORKPTY */
 
 /* Define to 1 if you have the `fpathconf' function. */
 #define HAVE_FPATHCONF 1
 
 /* Define to 1 if you have the `fseek64' function. */
 /* #undef HAVE_FSEEK64 */
 
@@ -406,332 +391,332 @@
 /* Define to 1 if you have the `ftruncate' function. */
 #define HAVE_FTRUNCATE 1
 
 /* Define to 1 if you have the `futimens' function. */
 #define HAVE_FUTIMENS 1
 
 /* Define to 1 if you have the `futimes' function. */
-#define HAVE_FUTIMES 1
+/* #undef HAVE_FUTIMES */
 
 /* Define to 1 if you have the `futimesat' function. */
-#define HAVE_FUTIMESAT 1
+/* #undef HAVE_FUTIMESAT */
 
 /* Define to 1 if you have the `gai_strerror' function. */
-#define HAVE_GAI_STRERROR 1
+/* #undef HAVE_GAI_STRERROR */
 
 /* Define to 1 if you have the `gamma' function. */
-#define HAVE_GAMMA 1
+/* #undef HAVE_GAMMA */
 
 /* Define if we can use gcc inline assembler to get and set mc68881 fpcr */
 /* #undef HAVE_GCC_ASM_FOR_MC68881 */
 
 /* Define if we can use x64 gcc inline assembler */
-#define HAVE_GCC_ASM_FOR_X64 1
+/* #undef HAVE_GCC_ASM_FOR_X64 */
 
 /* Define if we can use gcc inline assembler to get and set x87 control word
  */
-#define HAVE_GCC_ASM_FOR_X87 1
+/* #undef HAVE_GCC_ASM_FOR_X87 */
 
 /* Define if your compiler provides __uint128_t */
 #define HAVE_GCC_UINT128_T 1
 
 /* Define if you have the getaddrinfo function. */
-#define HAVE_GETADDRINFO 1
+/* #undef HAVE_GETADDRINFO */
 
 /* Define this if you have flockfile(), getc_unlocked(), and funlockfile() */
-#define HAVE_GETC_UNLOCKED 1
+/* #undef HAVE_GETC_UNLOCKED */
 
 /* Define to 1 if you have the `getentropy' function. */
 #define HAVE_GETENTROPY 1
 
 /* Define to 1 if you have the `getgrgid_r' function. */
-#define HAVE_GETGRGID_R 1
+/* #undef HAVE_GETGRGID_R */
 
 /* Define to 1 if you have the `getgrnam_r' function. */
-#define HAVE_GETGRNAM_R 1
+/* #undef HAVE_GETGRNAM_R */
 
 /* Define to 1 if you have the `getgrouplist' function. */
-#define HAVE_GETGROUPLIST 1
+/* #undef HAVE_GETGROUPLIST */
 
 /* Define to 1 if you have the `getgroups' function. */
-#define HAVE_GETGROUPS 1
+/* #undef HAVE_GETGROUPS */
 
 /* Define to 1 if you have the `gethostbyname' function. */
 /* #undef HAVE_GETHOSTBYNAME */
 
 /* Define this if you have some version of gethostbyname_r() */
-#define HAVE_GETHOSTBYNAME_R 1
+/* #undef HAVE_GETHOSTBYNAME_R */
 
 /* Define this if you have the 3-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_3_ARG */
 
 /* Define this if you have the 5-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_5_ARG */
 
 /* Define this if you have the 6-arg version of gethostbyname_r(). */
-#define HAVE_GETHOSTBYNAME_R_6_ARG 1
+/* #undef HAVE_GETHOSTBYNAME_R_6_ARG */
 
 /* Define to 1 if you have the `getitimer' function. */
-#define HAVE_GETITIMER 1
+/* #undef HAVE_GETITIMER */
 
 /* Define to 1 if you have the `getloadavg' function. */
-#define HAVE_GETLOADAVG 1
+/* #undef HAVE_GETLOADAVG */
 
 /* Define to 1 if you have the `getlogin' function. */
-#define HAVE_GETLOGIN 1
+/* #undef HAVE_GETLOGIN */
 
 /* Define to 1 if you have the `getnameinfo' function. */
-#define HAVE_GETNAMEINFO 1
+/* #undef HAVE_GETNAMEINFO */
 
 /* Define if you have the 'getpagesize' function. */
-#define HAVE_GETPAGESIZE 1
+/* #undef HAVE_GETPAGESIZE */
 
 /* Define to 1 if you have the `getpeername' function. */
-#define HAVE_GETPEERNAME 1
+/* #undef HAVE_GETPEERNAME */
 
 /* Define to 1 if you have the `getpgid' function. */
-#define HAVE_GETPGID 1
+/* #undef HAVE_GETPGID */
 
 /* Define to 1 if you have the `getpgrp' function. */
-#define HAVE_GETPGRP 1
+/* #undef HAVE_GETPGRP */
 
 /* Define to 1 if you have the `getpid' function. */
-#define HAVE_GETPID 1
+/* #undef HAVE_GETPID */
 
 /* Define to 1 if you have the `getpriority' function. */
-#define HAVE_GETPRIORITY 1
+/* #undef HAVE_GETPRIORITY */
 
 /* Define to 1 if you have the `getpwent' function. */
-#define HAVE_GETPWENT 1
+/* #undef HAVE_GETPWENT */
 
 /* Define to 1 if you have the `getpwnam_r' function. */
-#define HAVE_GETPWNAM_R 1
+/* #undef HAVE_GETPWNAM_R */
 
 /* Define to 1 if you have the `getpwuid_r' function. */
-#define HAVE_GETPWUID_R 1
+/* #undef HAVE_GETPWUID_R */
 
 /* Define to 1 if the getrandom() function is available */
-#define HAVE_GETRANDOM 1
+/* #undef HAVE_GETRANDOM */
 
 /* Define to 1 if the Linux getrandom() syscall is available */
-#define HAVE_GETRANDOM_SYSCALL 1
+/* #undef HAVE_GETRANDOM_SYSCALL */
 
 /* Define to 1 if you have the `getresgid' function. */
-#define HAVE_GETRESGID 1
+/* #undef HAVE_GETRESGID */
 
 /* Define to 1 if you have the `getresuid' function. */
-#define HAVE_GETRESUID 1
+/* #undef HAVE_GETRESUID */
 
 /* Define to 1 if you have the `getsid' function. */
-#define HAVE_GETSID 1
+/* #undef HAVE_GETSID */
 
 /* Define to 1 if you have the `getspent' function. */
-#define HAVE_GETSPENT 1
+/* #undef HAVE_GETSPENT */
 
 /* Define to 1 if you have the `getspnam' function. */
-#define HAVE_GETSPNAM 1
+/* #undef HAVE_GETSPNAM */
 
 /* Define to 1 if you have the `getwd' function. */
-#define HAVE_GETWD 1
+/* #undef HAVE_GETWD */
 
 /* Define if glibc has incorrect _FORTIFY_SOURCE wrappers for memmove and
    bcopy. */
 /* #undef HAVE_GLIBC_MEMMOVE_BUG */
 
 /* Define to 1 if you have the <grp.h> header file. */
-#define HAVE_GRP_H 1
+/* #undef HAVE_GRP_H */
 
 /* Define if you have the 'hstrerror' function. */
-#define HAVE_HSTRERROR 1
+/* #undef HAVE_HSTRERROR */
 
 /* Define this if you have le64toh() */
 #define HAVE_HTOLE64 1
 
 /* Define to 1 if you have the `hypot' function. */
 #define HAVE_HYPOT 1
 
 /* Define to 1 if you have the <ieeefp.h> header file. */
 /* #undef HAVE_IEEEFP_H */
 
 /* Define to 1 if you have the `if_nameindex' function. */
-#define HAVE_IF_NAMEINDEX 1
+/* #undef HAVE_IF_NAMEINDEX */
 
 /* Define if you have the 'inet_aton' function. */
 #define HAVE_INET_ATON 1
 
 /* Define if you have the 'inet_pton' function. */
 #define HAVE_INET_PTON 1
 
 /* Define to 1 if you have the `initgroups' function. */
-#define HAVE_INITGROUPS 1
+/* #undef HAVE_INITGROUPS */
 
 /* Define to 1 if you have the <inttypes.h> header file. */
 #define HAVE_INTTYPES_H 1
 
 /* Define to 1 if you have the <io.h> header file. */
 /* #undef HAVE_IO_H */
 
 /* Define if gcc has the ipa-pure-const bug. */
 /* #undef HAVE_IPA_PURE_CONST_BUG */
 
 /* Define to 1 if you have the `kill' function. */
-#define HAVE_KILL 1
+/* #undef HAVE_KILL */
 
 /* Define to 1 if you have the `killpg' function. */
-#define HAVE_KILLPG 1
+/* #undef HAVE_KILLPG */
 
 /* Define if you have the 'kqueue' functions. */
 /* #undef HAVE_KQUEUE */
 
 /* Define to 1 if you have the <langinfo.h> header file. */
 #define HAVE_LANGINFO_H 1
 
 /* Defined to enable large file support when an off_t is bigger than a long
    and long long is at least as big as an off_t. You may need to add some
    flags for configuration and compilation to enable this mode. (For Solaris
    and Linux, the necessary defines are already defined.) */
-/* #undef HAVE_LARGEFILE_SUPPORT */
+#define HAVE_LARGEFILE_SUPPORT 1
 
 /* Define to 1 if you have the 'lchflags' function. */
 /* #undef HAVE_LCHFLAGS */
 
 /* Define to 1 if you have the `lchmod' function. */
 /* #undef HAVE_LCHMOD */
 
 /* Define to 1 if you have the `lchown' function. */
-#define HAVE_LCHOWN 1
+/* #undef HAVE_LCHOWN */
 
 /* Define to 1 if you have the `lgamma' function. */
 #define HAVE_LGAMMA 1
 
 /* Define to 1 if you have the `dl' library (-ldl). */
 #define HAVE_LIBDL 1
 
 /* Define to 1 if you have the `dld' library (-ldld). */
 /* #undef HAVE_LIBDLD */
 
 /* Define to 1 if you have the `ieee' library (-lieee). */
 /* #undef HAVE_LIBIEEE */
 
 /* Define to 1 if you have the <libintl.h> header file. */
-#define HAVE_LIBINTL_H 1
+/* #undef HAVE_LIBINTL_H */
 
-/* Define to build the readline module. */
+/* Define if you have the readline library (-lreadline). */
 /* #undef HAVE_LIBREADLINE */
 
 /* Define to 1 if you have the `resolv' library (-lresolv). */
-/* #undef HAVE_LIBRESOLV */
+#define HAVE_LIBRESOLV 1
 
 /* Define to 1 if you have the `sendfile' library (-lsendfile). */
 /* #undef HAVE_LIBSENDFILE */
 
 /* Define to 1 if you have the <libutil.h> header file. */
-/* #undef HAVE_LIBUTIL_H */
+#define HAVE_LIBUTIL_H 1
 
 /* Define to 1 if you have the `uuid' library (-luuid). */
 /* #undef HAVE_LIBUUID */
 
 /* Define if you have the 'link' function. */
 #define HAVE_LINK 1
 
 /* Define to 1 if you have the `linkat' function. */
 #define HAVE_LINKAT 1
 
 /* Define to 1 if you have the <linux/auxvec.h> header file. */
-#define HAVE_LINUX_AUXVEC_H 1
+/* #undef HAVE_LINUX_AUXVEC_H */
 
 /* Define to 1 if you have the <linux/can/bcm.h> header file. */
-#define HAVE_LINUX_CAN_BCM_H 1
+/* #undef HAVE_LINUX_CAN_BCM_H */
 
 /* Define to 1 if you have the <linux/can.h> header file. */
-#define HAVE_LINUX_CAN_H 1
+/* #undef HAVE_LINUX_CAN_H */
 
 /* Define to 1 if you have the <linux/can/j1939.h> header file. */
-#define HAVE_LINUX_CAN_J1939_H 1
+/* #undef HAVE_LINUX_CAN_J1939_H */
 
 /* Define if compiling using Linux 3.6 or later. */
-#define HAVE_LINUX_CAN_RAW_FD_FRAMES 1
+/* #undef HAVE_LINUX_CAN_RAW_FD_FRAMES */
 
 /* Define to 1 if you have the <linux/can/raw.h> header file. */
-#define HAVE_LINUX_CAN_RAW_H 1
+/* #undef HAVE_LINUX_CAN_RAW_H */
 
 /* Define if compiling using Linux 4.1 or later. */
-#define HAVE_LINUX_CAN_RAW_JOIN_FILTERS 1
+/* #undef HAVE_LINUX_CAN_RAW_JOIN_FILTERS */
 
 /* Define to 1 if you have the <linux/memfd.h> header file. */
-#define HAVE_LINUX_MEMFD_H 1
+/* #undef HAVE_LINUX_MEMFD_H */
 
 /* Define to 1 if you have the <linux/netlink.h> header file. */
-#define HAVE_LINUX_NETLINK_H 1
+/* #undef HAVE_LINUX_NETLINK_H */
 
 /* Define to 1 if you have the <linux/qrtr.h> header file. */
-#define HAVE_LINUX_QRTR_H 1
+/* #undef HAVE_LINUX_QRTR_H */
 
 /* Define to 1 if you have the <linux/random.h> header file. */
-#define HAVE_LINUX_RANDOM_H 1
+/* #undef HAVE_LINUX_RANDOM_H */
 
 /* Define to 1 if you have the <linux/tipc.h> header file. */
-#define HAVE_LINUX_TIPC_H 1
+/* #undef HAVE_LINUX_TIPC_H */
 
 /* Define to 1 if you have the <linux/vm_sockets.h> header file. */
-#define HAVE_LINUX_VM_SOCKETS_H 1
+/* #undef HAVE_LINUX_VM_SOCKETS_H */
 
 /* Define to 1 if you have the <linux/wait.h> header file. */
-#define HAVE_LINUX_WAIT_H 1
+/* #undef HAVE_LINUX_WAIT_H */
 
 /* Define to 1 if you have the `lockf' function. */
-#define HAVE_LOCKF 1
+/* #undef HAVE_LOCKF */
 
 /* Define to 1 if you have the `log1p' function. */
 #define HAVE_LOG1P 1
 
 /* Define to 1 if you have the `log2' function. */
 #define HAVE_LOG2 1
 
 /* Define to 1 if the system has the type `long double'. */
 #define HAVE_LONG_DOUBLE 1
 
 /* Define to 1 if you have the `lstat' function. */
 #define HAVE_LSTAT 1
 
 /* Define to 1 if you have the `lutimes' function. */
-#define HAVE_LUTIMES 1
+/* #undef HAVE_LUTIMES */
 
 /* Define to 1 if you have the `madvise' function. */
-#define HAVE_MADVISE 1
+/* #undef HAVE_MADVISE */
 
 /* Define this if you have the makedev macro. */
-#define HAVE_MAKEDEV 1
+/* #undef HAVE_MAKEDEV */
 
 /* Define to 1 if you have the `mbrtowc' function. */
 #define HAVE_MBRTOWC 1
 
 /* Define if you have the 'memfd_create' function. */
-#define HAVE_MEMFD_CREATE 1
+/* #undef HAVE_MEMFD_CREATE */
 
 /* Define to 1 if you have the <memory.h> header file. */
 #define HAVE_MEMORY_H 1
 
 /* Define to 1 if you have the `memrchr' function. */
 #define HAVE_MEMRCHR 1
 
 /* Define to 1 if you have the `mkdirat' function. */
 #define HAVE_MKDIRAT 1
 
 /* Define to 1 if you have the `mkfifo' function. */
-#define HAVE_MKFIFO 1
+/* #undef HAVE_MKFIFO */
 
 /* Define to 1 if you have the `mkfifoat' function. */
-#define HAVE_MKFIFOAT 1
+/* #undef HAVE_MKFIFOAT */
 
 /* Define to 1 if you have the `mknod' function. */
-#define HAVE_MKNOD 1
+/* #undef HAVE_MKNOD */
 
 /* Define to 1 if you have the `mknodat' function. */
-#define HAVE_MKNODAT 1
+/* #undef HAVE_MKNODAT */
 
 /* Define to 1 if you have the `mktime' function. */
 #define HAVE_MKTIME 1
 
 /* Define to 1 if you have the `mmap' function. */
 #define HAVE_MMAP 1
 
@@ -744,37 +729,37 @@
 /* Define to 1 if you have the <ndir.h> header file, and it defines `DIR'. */
 /* #undef HAVE_NDIR_H */
 
 /* Define to 1 if you have the <netpacket/packet.h> header file. */
 #define HAVE_NETPACKET_PACKET_H 1
 
 /* Define to 1 if you have the <net/if.h> header file. */
-#define HAVE_NET_IF_H 1
+/* #undef HAVE_NET_IF_H */
 
 /* Define to 1 if you have the `nice' function. */
-#define HAVE_NICE 1
+/* #undef HAVE_NICE */
 
 /* Define if the internal form of wchar_t in non-Unicode locales is not
    Unicode. */
 /* #undef HAVE_NON_UNICODE_WCHAR_T_REPRESENTATION */
 
 /* Define to 1 if you have the `openat' function. */
 #define HAVE_OPENAT 1
 
 /* Define to 1 if you have the `openpty' function. */
-#define HAVE_OPENPTY 1
+/* #undef HAVE_OPENPTY */
 
 /* Define to 1 if you have the `pathconf' function. */
 #define HAVE_PATHCONF 1
 
 /* Define to 1 if you have the `pause' function. */
-#define HAVE_PAUSE 1
+/* #undef HAVE_PAUSE */
 
 /* Define to 1 if you have the `pipe2' function. */
-#define HAVE_PIPE2 1
+/* #undef HAVE_PIPE2 */
 
 /* Define to 1 if you have the `plock' function. */
 /* #undef HAVE_PLOCK */
 
 /* Define to 1 if you have the `poll' function. */
 #define HAVE_POLL 1
 
@@ -784,30 +769,30 @@
 /* Define to 1 if you have the `posix_fadvise' function. */
 #define HAVE_POSIX_FADVISE 1
 
 /* Define to 1 if you have the `posix_fallocate' function. */
 #define HAVE_POSIX_FALLOCATE 1
 
 /* Define to 1 if you have the `posix_spawn' function. */
-#define HAVE_POSIX_SPAWN 1
+/* #undef HAVE_POSIX_SPAWN */
 
 /* Define to 1 if you have the `posix_spawnp' function. */
-#define HAVE_POSIX_SPAWNP 1
+/* #undef HAVE_POSIX_SPAWNP */
 
 /* Define to 1 if you have the `pread' function. */
 #define HAVE_PREAD 1
 
 /* Define to 1 if you have the `preadv' function. */
 #define HAVE_PREADV 1
 
 /* Define to 1 if you have the `preadv2' function. */
-#define HAVE_PREADV2 1
+/* #undef HAVE_PREADV2 */
 
 /* Define if you have the 'prlimit' functions. */
-#define HAVE_PRLIMIT 1
+/* #undef HAVE_PRLIMIT */
 
 /* Define to 1 if you have the <process.h> header file. */
 /* #undef HAVE_PROCESS_H */
 
 /* Define if your compiler supports function prototype */
 #define HAVE_PROTOTYPES 1
 
@@ -823,42 +808,42 @@
 /* Define to 1 if you have the <pthread.h> header file. */
 #define HAVE_PTHREAD_H 1
 
 /* Define to 1 if you have the `pthread_init' function. */
 /* #undef HAVE_PTHREAD_INIT */
 
 /* Define to 1 if you have the `pthread_kill' function. */
-#define HAVE_PTHREAD_KILL 1
+/* #undef HAVE_PTHREAD_KILL */
 
 /* Define to 1 if you have the `pthread_sigmask' function. */
-#define HAVE_PTHREAD_SIGMASK 1
+/* #undef HAVE_PTHREAD_SIGMASK */
 
 /* Define to 1 if you have the <pty.h> header file. */
-#define HAVE_PTY_H 1
+/* #undef HAVE_PTY_H */
 
 /* Define to 1 if you have the `pwrite' function. */
 #define HAVE_PWRITE 1
 
 /* Define to 1 if you have the `pwritev' function. */
 #define HAVE_PWRITEV 1
 
 /* Define to 1 if you have the `pwritev2' function. */
-#define HAVE_PWRITEV2 1
+/* #undef HAVE_PWRITEV2 */
 
 /* Define to 1 if you have the `readlink' function. */
 #define HAVE_READLINK 1
 
 /* Define to 1 if you have the `readlinkat' function. */
 #define HAVE_READLINKAT 1
 
 /* Define to 1 if you have the `readv' function. */
 #define HAVE_READV 1
 
 /* Define to 1 if you have the `realpath' function. */
-#define HAVE_REALPATH 1
+/* #undef HAVE_REALPATH */
 
 /* Define to 1 if you have the `renameat' function. */
 #define HAVE_RENAMEAT 1
 
 /* Define if readline supports append_history */
 /* #undef HAVE_RL_APPEND_HISTORY */
 
@@ -886,168 +871,165 @@
 /* Define to 1 if you have the `round' function. */
 #define HAVE_ROUND 1
 
 /* Define to 1 if you have the `rtpSpawn' function. */
 /* #undef HAVE_RTPSPAWN */
 
 /* Define to 1 if you have the `sched_get_priority_max' function. */
-#define HAVE_SCHED_GET_PRIORITY_MAX 1
+/* #undef HAVE_SCHED_GET_PRIORITY_MAX */
 
 /* Define to 1 if you have the <sched.h> header file. */
 #define HAVE_SCHED_H 1
 
 /* Define to 1 if you have the `sched_rr_get_interval' function. */
-#define HAVE_SCHED_RR_GET_INTERVAL 1
+/* #undef HAVE_SCHED_RR_GET_INTERVAL */
 
 /* Define to 1 if you have the `sched_setaffinity' function. */
-#define HAVE_SCHED_SETAFFINITY 1
+/* #undef HAVE_SCHED_SETAFFINITY */
 
 /* Define to 1 if you have the `sched_setparam' function. */
-#define HAVE_SCHED_SETPARAM 1
+/* #undef HAVE_SCHED_SETPARAM */
 
 /* Define to 1 if you have the `sched_setscheduler' function. */
-#define HAVE_SCHED_SETSCHEDULER 1
+/* #undef HAVE_SCHED_SETSCHEDULER */
 
 /* Define to 1 if you have the `sem_clockwait' function. */
-#define HAVE_SEM_CLOCKWAIT 1
+/* #undef HAVE_SEM_CLOCKWAIT */
 
 /* Define to 1 if you have the `sem_getvalue' function. */
-#define HAVE_SEM_GETVALUE 1
+/* #undef HAVE_SEM_GETVALUE */
 
 /* Define to 1 if you have the `sem_open' function. */
-#define HAVE_SEM_OPEN 1
+/* #undef HAVE_SEM_OPEN */
 
 /* Define to 1 if you have the `sem_timedwait' function. */
-#define HAVE_SEM_TIMEDWAIT 1
+/* #undef HAVE_SEM_TIMEDWAIT */
 
 /* Define to 1 if you have the `sem_unlink' function. */
-#define HAVE_SEM_UNLINK 1
+/* #undef HAVE_SEM_UNLINK */
 
 /* Define to 1 if you have the `sendfile' function. */
-#define HAVE_SENDFILE 1
+/* #undef HAVE_SENDFILE */
 
 /* Define to 1 if you have the `setegid' function. */
-#define HAVE_SETEGID 1
+/* #undef HAVE_SETEGID */
 
 /* Define to 1 if you have the `seteuid' function. */
-#define HAVE_SETEUID 1
+/* #undef HAVE_SETEUID */
 
 /* Define to 1 if you have the `setgid' function. */
-#define HAVE_SETGID 1
+/* #undef HAVE_SETGID */
 
 /* Define if you have the 'setgroups' function. */
-#define HAVE_SETGROUPS 1
+/* #undef HAVE_SETGROUPS */
 
 /* Define to 1 if you have the `sethostname' function. */
-#define HAVE_SETHOSTNAME 1
+/* #undef HAVE_SETHOSTNAME */
 
 /* Define to 1 if you have the `setitimer' function. */
-#define HAVE_SETITIMER 1
+/* #undef HAVE_SETITIMER */
 
 /* Define to 1 if you have the `setlocale' function. */
 #define HAVE_SETLOCALE 1
 
 /* Define to 1 if you have the `setpgid' function. */
-#define HAVE_SETPGID 1
+/* #undef HAVE_SETPGID */
 
 /* Define to 1 if you have the `setpgrp' function. */
-#define HAVE_SETPGRP 1
+/* #undef HAVE_SETPGRP */
 
 /* Define to 1 if you have the `setpriority' function. */
-#define HAVE_SETPRIORITY 1
+/* #undef HAVE_SETPRIORITY */
 
 /* Define to 1 if you have the `setregid' function. */
-#define HAVE_SETREGID 1
+/* #undef HAVE_SETREGID */
 
 /* Define to 1 if you have the `setresgid' function. */
-#define HAVE_SETRESGID 1
+/* #undef HAVE_SETRESGID */
 
 /* Define to 1 if you have the `setresuid' function. */
-#define HAVE_SETRESUID 1
+/* #undef HAVE_SETRESUID */
 
 /* Define to 1 if you have the `setreuid' function. */
-#define HAVE_SETREUID 1
+/* #undef HAVE_SETREUID */
 
 /* Define to 1 if you have the `setsid' function. */
-#define HAVE_SETSID 1
+/* #undef HAVE_SETSID */
 
 /* Define to 1 if you have the `setuid' function. */
-#define HAVE_SETUID 1
+/* #undef HAVE_SETUID */
 
 /* Define to 1 if you have the `setvbuf' function. */
 #define HAVE_SETVBUF 1
 
 /* Define to 1 if you have the <shadow.h> header file. */
-#define HAVE_SHADOW_H 1
+/* #undef HAVE_SHADOW_H */
 
 /* Define to 1 if you have the `shm_open' function. */
-#define HAVE_SHM_OPEN 1
+/* #undef HAVE_SHM_OPEN */
 
 /* Define to 1 if you have the `shm_unlink' function. */
-#define HAVE_SHM_UNLINK 1
+/* #undef HAVE_SHM_UNLINK */
 
 /* Define to 1 if you have the `sigaction' function. */
-#define HAVE_SIGACTION 1
+/* #undef HAVE_SIGACTION */
 
 /* Define to 1 if you have the `sigaltstack' function. */
-#define HAVE_SIGALTSTACK 1
+/* #undef HAVE_SIGALTSTACK */
 
 /* Define to 1 if you have the `sigfillset' function. */
-#define HAVE_SIGFILLSET 1
+/* #undef HAVE_SIGFILLSET */
 
 /* Define to 1 if `si_band' is a member of `siginfo_t'. */
-#define HAVE_SIGINFO_T_SI_BAND 1
+/* #undef HAVE_SIGINFO_T_SI_BAND */
 
 /* Define to 1 if you have the `siginterrupt' function. */
-#define HAVE_SIGINTERRUPT 1
+/* #undef HAVE_SIGINTERRUPT */
 
 /* Define to 1 if you have the <signal.h> header file. */
-#define HAVE_SIGNAL_H 1
+/* #undef HAVE_SIGNAL_H */
 
 /* Define to 1 if you have the `sigpending' function. */
-#define HAVE_SIGPENDING 1
+/* #undef HAVE_SIGPENDING */
 
 /* Define to 1 if you have the `sigrelse' function. */
-#define HAVE_SIGRELSE 1
+/* #undef HAVE_SIGRELSE */
 
 /* Define to 1 if you have the `sigtimedwait' function. */
-#define HAVE_SIGTIMEDWAIT 1
+/* #undef HAVE_SIGTIMEDWAIT */
 
 /* Define to 1 if you have the `sigwait' function. */
-#define HAVE_SIGWAIT 1
+/* #undef HAVE_SIGWAIT */
 
 /* Define to 1 if you have the `sigwaitinfo' function. */
-#define HAVE_SIGWAITINFO 1
+/* #undef HAVE_SIGWAITINFO */
 
 /* Define to 1 if you have the `snprintf' function. */
 #define HAVE_SNPRINTF 1
 
 /* struct sockaddr_alg (linux/if_alg.h) */
-#define HAVE_SOCKADDR_ALG 1
+/* #undef HAVE_SOCKADDR_ALG */
 
 /* Define if sockaddr has sa_len member */
 /* #undef HAVE_SOCKADDR_SA_LEN */
 
 /* struct sockaddr_storage (sys/socket.h) */
 #define HAVE_SOCKADDR_STORAGE 1
 
 /* Define if you have the 'socketpair' function. */
-#define HAVE_SOCKETPAIR 1
+/* #undef HAVE_SOCKETPAIR */
 
 /* Define to 1 if you have the <spawn.h> header file. */
-#define HAVE_SPAWN_H 1
-
-/* Define to 1 if you have the `splice' function. */
-#define HAVE_SPLICE 1
+/* #undef HAVE_SPAWN_H */
 
 /* Define if your compiler provides ssize_t */
 #define HAVE_SSIZE_T 1
 
 /* Define to 1 if you have the `statvfs' function. */
-#define HAVE_STATVFS 1
+/* #undef HAVE_STATVFS */
 
 /* Define if you have struct stat.st_mtim.tv_nsec */
 #define HAVE_STAT_TV_NSEC 1
 
 /* Define if you have struct stat.st_mtimensec */
 /* #undef HAVE_STAT_TV_NSEC2 */
 
@@ -1060,37 +1042,40 @@
 
 /* Define to 1 if you have the <stdlib.h> header file. */
 #define HAVE_STDLIB_H 1
 
 /* Has stdatomic.h with atomic_int and atomic_uintptr_t */
 #define HAVE_STD_ATOMIC 1
 
+/* Define to 1 if you have the `strdup' function. */
+#define HAVE_STRDUP 1
+
 /* Define to 1 if you have the `strftime' function. */
 #define HAVE_STRFTIME 1
 
 /* Define to 1 if you have the <strings.h> header file. */
 #define HAVE_STRINGS_H 1
 
 /* Define to 1 if you have the <string.h> header file. */
 #define HAVE_STRING_H 1
 
 /* Define to 1 if you have the `strlcpy' function. */
-/* #undef HAVE_STRLCPY */
+#define HAVE_STRLCPY 1
 
 /* Define to 1 if you have the <stropts.h> header file. */
-/* #undef HAVE_STROPTS_H */
+#define HAVE_STROPTS_H 1
 
 /* Define to 1 if you have the `strsignal' function. */
-#define HAVE_STRSIGNAL 1
+/* #undef HAVE_STRSIGNAL */
 
 /* Define to 1 if `pw_gecos' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_GECOS 1
+/* #undef HAVE_STRUCT_PASSWD_PW_GECOS */
 
 /* Define to 1 if `pw_passwd' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_PASSWD 1
+/* #undef HAVE_STRUCT_PASSWD_PW_PASSWD */
 
 /* Define to 1 if `st_birthtime' is a member of `struct stat'. */
 /* #undef HAVE_STRUCT_STAT_ST_BIRTHTIME */
 
 /* Define to 1 if `st_blksize' is a member of `struct stat'. */
 #define HAVE_STRUCT_STAT_ST_BLKSIZE 1
 
@@ -1112,27 +1097,27 @@
 /* Define if you have the 'symlink' function. */
 #define HAVE_SYMLINK 1
 
 /* Define to 1 if you have the `symlinkat' function. */
 #define HAVE_SYMLINKAT 1
 
 /* Define to 1 if you have the `sync' function. */
-#define HAVE_SYNC 1
+/* #undef HAVE_SYNC */
 
 /* Define to 1 if you have the `sysconf' function. */
 #define HAVE_SYSCONF 1
 
 /* Define to 1 if you have the <sysexits.h> header file. */
 #define HAVE_SYSEXITS_H 1
 
 /* Define to 1 if you have the <sys/audioio.h> header file. */
 /* #undef HAVE_SYS_AUDIOIO_H */
 
 /* Define to 1 if you have the <sys/auxv.h> header file. */
-#define HAVE_SYS_AUXV_H 1
+/* #undef HAVE_SYS_AUXV_H */
 
 /* Define to 1 if you have the <sys/bsdtty.h> header file. */
 /* #undef HAVE_SYS_BSDTTY_H */
 
 /* Define to 1 if you have the <sys/devpoll.h> header file. */
 /* #undef HAVE_SYS_DEVPOLL_H */
 
@@ -1140,18 +1125,15 @@
  */
 /* #undef HAVE_SYS_DIR_H */
 
 /* Define to 1 if you have the <sys/endian.h> header file. */
 /* #undef HAVE_SYS_ENDIAN_H */
 
 /* Define to 1 if you have the <sys/epoll.h> header file. */
-#define HAVE_SYS_EPOLL_H 1
-
-/* Define to 1 if you have the <sys/eventfd.h> header file. */
-#define HAVE_SYS_EVENTFD_H 1
+/* #undef HAVE_SYS_EPOLL_H */
 
 /* Define to 1 if you have the <sys/event.h> header file. */
 /* #undef HAVE_SYS_EVENT_H */
 
 /* Define to 1 if you have the <sys/file.h> header file. */
 #define HAVE_SYS_FILE_H 1
 
@@ -1195,30 +1177,30 @@
 /* Define to 1 if you have the <sys/resource.h> header file. */
 #define HAVE_SYS_RESOURCE_H 1
 
 /* Define to 1 if you have the <sys/select.h> header file. */
 #define HAVE_SYS_SELECT_H 1
 
 /* Define to 1 if you have the <sys/sendfile.h> header file. */
-#define HAVE_SYS_SENDFILE_H 1
+/* #undef HAVE_SYS_SENDFILE_H */
 
 /* Define to 1 if you have the <sys/socket.h> header file. */
 #define HAVE_SYS_SOCKET_H 1
 
 /* Define to 1 if you have the <sys/statvfs.h> header file. */
-#define HAVE_SYS_STATVFS_H 1
+/* #undef HAVE_SYS_STATVFS_H */
 
 /* Define to 1 if you have the <sys/stat.h> header file. */
 #define HAVE_SYS_STAT_H 1
 
 /* Define to 1 if you have the <sys/syscall.h> header file. */
 #define HAVE_SYS_SYSCALL_H 1
 
 /* Define to 1 if you have the <sys/sysmacros.h> header file. */
-#define HAVE_SYS_SYSMACROS_H 1
+/* #undef HAVE_SYS_SYSMACROS_H */
 
 /* Define to 1 if you have the <sys/sys_domain.h> header file. */
 /* #undef HAVE_SYS_SYS_DOMAIN_H */
 
 /* Define to 1 if you have the <sys/termio.h> header file. */
 /* #undef HAVE_SYS_TERMIO_H */
 
@@ -1237,51 +1219,51 @@
 /* Define to 1 if you have the <sys/un.h> header file. */
 #define HAVE_SYS_UN_H 1
 
 /* Define to 1 if you have the <sys/utsname.h> header file. */
 #define HAVE_SYS_UTSNAME_H 1
 
 /* Define to 1 if you have the <sys/wait.h> header file. */
-#define HAVE_SYS_WAIT_H 1
+/* #undef HAVE_SYS_WAIT_H */
 
 /* Define to 1 if you have the <sys/xattr.h> header file. */
-#define HAVE_SYS_XATTR_H 1
+/* #undef HAVE_SYS_XATTR_H */
 
 /* Define to 1 if you have the `tcgetpgrp' function. */
-#define HAVE_TCGETPGRP 1
+/* #undef HAVE_TCGETPGRP */
 
 /* Define to 1 if you have the `tcsetpgrp' function. */
-#define HAVE_TCSETPGRP 1
+/* #undef HAVE_TCSETPGRP */
 
 /* Define to 1 if you have the `tempnam' function. */
-#define HAVE_TEMPNAM 1
+/* #undef HAVE_TEMPNAM */
 
 /* Define to 1 if you have the <termios.h> header file. */
-#define HAVE_TERMIOS_H 1
+/* #undef HAVE_TERMIOS_H */
 
 /* Define to 1 if you have the <term.h> header file. */
 /* #undef HAVE_TERM_H */
 
 /* Define to 1 if you have the `tgamma' function. */
 #define HAVE_TGAMMA 1
 
 /* Define to 1 if you have the `timegm' function. */
 #define HAVE_TIMEGM 1
 
 /* Define to 1 if you have the `times' function. */
 #define HAVE_TIMES 1
 
 /* Define to 1 if you have the `tmpfile' function. */
-#define HAVE_TMPFILE 1
+/* #undef HAVE_TMPFILE */
 
 /* Define to 1 if you have the `tmpnam' function. */
-#define HAVE_TMPNAM 1
+/* #undef HAVE_TMPNAM */
 
 /* Define to 1 if you have the `tmpnam_r' function. */
-#define HAVE_TMPNAM_R 1
+/* #undef HAVE_TMPNAM_R */
 
 /* Define to 1 if your `struct tm' has `tm_zone'. Deprecated, use
    `HAVE_STRUCT_TM_TM_ZONE' instead. */
 #define HAVE_TM_ZONE 1
 
 /* Define to 1 if you have the `truncate' function. */
 #define HAVE_TRUNCATE 1
@@ -1310,15 +1292,15 @@
 /* Define to 1 if you have the <util.h> header file. */
 /* #undef HAVE_UTIL_H */
 
 /* Define to 1 if you have the `utimensat' function. */
 #define HAVE_UTIMENSAT 1
 
 /* Define to 1 if you have the `utimes' function. */
-#define HAVE_UTIMES 1
+/* #undef HAVE_UTIMES */
 
 /* Define to 1 if you have the <utime.h> header file. */
 #define HAVE_UTIME_H 1
 
 /* Define if uuid_create() exists. */
 /* #undef HAVE_UUID_CREATE */
 
@@ -1330,28 +1312,25 @@
 
 /* Define to 1 if you have the <uuid.h> header file. */
 /* #undef HAVE_UUID_H */
 
 /* Define to 1 if you have the <uuid/uuid.h> header file. */
 /* #undef HAVE_UUID_UUID_H */
 
-/* Define to 1 if you have the `vfork' function. */
-#define HAVE_VFORK 1
-
 /* Define to 1 if you have the `wait3' function. */
-#define HAVE_WAIT3 1
+/* #undef HAVE_WAIT3 */
 
 /* Define to 1 if you have the `wait4' function. */
-#define HAVE_WAIT4 1
+/* #undef HAVE_WAIT4 */
 
 /* Define to 1 if you have the `waitid' function. */
-#define HAVE_WAITID 1
+/* #undef HAVE_WAITID */
 
 /* Define to 1 if you have the `waitpid' function. */
-#define HAVE_WAITPID 1
+/* #undef HAVE_WAITPID */
 
 /* Define if the compiler provides a wchar.h header file. */
 #define HAVE_WCHAR_H 1
 
 /* Define to 1 if you have the `wcscoll' function. */
 #define HAVE_WCSCOLL 1
 
@@ -1362,32 +1341,35 @@
 #define HAVE_WCSXFRM 1
 
 /* Define to 1 if you have the `wmemcmp' function. */
 #define HAVE_WMEMCMP 1
 
 /* Define if tzset() actually switches the local timezone in a meaningful way.
  */
-#define HAVE_WORKING_TZSET 1
+/* #undef HAVE_WORKING_TZSET */
 
 /* Define to 1 if you have the `writev' function. */
 #define HAVE_WRITEV 1
 
+/* Define if libssl has X509_VERIFY_PARAM_set1_host and related function */
+/* #undef HAVE_X509_VERIFY_PARAM_SET1_HOST */
+
 /* Define if the zlib library has inflateCopy */
-#define HAVE_ZLIB_COPY 1
+/* #undef HAVE_ZLIB_COPY */
 
 /* Define to 1 if you have the `_getpty' function. */
 /* #undef HAVE__GETPTY */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in <mkdev.h>.
  */
 /* #undef MAJOR_IN_MKDEV */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in
    <sysmacros.h>. */
-#define MAJOR_IN_SYSMACROS 1
+/* #undef MAJOR_IN_SYSMACROS */
 
 /* Define if mvwdelch in curses.h is an expression. */
 /* #undef MVWDELCH_IS_EXPRESSION */
 
 /* Define to the address where bug reports for this package should be sent. */
 /* #undef PACKAGE_BUGREPORT */
 
@@ -1406,18 +1388,18 @@
 /* Define to the version of this package. */
 /* #undef PACKAGE_VERSION */
 
 /* Define if POSIX semaphores aren't enabled on your system */
 /* #undef POSIX_SEMAPHORES_NOT_ENABLED */
 
 /* Define if pthread_key_t is compatible with int. */
-#define PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT 1
+/* #undef PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT */
 
 /* Defined if PTHREAD_SCOPE_SYSTEM supported. */
-#define PTHREAD_SYSTEM_SCHED_SUPPORTED 1
+/* #undef PTHREAD_SYSTEM_SCHED_SUPPORTED */
 
 /* Define as the preferred size in bits of long digits */
 /* #undef PYLONG_BITS_IN_DIGIT */
 
 /* enabled builtin hash modules */
 #define PY_BUILTIN_HASHLIB_HASHES "md5,sha1,sha256,sha512,sha3,blake2"
 
@@ -1468,15 +1450,15 @@
 /* The size of `fpos_t', as computed by sizeof. */
 #define SIZEOF_FPOS_T 16
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
-#define SIZEOF_LONG 8
+#define SIZEOF_LONG 4
 
 /* The size of `long double', as computed by sizeof. */
 #define SIZEOF_LONG_DOUBLE 16
 
 /* The size of `long long', as computed by sizeof. */
 #define SIZEOF_LONG_LONG 8
 
@@ -1486,47 +1468,44 @@
 /* The size of `pid_t', as computed by sizeof. */
 #define SIZEOF_PID_T 4
 
 /* The size of `pthread_key_t', as computed by sizeof. */
 #define SIZEOF_PTHREAD_KEY_T 4
 
 /* The size of `pthread_t', as computed by sizeof. */
-#define SIZEOF_PTHREAD_T 8
+#define SIZEOF_PTHREAD_T 4
 
 /* The size of `short', as computed by sizeof. */
 #define SIZEOF_SHORT 2
 
 /* The size of `size_t', as computed by sizeof. */
 #define SIZEOF_SIZE_T 8
 
 /* The size of `time_t', as computed by sizeof. */
 #define SIZEOF_TIME_T 8
 
 /* The size of `uintptr_t', as computed by sizeof. */
-#define SIZEOF_UINTPTR_T 8
+#define SIZEOF_UINTPTR_T 4
 
 /* The size of `void *', as computed by sizeof. */
-#define SIZEOF_VOID_P 8
+#define SIZEOF_VOID_P 4
 
 /* The size of `wchar_t', as computed by sizeof. */
 #define SIZEOF_WCHAR_T 4
 
 /* The size of `_Bool', as computed by sizeof. */
 #define SIZEOF__BOOL 1
 
 /* Define to 1 if you have the ANSI C header files. */
 #define STDC_HEADERS 1
 
 /* Define if you can safely include both <sys/select.h> and <sys/time.h>
    (which you can't on SCO ODT 3.0). */
 #define SYS_SELECT_WITH_SYS_TIME 1
 
-/* Custom thread stack size depending on chosen sanitizer runtimes. */
-/* #undef THREAD_STACK_SIZE */
-
 /* Library needed by timemodule.c: librt may be needed for clock_gettime() */
 /* #undef TIMEMODULE_LIB */
 
 /* Define to 1 if you can safely include both <sys/time.h> and <time.h>. */
 #define TIME_WITH_SYS_TIME 1
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
@@ -1570,17 +1549,14 @@
 /* #undef WITH_DTRACE */
 
 /* Define if you want to use the new-style (Openstep, Rhapsody, MacOS) dynamic
    linker (dyld) instead of the old-style (NextStep) dynamic linker (rld).
    Dyld is necessary to support frameworks. */
 /* #undef WITH_DYLD */
 
-/* Define to build the readline module against Editline. */
-/* #undef WITH_EDITLINE */
-
 /* Define to 1 if libintl is needed for locale functions. */
 /* #undef WITH_LIBINTL */
 
 /* Define if you want to produce an OpenStep/Rhapsody framework (shared
    library plus accessory files). */
 /* #undef WITH_NEXT_FRAMEWORK */
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.d` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyexpat.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacro.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymath.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pyport.h`

 * *Files 1% similar despite different names*

```diff
@@ -665,15 +665,15 @@
 
 #include "exports.h"
 
 /* only get special linkage if built as shared or platform is Cygwin */
 #if defined(Py_ENABLE_SHARED) || defined(__CYGWIN__)
 #       if defined(HAVE_DECLSPEC_DLL)
 #               if defined(Py_BUILD_CORE) && !defined(Py_BUILD_CORE_MODULE)
-#                       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#                       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #                       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
         /* module init functions inside the core need no external linkage */
         /* except for Cygwin to handle embedding */
 #                       if defined(__CYGWIN__)
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __CYGWIN__ */
 #                               define PyMODINIT_FUNC PyObject*
@@ -681,30 +681,30 @@
 #               else /* Py_BUILD_CORE */
         /* Building an extension module, or an embedded situation */
         /* public Python functions and data are imported */
         /* Under Cygwin, auto-import functions to prevent compilation */
         /* failures similar to those described at the bottom of 4.1: */
         /* http://docs.python.org/extending/windows.html#a-cookbook-approach */
 #                       if !defined(__CYGWIN__)
-#                               define PyAPI_FUNC(RTYPE) Py_IMPORTED_SYMBOL RTYPE
+#                               define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_IMPORTED_SYMBOL RTYPE
 #                       endif /* !__CYGWIN__ */
 #                       define PyAPI_DATA(RTYPE) extern Py_IMPORTED_SYMBOL RTYPE
         /* module init functions outside the core must be exported */
 #                       if defined(__cplusplus)
 #                               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __cplusplus */
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       endif /* __cplusplus */
 #               endif /* Py_BUILD_CORE */
 #       endif /* HAVE_DECLSPEC_DLL */
 #endif /* Py_ENABLE_SHARED */
 
 /* If no external linkage macros defined by now, create defaults */
 #ifndef PyAPI_FUNC
-#       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyAPI_DATA
 #       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyMODINIT_FUNC
 #       if defined(__cplusplus)
 #               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrhex.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrtod.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythread.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/rangeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/setobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/sliceobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/structmember.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/structseq.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/token.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/tracemalloc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/typeslots.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp310/weakrefobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp310/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/LICENSE` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/Python.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/boolobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/codecs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/complexobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/cellobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/classobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/complexobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/descrobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/frameobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/funcobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/genobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longintrepr.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/modsupport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/odictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/picklebufobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyctype.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pydebug.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyframe.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythread.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pytime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/setobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/weakrefobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/datetime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/descrobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/dynamic_annotations.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/errcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/exports.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_accu.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_asdl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_call.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_condvar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dict.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_frame.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_genobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gil.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hamt.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interp.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_list.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_long.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_opcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_parser.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymath.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_signal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_strhex.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_structseq.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_symtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_tuple.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/intrcheck.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/iterobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/longobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/marshal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/memoryobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/modsupport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/opcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/osdefs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/patchlevel.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/py_curses.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pybuffer.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pycapsule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyconfig.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,14 @@
    build system. */
 /* #undef AIX_BUILDDATE */
 
 /* Define for AIX if your compiler is a genuine IBM xlC/xlC_r and you want
    support for AIX C++ shared extension modules. */
 /* #undef AIX_GENUINE_CPLUSPLUS */
 
-/* The normal alignment of `long', in bytes. */
-#define ALIGNOF_LONG 8
-
-/* The normal alignment of `size_t', in bytes. */
-#define ALIGNOF_SIZE_T 8
-
 /* Alternative SOABI used in debug build to load C extensions built in release
    mode */
 /* #undef ALT_SOABI */
 
 /* The Android API level. */
 /* #undef ANDROID_API_LEVEL */
 
@@ -37,34 +31,34 @@
 /* #undef DOUBLE_IS_BIG_ENDIAN_IEEE754 */
 
 /* Define if C doubles are 64-bit IEEE 754 binary format, stored with the
    least significant byte first */
 #define DOUBLE_IS_LITTLE_ENDIAN_IEEE754 1
 
 /* Define if --enable-ipv6 is specified */
-#define ENABLE_IPV6 1
+/* #undef ENABLE_IPV6 */
 
 /* Define to 1 if your system stores words within floats with the most
    significant word first */
 /* #undef FLOAT_WORDS_BIGENDIAN */
 
+/* Define if flock needs to be linked with bsd library. */
+/* #undef FLOCK_NEEDS_LIBBSD */
+
 /* Define if getpgrp() must be called as getpgrp(0). */
 /* #undef GETPGRP_HAVE_ARG */
 
-/* Define if you have the 'accept' function. */
-#define HAVE_ACCEPT 1
-
 /* Define to 1 if you have the `accept4' function. */
 #define HAVE_ACCEPT4 1
 
 /* Define to 1 if you have the `acosh' function. */
 #define HAVE_ACOSH 1
 
 /* struct addrinfo (netdb.h) */
-#define HAVE_ADDRINFO 1
+/* #undef HAVE_ADDRINFO */
 
 /* Define to 1 if you have the `alarm' function. */
 #define HAVE_ALARM 1
 
 /* Define if aligned memory access is required */
 /* #undef HAVE_ALIGNED_REQUIRED */
 
@@ -74,22 +68,19 @@
 /* Define this if your time.h defines altzone. */
 /* #undef HAVE_ALTZONE */
 
 /* Define to 1 if you have the `asinh' function. */
 #define HAVE_ASINH 1
 
 /* Define to 1 if you have the <asm/types.h> header file. */
-#define HAVE_ASM_TYPES_H 1
+/* #undef HAVE_ASM_TYPES_H */
 
 /* Define to 1 if you have the `atanh' function. */
 #define HAVE_ATANH 1
 
-/* Define if you have the 'bind' function. */
-#define HAVE_BIND 1
-
 /* Define to 1 if you have the `bind_textdomain_codeset' function. */
 #define HAVE_BIND_TEXTDOMAIN_CODESET 1
 
 /* Define to 1 if you have the <bluetooth/bluetooth.h> header file. */
 /* #undef HAVE_BLUETOOTH_BLUETOOTH_H */
 
 /* Define to 1 if you have the <bluetooth.h> header file. */
@@ -113,29 +104,23 @@
 
 /* Define if pthread_sigmask() does not work on your system. */
 /* #undef HAVE_BROKEN_PTHREAD_SIGMASK */
 
 /* define to 1 if your sem_getvalue is broken. */
 /* #undef HAVE_BROKEN_SEM_GETVALUE */
 
-/* Define if 'unsetenv' does not return an int. */
+/* Define if `unsetenv` does not return an int. */
 /* #undef HAVE_BROKEN_UNSETENV */
 
-/* Has builtin __atomic_load_n() and __atomic_store_n() functions */
+/* Has builtin atomics */
 #define HAVE_BUILTIN_ATOMIC 1
 
-/* Define to 1 if you have the <bzlib.h> header file. */
-/* #undef HAVE_BZLIB_H */
-
 /* Define to 1 if you have the 'chflags' function. */
 /* #undef HAVE_CHFLAGS */
 
-/* Define to 1 if you have the `chmod' function. */
-#define HAVE_CHMOD 1
-
 /* Define to 1 if you have the `chown' function. */
 #define HAVE_CHOWN 1
 
 /* Define if you have the 'chroot' function. */
 #define HAVE_CHROOT 1
 
 /* Define to 1 if you have the `clock' function. */
@@ -143,34 +128,28 @@
 
 /* Define to 1 if you have the `clock_getres' function. */
 #define HAVE_CLOCK_GETRES 1
 
 /* Define to 1 if you have the `clock_gettime' function. */
 #define HAVE_CLOCK_GETTIME 1
 
-/* Define to 1 if you have the `clock_nanosleep' function. */
-#define HAVE_CLOCK_NANOSLEEP 1
-
 /* Define to 1 if you have the `clock_settime' function. */
 #define HAVE_CLOCK_SETTIME 1
 
-/* Define to 1 if you have the `close_range' function. */
-#define HAVE_CLOSE_RANGE 1
-
 /* Define if the C compiler supports computed gotos. */
 #define HAVE_COMPUTED_GOTOS 1
 
 /* Define to 1 if you have the `confstr' function. */
 #define HAVE_CONFSTR 1
 
 /* Define to 1 if you have the <conio.h> header file. */
 /* #undef HAVE_CONIO_H */
 
-/* Define if you have the 'connect' function. */
-#define HAVE_CONNECT 1
+/* Define to 1 if you have the `copysign' function. */
+#define HAVE_COPYSIGN 1
 
 /* Define to 1 if you have the `copy_file_range' function. */
 #define HAVE_COPY_FILE_RANGE 1
 
 /* Define to 1 if you have the <crypt.h> header file. */
 #define HAVE_CRYPT_H 1
 
@@ -191,15 +170,15 @@
 
 /* Define if you have the 'has_key' function. */
 /* #undef HAVE_CURSES_HAS_KEY */
 
 /* Define if you have the 'immedok' function. */
 /* #undef HAVE_CURSES_IMMEDOK */
 
-/* Define if you have the 'is_pad' function. */
+/* Define if you have the 'is_pad' function or macro. */
 /* #undef HAVE_CURSES_IS_PAD */
 
 /* Define if you have the 'is_term_resized' function. */
 /* #undef HAVE_CURSES_IS_TERM_RESIZED */
 
 /* Define if you have the 'resizeterm' function. */
 /* #undef HAVE_CURSES_RESIZETERM */
@@ -215,61 +194,70 @@
 
 /* Define if you have the 'use_env' function. */
 /* #undef HAVE_CURSES_USE_ENV */
 
 /* Define if you have the 'wchgat' function. */
 /* #undef HAVE_CURSES_WCHGAT */
 
-/* Define to 1 if you have the <db.h> header file. */
-/* #undef HAVE_DB_H */
+/* Define to 1 if you have the declaration of `isfinite', and to 0 if you
+   don't. */
+#define HAVE_DECL_ISFINITE 1
+
+/* Define to 1 if you have the declaration of `isinf', and to 0 if you don't.
+ */
+#define HAVE_DECL_ISINF 1
+
+/* Define to 1 if you have the declaration of `isnan', and to 0 if you don't.
+ */
+#define HAVE_DECL_ISNAN 1
 
 /* Define to 1 if you have the declaration of `RTLD_DEEPBIND', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_DEEPBIND 1
+/* #undef HAVE_DECL_RTLD_DEEPBIND */
 
 /* Define to 1 if you have the declaration of `RTLD_GLOBAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_GLOBAL 1
+/* #undef HAVE_DECL_RTLD_GLOBAL */
 
 /* Define to 1 if you have the declaration of `RTLD_LAZY', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LAZY 1
+/* #undef HAVE_DECL_RTLD_LAZY */
 
 /* Define to 1 if you have the declaration of `RTLD_LOCAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LOCAL 1
+/* #undef HAVE_DECL_RTLD_LOCAL */
 
 /* Define to 1 if you have the declaration of `RTLD_MEMBER', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_MEMBER 0
+/* #undef HAVE_DECL_RTLD_MEMBER */
 
 /* Define to 1 if you have the declaration of `RTLD_NODELETE', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NODELETE 1
+/* #undef HAVE_DECL_RTLD_NODELETE */
 
 /* Define to 1 if you have the declaration of `RTLD_NOLOAD', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOLOAD 1
+/* #undef HAVE_DECL_RTLD_NOLOAD */
 
 /* Define to 1 if you have the declaration of `RTLD_NOW', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOW 1
+/* #undef HAVE_DECL_RTLD_NOW */
 
 /* Define to 1 if you have the declaration of `tzname', and to 0 if you don't.
  */
 /* #undef HAVE_DECL_TZNAME */
 
 /* Define to 1 if you have the device macros. */
-#define HAVE_DEVICE_MACROS 1
+/* #undef HAVE_DEVICE_MACROS */
 
 /* Define to 1 if you have the /dev/ptc device file. */
 /* #undef HAVE_DEV_PTC */
 
 /* Define to 1 if you have the /dev/ptmx device file. */
-#define HAVE_DEV_PTMX 1
+/* #undef HAVE_DEV_PTMX */
 
 /* Define to 1 if you have the <direct.h> header file. */
 /* #undef HAVE_DIRECT_H */
 
 /* Define to 1 if the dirent structure has a d_type field */
 #define HAVE_DIRENT_D_TYPE 1
 
@@ -277,111 +265,105 @@
  */
 #define HAVE_DIRENT_H 1
 
 /* Define if you have the 'dirfd' function or macro. */
 #define HAVE_DIRFD 1
 
 /* Define to 1 if you have the <dlfcn.h> header file. */
-#define HAVE_DLFCN_H 1
+/* #undef HAVE_DLFCN_H */
 
 /* Define to 1 if you have the `dlopen' function. */
-#define HAVE_DLOPEN 1
-
-/* Define to 1 if you have the `dup' function. */
-#define HAVE_DUP 1
+/* #undef HAVE_DLOPEN */
 
 /* Define to 1 if you have the `dup2' function. */
-#define HAVE_DUP2 1
+/* #undef HAVE_DUP2 */
 
 /* Define to 1 if you have the `dup3' function. */
-#define HAVE_DUP3 1
+/* #undef HAVE_DUP3 */
 
 /* Define if you have the '_dyld_shared_cache_contains_path' function. */
 /* #undef HAVE_DYLD_SHARED_CACHE_CONTAINS_PATH */
 
 /* Defined when any dynamic module loading is enabled. */
 #define HAVE_DYNAMIC_LOADING 1
 
 /* Define to 1 if you have the <endian.h> header file. */
 #define HAVE_ENDIAN_H 1
 
-/* Define if you have the 'epoll_create' function. */
-#define HAVE_EPOLL 1
+/* Define if you have the 'epoll' functions. */
+/* #undef HAVE_EPOLL */
 
 /* Define if you have the 'epoll_create1' function. */
-#define HAVE_EPOLL_CREATE1 1
+/* #undef HAVE_EPOLL_CREATE1 */
 
 /* Define to 1 if you have the `erf' function. */
 #define HAVE_ERF 1
 
 /* Define to 1 if you have the `erfc' function. */
 #define HAVE_ERFC 1
 
 /* Define to 1 if you have the <errno.h> header file. */
 #define HAVE_ERRNO_H 1
 
-/* Define if you have the 'eventfd' function. */
-#define HAVE_EVENTFD 1
-
 /* Define to 1 if you have the `execv' function. */
-#define HAVE_EXECV 1
+/* #undef HAVE_EXECV */
 
 /* Define to 1 if you have the `explicit_bzero' function. */
 #define HAVE_EXPLICIT_BZERO 1
 
 /* Define to 1 if you have the `explicit_memset' function. */
 /* #undef HAVE_EXPLICIT_MEMSET */
 
 /* Define to 1 if you have the `expm1' function. */
 #define HAVE_EXPM1 1
 
 /* Define to 1 if you have the `faccessat' function. */
 #define HAVE_FACCESSAT 1
 
 /* Define if you have the 'fchdir' function. */
-#define HAVE_FCHDIR 1
+/* #undef HAVE_FCHDIR */
 
 /* Define to 1 if you have the `fchmod' function. */
-#define HAVE_FCHMOD 1
+/* #undef HAVE_FCHMOD */
 
 /* Define to 1 if you have the `fchmodat' function. */
-#define HAVE_FCHMODAT 1
+/* #undef HAVE_FCHMODAT */
 
 /* Define to 1 if you have the `fchown' function. */
-#define HAVE_FCHOWN 1
+/* #undef HAVE_FCHOWN */
 
 /* Define to 1 if you have the `fchownat' function. */
-#define HAVE_FCHOWNAT 1
+/* #undef HAVE_FCHOWNAT */
 
 /* Define to 1 if you have the <fcntl.h> header file. */
 #define HAVE_FCNTL_H 1
 
 /* Define if you have the 'fdatasync' function. */
 #define HAVE_FDATASYNC 1
 
 /* Define to 1 if you have the `fdopendir' function. */
 #define HAVE_FDOPENDIR 1
 
 /* Define to 1 if you have the `fdwalk' function. */
 /* #undef HAVE_FDWALK */
 
 /* Define to 1 if you have the `fexecve' function. */
-#define HAVE_FEXECVE 1
+/* #undef HAVE_FEXECVE */
+
+/* Define to 1 if you have the `finite' function. */
+#define HAVE_FINITE 1
 
 /* Define to 1 if you have the `flock' function. */
-#define HAVE_FLOCK 1
+/* #undef HAVE_FLOCK */
 
 /* Define to 1 if you have the `fork' function. */
-#define HAVE_FORK 1
-
-/* Define to 1 if you have the `fork1' function. */
-/* #undef HAVE_FORK1 */
+/* #undef HAVE_FORK */
 
 /* Define to 1 if you have the `forkpty' function. */
-#define HAVE_FORKPTY 1
+/* #undef HAVE_FORKPTY */
 
 /* Define to 1 if you have the `fpathconf' function. */
 #define HAVE_FPATHCONF 1
 
 /* Define to 1 if you have the `fseek64' function. */
 /* #undef HAVE_FSEEK64 */
 
@@ -409,465 +391,375 @@
 /* Define to 1 if you have the `ftruncate' function. */
 #define HAVE_FTRUNCATE 1
 
 /* Define to 1 if you have the `futimens' function. */
 #define HAVE_FUTIMENS 1
 
 /* Define to 1 if you have the `futimes' function. */
-#define HAVE_FUTIMES 1
+/* #undef HAVE_FUTIMES */
 
 /* Define to 1 if you have the `futimesat' function. */
-#define HAVE_FUTIMESAT 1
+/* #undef HAVE_FUTIMESAT */
 
 /* Define to 1 if you have the `gai_strerror' function. */
-#define HAVE_GAI_STRERROR 1
+/* #undef HAVE_GAI_STRERROR */
+
+/* Define to 1 if you have the `gamma' function. */
+/* #undef HAVE_GAMMA */
 
 /* Define if we can use gcc inline assembler to get and set mc68881 fpcr */
 /* #undef HAVE_GCC_ASM_FOR_MC68881 */
 
 /* Define if we can use x64 gcc inline assembler */
-#define HAVE_GCC_ASM_FOR_X64 1
+/* #undef HAVE_GCC_ASM_FOR_X64 */
 
 /* Define if we can use gcc inline assembler to get and set x87 control word
  */
-#define HAVE_GCC_ASM_FOR_X87 1
+/* #undef HAVE_GCC_ASM_FOR_X87 */
 
 /* Define if your compiler provides __uint128_t */
 #define HAVE_GCC_UINT128_T 1
 
-/* Define to 1 if you have the <gdbm-ndbm.h> header file. */
-/* #undef HAVE_GDBM_DASH_NDBM_H */
-
-/* Define to 1 if you have the <gdbm.h> header file. */
-/* #undef HAVE_GDBM_H */
-
-/* Define to 1 if you have the <gdbm/ndbm.h> header file. */
-/* #undef HAVE_GDBM_NDBM_H */
-
 /* Define if you have the getaddrinfo function. */
-#define HAVE_GETADDRINFO 1
+/* #undef HAVE_GETADDRINFO */
 
 /* Define this if you have flockfile(), getc_unlocked(), and funlockfile() */
-#define HAVE_GETC_UNLOCKED 1
-
-/* Define to 1 if you have the `getegid' function. */
-#define HAVE_GETEGID 1
+/* #undef HAVE_GETC_UNLOCKED */
 
 /* Define to 1 if you have the `getentropy' function. */
 #define HAVE_GETENTROPY 1
 
-/* Define to 1 if you have the `geteuid' function. */
-#define HAVE_GETEUID 1
-
-/* Define to 1 if you have the `getgid' function. */
-#define HAVE_GETGID 1
-
-/* Define to 1 if you have the `getgrgid' function. */
-#define HAVE_GETGRGID 1
-
 /* Define to 1 if you have the `getgrgid_r' function. */
-#define HAVE_GETGRGID_R 1
+/* #undef HAVE_GETGRGID_R */
 
 /* Define to 1 if you have the `getgrnam_r' function. */
-#define HAVE_GETGRNAM_R 1
+/* #undef HAVE_GETGRNAM_R */
 
 /* Define to 1 if you have the `getgrouplist' function. */
-#define HAVE_GETGROUPLIST 1
+/* #undef HAVE_GETGROUPLIST */
 
 /* Define to 1 if you have the `getgroups' function. */
-#define HAVE_GETGROUPS 1
-
-/* Define if you have the 'gethostbyaddr' function. */
-#define HAVE_GETHOSTBYADDR 1
+/* #undef HAVE_GETGROUPS */
 
 /* Define to 1 if you have the `gethostbyname' function. */
-#define HAVE_GETHOSTBYNAME 1
+/* #undef HAVE_GETHOSTBYNAME */
 
 /* Define this if you have some version of gethostbyname_r() */
-#define HAVE_GETHOSTBYNAME_R 1
+/* #undef HAVE_GETHOSTBYNAME_R */
 
 /* Define this if you have the 3-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_3_ARG */
 
 /* Define this if you have the 5-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_5_ARG */
 
 /* Define this if you have the 6-arg version of gethostbyname_r(). */
-#define HAVE_GETHOSTBYNAME_R_6_ARG 1
-
-/* Define to 1 if you have the `gethostname' function. */
-#define HAVE_GETHOSTNAME 1
+/* #undef HAVE_GETHOSTBYNAME_R_6_ARG */
 
 /* Define to 1 if you have the `getitimer' function. */
-#define HAVE_GETITIMER 1
+/* #undef HAVE_GETITIMER */
 
 /* Define to 1 if you have the `getloadavg' function. */
-#define HAVE_GETLOADAVG 1
+/* #undef HAVE_GETLOADAVG */
 
 /* Define to 1 if you have the `getlogin' function. */
-#define HAVE_GETLOGIN 1
+/* #undef HAVE_GETLOGIN */
 
 /* Define to 1 if you have the `getnameinfo' function. */
-#define HAVE_GETNAMEINFO 1
+/* #undef HAVE_GETNAMEINFO */
 
 /* Define if you have the 'getpagesize' function. */
-#define HAVE_GETPAGESIZE 1
+/* #undef HAVE_GETPAGESIZE */
 
-/* Define if you have the 'getpeername' function. */
-#define HAVE_GETPEERNAME 1
+/* Define to 1 if you have the `getpeername' function. */
+/* #undef HAVE_GETPEERNAME */
 
 /* Define to 1 if you have the `getpgid' function. */
-#define HAVE_GETPGID 1
+/* #undef HAVE_GETPGID */
 
 /* Define to 1 if you have the `getpgrp' function. */
-#define HAVE_GETPGRP 1
+/* #undef HAVE_GETPGRP */
 
 /* Define to 1 if you have the `getpid' function. */
-#define HAVE_GETPID 1
-
-/* Define to 1 if you have the `getppid' function. */
-#define HAVE_GETPPID 1
+/* #undef HAVE_GETPID */
 
 /* Define to 1 if you have the `getpriority' function. */
-#define HAVE_GETPRIORITY 1
-
-/* Define if you have the 'getprotobyname' function. */
-#define HAVE_GETPROTOBYNAME 1
+/* #undef HAVE_GETPRIORITY */
 
 /* Define to 1 if you have the `getpwent' function. */
-#define HAVE_GETPWENT 1
+/* #undef HAVE_GETPWENT */
 
 /* Define to 1 if you have the `getpwnam_r' function. */
-#define HAVE_GETPWNAM_R 1
-
-/* Define to 1 if you have the `getpwuid' function. */
-#define HAVE_GETPWUID 1
+/* #undef HAVE_GETPWNAM_R */
 
 /* Define to 1 if you have the `getpwuid_r' function. */
-#define HAVE_GETPWUID_R 1
+/* #undef HAVE_GETPWUID_R */
 
 /* Define to 1 if the getrandom() function is available */
-#define HAVE_GETRANDOM 1
+/* #undef HAVE_GETRANDOM */
 
 /* Define to 1 if the Linux getrandom() syscall is available */
-#define HAVE_GETRANDOM_SYSCALL 1
+/* #undef HAVE_GETRANDOM_SYSCALL */
 
 /* Define to 1 if you have the `getresgid' function. */
-#define HAVE_GETRESGID 1
+/* #undef HAVE_GETRESGID */
 
 /* Define to 1 if you have the `getresuid' function. */
-#define HAVE_GETRESUID 1
-
-/* Define to 1 if you have the `getrusage' function. */
-#define HAVE_GETRUSAGE 1
-
-/* Define if you have the 'getservbyname' function. */
-#define HAVE_GETSERVBYNAME 1
-
-/* Define if you have the 'getservbyport' function. */
-#define HAVE_GETSERVBYPORT 1
+/* #undef HAVE_GETRESUID */
 
 /* Define to 1 if you have the `getsid' function. */
-#define HAVE_GETSID 1
-
-/* Define if you have the 'getsockname' function. */
-#define HAVE_GETSOCKNAME 1
+/* #undef HAVE_GETSID */
 
 /* Define to 1 if you have the `getspent' function. */
-#define HAVE_GETSPENT 1
+/* #undef HAVE_GETSPENT */
 
 /* Define to 1 if you have the `getspnam' function. */
-#define HAVE_GETSPNAM 1
-
-/* Define to 1 if you have the `getuid' function. */
-#define HAVE_GETUID 1
+/* #undef HAVE_GETSPNAM */
 
 /* Define to 1 if you have the `getwd' function. */
-#define HAVE_GETWD 1
+/* #undef HAVE_GETWD */
 
 /* Define if glibc has incorrect _FORTIFY_SOURCE wrappers for memmove and
    bcopy. */
 /* #undef HAVE_GLIBC_MEMMOVE_BUG */
 
 /* Define to 1 if you have the <grp.h> header file. */
-#define HAVE_GRP_H 1
+/* #undef HAVE_GRP_H */
 
 /* Define if you have the 'hstrerror' function. */
-#define HAVE_HSTRERROR 1
+/* #undef HAVE_HSTRERROR */
 
 /* Define this if you have le64toh() */
 #define HAVE_HTOLE64 1
 
+/* Define to 1 if you have the `hypot' function. */
+#define HAVE_HYPOT 1
+
 /* Define to 1 if you have the <ieeefp.h> header file. */
 /* #undef HAVE_IEEEFP_H */
 
 /* Define to 1 if you have the `if_nameindex' function. */
-#define HAVE_IF_NAMEINDEX 1
+/* #undef HAVE_IF_NAMEINDEX */
 
 /* Define if you have the 'inet_aton' function. */
 #define HAVE_INET_ATON 1
 
-/* Define if you have the 'inet_ntoa' function. */
-#define HAVE_INET_NTOA 1
-
 /* Define if you have the 'inet_pton' function. */
 #define HAVE_INET_PTON 1
 
 /* Define to 1 if you have the `initgroups' function. */
-#define HAVE_INITGROUPS 1
+/* #undef HAVE_INITGROUPS */
 
 /* Define to 1 if you have the <inttypes.h> header file. */
 #define HAVE_INTTYPES_H 1
 
 /* Define to 1 if you have the <io.h> header file. */
 /* #undef HAVE_IO_H */
 
 /* Define if gcc has the ipa-pure-const bug. */
 /* #undef HAVE_IPA_PURE_CONST_BUG */
 
 /* Define to 1 if you have the `kill' function. */
-#define HAVE_KILL 1
+/* #undef HAVE_KILL */
 
 /* Define to 1 if you have the `killpg' function. */
-#define HAVE_KILLPG 1
+/* #undef HAVE_KILLPG */
 
-/* Define if you have the 'kqueue' function. */
+/* Define if you have the 'kqueue' functions. */
 /* #undef HAVE_KQUEUE */
 
 /* Define to 1 if you have the <langinfo.h> header file. */
 #define HAVE_LANGINFO_H 1
 
 /* Defined to enable large file support when an off_t is bigger than a long
    and long long is at least as big as an off_t. You may need to add some
    flags for configuration and compilation to enable this mode. (For Solaris
    and Linux, the necessary defines are already defined.) */
-/* #undef HAVE_LARGEFILE_SUPPORT */
+#define HAVE_LARGEFILE_SUPPORT 1
 
 /* Define to 1 if you have the 'lchflags' function. */
 /* #undef HAVE_LCHFLAGS */
 
 /* Define to 1 if you have the `lchmod' function. */
 /* #undef HAVE_LCHMOD */
 
 /* Define to 1 if you have the `lchown' function. */
-#define HAVE_LCHOWN 1
-
-/* Define to 1 if you want to build _blake2 module with libb2 */
-/* #undef HAVE_LIBB2 */
+/* #undef HAVE_LCHOWN */
 
-/* Define to 1 if you have the `db' library (-ldb). */
-/* #undef HAVE_LIBDB */
+/* Define to 1 if you have the `lgamma' function. */
+#define HAVE_LGAMMA 1
 
 /* Define to 1 if you have the `dl' library (-ldl). */
 #define HAVE_LIBDL 1
 
 /* Define to 1 if you have the `dld' library (-ldld). */
 /* #undef HAVE_LIBDLD */
 
-/* Define to 1 if you have the `gdbm_compat' library (-lgdbm_compat). */
-/* #undef HAVE_LIBGDBM_COMPAT */
-
 /* Define to 1 if you have the `ieee' library (-lieee). */
 /* #undef HAVE_LIBIEEE */
 
 /* Define to 1 if you have the <libintl.h> header file. */
-#define HAVE_LIBINTL_H 1
-
-/* Define to 1 if you have the `ndbm' library (-lndbm). */
-/* #undef HAVE_LIBNDBM */
+/* #undef HAVE_LIBINTL_H */
 
-/* Define to build the readline module. */
+/* Define if you have the readline library (-lreadline). */
 /* #undef HAVE_LIBREADLINE */
 
 /* Define to 1 if you have the `resolv' library (-lresolv). */
-/* #undef HAVE_LIBRESOLV */
+#define HAVE_LIBRESOLV 1
 
 /* Define to 1 if you have the `sendfile' library (-lsendfile). */
 /* #undef HAVE_LIBSENDFILE */
 
-/* Define to 1 if you have the `sqlite3' library (-lsqlite3). */
-/* #undef HAVE_LIBSQLITE3 */
-
 /* Define to 1 if you have the <libutil.h> header file. */
-/* #undef HAVE_LIBUTIL_H */
+#define HAVE_LIBUTIL_H 1
+
+/* Define to 1 if you have the `uuid' library (-luuid). */
+/* #undef HAVE_LIBUUID */
 
 /* Define if you have the 'link' function. */
 #define HAVE_LINK 1
 
 /* Define to 1 if you have the `linkat' function. */
 #define HAVE_LINKAT 1
 
 /* Define to 1 if you have the <linux/auxvec.h> header file. */
-#define HAVE_LINUX_AUXVEC_H 1
+/* #undef HAVE_LINUX_AUXVEC_H */
 
 /* Define to 1 if you have the <linux/can/bcm.h> header file. */
-#define HAVE_LINUX_CAN_BCM_H 1
+/* #undef HAVE_LINUX_CAN_BCM_H */
 
 /* Define to 1 if you have the <linux/can.h> header file. */
-#define HAVE_LINUX_CAN_H 1
+/* #undef HAVE_LINUX_CAN_H */
 
 /* Define to 1 if you have the <linux/can/j1939.h> header file. */
-#define HAVE_LINUX_CAN_J1939_H 1
+/* #undef HAVE_LINUX_CAN_J1939_H */
 
 /* Define if compiling using Linux 3.6 or later. */
-#define HAVE_LINUX_CAN_RAW_FD_FRAMES 1
+/* #undef HAVE_LINUX_CAN_RAW_FD_FRAMES */
 
 /* Define to 1 if you have the <linux/can/raw.h> header file. */
-#define HAVE_LINUX_CAN_RAW_H 1
+/* #undef HAVE_LINUX_CAN_RAW_H */
 
 /* Define if compiling using Linux 4.1 or later. */
-#define HAVE_LINUX_CAN_RAW_JOIN_FILTERS 1
+/* #undef HAVE_LINUX_CAN_RAW_JOIN_FILTERS */
 
 /* Define to 1 if you have the <linux/memfd.h> header file. */
-#define HAVE_LINUX_MEMFD_H 1
+/* #undef HAVE_LINUX_MEMFD_H */
 
 /* Define to 1 if you have the <linux/netlink.h> header file. */
-#define HAVE_LINUX_NETLINK_H 1
+/* #undef HAVE_LINUX_NETLINK_H */
 
 /* Define to 1 if you have the <linux/qrtr.h> header file. */
-#define HAVE_LINUX_QRTR_H 1
+/* #undef HAVE_LINUX_QRTR_H */
 
 /* Define to 1 if you have the <linux/random.h> header file. */
-#define HAVE_LINUX_RANDOM_H 1
-
-/* Define to 1 if you have the <linux/soundcard.h> header file. */
-#define HAVE_LINUX_SOUNDCARD_H 1
+/* #undef HAVE_LINUX_RANDOM_H */
 
 /* Define to 1 if you have the <linux/tipc.h> header file. */
-#define HAVE_LINUX_TIPC_H 1
+/* #undef HAVE_LINUX_TIPC_H */
 
 /* Define to 1 if you have the <linux/vm_sockets.h> header file. */
-#define HAVE_LINUX_VM_SOCKETS_H 1
+/* #undef HAVE_LINUX_VM_SOCKETS_H */
 
 /* Define to 1 if you have the <linux/wait.h> header file. */
-#define HAVE_LINUX_WAIT_H 1
-
-/* Define if you have the 'listen' function. */
-#define HAVE_LISTEN 1
+/* #undef HAVE_LINUX_WAIT_H */
 
 /* Define to 1 if you have the `lockf' function. */
-#define HAVE_LOCKF 1
+/* #undef HAVE_LOCKF */
 
 /* Define to 1 if you have the `log1p' function. */
 #define HAVE_LOG1P 1
 
 /* Define to 1 if you have the `log2' function. */
 #define HAVE_LOG2 1
 
-/* Define to 1 if you have the `login_tty' function. */
-#define HAVE_LOGIN_TTY 1
-
 /* Define to 1 if the system has the type `long double'. */
 #define HAVE_LONG_DOUBLE 1
 
 /* Define to 1 if you have the `lstat' function. */
 #define HAVE_LSTAT 1
 
 /* Define to 1 if you have the `lutimes' function. */
-#define HAVE_LUTIMES 1
-
-/* Define to 1 if you have the <lzma.h> header file. */
-/* #undef HAVE_LZMA_H */
+/* #undef HAVE_LUTIMES */
 
 /* Define to 1 if you have the `madvise' function. */
-#define HAVE_MADVISE 1
+/* #undef HAVE_MADVISE */
 
 /* Define this if you have the makedev macro. */
-#define HAVE_MAKEDEV 1
+/* #undef HAVE_MAKEDEV */
 
 /* Define to 1 if you have the `mbrtowc' function. */
 #define HAVE_MBRTOWC 1
 
 /* Define if you have the 'memfd_create' function. */
-#define HAVE_MEMFD_CREATE 1
+/* #undef HAVE_MEMFD_CREATE */
 
 /* Define to 1 if you have the <memory.h> header file. */
 #define HAVE_MEMORY_H 1
 
 /* Define to 1 if you have the `memrchr' function. */
 #define HAVE_MEMRCHR 1
 
 /* Define to 1 if you have the `mkdirat' function. */
 #define HAVE_MKDIRAT 1
 
 /* Define to 1 if you have the `mkfifo' function. */
-#define HAVE_MKFIFO 1
+/* #undef HAVE_MKFIFO */
 
 /* Define to 1 if you have the `mkfifoat' function. */
-#define HAVE_MKFIFOAT 1
+/* #undef HAVE_MKFIFOAT */
 
 /* Define to 1 if you have the `mknod' function. */
-#define HAVE_MKNOD 1
+/* #undef HAVE_MKNOD */
 
 /* Define to 1 if you have the `mknodat' function. */
-#define HAVE_MKNODAT 1
+/* #undef HAVE_MKNODAT */
 
 /* Define to 1 if you have the `mktime' function. */
 #define HAVE_MKTIME 1
 
 /* Define to 1 if you have the `mmap' function. */
 #define HAVE_MMAP 1
 
 /* Define to 1 if you have the `mremap' function. */
 #define HAVE_MREMAP 1
 
-/* Define to 1 if you have the `nanosleep' function. */
-#define HAVE_NANOSLEEP 1
-
 /* Define to 1 if you have the <ncurses.h> header file. */
 /* #undef HAVE_NCURSES_H */
 
-/* Define to 1 if you have the <ndbm.h> header file. */
-/* #undef HAVE_NDBM_H */
-
 /* Define to 1 if you have the <ndir.h> header file, and it defines `DIR'. */
 /* #undef HAVE_NDIR_H */
 
-/* Define to 1 if you have the <netcan/can.h> header file. */
-/* #undef HAVE_NETCAN_CAN_H */
-
-/* Define to 1 if you have the <netdb.h> header file. */
-#define HAVE_NETDB_H 1
-
-/* Define to 1 if you have the <netinet/in.h> header file. */
-#define HAVE_NETINET_IN_H 1
-
 /* Define to 1 if you have the <netpacket/packet.h> header file. */
 #define HAVE_NETPACKET_PACKET_H 1
 
 /* Define to 1 if you have the <net/if.h> header file. */
-#define HAVE_NET_IF_H 1
+/* #undef HAVE_NET_IF_H */
 
 /* Define to 1 if you have the `nice' function. */
-#define HAVE_NICE 1
+/* #undef HAVE_NICE */
 
 /* Define if the internal form of wchar_t in non-Unicode locales is not
    Unicode. */
 /* #undef HAVE_NON_UNICODE_WCHAR_T_REPRESENTATION */
 
 /* Define to 1 if you have the `openat' function. */
 #define HAVE_OPENAT 1
 
-/* Define to 1 if you have the `opendir' function. */
-#define HAVE_OPENDIR 1
-
 /* Define to 1 if you have the `openpty' function. */
-#define HAVE_OPENPTY 1
+/* #undef HAVE_OPENPTY */
 
 /* Define to 1 if you have the `pathconf' function. */
 #define HAVE_PATHCONF 1
 
 /* Define to 1 if you have the `pause' function. */
-#define HAVE_PAUSE 1
-
-/* Define to 1 if you have the `pipe' function. */
-#define HAVE_PIPE 1
+/* #undef HAVE_PAUSE */
 
 /* Define to 1 if you have the `pipe2' function. */
-#define HAVE_PIPE2 1
+/* #undef HAVE_PIPE2 */
 
 /* Define to 1 if you have the `plock' function. */
 /* #undef HAVE_PLOCK */
 
 /* Define to 1 if you have the `poll' function. */
 #define HAVE_POLL 1
 
@@ -877,30 +769,30 @@
 /* Define to 1 if you have the `posix_fadvise' function. */
 #define HAVE_POSIX_FADVISE 1
 
 /* Define to 1 if you have the `posix_fallocate' function. */
 #define HAVE_POSIX_FALLOCATE 1
 
 /* Define to 1 if you have the `posix_spawn' function. */
-#define HAVE_POSIX_SPAWN 1
+/* #undef HAVE_POSIX_SPAWN */
 
 /* Define to 1 if you have the `posix_spawnp' function. */
-#define HAVE_POSIX_SPAWNP 1
+/* #undef HAVE_POSIX_SPAWNP */
 
 /* Define to 1 if you have the `pread' function. */
 #define HAVE_PREAD 1
 
 /* Define to 1 if you have the `preadv' function. */
 #define HAVE_PREADV 1
 
 /* Define to 1 if you have the `preadv2' function. */
-#define HAVE_PREADV2 1
+/* #undef HAVE_PREADV2 */
 
-/* Define if you have the 'prlimit' function. */
-#define HAVE_PRLIMIT 1
+/* Define if you have the 'prlimit' functions. */
+/* #undef HAVE_PRLIMIT */
 
 /* Define to 1 if you have the <process.h> header file. */
 /* #undef HAVE_PROCESS_H */
 
 /* Define if your compiler supports function prototype */
 #define HAVE_PROTOTYPES 1
 
@@ -916,48 +808,42 @@
 /* Define to 1 if you have the <pthread.h> header file. */
 #define HAVE_PTHREAD_H 1
 
 /* Define to 1 if you have the `pthread_init' function. */
 /* #undef HAVE_PTHREAD_INIT */
 
 /* Define to 1 if you have the `pthread_kill' function. */
-#define HAVE_PTHREAD_KILL 1
+/* #undef HAVE_PTHREAD_KILL */
 
 /* Define to 1 if you have the `pthread_sigmask' function. */
-#define HAVE_PTHREAD_SIGMASK 1
-
-/* Define if platform requires stubbed pthreads support */
-/* #undef HAVE_PTHREAD_STUBS */
+/* #undef HAVE_PTHREAD_SIGMASK */
 
 /* Define to 1 if you have the <pty.h> header file. */
-#define HAVE_PTY_H 1
+/* #undef HAVE_PTY_H */
 
 /* Define to 1 if you have the `pwrite' function. */
 #define HAVE_PWRITE 1
 
 /* Define to 1 if you have the `pwritev' function. */
 #define HAVE_PWRITEV 1
 
 /* Define to 1 if you have the `pwritev2' function. */
-#define HAVE_PWRITEV2 1
+/* #undef HAVE_PWRITEV2 */
 
 /* Define to 1 if you have the `readlink' function. */
 #define HAVE_READLINK 1
 
 /* Define to 1 if you have the `readlinkat' function. */
 #define HAVE_READLINKAT 1
 
 /* Define to 1 if you have the `readv' function. */
 #define HAVE_READV 1
 
 /* Define to 1 if you have the `realpath' function. */
-#define HAVE_REALPATH 1
-
-/* Define if you have the 'recvfrom' function. */
-#define HAVE_RECVFROM 1
+/* #undef HAVE_REALPATH */
 
 /* Define to 1 if you have the `renameat' function. */
 #define HAVE_RENAMEAT 1
 
 /* Define if readline supports append_history */
 /* #undef HAVE_RL_APPEND_HISTORY */
 
@@ -978,190 +864,172 @@
 
 /* Define if you have readline 4.0 */
 /* #undef HAVE_RL_PRE_INPUT_HOOK */
 
 /* Define if you have readline 4.0 */
 /* #undef HAVE_RL_RESIZE_TERMINAL */
 
-/* Define to 1 if you have the <rpc/rpc.h> header file. */
-/* #undef HAVE_RPC_RPC_H */
+/* Define to 1 if you have the `round' function. */
+#define HAVE_ROUND 1
 
 /* Define to 1 if you have the `rtpSpawn' function. */
 /* #undef HAVE_RTPSPAWN */
 
 /* Define to 1 if you have the `sched_get_priority_max' function. */
-#define HAVE_SCHED_GET_PRIORITY_MAX 1
+/* #undef HAVE_SCHED_GET_PRIORITY_MAX */
 
 /* Define to 1 if you have the <sched.h> header file. */
 #define HAVE_SCHED_H 1
 
 /* Define to 1 if you have the `sched_rr_get_interval' function. */
-#define HAVE_SCHED_RR_GET_INTERVAL 1
+/* #undef HAVE_SCHED_RR_GET_INTERVAL */
 
 /* Define to 1 if you have the `sched_setaffinity' function. */
-#define HAVE_SCHED_SETAFFINITY 1
+/* #undef HAVE_SCHED_SETAFFINITY */
 
 /* Define to 1 if you have the `sched_setparam' function. */
-#define HAVE_SCHED_SETPARAM 1
+/* #undef HAVE_SCHED_SETPARAM */
 
 /* Define to 1 if you have the `sched_setscheduler' function. */
-#define HAVE_SCHED_SETSCHEDULER 1
+/* #undef HAVE_SCHED_SETSCHEDULER */
 
 /* Define to 1 if you have the `sem_clockwait' function. */
-#define HAVE_SEM_CLOCKWAIT 1
+/* #undef HAVE_SEM_CLOCKWAIT */
 
 /* Define to 1 if you have the `sem_getvalue' function. */
-#define HAVE_SEM_GETVALUE 1
+/* #undef HAVE_SEM_GETVALUE */
 
 /* Define to 1 if you have the `sem_open' function. */
-#define HAVE_SEM_OPEN 1
+/* #undef HAVE_SEM_OPEN */
 
 /* Define to 1 if you have the `sem_timedwait' function. */
-#define HAVE_SEM_TIMEDWAIT 1
+/* #undef HAVE_SEM_TIMEDWAIT */
 
 /* Define to 1 if you have the `sem_unlink' function. */
-#define HAVE_SEM_UNLINK 1
+/* #undef HAVE_SEM_UNLINK */
 
 /* Define to 1 if you have the `sendfile' function. */
-#define HAVE_SENDFILE 1
-
-/* Define if you have the 'sendto' function. */
-#define HAVE_SENDTO 1
+/* #undef HAVE_SENDFILE */
 
 /* Define to 1 if you have the `setegid' function. */
-#define HAVE_SETEGID 1
+/* #undef HAVE_SETEGID */
 
 /* Define to 1 if you have the `seteuid' function. */
-#define HAVE_SETEUID 1
+/* #undef HAVE_SETEUID */
 
 /* Define to 1 if you have the `setgid' function. */
-#define HAVE_SETGID 1
+/* #undef HAVE_SETGID */
 
 /* Define if you have the 'setgroups' function. */
-#define HAVE_SETGROUPS 1
+/* #undef HAVE_SETGROUPS */
 
 /* Define to 1 if you have the `sethostname' function. */
-#define HAVE_SETHOSTNAME 1
+/* #undef HAVE_SETHOSTNAME */
 
 /* Define to 1 if you have the `setitimer' function. */
-#define HAVE_SETITIMER 1
-
-/* Define to 1 if you have the <setjmp.h> header file. */
-#define HAVE_SETJMP_H 1
+/* #undef HAVE_SETITIMER */
 
 /* Define to 1 if you have the `setlocale' function. */
 #define HAVE_SETLOCALE 1
 
 /* Define to 1 if you have the `setpgid' function. */
-#define HAVE_SETPGID 1
+/* #undef HAVE_SETPGID */
 
 /* Define to 1 if you have the `setpgrp' function. */
-#define HAVE_SETPGRP 1
+/* #undef HAVE_SETPGRP */
 
 /* Define to 1 if you have the `setpriority' function. */
-#define HAVE_SETPRIORITY 1
+/* #undef HAVE_SETPRIORITY */
 
 /* Define to 1 if you have the `setregid' function. */
-#define HAVE_SETREGID 1
+/* #undef HAVE_SETREGID */
 
 /* Define to 1 if you have the `setresgid' function. */
-#define HAVE_SETRESGID 1
+/* #undef HAVE_SETRESGID */
 
 /* Define to 1 if you have the `setresuid' function. */
-#define HAVE_SETRESUID 1
+/* #undef HAVE_SETRESUID */
 
 /* Define to 1 if you have the `setreuid' function. */
-#define HAVE_SETREUID 1
+/* #undef HAVE_SETREUID */
 
 /* Define to 1 if you have the `setsid' function. */
-#define HAVE_SETSID 1
-
-/* Define if you have the 'setsockopt' function. */
-#define HAVE_SETSOCKOPT 1
+/* #undef HAVE_SETSID */
 
 /* Define to 1 if you have the `setuid' function. */
-#define HAVE_SETUID 1
+/* #undef HAVE_SETUID */
 
 /* Define to 1 if you have the `setvbuf' function. */
 #define HAVE_SETVBUF 1
 
 /* Define to 1 if you have the <shadow.h> header file. */
-#define HAVE_SHADOW_H 1
+/* #undef HAVE_SHADOW_H */
 
 /* Define to 1 if you have the `shm_open' function. */
-#define HAVE_SHM_OPEN 1
+/* #undef HAVE_SHM_OPEN */
 
 /* Define to 1 if you have the `shm_unlink' function. */
-#define HAVE_SHM_UNLINK 1
-
-/* Define to 1 if you have the `shutdown' function. */
-#define HAVE_SHUTDOWN 1
+/* #undef HAVE_SHM_UNLINK */
 
 /* Define to 1 if you have the `sigaction' function. */
-#define HAVE_SIGACTION 1
+/* #undef HAVE_SIGACTION */
 
 /* Define to 1 if you have the `sigaltstack' function. */
-#define HAVE_SIGALTSTACK 1
+/* #undef HAVE_SIGALTSTACK */
 
 /* Define to 1 if you have the `sigfillset' function. */
-#define HAVE_SIGFILLSET 1
+/* #undef HAVE_SIGFILLSET */
 
 /* Define to 1 if `si_band' is a member of `siginfo_t'. */
-#define HAVE_SIGINFO_T_SI_BAND 1
+/* #undef HAVE_SIGINFO_T_SI_BAND */
 
 /* Define to 1 if you have the `siginterrupt' function. */
-#define HAVE_SIGINTERRUPT 1
+/* #undef HAVE_SIGINTERRUPT */
 
 /* Define to 1 if you have the <signal.h> header file. */
-#define HAVE_SIGNAL_H 1
+/* #undef HAVE_SIGNAL_H */
 
 /* Define to 1 if you have the `sigpending' function. */
-#define HAVE_SIGPENDING 1
+/* #undef HAVE_SIGPENDING */
 
 /* Define to 1 if you have the `sigrelse' function. */
-#define HAVE_SIGRELSE 1
+/* #undef HAVE_SIGRELSE */
 
 /* Define to 1 if you have the `sigtimedwait' function. */
-#define HAVE_SIGTIMEDWAIT 1
+/* #undef HAVE_SIGTIMEDWAIT */
 
 /* Define to 1 if you have the `sigwait' function. */
-#define HAVE_SIGWAIT 1
+/* #undef HAVE_SIGWAIT */
 
 /* Define to 1 if you have the `sigwaitinfo' function. */
-#define HAVE_SIGWAITINFO 1
+/* #undef HAVE_SIGWAITINFO */
 
 /* Define to 1 if you have the `snprintf' function. */
 #define HAVE_SNPRINTF 1
 
 /* struct sockaddr_alg (linux/if_alg.h) */
-#define HAVE_SOCKADDR_ALG 1
+/* #undef HAVE_SOCKADDR_ALG */
 
 /* Define if sockaddr has sa_len member */
 /* #undef HAVE_SOCKADDR_SA_LEN */
 
 /* struct sockaddr_storage (sys/socket.h) */
 #define HAVE_SOCKADDR_STORAGE 1
 
-/* Define if you have the 'socket' function. */
-#define HAVE_SOCKET 1
-
 /* Define if you have the 'socketpair' function. */
-#define HAVE_SOCKETPAIR 1
+/* #undef HAVE_SOCKETPAIR */
 
 /* Define to 1 if you have the <spawn.h> header file. */
-#define HAVE_SPAWN_H 1
-
-/* Define to 1 if you have the `splice' function. */
-#define HAVE_SPLICE 1
+/* #undef HAVE_SPAWN_H */
 
 /* Define if your compiler provides ssize_t */
 #define HAVE_SSIZE_T 1
 
 /* Define to 1 if you have the `statvfs' function. */
-#define HAVE_STATVFS 1
+/* #undef HAVE_STATVFS */
 
 /* Define if you have struct stat.st_mtim.tv_nsec */
 #define HAVE_STAT_TV_NSEC 1
 
 /* Define if you have struct stat.st_mtimensec */
 /* #undef HAVE_STAT_TV_NSEC2 */
 
@@ -1174,37 +1042,40 @@
 
 /* Define to 1 if you have the <stdlib.h> header file. */
 #define HAVE_STDLIB_H 1
 
 /* Has stdatomic.h with atomic_int and atomic_uintptr_t */
 #define HAVE_STD_ATOMIC 1
 
+/* Define to 1 if you have the `strdup' function. */
+#define HAVE_STRDUP 1
+
 /* Define to 1 if you have the `strftime' function. */
 #define HAVE_STRFTIME 1
 
 /* Define to 1 if you have the <strings.h> header file. */
 #define HAVE_STRINGS_H 1
 
 /* Define to 1 if you have the <string.h> header file. */
 #define HAVE_STRING_H 1
 
 /* Define to 1 if you have the `strlcpy' function. */
-/* #undef HAVE_STRLCPY */
+#define HAVE_STRLCPY 1
 
 /* Define to 1 if you have the <stropts.h> header file. */
-/* #undef HAVE_STROPTS_H */
+#define HAVE_STROPTS_H 1
 
 /* Define to 1 if you have the `strsignal' function. */
-#define HAVE_STRSIGNAL 1
+/* #undef HAVE_STRSIGNAL */
 
 /* Define to 1 if `pw_gecos' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_GECOS 1
+/* #undef HAVE_STRUCT_PASSWD_PW_GECOS */
 
 /* Define to 1 if `pw_passwd' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_PASSWD 1
+/* #undef HAVE_STRUCT_PASSWD_PW_PASSWD */
 
 /* Define to 1 if `st_birthtime' is a member of `struct stat'. */
 /* #undef HAVE_STRUCT_STAT_ST_BIRTHTIME */
 
 /* Define to 1 if `st_blksize' is a member of `struct stat'. */
 #define HAVE_STRUCT_STAT_ST_BLKSIZE 1
 
@@ -1226,33 +1097,27 @@
 /* Define if you have the 'symlink' function. */
 #define HAVE_SYMLINK 1
 
 /* Define to 1 if you have the `symlinkat' function. */
 #define HAVE_SYMLINKAT 1
 
 /* Define to 1 if you have the `sync' function. */
-#define HAVE_SYNC 1
+/* #undef HAVE_SYNC */
 
 /* Define to 1 if you have the `sysconf' function. */
 #define HAVE_SYSCONF 1
 
 /* Define to 1 if you have the <sysexits.h> header file. */
 #define HAVE_SYSEXITS_H 1
 
-/* Define to 1 if you have the <syslog.h> header file. */
-#define HAVE_SYSLOG_H 1
-
-/* Define to 1 if you have the `system' function. */
-#define HAVE_SYSTEM 1
-
 /* Define to 1 if you have the <sys/audioio.h> header file. */
 /* #undef HAVE_SYS_AUDIOIO_H */
 
 /* Define to 1 if you have the <sys/auxv.h> header file. */
-#define HAVE_SYS_AUXV_H 1
+/* #undef HAVE_SYS_AUXV_H */
 
 /* Define to 1 if you have the <sys/bsdtty.h> header file. */
 /* #undef HAVE_SYS_BSDTTY_H */
 
 /* Define to 1 if you have the <sys/devpoll.h> header file. */
 /* #undef HAVE_SYS_DEVPOLL_H */
 
@@ -1260,18 +1125,15 @@
  */
 /* #undef HAVE_SYS_DIR_H */
 
 /* Define to 1 if you have the <sys/endian.h> header file. */
 /* #undef HAVE_SYS_ENDIAN_H */
 
 /* Define to 1 if you have the <sys/epoll.h> header file. */
-#define HAVE_SYS_EPOLL_H 1
-
-/* Define to 1 if you have the <sys/eventfd.h> header file. */
-#define HAVE_SYS_EVENTFD_H 1
+/* #undef HAVE_SYS_EPOLL_H */
 
 /* Define to 1 if you have the <sys/event.h> header file. */
 /* #undef HAVE_SYS_EVENT_H */
 
 /* Define to 1 if you have the <sys/file.h> header file. */
 #define HAVE_SYS_FILE_H 1
 
@@ -1315,33 +1177,30 @@
 /* Define to 1 if you have the <sys/resource.h> header file. */
 #define HAVE_SYS_RESOURCE_H 1
 
 /* Define to 1 if you have the <sys/select.h> header file. */
 #define HAVE_SYS_SELECT_H 1
 
 /* Define to 1 if you have the <sys/sendfile.h> header file. */
-#define HAVE_SYS_SENDFILE_H 1
+/* #undef HAVE_SYS_SENDFILE_H */
 
 /* Define to 1 if you have the <sys/socket.h> header file. */
 #define HAVE_SYS_SOCKET_H 1
 
-/* Define to 1 if you have the <sys/soundcard.h> header file. */
-#define HAVE_SYS_SOUNDCARD_H 1
-
 /* Define to 1 if you have the <sys/statvfs.h> header file. */
-#define HAVE_SYS_STATVFS_H 1
+/* #undef HAVE_SYS_STATVFS_H */
 
 /* Define to 1 if you have the <sys/stat.h> header file. */
 #define HAVE_SYS_STAT_H 1
 
 /* Define to 1 if you have the <sys/syscall.h> header file. */
 #define HAVE_SYS_SYSCALL_H 1
 
 /* Define to 1 if you have the <sys/sysmacros.h> header file. */
-#define HAVE_SYS_SYSMACROS_H 1
+/* #undef HAVE_SYS_SYSMACROS_H */
 
 /* Define to 1 if you have the <sys/sys_domain.h> header file. */
 /* #undef HAVE_SYS_SYS_DOMAIN_H */
 
 /* Define to 1 if you have the <sys/termio.h> header file. */
 /* #undef HAVE_SYS_TERMIO_H */
 
@@ -1360,65 +1219,65 @@
 /* Define to 1 if you have the <sys/un.h> header file. */
 #define HAVE_SYS_UN_H 1
 
 /* Define to 1 if you have the <sys/utsname.h> header file. */
 #define HAVE_SYS_UTSNAME_H 1
 
 /* Define to 1 if you have the <sys/wait.h> header file. */
-#define HAVE_SYS_WAIT_H 1
+/* #undef HAVE_SYS_WAIT_H */
 
 /* Define to 1 if you have the <sys/xattr.h> header file. */
-#define HAVE_SYS_XATTR_H 1
+/* #undef HAVE_SYS_XATTR_H */
 
 /* Define to 1 if you have the `tcgetpgrp' function. */
-#define HAVE_TCGETPGRP 1
+/* #undef HAVE_TCGETPGRP */
 
 /* Define to 1 if you have the `tcsetpgrp' function. */
-#define HAVE_TCSETPGRP 1
+/* #undef HAVE_TCSETPGRP */
 
 /* Define to 1 if you have the `tempnam' function. */
-#define HAVE_TEMPNAM 1
+/* #undef HAVE_TEMPNAM */
 
 /* Define to 1 if you have the <termios.h> header file. */
-#define HAVE_TERMIOS_H 1
+/* #undef HAVE_TERMIOS_H */
 
 /* Define to 1 if you have the <term.h> header file. */
 /* #undef HAVE_TERM_H */
 
+/* Define to 1 if you have the `tgamma' function. */
+#define HAVE_TGAMMA 1
+
 /* Define to 1 if you have the `timegm' function. */
 #define HAVE_TIMEGM 1
 
 /* Define to 1 if you have the `times' function. */
 #define HAVE_TIMES 1
 
 /* Define to 1 if you have the `tmpfile' function. */
-#define HAVE_TMPFILE 1
+/* #undef HAVE_TMPFILE */
 
 /* Define to 1 if you have the `tmpnam' function. */
-#define HAVE_TMPNAM 1
+/* #undef HAVE_TMPNAM */
 
 /* Define to 1 if you have the `tmpnam_r' function. */
-#define HAVE_TMPNAM_R 1
+/* #undef HAVE_TMPNAM_R */
 
 /* Define to 1 if your `struct tm' has `tm_zone'. Deprecated, use
    `HAVE_STRUCT_TM_TM_ZONE' instead. */
 #define HAVE_TM_ZONE 1
 
 /* Define to 1 if you have the `truncate' function. */
 #define HAVE_TRUNCATE 1
 
-/* Define to 1 if you have the `ttyname' function. */
-#define HAVE_TTYNAME 1
-
 /* Define to 1 if you don't have `tm_zone' but do have the external array
    `tzname'. */
 /* #undef HAVE_TZNAME */
 
-/* Define to 1 if you have the `umask' function. */
-#define HAVE_UMASK 1
+/* Define this if you have tcl and TCL_UTF_MAX==6 */
+/* #undef HAVE_UCS4_TCL */
 
 /* Define to 1 if you have the `uname' function. */
 #define HAVE_UNAME 1
 
 /* Define to 1 if you have the <unistd.h> header file. */
 #define HAVE_UNISTD_H 1
 
@@ -1433,54 +1292,45 @@
 /* Define to 1 if you have the <util.h> header file. */
 /* #undef HAVE_UTIL_H */
 
 /* Define to 1 if you have the `utimensat' function. */
 #define HAVE_UTIMENSAT 1
 
 /* Define to 1 if you have the `utimes' function. */
-#define HAVE_UTIMES 1
+/* #undef HAVE_UTIMES */
 
 /* Define to 1 if you have the <utime.h> header file. */
 #define HAVE_UTIME_H 1
 
-/* Define to 1 if you have the <utmp.h> header file. */
-#define HAVE_UTMP_H 1
-
-/* Define to 1 if you have the `uuid_create' function. */
+/* Define if uuid_create() exists. */
 /* #undef HAVE_UUID_CREATE */
 
-/* Define to 1 if you have the `uuid_enc_be' function. */
+/* Define if uuid_enc_be() exists. */
 /* #undef HAVE_UUID_ENC_BE */
 
 /* Define if uuid_generate_time_safe() exists. */
 /* #undef HAVE_UUID_GENERATE_TIME_SAFE */
 
 /* Define to 1 if you have the <uuid.h> header file. */
 /* #undef HAVE_UUID_H */
 
 /* Define to 1 if you have the <uuid/uuid.h> header file. */
 /* #undef HAVE_UUID_UUID_H */
 
-/* Define to 1 if you have the `vfork' function. */
-#define HAVE_VFORK 1
-
-/* Define to 1 if you have the `wait' function. */
-#define HAVE_WAIT 1
-
 /* Define to 1 if you have the `wait3' function. */
-#define HAVE_WAIT3 1
+/* #undef HAVE_WAIT3 */
 
 /* Define to 1 if you have the `wait4' function. */
-#define HAVE_WAIT4 1
+/* #undef HAVE_WAIT4 */
 
 /* Define to 1 if you have the `waitid' function. */
-#define HAVE_WAITID 1
+/* #undef HAVE_WAITID */
 
 /* Define to 1 if you have the `waitpid' function. */
-#define HAVE_WAITPID 1
+/* #undef HAVE_WAITPID */
 
 /* Define if the compiler provides a wchar.h header file. */
 #define HAVE_WCHAR_H 1
 
 /* Define to 1 if you have the `wcscoll' function. */
 #define HAVE_WCSCOLL 1
 
@@ -1491,35 +1341,35 @@
 #define HAVE_WCSXFRM 1
 
 /* Define to 1 if you have the `wmemcmp' function. */
 #define HAVE_WMEMCMP 1
 
 /* Define if tzset() actually switches the local timezone in a meaningful way.
  */
-#define HAVE_WORKING_TZSET 1
+/* #undef HAVE_WORKING_TZSET */
 
 /* Define to 1 if you have the `writev' function. */
 #define HAVE_WRITEV 1
 
-/* Define if the zlib library has inflateCopy */
-#define HAVE_ZLIB_COPY 1
+/* Define if libssl has X509_VERIFY_PARAM_set1_host and related function */
+/* #undef HAVE_X509_VERIFY_PARAM_SET1_HOST */
 
-/* Define to 1 if you have the <zlib.h> header file. */
-#define HAVE_ZLIB_H 1
+/* Define if the zlib library has inflateCopy */
+/* #undef HAVE_ZLIB_COPY */
 
 /* Define to 1 if you have the `_getpty' function. */
 /* #undef HAVE__GETPTY */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in <mkdev.h>.
  */
 /* #undef MAJOR_IN_MKDEV */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in
    <sysmacros.h>. */
-#define MAJOR_IN_SYSMACROS 1
+/* #undef MAJOR_IN_SYSMACROS */
 
 /* Define if mvwdelch in curses.h is an expression. */
 /* #undef MVWDELCH_IS_EXPRESSION */
 
 /* Define to the address where bug reports for this package should be sent. */
 /* #undef PACKAGE_BUGREPORT */
 
@@ -1538,69 +1388,60 @@
 /* Define to the version of this package. */
 /* #undef PACKAGE_VERSION */
 
 /* Define if POSIX semaphores aren't enabled on your system */
 /* #undef POSIX_SEMAPHORES_NOT_ENABLED */
 
 /* Define if pthread_key_t is compatible with int. */
-#define PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT 1
+/* #undef PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT */
 
 /* Defined if PTHREAD_SCOPE_SYSTEM supported. */
-#define PTHREAD_SYSTEM_SCHED_SUPPORTED 1
+/* #undef PTHREAD_SYSTEM_SCHED_SUPPORTED */
 
 /* Define as the preferred size in bits of long digits */
 /* #undef PYLONG_BITS_IN_DIGIT */
 
 /* enabled builtin hash modules */
 #define PY_BUILTIN_HASHLIB_HASHES "md5,sha1,sha256,sha512,sha3,blake2"
 
 /* Define if you want to coerce the C locale to a UTF-8 based locale */
 #define PY_COERCE_C_LOCALE 1
 
 /* Define to printf format modifier for Py_ssize_t */
 #define PY_FORMAT_SIZE_T "z"
 
-/* Define to 1 to build the sqlite module with loadable extensions support. */
-/* #undef PY_SQLITE_ENABLE_LOAD_EXTENSION */
-
-/* Define if SQLite was compiled with the serialize API */
-/* #undef PY_SQLITE_HAVE_SERIALIZE */
-
 /* Default cipher suites list for ssl module. 1: Python's preferred selection,
    2: leave OpenSSL defaults untouched, 0: custom string */
 #define PY_SSL_DEFAULT_CIPHERS 1
 
 /* Cipher suite string for PY_SSL_DEFAULT_CIPHERS=0 */
 /* #undef PY_SSL_DEFAULT_CIPHER_STRING */
 
-/* PEP 11 Support tier (1, 2, 3 or 0 for unsupported) */
-#define PY_SUPPORT_TIER 1
-
 /* Define if you want to build an interpreter with many run-time checks. */
 /* #undef Py_DEBUG */
 
 /* Defined if Python is built as a shared library. */
 /* #undef Py_ENABLE_SHARED */
 
 /* Define hash algorithm for str, bytes and memoryview. SipHash24: 1, FNV: 2,
-   SipHash13: 3, externally defined: 0 */
+   externally defined: 0 */
 /* #undef Py_HASH_ALGORITHM */
 
-/* Define if you want to enable internal statistics gathering. */
-/* #undef Py_STATS */
-
 /* Define if you want to enable tracing references for debugging purpose */
 /* #undef Py_TRACE_REFS */
 
 /* assume C89 semantics that RETSIGTYPE is always void */
 #define RETSIGTYPE void
 
 /* Define if setpgrp() must be called as setpgrp(0, 0). */
 /* #undef SETPGRP_HAVE_ARG */
 
+/* Define to 1 if you must link with -lrt for shm_open(). */
+/* #undef SHM_NEEDS_LIBRT */
+
 /* Define if i>>j for signed int i does not extend the sign bit when i < 0 */
 /* #undef SIGNED_RIGHT_SHIFT_ZERO_FILLS */
 
 /* The size of `double', as computed by sizeof. */
 #define SIZEOF_DOUBLE 8
 
 /* The size of `float', as computed by sizeof. */
@@ -1627,27 +1468,27 @@
 /* The size of `pid_t', as computed by sizeof. */
 #define SIZEOF_PID_T 4
 
 /* The size of `pthread_key_t', as computed by sizeof. */
 #define SIZEOF_PTHREAD_KEY_T 4
 
 /* The size of `pthread_t', as computed by sizeof. */
-#define SIZEOF_PTHREAD_T 8
+#define SIZEOF_PTHREAD_T 4
 
 /* The size of `short', as computed by sizeof. */
 #define SIZEOF_SHORT 2
 
 /* The size of `size_t', as computed by sizeof. */
 #define SIZEOF_SIZE_T 8
 
 /* The size of `time_t', as computed by sizeof. */
 #define SIZEOF_TIME_T 8
 
 /* The size of `uintptr_t', as computed by sizeof. */
-#define SIZEOF_UINTPTR_T 8
+#define SIZEOF_UINTPTR_T 4
 
 /* The size of `void *', as computed by sizeof. */
 #define SIZEOF_VOID_P 4
 
 /* The size of `wchar_t', as computed by sizeof. */
 #define SIZEOF_WCHAR_T 4
 
@@ -1657,17 +1498,14 @@
 /* Define to 1 if you have the ANSI C header files. */
 #define STDC_HEADERS 1
 
 /* Define if you can safely include both <sys/select.h> and <sys/time.h>
    (which you can't on SCO ODT 3.0). */
 #define SYS_SELECT_WITH_SYS_TIME 1
 
-/* Custom thread stack size depending on chosen sanitizer runtimes. */
-/* #undef THREAD_STACK_SIZE */
-
 /* Library needed by timemodule.c: librt may be needed for clock_gettime() */
 /* #undef TIMEMODULE_LIB */
 
 /* Define to 1 if you can safely include both <sys/time.h> and <time.h>. */
 #define TIME_WITH_SYS_TIME 1
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
@@ -1711,20 +1549,14 @@
 /* #undef WITH_DTRACE */
 
 /* Define if you want to use the new-style (Openstep, Rhapsody, MacOS) dynamic
    linker (dyld) instead of the old-style (NextStep) dynamic linker (rld).
    Dyld is necessary to support frameworks. */
 /* #undef WITH_DYLD */
 
-/* Define to build the readline module against Editline. */
-/* #undef WITH_EDITLINE */
-
-/* Define if you want to compile in object freelists optimization */
-#define WITH_FREELISTS 1
-
 /* Define to 1 if libintl is needed for locale functions. */
 /* #undef WITH_LIBINTL */
 
 /* Define if you want to produce an OpenStep/Rhapsody framework (shared
    library plus accessory files). */
 /* #undef WITH_NEXT_FRAMEWORK */
 
@@ -1754,14 +1586,17 @@
 
 /* Define on Darwin to activate all library features */
 #define _DARWIN_C_SOURCE 1
 
 /* This must be set to 64 on some systems to enable large file support. */
 #define _FILE_OFFSET_BITS 64
 
+/* Define on Linux to activate all library features */
+#define _GNU_SOURCE 1
+
 /* Define to include mbstate_t for mbrtowc */
 /* #undef _INCLUDE__STDC_A1_SOURCE */
 
 /* This must be defined on some systems to enable large file support. */
 #define _LARGEFILE_SOURCE 1
 
 /* This must be defined on AIX systems to enable large file support. */
@@ -1788,23 +1623,14 @@
 
 /* framework name */
 #define _PYTHONFRAMEWORK ""
 
 /* Define to force use of thread-safe errno, h_errno, and other functions */
 #define _REENTRANT 1
 
-/* Define to 1 if you want to emulate getpid() on WASI */
-/* #undef _WASI_EMULATED_GETPID */
-
-/* Define to 1 if you want to emulate process clocks on WASI */
-/* #undef _WASI_EMULATED_PROCESS_CLOCKS */
-
-/* Define to 1 if you want to emulate signals on WASI */
-/* #undef _WASI_EMULATED_SIGNAL */
-
 /* Define to the level of X/Open that your system supports */
 #define _XOPEN_SOURCE 700
 
 /* Define to activate Unix95-and-earlier features */
 #define _XOPEN_SOURCE_EXTENDED 1
 
 /* Define on FreeBSD to activate all library features */
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.d` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyexpat.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyframe.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacro.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymath.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pyport.h`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
 
 #include "exports.h"
 
 /* only get special linkage if built as shared or platform is Cygwin */
 #if defined(Py_ENABLE_SHARED) || defined(__CYGWIN__)
 #       if defined(HAVE_DECLSPEC_DLL)
 #               if defined(Py_BUILD_CORE) && !defined(Py_BUILD_CORE_MODULE)
-#                       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#                       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #                       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
         /* module init functions inside the core need no external linkage */
         /* except for Cygwin to handle embedding */
 #                       if defined(__CYGWIN__)
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __CYGWIN__ */
 #                               define PyMODINIT_FUNC PyObject*
@@ -536,30 +536,30 @@
 #               else /* Py_BUILD_CORE */
         /* Building an extension module, or an embedded situation */
         /* public Python functions and data are imported */
         /* Under Cygwin, auto-import functions to prevent compilation */
         /* failures similar to those described at the bottom of 4.1: */
         /* http://docs.python.org/extending/windows.html#a-cookbook-approach */
 #                       if !defined(__CYGWIN__)
-#                               define PyAPI_FUNC(RTYPE) Py_IMPORTED_SYMBOL RTYPE
+#                               define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_IMPORTED_SYMBOL RTYPE
 #                       endif /* !__CYGWIN__ */
 #                       define PyAPI_DATA(RTYPE) extern Py_IMPORTED_SYMBOL RTYPE
         /* module init functions outside the core must be exported */
 #                       if defined(__cplusplus)
 #                               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __cplusplus */
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       endif /* __cplusplus */
 #               endif /* Py_BUILD_CORE */
 #       endif /* HAVE_DECLSPEC_DLL */
 #endif /* Py_ENABLE_SHARED */
 
 /* If no external linkage macros defined by now, create defaults */
 #ifndef PyAPI_FUNC
-#       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyAPI_DATA
 #       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyMODINIT_FUNC
 #       if defined(__cplusplus)
 #               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrtod.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythread.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pytypedefs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/rangeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/setobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/sliceobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/structmember.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/structseq.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/token.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/tracemalloc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/typeslots.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp311/weakrefobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp311/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/LICENSE` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python-ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/asdl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/boolobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytes_methods.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cellobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/classobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/codecs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/complexobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/datetime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/descrobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/dynamic_annotations.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/errcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/eval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/frameobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/funcobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/genobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/graminit.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/grammar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_accu.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_atomic.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_condvar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_gil.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_hamt.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_long.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/intrcheck.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/iterobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/longintrepr.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/longobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/marshal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/memoryobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/modsupport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/node.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/odictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/opcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/osdefs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/parsetok.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/patchlevel.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/picklebufobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/py_curses.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyarena.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pycapsule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyconfig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 /* pyconfig.h.  Generated from pyconfig.h.in by configure.  */
 /* pyconfig.h.in.  Generated from configure.ac by autoheader.  */
 
-
 #ifndef Py_PYCONFIG_H
 #define Py_PYCONFIG_H
 
-
 /* Define if building universal (internal helper macro) */
 /* #undef AC_APPLE_UNIVERSAL_BUILD */
 
+/* BUILD_GNU_TYPE + AIX_BUILDDATE are used to construct the PEP425 tag of the
+   build system. */
+/* #undef AIX_BUILDDATE */
+
 /* Define for AIX if your compiler is a genuine IBM xlC/xlC_r and you want
    support for AIX C++ shared extension modules. */
 /* #undef AIX_GENUINE_CPLUSPLUS */
 
 /* Alternative SOABI used in debug build to load C extensions built in release
    mode */
 /* #undef ALT_SOABI */
@@ -29,38 +31,34 @@
 /* #undef DOUBLE_IS_BIG_ENDIAN_IEEE754 */
 
 /* Define if C doubles are 64-bit IEEE 754 binary format, stored with the
    least significant byte first */
 #define DOUBLE_IS_LITTLE_ENDIAN_IEEE754 1
 
 /* Define if --enable-ipv6 is specified */
-#define ENABLE_IPV6 1
+/* #undef ENABLE_IPV6 */
 
 /* Define to 1 if your system stores words within floats with the most
    significant word first */
 /* #undef FLOAT_WORDS_BIGENDIAN */
 
 /* Define if flock needs to be linked with bsd library. */
 /* #undef FLOCK_NEEDS_LIBBSD */
 
 /* Define if getpgrp() must be called as getpgrp(0). */
 /* #undef GETPGRP_HAVE_ARG */
 
-/* Define if gettimeofday() does not have second (timezone) argument This is
-   the case on Motorola V4 (R40V4.2) */
-/* #undef GETTIMEOFDAY_NO_TZ */
-
 /* Define to 1 if you have the `accept4' function. */
 #define HAVE_ACCEPT4 1
 
 /* Define to 1 if you have the `acosh' function. */
 #define HAVE_ACOSH 1
 
 /* struct addrinfo (netdb.h) */
-#define HAVE_ADDRINFO 1
+/* #undef HAVE_ADDRINFO */
 
 /* Define to 1 if you have the `alarm' function. */
 #define HAVE_ALARM 1
 
 /* Define if aligned memory access is required */
 /* #undef HAVE_ALIGNED_REQUIRED */
 
@@ -70,15 +68,15 @@
 /* Define this if your time.h defines altzone. */
 /* #undef HAVE_ALTZONE */
 
 /* Define to 1 if you have the `asinh' function. */
 #define HAVE_ASINH 1
 
 /* Define to 1 if you have the <asm/types.h> header file. */
-#define HAVE_ASM_TYPES_H 1
+/* #undef HAVE_ASM_TYPES_H */
 
 /* Define to 1 if you have the `atanh' function. */
 #define HAVE_ATANH 1
 
 /* Define to 1 if you have the `bind_textdomain_codeset' function. */
 #define HAVE_BIND_TEXTDOMAIN_CODESET 1
 
@@ -201,168 +199,171 @@
 /* #undef HAVE_CURSES_WCHGAT */
 
 /* Define to 1 if you have the declaration of `isfinite', and to 0 if you
    don't. */
 #define HAVE_DECL_ISFINITE 1
 
 /* Define to 1 if you have the declaration of `isinf', and to 0 if you don't.
-   */
+ */
 #define HAVE_DECL_ISINF 1
 
 /* Define to 1 if you have the declaration of `isnan', and to 0 if you don't.
-   */
+ */
 #define HAVE_DECL_ISNAN 1
 
 /* Define to 1 if you have the declaration of `RTLD_DEEPBIND', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_DEEPBIND 1
+/* #undef HAVE_DECL_RTLD_DEEPBIND */
 
 /* Define to 1 if you have the declaration of `RTLD_GLOBAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_GLOBAL 1
+/* #undef HAVE_DECL_RTLD_GLOBAL */
 
 /* Define to 1 if you have the declaration of `RTLD_LAZY', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LAZY 1
+/* #undef HAVE_DECL_RTLD_LAZY */
 
 /* Define to 1 if you have the declaration of `RTLD_LOCAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LOCAL 1
+/* #undef HAVE_DECL_RTLD_LOCAL */
 
 /* Define to 1 if you have the declaration of `RTLD_MEMBER', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_MEMBER 0
+/* #undef HAVE_DECL_RTLD_MEMBER */
 
 /* Define to 1 if you have the declaration of `RTLD_NODELETE', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NODELETE 1
+/* #undef HAVE_DECL_RTLD_NODELETE */
 
 /* Define to 1 if you have the declaration of `RTLD_NOLOAD', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOLOAD 1
+/* #undef HAVE_DECL_RTLD_NOLOAD */
 
 /* Define to 1 if you have the declaration of `RTLD_NOW', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOW 1
+/* #undef HAVE_DECL_RTLD_NOW */
 
 /* Define to 1 if you have the declaration of `tzname', and to 0 if you don't.
-   */
+ */
 /* #undef HAVE_DECL_TZNAME */
 
 /* Define to 1 if you have the device macros. */
-#define HAVE_DEVICE_MACROS 1
+/* #undef HAVE_DEVICE_MACROS */
 
 /* Define to 1 if you have the /dev/ptc device file. */
 /* #undef HAVE_DEV_PTC */
 
 /* Define to 1 if you have the /dev/ptmx device file. */
-#define HAVE_DEV_PTMX 1
+/* #undef HAVE_DEV_PTMX */
 
 /* Define to 1 if you have the <direct.h> header file. */
 /* #undef HAVE_DIRECT_H */
 
 /* Define to 1 if the dirent structure has a d_type field */
 #define HAVE_DIRENT_D_TYPE 1
 
 /* Define to 1 if you have the <dirent.h> header file, and it defines `DIR'.
-   */
+ */
 #define HAVE_DIRENT_H 1
 
 /* Define if you have the 'dirfd' function or macro. */
 #define HAVE_DIRFD 1
 
 /* Define to 1 if you have the <dlfcn.h> header file. */
-#define HAVE_DLFCN_H 1
+/* #undef HAVE_DLFCN_H */
 
 /* Define to 1 if you have the `dlopen' function. */
-#define HAVE_DLOPEN 1
+/* #undef HAVE_DLOPEN */
 
 /* Define to 1 if you have the `dup2' function. */
-#define HAVE_DUP2 1
+/* #undef HAVE_DUP2 */
 
 /* Define to 1 if you have the `dup3' function. */
-#define HAVE_DUP3 1
+/* #undef HAVE_DUP3 */
+
+/* Define if you have the '_dyld_shared_cache_contains_path' function. */
+/* #undef HAVE_DYLD_SHARED_CACHE_CONTAINS_PATH */
 
 /* Defined when any dynamic module loading is enabled. */
 #define HAVE_DYNAMIC_LOADING 1
 
 /* Define to 1 if you have the <endian.h> header file. */
 #define HAVE_ENDIAN_H 1
 
 /* Define if you have the 'epoll' functions. */
-#define HAVE_EPOLL 1
+/* #undef HAVE_EPOLL */
 
 /* Define if you have the 'epoll_create1' function. */
-#define HAVE_EPOLL_CREATE1 1
+/* #undef HAVE_EPOLL_CREATE1 */
 
 /* Define to 1 if you have the `erf' function. */
 #define HAVE_ERF 1
 
 /* Define to 1 if you have the `erfc' function. */
 #define HAVE_ERFC 1
 
 /* Define to 1 if you have the <errno.h> header file. */
 #define HAVE_ERRNO_H 1
 
 /* Define to 1 if you have the `execv' function. */
-#define HAVE_EXECV 1
+/* #undef HAVE_EXECV */
 
 /* Define to 1 if you have the `explicit_bzero' function. */
 #define HAVE_EXPLICIT_BZERO 1
 
 /* Define to 1 if you have the `explicit_memset' function. */
 /* #undef HAVE_EXPLICIT_MEMSET */
 
 /* Define to 1 if you have the `expm1' function. */
 #define HAVE_EXPM1 1
 
 /* Define to 1 if you have the `faccessat' function. */
 #define HAVE_FACCESSAT 1
 
 /* Define if you have the 'fchdir' function. */
-#define HAVE_FCHDIR 1
+/* #undef HAVE_FCHDIR */
 
 /* Define to 1 if you have the `fchmod' function. */
-#define HAVE_FCHMOD 1
+/* #undef HAVE_FCHMOD */
 
 /* Define to 1 if you have the `fchmodat' function. */
-#define HAVE_FCHMODAT 1
+/* #undef HAVE_FCHMODAT */
 
 /* Define to 1 if you have the `fchown' function. */
-#define HAVE_FCHOWN 1
+/* #undef HAVE_FCHOWN */
 
 /* Define to 1 if you have the `fchownat' function. */
-#define HAVE_FCHOWNAT 1
+/* #undef HAVE_FCHOWNAT */
 
 /* Define to 1 if you have the <fcntl.h> header file. */
 #define HAVE_FCNTL_H 1
 
 /* Define if you have the 'fdatasync' function. */
 #define HAVE_FDATASYNC 1
 
 /* Define to 1 if you have the `fdopendir' function. */
 #define HAVE_FDOPENDIR 1
 
 /* Define to 1 if you have the `fdwalk' function. */
 /* #undef HAVE_FDWALK */
 
 /* Define to 1 if you have the `fexecve' function. */
-#define HAVE_FEXECVE 1
+/* #undef HAVE_FEXECVE */
 
 /* Define to 1 if you have the `finite' function. */
 #define HAVE_FINITE 1
 
 /* Define to 1 if you have the `flock' function. */
-#define HAVE_FLOCK 1
+/* #undef HAVE_FLOCK */
 
 /* Define to 1 if you have the `fork' function. */
-#define HAVE_FORK 1
+/* #undef HAVE_FORK */
 
 /* Define to 1 if you have the `forkpty' function. */
-#define HAVE_FORKPTY 1
+/* #undef HAVE_FORKPTY */
 
 /* Define to 1 if you have the `fpathconf' function. */
 #define HAVE_FPATHCONF 1
 
 /* Define to 1 if you have the `fseek64' function. */
 /* #undef HAVE_FSEEK64 */
 
@@ -390,320 +391,332 @@
 /* Define to 1 if you have the `ftruncate' function. */
 #define HAVE_FTRUNCATE 1
 
 /* Define to 1 if you have the `futimens' function. */
 #define HAVE_FUTIMENS 1
 
 /* Define to 1 if you have the `futimes' function. */
-#define HAVE_FUTIMES 1
+/* #undef HAVE_FUTIMES */
 
 /* Define to 1 if you have the `futimesat' function. */
-#define HAVE_FUTIMESAT 1
+/* #undef HAVE_FUTIMESAT */
 
 /* Define to 1 if you have the `gai_strerror' function. */
-#define HAVE_GAI_STRERROR 1
+/* #undef HAVE_GAI_STRERROR */
 
 /* Define to 1 if you have the `gamma' function. */
-#define HAVE_GAMMA 1
+/* #undef HAVE_GAMMA */
 
 /* Define if we can use gcc inline assembler to get and set mc68881 fpcr */
 /* #undef HAVE_GCC_ASM_FOR_MC68881 */
 
 /* Define if we can use x64 gcc inline assembler */
-#define HAVE_GCC_ASM_FOR_X64 1
+/* #undef HAVE_GCC_ASM_FOR_X64 */
 
 /* Define if we can use gcc inline assembler to get and set x87 control word
-   */
-#define HAVE_GCC_ASM_FOR_X87 1
+ */
+/* #undef HAVE_GCC_ASM_FOR_X87 */
 
 /* Define if your compiler provides __uint128_t */
 #define HAVE_GCC_UINT128_T 1
 
 /* Define if you have the getaddrinfo function. */
-#define HAVE_GETADDRINFO 1
+/* #undef HAVE_GETADDRINFO */
 
 /* Define this if you have flockfile(), getc_unlocked(), and funlockfile() */
-#define HAVE_GETC_UNLOCKED 1
+/* #undef HAVE_GETC_UNLOCKED */
 
 /* Define to 1 if you have the `getentropy' function. */
 #define HAVE_GETENTROPY 1
 
 /* Define to 1 if you have the `getgrgid_r' function. */
-#define HAVE_GETGRGID_R 1
+/* #undef HAVE_GETGRGID_R */
 
 /* Define to 1 if you have the `getgrnam_r' function. */
-#define HAVE_GETGRNAM_R 1
+/* #undef HAVE_GETGRNAM_R */
 
 /* Define to 1 if you have the `getgrouplist' function. */
-#define HAVE_GETGROUPLIST 1
+/* #undef HAVE_GETGROUPLIST */
 
 /* Define to 1 if you have the `getgroups' function. */
-#define HAVE_GETGROUPS 1
+/* #undef HAVE_GETGROUPS */
 
 /* Define to 1 if you have the `gethostbyname' function. */
 /* #undef HAVE_GETHOSTBYNAME */
 
 /* Define this if you have some version of gethostbyname_r() */
-#define HAVE_GETHOSTBYNAME_R 1
+/* #undef HAVE_GETHOSTBYNAME_R */
 
 /* Define this if you have the 3-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_3_ARG */
 
 /* Define this if you have the 5-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_5_ARG */
 
 /* Define this if you have the 6-arg version of gethostbyname_r(). */
-#define HAVE_GETHOSTBYNAME_R_6_ARG 1
+/* #undef HAVE_GETHOSTBYNAME_R_6_ARG */
 
 /* Define to 1 if you have the `getitimer' function. */
-#define HAVE_GETITIMER 1
+/* #undef HAVE_GETITIMER */
 
 /* Define to 1 if you have the `getloadavg' function. */
-#define HAVE_GETLOADAVG 1
+/* #undef HAVE_GETLOADAVG */
 
 /* Define to 1 if you have the `getlogin' function. */
-#define HAVE_GETLOGIN 1
+/* #undef HAVE_GETLOGIN */
 
 /* Define to 1 if you have the `getnameinfo' function. */
-#define HAVE_GETNAMEINFO 1
+/* #undef HAVE_GETNAMEINFO */
 
 /* Define if you have the 'getpagesize' function. */
-#define HAVE_GETPAGESIZE 1
+/* #undef HAVE_GETPAGESIZE */
 
 /* Define to 1 if you have the `getpeername' function. */
-#define HAVE_GETPEERNAME 1
+/* #undef HAVE_GETPEERNAME */
 
 /* Define to 1 if you have the `getpgid' function. */
-#define HAVE_GETPGID 1
+/* #undef HAVE_GETPGID */
 
 /* Define to 1 if you have the `getpgrp' function. */
-#define HAVE_GETPGRP 1
+/* #undef HAVE_GETPGRP */
 
 /* Define to 1 if you have the `getpid' function. */
-#define HAVE_GETPID 1
+/* #undef HAVE_GETPID */
 
 /* Define to 1 if you have the `getpriority' function. */
-#define HAVE_GETPRIORITY 1
+/* #undef HAVE_GETPRIORITY */
 
 /* Define to 1 if you have the `getpwent' function. */
-#define HAVE_GETPWENT 1
+/* #undef HAVE_GETPWENT */
 
 /* Define to 1 if you have the `getpwnam_r' function. */
-#define HAVE_GETPWNAM_R 1
+/* #undef HAVE_GETPWNAM_R */
 
 /* Define to 1 if you have the `getpwuid_r' function. */
-#define HAVE_GETPWUID_R 1
+/* #undef HAVE_GETPWUID_R */
 
 /* Define to 1 if the getrandom() function is available */
-#define HAVE_GETRANDOM 1
+/* #undef HAVE_GETRANDOM */
 
 /* Define to 1 if the Linux getrandom() syscall is available */
-#define HAVE_GETRANDOM_SYSCALL 1
+/* #undef HAVE_GETRANDOM_SYSCALL */
 
 /* Define to 1 if you have the `getresgid' function. */
-#define HAVE_GETRESGID 1
+/* #undef HAVE_GETRESGID */
 
 /* Define to 1 if you have the `getresuid' function. */
-#define HAVE_GETRESUID 1
+/* #undef HAVE_GETRESUID */
 
 /* Define to 1 if you have the `getsid' function. */
-#define HAVE_GETSID 1
+/* #undef HAVE_GETSID */
 
 /* Define to 1 if you have the `getspent' function. */
-#define HAVE_GETSPENT 1
+/* #undef HAVE_GETSPENT */
 
 /* Define to 1 if you have the `getspnam' function. */
-#define HAVE_GETSPNAM 1
-
-/* Define to 1 if you have the `gettimeofday' function. */
-#define HAVE_GETTIMEOFDAY 1
+/* #undef HAVE_GETSPNAM */
 
 /* Define to 1 if you have the `getwd' function. */
-#define HAVE_GETWD 1
+/* #undef HAVE_GETWD */
 
 /* Define if glibc has incorrect _FORTIFY_SOURCE wrappers for memmove and
    bcopy. */
 /* #undef HAVE_GLIBC_MEMMOVE_BUG */
 
 /* Define to 1 if you have the <grp.h> header file. */
-#define HAVE_GRP_H 1
+/* #undef HAVE_GRP_H */
 
 /* Define if you have the 'hstrerror' function. */
-#define HAVE_HSTRERROR 1
+/* #undef HAVE_HSTRERROR */
 
 /* Define this if you have le64toh() */
 #define HAVE_HTOLE64 1
 
 /* Define to 1 if you have the `hypot' function. */
 #define HAVE_HYPOT 1
 
 /* Define to 1 if you have the <ieeefp.h> header file. */
 /* #undef HAVE_IEEEFP_H */
 
 /* Define to 1 if you have the `if_nameindex' function. */
-#define HAVE_IF_NAMEINDEX 1
+/* #undef HAVE_IF_NAMEINDEX */
 
 /* Define if you have the 'inet_aton' function. */
 #define HAVE_INET_ATON 1
 
 /* Define if you have the 'inet_pton' function. */
 #define HAVE_INET_PTON 1
 
 /* Define to 1 if you have the `initgroups' function. */
-#define HAVE_INITGROUPS 1
+/* #undef HAVE_INITGROUPS */
 
 /* Define to 1 if you have the <inttypes.h> header file. */
 #define HAVE_INTTYPES_H 1
 
 /* Define to 1 if you have the <io.h> header file. */
 /* #undef HAVE_IO_H */
 
 /* Define if gcc has the ipa-pure-const bug. */
 /* #undef HAVE_IPA_PURE_CONST_BUG */
 
 /* Define to 1 if you have the `kill' function. */
-#define HAVE_KILL 1
+/* #undef HAVE_KILL */
 
 /* Define to 1 if you have the `killpg' function. */
-#define HAVE_KILLPG 1
+/* #undef HAVE_KILLPG */
 
 /* Define if you have the 'kqueue' functions. */
 /* #undef HAVE_KQUEUE */
 
 /* Define to 1 if you have the <langinfo.h> header file. */
 #define HAVE_LANGINFO_H 1
 
 /* Defined to enable large file support when an off_t is bigger than a long
    and long long is at least as big as an off_t. You may need to add some
    flags for configuration and compilation to enable this mode. (For Solaris
    and Linux, the necessary defines are already defined.) */
-/* #undef HAVE_LARGEFILE_SUPPORT */
+#define HAVE_LARGEFILE_SUPPORT 1
 
 /* Define to 1 if you have the 'lchflags' function. */
 /* #undef HAVE_LCHFLAGS */
 
 /* Define to 1 if you have the `lchmod' function. */
 /* #undef HAVE_LCHMOD */
 
 /* Define to 1 if you have the `lchown' function. */
-#define HAVE_LCHOWN 1
+/* #undef HAVE_LCHOWN */
 
 /* Define to 1 if you have the `lgamma' function. */
 #define HAVE_LGAMMA 1
 
 /* Define to 1 if you have the `dl' library (-ldl). */
 #define HAVE_LIBDL 1
 
 /* Define to 1 if you have the `dld' library (-ldld). */
 /* #undef HAVE_LIBDLD */
 
 /* Define to 1 if you have the `ieee' library (-lieee). */
 /* #undef HAVE_LIBIEEE */
 
 /* Define to 1 if you have the <libintl.h> header file. */
-#define HAVE_LIBINTL_H 1
+/* #undef HAVE_LIBINTL_H */
 
 /* Define if you have the readline library (-lreadline). */
 /* #undef HAVE_LIBREADLINE */
 
 /* Define to 1 if you have the `resolv' library (-lresolv). */
-/* #undef HAVE_LIBRESOLV */
+#define HAVE_LIBRESOLV 1
 
 /* Define to 1 if you have the `sendfile' library (-lsendfile). */
 /* #undef HAVE_LIBSENDFILE */
 
 /* Define to 1 if you have the <libutil.h> header file. */
-/* #undef HAVE_LIBUTIL_H */
+#define HAVE_LIBUTIL_H 1
+
+/* Define to 1 if you have the `uuid' library (-luuid). */
+/* #undef HAVE_LIBUUID */
 
 /* Define if you have the 'link' function. */
 #define HAVE_LINK 1
 
 /* Define to 1 if you have the `linkat' function. */
 #define HAVE_LINKAT 1
 
+/* Define to 1 if you have the <linux/auxvec.h> header file. */
+/* #undef HAVE_LINUX_AUXVEC_H */
+
 /* Define to 1 if you have the <linux/can/bcm.h> header file. */
-#define HAVE_LINUX_CAN_BCM_H 1
+/* #undef HAVE_LINUX_CAN_BCM_H */
 
 /* Define to 1 if you have the <linux/can.h> header file. */
-#define HAVE_LINUX_CAN_H 1
+/* #undef HAVE_LINUX_CAN_H */
+
+/* Define to 1 if you have the <linux/can/j1939.h> header file. */
+/* #undef HAVE_LINUX_CAN_J1939_H */
 
 /* Define if compiling using Linux 3.6 or later. */
-#define HAVE_LINUX_CAN_RAW_FD_FRAMES 1
+/* #undef HAVE_LINUX_CAN_RAW_FD_FRAMES */
 
 /* Define to 1 if you have the <linux/can/raw.h> header file. */
-#define HAVE_LINUX_CAN_RAW_H 1
+/* #undef HAVE_LINUX_CAN_RAW_H */
+
+/* Define if compiling using Linux 4.1 or later. */
+/* #undef HAVE_LINUX_CAN_RAW_JOIN_FILTERS */
 
 /* Define to 1 if you have the <linux/memfd.h> header file. */
-#define HAVE_LINUX_MEMFD_H 1
+/* #undef HAVE_LINUX_MEMFD_H */
 
 /* Define to 1 if you have the <linux/netlink.h> header file. */
-#define HAVE_LINUX_NETLINK_H 1
+/* #undef HAVE_LINUX_NETLINK_H */
 
 /* Define to 1 if you have the <linux/qrtr.h> header file. */
-#define HAVE_LINUX_QRTR_H 1
+/* #undef HAVE_LINUX_QRTR_H */
 
 /* Define to 1 if you have the <linux/random.h> header file. */
-#define HAVE_LINUX_RANDOM_H 1
+/* #undef HAVE_LINUX_RANDOM_H */
 
 /* Define to 1 if you have the <linux/tipc.h> header file. */
-#define HAVE_LINUX_TIPC_H 1
+/* #undef HAVE_LINUX_TIPC_H */
 
 /* Define to 1 if you have the <linux/vm_sockets.h> header file. */
-#define HAVE_LINUX_VM_SOCKETS_H 1
+/* #undef HAVE_LINUX_VM_SOCKETS_H */
+
+/* Define to 1 if you have the <linux/wait.h> header file. */
+/* #undef HAVE_LINUX_WAIT_H */
 
 /* Define to 1 if you have the `lockf' function. */
-#define HAVE_LOCKF 1
+/* #undef HAVE_LOCKF */
 
 /* Define to 1 if you have the `log1p' function. */
 #define HAVE_LOG1P 1
 
 /* Define to 1 if you have the `log2' function. */
 #define HAVE_LOG2 1
 
 /* Define to 1 if the system has the type `long double'. */
 #define HAVE_LONG_DOUBLE 1
 
 /* Define to 1 if you have the `lstat' function. */
 #define HAVE_LSTAT 1
 
 /* Define to 1 if you have the `lutimes' function. */
-#define HAVE_LUTIMES 1
+/* #undef HAVE_LUTIMES */
 
 /* Define to 1 if you have the `madvise' function. */
-#define HAVE_MADVISE 1
+/* #undef HAVE_MADVISE */
 
 /* Define this if you have the makedev macro. */
-#define HAVE_MAKEDEV 1
+/* #undef HAVE_MAKEDEV */
 
 /* Define to 1 if you have the `mbrtowc' function. */
 #define HAVE_MBRTOWC 1
 
 /* Define if you have the 'memfd_create' function. */
-#define HAVE_MEMFD_CREATE 1
+/* #undef HAVE_MEMFD_CREATE */
 
 /* Define to 1 if you have the <memory.h> header file. */
 #define HAVE_MEMORY_H 1
 
 /* Define to 1 if you have the `memrchr' function. */
 #define HAVE_MEMRCHR 1
 
 /* Define to 1 if you have the `mkdirat' function. */
 #define HAVE_MKDIRAT 1
 
 /* Define to 1 if you have the `mkfifo' function. */
-#define HAVE_MKFIFO 1
+/* #undef HAVE_MKFIFO */
 
 /* Define to 1 if you have the `mkfifoat' function. */
-#define HAVE_MKFIFOAT 1
+/* #undef HAVE_MKFIFOAT */
 
 /* Define to 1 if you have the `mknod' function. */
-#define HAVE_MKNOD 1
+/* #undef HAVE_MKNOD */
 
 /* Define to 1 if you have the `mknodat' function. */
-#define HAVE_MKNODAT 1
+/* #undef HAVE_MKNODAT */
 
 /* Define to 1 if you have the `mktime' function. */
 #define HAVE_MKTIME 1
 
 /* Define to 1 if you have the `mmap' function. */
 #define HAVE_MMAP 1
 
@@ -716,33 +729,37 @@
 /* Define to 1 if you have the <ndir.h> header file, and it defines `DIR'. */
 /* #undef HAVE_NDIR_H */
 
 /* Define to 1 if you have the <netpacket/packet.h> header file. */
 #define HAVE_NETPACKET_PACKET_H 1
 
 /* Define to 1 if you have the <net/if.h> header file. */
-#define HAVE_NET_IF_H 1
+/* #undef HAVE_NET_IF_H */
 
 /* Define to 1 if you have the `nice' function. */
-#define HAVE_NICE 1
+/* #undef HAVE_NICE */
+
+/* Define if the internal form of wchar_t in non-Unicode locales is not
+   Unicode. */
+/* #undef HAVE_NON_UNICODE_WCHAR_T_REPRESENTATION */
 
 /* Define to 1 if you have the `openat' function. */
 #define HAVE_OPENAT 1
 
 /* Define to 1 if you have the `openpty' function. */
-#define HAVE_OPENPTY 1
+/* #undef HAVE_OPENPTY */
 
 /* Define to 1 if you have the `pathconf' function. */
 #define HAVE_PATHCONF 1
 
 /* Define to 1 if you have the `pause' function. */
-#define HAVE_PAUSE 1
+/* #undef HAVE_PAUSE */
 
 /* Define to 1 if you have the `pipe2' function. */
-#define HAVE_PIPE2 1
+/* #undef HAVE_PIPE2 */
 
 /* Define to 1 if you have the `plock' function. */
 /* #undef HAVE_PLOCK */
 
 /* Define to 1 if you have the `poll' function. */
 #define HAVE_POLL 1
 
@@ -752,33 +769,30 @@
 /* Define to 1 if you have the `posix_fadvise' function. */
 #define HAVE_POSIX_FADVISE 1
 
 /* Define to 1 if you have the `posix_fallocate' function. */
 #define HAVE_POSIX_FALLOCATE 1
 
 /* Define to 1 if you have the `posix_spawn' function. */
-#define HAVE_POSIX_SPAWN 1
+/* #undef HAVE_POSIX_SPAWN */
 
 /* Define to 1 if you have the `posix_spawnp' function. */
-#define HAVE_POSIX_SPAWNP 1
+/* #undef HAVE_POSIX_SPAWNP */
 
 /* Define to 1 if you have the `pread' function. */
 #define HAVE_PREAD 1
 
 /* Define to 1 if you have the `preadv' function. */
 #define HAVE_PREADV 1
 
 /* Define to 1 if you have the `preadv2' function. */
-#define HAVE_PREADV2 1
+/* #undef HAVE_PREADV2 */
 
 /* Define if you have the 'prlimit' functions. */
-#define HAVE_PRLIMIT 1
-
-/* Define if you have the '_dyld_shared_cache_contains_path' function. */
-/* #undef HAVE_DYLD_SHARED_CACHE_CONTAINS_PATH */
+/* #undef HAVE_PRLIMIT */
 
 /* Define to 1 if you have the <process.h> header file. */
 /* #undef HAVE_PROCESS_H */
 
 /* Define if your compiler supports function prototype */
 #define HAVE_PROTOTYPES 1
 
@@ -794,45 +808,42 @@
 /* Define to 1 if you have the <pthread.h> header file. */
 #define HAVE_PTHREAD_H 1
 
 /* Define to 1 if you have the `pthread_init' function. */
 /* #undef HAVE_PTHREAD_INIT */
 
 /* Define to 1 if you have the `pthread_kill' function. */
-#define HAVE_PTHREAD_KILL 1
+/* #undef HAVE_PTHREAD_KILL */
 
 /* Define to 1 if you have the `pthread_sigmask' function. */
-#define HAVE_PTHREAD_SIGMASK 1
+/* #undef HAVE_PTHREAD_SIGMASK */
 
 /* Define to 1 if you have the <pty.h> header file. */
-#define HAVE_PTY_H 1
-
-/* Define to 1 if you have the `putenv' function. */
-#define HAVE_PUTENV 1
+/* #undef HAVE_PTY_H */
 
 /* Define to 1 if you have the `pwrite' function. */
 #define HAVE_PWRITE 1
 
 /* Define to 1 if you have the `pwritev' function. */
 #define HAVE_PWRITEV 1
 
 /* Define to 1 if you have the `pwritev2' function. */
-#define HAVE_PWRITEV2 1
+/* #undef HAVE_PWRITEV2 */
 
 /* Define to 1 if you have the `readlink' function. */
 #define HAVE_READLINK 1
 
 /* Define to 1 if you have the `readlinkat' function. */
 #define HAVE_READLINKAT 1
 
 /* Define to 1 if you have the `readv' function. */
 #define HAVE_READV 1
 
 /* Define to 1 if you have the `realpath' function. */
-#define HAVE_REALPATH 1
+/* #undef HAVE_REALPATH */
 
 /* Define to 1 if you have the `renameat' function. */
 #define HAVE_RENAMEAT 1
 
 /* Define if readline supports append_history */
 /* #undef HAVE_RL_APPEND_HISTORY */
 
@@ -860,162 +871,165 @@
 /* Define to 1 if you have the `round' function. */
 #define HAVE_ROUND 1
 
 /* Define to 1 if you have the `rtpSpawn' function. */
 /* #undef HAVE_RTPSPAWN */
 
 /* Define to 1 if you have the `sched_get_priority_max' function. */
-#define HAVE_SCHED_GET_PRIORITY_MAX 1
+/* #undef HAVE_SCHED_GET_PRIORITY_MAX */
 
 /* Define to 1 if you have the <sched.h> header file. */
 #define HAVE_SCHED_H 1
 
 /* Define to 1 if you have the `sched_rr_get_interval' function. */
-#define HAVE_SCHED_RR_GET_INTERVAL 1
+/* #undef HAVE_SCHED_RR_GET_INTERVAL */
 
 /* Define to 1 if you have the `sched_setaffinity' function. */
-#define HAVE_SCHED_SETAFFINITY 1
+/* #undef HAVE_SCHED_SETAFFINITY */
 
 /* Define to 1 if you have the `sched_setparam' function. */
-#define HAVE_SCHED_SETPARAM 1
+/* #undef HAVE_SCHED_SETPARAM */
 
 /* Define to 1 if you have the `sched_setscheduler' function. */
-#define HAVE_SCHED_SETSCHEDULER 1
+/* #undef HAVE_SCHED_SETSCHEDULER */
+
+/* Define to 1 if you have the `sem_clockwait' function. */
+/* #undef HAVE_SEM_CLOCKWAIT */
 
 /* Define to 1 if you have the `sem_getvalue' function. */
-#define HAVE_SEM_GETVALUE 1
+/* #undef HAVE_SEM_GETVALUE */
 
 /* Define to 1 if you have the `sem_open' function. */
-#define HAVE_SEM_OPEN 1
+/* #undef HAVE_SEM_OPEN */
 
 /* Define to 1 if you have the `sem_timedwait' function. */
-#define HAVE_SEM_TIMEDWAIT 1
+/* #undef HAVE_SEM_TIMEDWAIT */
 
 /* Define to 1 if you have the `sem_unlink' function. */
-#define HAVE_SEM_UNLINK 1
+/* #undef HAVE_SEM_UNLINK */
 
 /* Define to 1 if you have the `sendfile' function. */
-#define HAVE_SENDFILE 1
+/* #undef HAVE_SENDFILE */
 
 /* Define to 1 if you have the `setegid' function. */
-#define HAVE_SETEGID 1
+/* #undef HAVE_SETEGID */
 
 /* Define to 1 if you have the `seteuid' function. */
-#define HAVE_SETEUID 1
+/* #undef HAVE_SETEUID */
 
 /* Define to 1 if you have the `setgid' function. */
-#define HAVE_SETGID 1
+/* #undef HAVE_SETGID */
 
 /* Define if you have the 'setgroups' function. */
-#define HAVE_SETGROUPS 1
+/* #undef HAVE_SETGROUPS */
 
 /* Define to 1 if you have the `sethostname' function. */
-#define HAVE_SETHOSTNAME 1
+/* #undef HAVE_SETHOSTNAME */
 
 /* Define to 1 if you have the `setitimer' function. */
-#define HAVE_SETITIMER 1
+/* #undef HAVE_SETITIMER */
 
 /* Define to 1 if you have the `setlocale' function. */
 #define HAVE_SETLOCALE 1
 
 /* Define to 1 if you have the `setpgid' function. */
-#define HAVE_SETPGID 1
+/* #undef HAVE_SETPGID */
 
 /* Define to 1 if you have the `setpgrp' function. */
-#define HAVE_SETPGRP 1
+/* #undef HAVE_SETPGRP */
 
 /* Define to 1 if you have the `setpriority' function. */
-#define HAVE_SETPRIORITY 1
+/* #undef HAVE_SETPRIORITY */
 
 /* Define to 1 if you have the `setregid' function. */
-#define HAVE_SETREGID 1
+/* #undef HAVE_SETREGID */
 
 /* Define to 1 if you have the `setresgid' function. */
-#define HAVE_SETRESGID 1
+/* #undef HAVE_SETRESGID */
 
 /* Define to 1 if you have the `setresuid' function. */
-#define HAVE_SETRESUID 1
+/* #undef HAVE_SETRESUID */
 
 /* Define to 1 if you have the `setreuid' function. */
-#define HAVE_SETREUID 1
+/* #undef HAVE_SETREUID */
 
 /* Define to 1 if you have the `setsid' function. */
-#define HAVE_SETSID 1
+/* #undef HAVE_SETSID */
 
 /* Define to 1 if you have the `setuid' function. */
-#define HAVE_SETUID 1
+/* #undef HAVE_SETUID */
 
 /* Define to 1 if you have the `setvbuf' function. */
 #define HAVE_SETVBUF 1
 
 /* Define to 1 if you have the <shadow.h> header file. */
-#define HAVE_SHADOW_H 1
+/* #undef HAVE_SHADOW_H */
 
 /* Define to 1 if you have the `shm_open' function. */
-#define HAVE_SHM_OPEN 1
+/* #undef HAVE_SHM_OPEN */
 
 /* Define to 1 if you have the `shm_unlink' function. */
-#define HAVE_SHM_UNLINK 1
+/* #undef HAVE_SHM_UNLINK */
 
 /* Define to 1 if you have the `sigaction' function. */
-#define HAVE_SIGACTION 1
+/* #undef HAVE_SIGACTION */
 
 /* Define to 1 if you have the `sigaltstack' function. */
-#define HAVE_SIGALTSTACK 1
+/* #undef HAVE_SIGALTSTACK */
 
 /* Define to 1 if you have the `sigfillset' function. */
-#define HAVE_SIGFILLSET 1
+/* #undef HAVE_SIGFILLSET */
 
 /* Define to 1 if `si_band' is a member of `siginfo_t'. */
-#define HAVE_SIGINFO_T_SI_BAND 1
+/* #undef HAVE_SIGINFO_T_SI_BAND */
 
 /* Define to 1 if you have the `siginterrupt' function. */
-#define HAVE_SIGINTERRUPT 1
+/* #undef HAVE_SIGINTERRUPT */
 
 /* Define to 1 if you have the <signal.h> header file. */
-#define HAVE_SIGNAL_H 1
+/* #undef HAVE_SIGNAL_H */
 
 /* Define to 1 if you have the `sigpending' function. */
-#define HAVE_SIGPENDING 1
+/* #undef HAVE_SIGPENDING */
 
 /* Define to 1 if you have the `sigrelse' function. */
-#define HAVE_SIGRELSE 1
+/* #undef HAVE_SIGRELSE */
 
 /* Define to 1 if you have the `sigtimedwait' function. */
-#define HAVE_SIGTIMEDWAIT 1
+/* #undef HAVE_SIGTIMEDWAIT */
 
 /* Define to 1 if you have the `sigwait' function. */
-#define HAVE_SIGWAIT 1
+/* #undef HAVE_SIGWAIT */
 
 /* Define to 1 if you have the `sigwaitinfo' function. */
-#define HAVE_SIGWAITINFO 1
+/* #undef HAVE_SIGWAITINFO */
 
 /* Define to 1 if you have the `snprintf' function. */
 #define HAVE_SNPRINTF 1
 
 /* struct sockaddr_alg (linux/if_alg.h) */
-#define HAVE_SOCKADDR_ALG 1
+/* #undef HAVE_SOCKADDR_ALG */
 
 /* Define if sockaddr has sa_len member */
 /* #undef HAVE_SOCKADDR_SA_LEN */
 
 /* struct sockaddr_storage (sys/socket.h) */
 #define HAVE_SOCKADDR_STORAGE 1
 
 /* Define if you have the 'socketpair' function. */
-#define HAVE_SOCKETPAIR 1
+/* #undef HAVE_SOCKETPAIR */
 
 /* Define to 1 if you have the <spawn.h> header file. */
-#define HAVE_SPAWN_H 1
+/* #undef HAVE_SPAWN_H */
 
 /* Define if your compiler provides ssize_t */
 #define HAVE_SSIZE_T 1
 
 /* Define to 1 if you have the `statvfs' function. */
-#define HAVE_STATVFS 1
+/* #undef HAVE_STATVFS */
 
 /* Define if you have struct stat.st_mtim.tv_nsec */
 #define HAVE_STAT_TV_NSEC 1
 
 /* Define if you have struct stat.st_mtimensec */
 /* #undef HAVE_STAT_TV_NSEC2 */
 
@@ -1041,27 +1055,27 @@
 /* Define to 1 if you have the <strings.h> header file. */
 #define HAVE_STRINGS_H 1
 
 /* Define to 1 if you have the <string.h> header file. */
 #define HAVE_STRING_H 1
 
 /* Define to 1 if you have the `strlcpy' function. */
-/* #undef HAVE_STRLCPY */
+#define HAVE_STRLCPY 1
 
 /* Define to 1 if you have the <stropts.h> header file. */
-/* #undef HAVE_STROPTS_H */
+#define HAVE_STROPTS_H 1
 
 /* Define to 1 if you have the `strsignal' function. */
-#define HAVE_STRSIGNAL 1
+/* #undef HAVE_STRSIGNAL */
 
 /* Define to 1 if `pw_gecos' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_GECOS 1
+/* #undef HAVE_STRUCT_PASSWD_PW_GECOS */
 
 /* Define to 1 if `pw_passwd' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_PASSWD 1
+/* #undef HAVE_STRUCT_PASSWD_PW_PASSWD */
 
 /* Define to 1 if `st_birthtime' is a member of `struct stat'. */
 /* #undef HAVE_STRUCT_STAT_ST_BIRTHTIME */
 
 /* Define to 1 if `st_blksize' is a member of `struct stat'. */
 #define HAVE_STRUCT_STAT_ST_BLKSIZE 1
 
@@ -1083,40 +1097,43 @@
 /* Define if you have the 'symlink' function. */
 #define HAVE_SYMLINK 1
 
 /* Define to 1 if you have the `symlinkat' function. */
 #define HAVE_SYMLINKAT 1
 
 /* Define to 1 if you have the `sync' function. */
-#define HAVE_SYNC 1
+/* #undef HAVE_SYNC */
 
 /* Define to 1 if you have the `sysconf' function. */
 #define HAVE_SYSCONF 1
 
 /* Define to 1 if you have the <sysexits.h> header file. */
 #define HAVE_SYSEXITS_H 1
 
 /* Define to 1 if you have the <sys/audioio.h> header file. */
 /* #undef HAVE_SYS_AUDIOIO_H */
 
+/* Define to 1 if you have the <sys/auxv.h> header file. */
+/* #undef HAVE_SYS_AUXV_H */
+
 /* Define to 1 if you have the <sys/bsdtty.h> header file. */
 /* #undef HAVE_SYS_BSDTTY_H */
 
 /* Define to 1 if you have the <sys/devpoll.h> header file. */
 /* #undef HAVE_SYS_DEVPOLL_H */
 
 /* Define to 1 if you have the <sys/dir.h> header file, and it defines `DIR'.
-   */
+ */
 /* #undef HAVE_SYS_DIR_H */
 
 /* Define to 1 if you have the <sys/endian.h> header file. */
 /* #undef HAVE_SYS_ENDIAN_H */
 
 /* Define to 1 if you have the <sys/epoll.h> header file. */
-#define HAVE_SYS_EPOLL_H 1
+/* #undef HAVE_SYS_EPOLL_H */
 
 /* Define to 1 if you have the <sys/event.h> header file. */
 /* #undef HAVE_SYS_EVENT_H */
 
 /* Define to 1 if you have the <sys/file.h> header file. */
 #define HAVE_SYS_FILE_H 1
 
@@ -1141,15 +1158,15 @@
 /* Define to 1 if you have the <sys/mman.h> header file. */
 #define HAVE_SYS_MMAN_H 1
 
 /* Define to 1 if you have the <sys/modem.h> header file. */
 /* #undef HAVE_SYS_MODEM_H */
 
 /* Define to 1 if you have the <sys/ndir.h> header file, and it defines `DIR'.
-   */
+ */
 /* #undef HAVE_SYS_NDIR_H */
 
 /* Define to 1 if you have the <sys/param.h> header file. */
 #define HAVE_SYS_PARAM_H 1
 
 /* Define to 1 if you have the <sys/poll.h> header file. */
 #define HAVE_SYS_POLL_H 1
@@ -1160,30 +1177,30 @@
 /* Define to 1 if you have the <sys/resource.h> header file. */
 #define HAVE_SYS_RESOURCE_H 1
 
 /* Define to 1 if you have the <sys/select.h> header file. */
 #define HAVE_SYS_SELECT_H 1
 
 /* Define to 1 if you have the <sys/sendfile.h> header file. */
-#define HAVE_SYS_SENDFILE_H 1
+/* #undef HAVE_SYS_SENDFILE_H */
 
 /* Define to 1 if you have the <sys/socket.h> header file. */
 #define HAVE_SYS_SOCKET_H 1
 
 /* Define to 1 if you have the <sys/statvfs.h> header file. */
-#define HAVE_SYS_STATVFS_H 1
+/* #undef HAVE_SYS_STATVFS_H */
 
 /* Define to 1 if you have the <sys/stat.h> header file. */
 #define HAVE_SYS_STAT_H 1
 
 /* Define to 1 if you have the <sys/syscall.h> header file. */
 #define HAVE_SYS_SYSCALL_H 1
 
 /* Define to 1 if you have the <sys/sysmacros.h> header file. */
-#define HAVE_SYS_SYSMACROS_H 1
+/* #undef HAVE_SYS_SYSMACROS_H */
 
 /* Define to 1 if you have the <sys/sys_domain.h> header file. */
 /* #undef HAVE_SYS_SYS_DOMAIN_H */
 
 /* Define to 1 if you have the <sys/termio.h> header file. */
 /* #undef HAVE_SYS_TERMIO_H */
 
@@ -1202,51 +1219,51 @@
 /* Define to 1 if you have the <sys/un.h> header file. */
 #define HAVE_SYS_UN_H 1
 
 /* Define to 1 if you have the <sys/utsname.h> header file. */
 #define HAVE_SYS_UTSNAME_H 1
 
 /* Define to 1 if you have the <sys/wait.h> header file. */
-#define HAVE_SYS_WAIT_H 1
+/* #undef HAVE_SYS_WAIT_H */
 
 /* Define to 1 if you have the <sys/xattr.h> header file. */
-#define HAVE_SYS_XATTR_H 1
+/* #undef HAVE_SYS_XATTR_H */
 
 /* Define to 1 if you have the `tcgetpgrp' function. */
-#define HAVE_TCGETPGRP 1
+/* #undef HAVE_TCGETPGRP */
 
 /* Define to 1 if you have the `tcsetpgrp' function. */
-#define HAVE_TCSETPGRP 1
+/* #undef HAVE_TCSETPGRP */
 
 /* Define to 1 if you have the `tempnam' function. */
-#define HAVE_TEMPNAM 1
+/* #undef HAVE_TEMPNAM */
 
 /* Define to 1 if you have the <termios.h> header file. */
-#define HAVE_TERMIOS_H 1
+/* #undef HAVE_TERMIOS_H */
 
 /* Define to 1 if you have the <term.h> header file. */
 /* #undef HAVE_TERM_H */
 
 /* Define to 1 if you have the `tgamma' function. */
 #define HAVE_TGAMMA 1
 
 /* Define to 1 if you have the `timegm' function. */
 #define HAVE_TIMEGM 1
 
 /* Define to 1 if you have the `times' function. */
 #define HAVE_TIMES 1
 
 /* Define to 1 if you have the `tmpfile' function. */
-#define HAVE_TMPFILE 1
+/* #undef HAVE_TMPFILE */
 
 /* Define to 1 if you have the `tmpnam' function. */
-#define HAVE_TMPNAM 1
+/* #undef HAVE_TMPNAM */
 
 /* Define to 1 if you have the `tmpnam_r' function. */
-#define HAVE_TMPNAM_R 1
+/* #undef HAVE_TMPNAM_R */
 
 /* Define to 1 if your `struct tm' has `tm_zone'. Deprecated, use
    `HAVE_STRUCT_TM_TM_ZONE' instead. */
 #define HAVE_TM_ZONE 1
 
 /* Define to 1 if you have the `truncate' function. */
 #define HAVE_TRUNCATE 1
@@ -1263,30 +1280,27 @@
 
 /* Define to 1 if you have the <unistd.h> header file. */
 #define HAVE_UNISTD_H 1
 
 /* Define to 1 if you have the `unlinkat' function. */
 #define HAVE_UNLINKAT 1
 
-/* Define to 1 if you have the `unsetenv' function. */
-#define HAVE_UNSETENV 1
-
 /* Define if you have a useable wchar_t type defined in wchar.h; useable means
    wchar_t must be an unsigned type with at least 16 bits. (see
    Include/unicodeobject.h). */
 /* #undef HAVE_USABLE_WCHAR_T */
 
 /* Define to 1 if you have the <util.h> header file. */
 /* #undef HAVE_UTIL_H */
 
 /* Define to 1 if you have the `utimensat' function. */
 #define HAVE_UTIMENSAT 1
 
 /* Define to 1 if you have the `utimes' function. */
-#define HAVE_UTIMES 1
+/* #undef HAVE_UTIMES */
 
 /* Define to 1 if you have the <utime.h> header file. */
 #define HAVE_UTIME_H 1
 
 /* Define if uuid_create() exists. */
 /* #undef HAVE_UUID_CREATE */
 
@@ -1299,24 +1313,24 @@
 /* Define to 1 if you have the <uuid.h> header file. */
 /* #undef HAVE_UUID_H */
 
 /* Define to 1 if you have the <uuid/uuid.h> header file. */
 /* #undef HAVE_UUID_UUID_H */
 
 /* Define to 1 if you have the `wait3' function. */
-#define HAVE_WAIT3 1
+/* #undef HAVE_WAIT3 */
 
 /* Define to 1 if you have the `wait4' function. */
-#define HAVE_WAIT4 1
+/* #undef HAVE_WAIT4 */
 
 /* Define to 1 if you have the `waitid' function. */
-#define HAVE_WAITID 1
+/* #undef HAVE_WAITID */
 
 /* Define to 1 if you have the `waitpid' function. */
-#define HAVE_WAITPID 1
+/* #undef HAVE_WAITPID */
 
 /* Define if the compiler provides a wchar.h header file. */
 #define HAVE_WCHAR_H 1
 
 /* Define to 1 if you have the `wcscoll' function. */
 #define HAVE_WCSCOLL 1
 
@@ -1326,36 +1340,36 @@
 /* Define to 1 if you have the `wcsxfrm' function. */
 #define HAVE_WCSXFRM 1
 
 /* Define to 1 if you have the `wmemcmp' function. */
 #define HAVE_WMEMCMP 1
 
 /* Define if tzset() actually switches the local timezone in a meaningful way.
-   */
-#define HAVE_WORKING_TZSET 1
+ */
+/* #undef HAVE_WORKING_TZSET */
 
 /* Define to 1 if you have the `writev' function. */
 #define HAVE_WRITEV 1
 
 /* Define if libssl has X509_VERIFY_PARAM_set1_host and related function */
 /* #undef HAVE_X509_VERIFY_PARAM_SET1_HOST */
 
 /* Define if the zlib library has inflateCopy */
-#define HAVE_ZLIB_COPY 1
+/* #undef HAVE_ZLIB_COPY */
 
 /* Define to 1 if you have the `_getpty' function. */
 /* #undef HAVE__GETPTY */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in <mkdev.h>.
-   */
+ */
 /* #undef MAJOR_IN_MKDEV */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in
    <sysmacros.h>. */
-#define MAJOR_IN_SYSMACROS 1
+/* #undef MAJOR_IN_SYSMACROS */
 
 /* Define if mvwdelch in curses.h is an expression. */
 /* #undef MVWDELCH_IS_EXPRESSION */
 
 /* Define to the address where bug reports for this package should be sent. */
 /* #undef PACKAGE_BUGREPORT */
 
@@ -1374,22 +1388,25 @@
 /* Define to the version of this package. */
 /* #undef PACKAGE_VERSION */
 
 /* Define if POSIX semaphores aren't enabled on your system */
 /* #undef POSIX_SEMAPHORES_NOT_ENABLED */
 
 /* Define if pthread_key_t is compatible with int. */
-#define PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT 1
+/* #undef PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT */
 
 /* Defined if PTHREAD_SCOPE_SYSTEM supported. */
-#define PTHREAD_SYSTEM_SCHED_SUPPORTED 1
+/* #undef PTHREAD_SYSTEM_SCHED_SUPPORTED */
 
 /* Define as the preferred size in bits of long digits */
 /* #undef PYLONG_BITS_IN_DIGIT */
 
+/* enabled builtin hash modules */
+#define PY_BUILTIN_HASHLIB_HASHES "md5,sha1,sha256,sha512,sha3,blake2"
+
 /* Define if you want to coerce the C locale to a UTF-8 based locale */
 #define PY_COERCE_C_LOCALE 1
 
 /* Define to printf format modifier for Py_ssize_t */
 #define PY_FORMAT_SIZE_T "z"
 
 /* Default cipher suites list for ssl module. 1: Python's preferred selection,
@@ -1433,15 +1450,15 @@
 /* The size of `fpos_t', as computed by sizeof. */
 #define SIZEOF_FPOS_T 16
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
-#define SIZEOF_LONG 8
+#define SIZEOF_LONG 4
 
 /* The size of `long double', as computed by sizeof. */
 #define SIZEOF_LONG_DOUBLE 16
 
 /* The size of `long long', as computed by sizeof. */
 #define SIZEOF_LONG_LONG 8
 
@@ -1451,30 +1468,30 @@
 /* The size of `pid_t', as computed by sizeof. */
 #define SIZEOF_PID_T 4
 
 /* The size of `pthread_key_t', as computed by sizeof. */
 #define SIZEOF_PTHREAD_KEY_T 4
 
 /* The size of `pthread_t', as computed by sizeof. */
-#define SIZEOF_PTHREAD_T 8
+#define SIZEOF_PTHREAD_T 4
 
 /* The size of `short', as computed by sizeof. */
 #define SIZEOF_SHORT 2
 
 /* The size of `size_t', as computed by sizeof. */
 #define SIZEOF_SIZE_T 8
 
 /* The size of `time_t', as computed by sizeof. */
 #define SIZEOF_TIME_T 8
 
 /* The size of `uintptr_t', as computed by sizeof. */
-#define SIZEOF_UINTPTR_T 8
+#define SIZEOF_UINTPTR_T 4
 
 /* The size of `void *', as computed by sizeof. */
-#define SIZEOF_VOID_P 8
+#define SIZEOF_VOID_P 4
 
 /* The size of `wchar_t', as computed by sizeof. */
 #define SIZEOF_WCHAR_T 4
 
 /* The size of `_Bool', as computed by sizeof. */
 #define SIZEOF__BOOL 1
 
@@ -1495,34 +1512,33 @@
 /* #undef TM_IN_SYS_TIME */
 
 /* Define if you want to use computed gotos in ceval.c. */
 /* #undef USE_COMPUTED_GOTOS */
 
 /* Enable extensions on AIX 3, Interix.  */
 #ifndef _ALL_SOURCE
-# define _ALL_SOURCE 1
+#define _ALL_SOURCE 1
 #endif
 /* Enable GNU extensions on systems that have them.  */
 #ifndef _GNU_SOURCE
-# define _GNU_SOURCE 1
+#define _GNU_SOURCE 1
 #endif
 /* Enable threading extensions on Solaris.  */
 #ifndef _POSIX_PTHREAD_SEMANTICS
-# define _POSIX_PTHREAD_SEMANTICS 1
+#define _POSIX_PTHREAD_SEMANTICS 1
 #endif
 /* Enable extensions on HP NonStop.  */
 #ifndef _TANDEM_SOURCE
-# define _TANDEM_SOURCE 1
+#define _TANDEM_SOURCE 1
 #endif
 /* Enable general extensions on Solaris.  */
 #ifndef __EXTENSIONS__
-# define __EXTENSIONS__ 1
+#define __EXTENSIONS__ 1
 #endif
 
-
 /* Define if WINDOW in curses.h offers a field _flags. */
 /* #undef WINDOW_HAS_FLAGS */
 
 /* Define if you want build the _decimal module using a coroutine-local rather
    than a thread-local context */
 #define WITH_DECIMAL_CONTEXTVAR 1
 
@@ -1549,21 +1565,21 @@
 
 /* Define if you want pymalloc to be disabled when running under valgrind */
 /* #undef WITH_VALGRIND */
 
 /* Define WORDS_BIGENDIAN to 1 if your processor stores words with the most
    significant byte first (like Motorola and SPARC, unlike Intel). */
 #if defined AC_APPLE_UNIVERSAL_BUILD
-# if defined __BIG_ENDIAN__
-#  define WORDS_BIGENDIAN 1
-# endif
+#if defined __BIG_ENDIAN__
+#define WORDS_BIGENDIAN 1
+#endif
 #else
-# ifndef WORDS_BIGENDIAN
+#ifndef WORDS_BIGENDIAN
 /* #  undef WORDS_BIGENDIAN */
-# endif
+#endif
 #endif
 
 /* Define if arithmetic is subject to x87-style double rounding issue */
 /* #undef X87_DOUBLE_ROUNDING */
 
 /* Define on OpenBSD to activate all library features */
 /* #undef _BSD_SOURCE */
@@ -1616,19 +1632,14 @@
 
 /* Define to activate Unix95-and-earlier features */
 #define _XOPEN_SOURCE_EXTENDED 1
 
 /* Define on FreeBSD to activate all library features */
 #define __BSD_VISIBLE 1
 
-/* Define to 1 if type `char' is unsigned and you are not using gcc.  */
-#ifndef __CHAR_UNSIGNED__
-/* # undef __CHAR_UNSIGNED__ */
-#endif
-
 /* Define to 'long' if <time.h> doesn't define. */
 /* #undef clock_t */
 
 /* Define to empty if `const' does not conform to ANSI C. */
 /* #undef const */
 
 /* Define to `int' if <sys/types.h> doesn't define. */
@@ -1651,15 +1662,13 @@
 
 /* Define to `int' if <sys/socket.h> does not define. */
 /* #undef socklen_t */
 
 /* Define to `int' if <sys/types.h> doesn't define. */
 /* #undef uid_t */
 
-
 /* Define the macros needed if on a UnixWare 7.x system. */
 #if defined(__USLC__) && defined(__SCO_VERSION__)
 #define STRICT_SYSV_CURSES /* Don't use ncurses extensions */
 #endif
 
 #endif /*Py_PYCONFIG_H*/
-
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyctype.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydebug.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.d` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyexpat.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacro.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymath.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pyport.h`

 * *Files 1% similar despite different names*

```diff
@@ -645,15 +645,15 @@
 #       define HAVE_DECLSPEC_DLL
 #endif
 
 /* only get special linkage if built as shared or platform is Cygwin */
 #if defined(Py_ENABLE_SHARED) || defined(__CYGWIN__)
 #       if defined(HAVE_DECLSPEC_DLL)
 #               if defined(Py_BUILD_CORE) && !defined(Py_BUILD_CORE_MODULE)
-#                       define PyAPI_FUNC(RTYPE) __declspec(dllexport) RTYPE
+#                       define PyAPI_FUNC(RTYPE) __attribute__((visibility ("default"), import_module ("capi"))) RTYPE
 #                       define PyAPI_DATA(RTYPE) extern __declspec(dllexport) RTYPE
         /* module init functions inside the core need no external linkage */
         /* except for Cygwin to handle embedding */
 #                       if defined(__CYGWIN__)
 #                               define PyMODINIT_FUNC __declspec(dllexport) PyObject*
 #                       else /* __CYGWIN__ */
 #                               define PyMODINIT_FUNC PyObject*
@@ -661,30 +661,30 @@
 #               else /* Py_BUILD_CORE */
         /* Building an extension module, or an embedded situation */
         /* public Python functions and data are imported */
         /* Under Cygwin, auto-import functions to prevent compilation */
         /* failures similar to those described at the bottom of 4.1: */
         /* http://docs.python.org/extending/windows.html#a-cookbook-approach */
 #                       if !defined(__CYGWIN__)
-#                               define PyAPI_FUNC(RTYPE) __declspec(dllimport) RTYPE
+#                               define PyAPI_FUNC(RTYPE) __attribute__((visibility ("default"), import_module ("capi"))) RTYPE
 #                       endif /* !__CYGWIN__ */
 #                       define PyAPI_DATA(RTYPE) extern __declspec(dllimport) RTYPE
         /* module init functions outside the core must be exported */
 #                       if defined(__cplusplus)
 #                               define PyMODINIT_FUNC extern "C" __declspec(dllexport) PyObject*
 #                       else /* __cplusplus */
 #                               define PyMODINIT_FUNC __declspec(dllexport) PyObject*
 #                       endif /* __cplusplus */
 #               endif /* Py_BUILD_CORE */
 #       endif /* HAVE_DECLSPEC_DLL */
 #endif /* Py_ENABLE_SHARED */
 
 /* If no external linkage macros defined by now, create defaults */
 #ifndef PyAPI_FUNC
-#       define PyAPI_FUNC(RTYPE) RTYPE
+#       define PyAPI_FUNC(RTYPE) __attribute__((visibility ("default"), import_module ("capi"))) RTYPE
 #endif
 #ifndef PyAPI_DATA
 #       define PyAPI_DATA(RTYPE) extern RTYPE
 #endif
 #ifndef PyMODINIT_FUNC
 #       if defined(__cplusplus)
 #               define PyMODINIT_FUNC extern "C" PyObject*
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrhex.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrtod.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythread.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pytime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/rangeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/setobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/sliceobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/structmember.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/structseq.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/symtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/token.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/tracemalloc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/typeslots.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ucnhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp38/weakrefobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp38/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/LICENSE` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python-ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/asdl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ast.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/boolobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cellobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/classobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/codecs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/compile.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/complexobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/abstract.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytesobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/frameobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/datetime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/descrobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/dictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/dynamic_annotations.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/errcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/eval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/exports.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/floatobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/funcobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/genobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/graminit.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/grammar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/import.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pegen_interface.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pegen_interface.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_accu.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_atomic.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_byteswap.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_call.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_ceval.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_code.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_condvar.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_context.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gil.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hamt.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_interp.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_long.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_runtime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/intrcheck.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/iterobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/listobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/longintrepr.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/longobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/marshal.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/memoryobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/methodobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/modsupport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/moduleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/node.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/object.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/objimpl.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/odictobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/opcode.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/osdefs.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/parsetok.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/patchlevel.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/picklebufobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/py_curses.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyarena.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pycapsule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyconfig.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 /* pyconfig.h.  Generated from pyconfig.h.in by configure.  */
 /* pyconfig.h.in.  Generated from configure.ac by autoheader.  */
 
-
 #ifndef Py_PYCONFIG_H
 #define Py_PYCONFIG_H
 
-
 /* Define if building universal (internal helper macro) */
 /* #undef AC_APPLE_UNIVERSAL_BUILD */
 
 /* BUILD_GNU_TYPE + AIX_BUILDDATE are used to construct the PEP425 tag of the
    build system. */
 /* #undef AIX_BUILDDATE */
 
@@ -33,15 +31,15 @@
 /* #undef DOUBLE_IS_BIG_ENDIAN_IEEE754 */
 
 /* Define if C doubles are 64-bit IEEE 754 binary format, stored with the
    least significant byte first */
 #define DOUBLE_IS_LITTLE_ENDIAN_IEEE754 1
 
 /* Define if --enable-ipv6 is specified */
-#define ENABLE_IPV6 1
+/* #undef ENABLE_IPV6 */
 
 /* Define to 1 if your system stores words within floats with the most
    significant word first */
 /* #undef FLOAT_WORDS_BIGENDIAN */
 
 /* Define if flock needs to be linked with bsd library. */
 /* #undef FLOCK_NEEDS_LIBBSD */
@@ -52,15 +50,15 @@
 /* Define to 1 if you have the `accept4' function. */
 #define HAVE_ACCEPT4 1
 
 /* Define to 1 if you have the `acosh' function. */
 #define HAVE_ACOSH 1
 
 /* struct addrinfo (netdb.h) */
-#define HAVE_ADDRINFO 1
+/* #undef HAVE_ADDRINFO */
 
 /* Define to 1 if you have the `alarm' function. */
 #define HAVE_ALARM 1
 
 /* Define if aligned memory access is required */
 /* #undef HAVE_ALIGNED_REQUIRED */
 
@@ -70,15 +68,15 @@
 /* Define this if your time.h defines altzone. */
 /* #undef HAVE_ALTZONE */
 
 /* Define to 1 if you have the `asinh' function. */
 #define HAVE_ASINH 1
 
 /* Define to 1 if you have the <asm/types.h> header file. */
-#define HAVE_ASM_TYPES_H 1
+/* #undef HAVE_ASM_TYPES_H */
 
 /* Define to 1 if you have the `atanh' function. */
 #define HAVE_ATANH 1
 
 /* Define to 1 if you have the `bind_textdomain_codeset' function. */
 #define HAVE_BIND_TEXTDOMAIN_CODESET 1
 
@@ -201,171 +199,171 @@
 /* #undef HAVE_CURSES_WCHGAT */
 
 /* Define to 1 if you have the declaration of `isfinite', and to 0 if you
    don't. */
 #define HAVE_DECL_ISFINITE 1
 
 /* Define to 1 if you have the declaration of `isinf', and to 0 if you don't.
-   */
+ */
 #define HAVE_DECL_ISINF 1
 
 /* Define to 1 if you have the declaration of `isnan', and to 0 if you don't.
-   */
+ */
 #define HAVE_DECL_ISNAN 1
 
 /* Define to 1 if you have the declaration of `RTLD_DEEPBIND', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_DEEPBIND 1
+/* #undef HAVE_DECL_RTLD_DEEPBIND */
 
 /* Define to 1 if you have the declaration of `RTLD_GLOBAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_GLOBAL 1
+/* #undef HAVE_DECL_RTLD_GLOBAL */
 
 /* Define to 1 if you have the declaration of `RTLD_LAZY', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LAZY 1
+/* #undef HAVE_DECL_RTLD_LAZY */
 
 /* Define to 1 if you have the declaration of `RTLD_LOCAL', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_LOCAL 1
+/* #undef HAVE_DECL_RTLD_LOCAL */
 
 /* Define to 1 if you have the declaration of `RTLD_MEMBER', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_MEMBER 0
+/* #undef HAVE_DECL_RTLD_MEMBER */
 
 /* Define to 1 if you have the declaration of `RTLD_NODELETE', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NODELETE 1
+/* #undef HAVE_DECL_RTLD_NODELETE */
 
 /* Define to 1 if you have the declaration of `RTLD_NOLOAD', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOLOAD 1
+/* #undef HAVE_DECL_RTLD_NOLOAD */
 
 /* Define to 1 if you have the declaration of `RTLD_NOW', and to 0 if you
    don't. */
-#define HAVE_DECL_RTLD_NOW 1
+/* #undef HAVE_DECL_RTLD_NOW */
 
 /* Define to 1 if you have the declaration of `tzname', and to 0 if you don't.
-   */
+ */
 /* #undef HAVE_DECL_TZNAME */
 
 /* Define to 1 if you have the device macros. */
-#define HAVE_DEVICE_MACROS 1
+/* #undef HAVE_DEVICE_MACROS */
 
 /* Define to 1 if you have the /dev/ptc device file. */
 /* #undef HAVE_DEV_PTC */
 
 /* Define to 1 if you have the /dev/ptmx device file. */
-#define HAVE_DEV_PTMX 1
+/* #undef HAVE_DEV_PTMX */
 
 /* Define to 1 if you have the <direct.h> header file. */
 /* #undef HAVE_DIRECT_H */
 
 /* Define to 1 if the dirent structure has a d_type field */
 #define HAVE_DIRENT_D_TYPE 1
 
 /* Define to 1 if you have the <dirent.h> header file, and it defines `DIR'.
-   */
+ */
 #define HAVE_DIRENT_H 1
 
 /* Define if you have the 'dirfd' function or macro. */
 #define HAVE_DIRFD 1
 
 /* Define to 1 if you have the <dlfcn.h> header file. */
-#define HAVE_DLFCN_H 1
+/* #undef HAVE_DLFCN_H */
 
 /* Define to 1 if you have the `dlopen' function. */
-#define HAVE_DLOPEN 1
+/* #undef HAVE_DLOPEN */
 
 /* Define to 1 if you have the `dup2' function. */
-#define HAVE_DUP2 1
+/* #undef HAVE_DUP2 */
 
 /* Define to 1 if you have the `dup3' function. */
-#define HAVE_DUP3 1
+/* #undef HAVE_DUP3 */
 
 /* Define if you have the '_dyld_shared_cache_contains_path' function. */
 /* #undef HAVE_DYLD_SHARED_CACHE_CONTAINS_PATH */
 
 /* Defined when any dynamic module loading is enabled. */
 #define HAVE_DYNAMIC_LOADING 1
 
 /* Define to 1 if you have the <endian.h> header file. */
 #define HAVE_ENDIAN_H 1
 
 /* Define if you have the 'epoll' functions. */
-#define HAVE_EPOLL 1
+/* #undef HAVE_EPOLL */
 
 /* Define if you have the 'epoll_create1' function. */
-#define HAVE_EPOLL_CREATE1 1
+/* #undef HAVE_EPOLL_CREATE1 */
 
 /* Define to 1 if you have the `erf' function. */
 #define HAVE_ERF 1
 
 /* Define to 1 if you have the `erfc' function. */
 #define HAVE_ERFC 1
 
 /* Define to 1 if you have the <errno.h> header file. */
 #define HAVE_ERRNO_H 1
 
 /* Define to 1 if you have the `execv' function. */
-#define HAVE_EXECV 1
+/* #undef HAVE_EXECV */
 
 /* Define to 1 if you have the `explicit_bzero' function. */
 #define HAVE_EXPLICIT_BZERO 1
 
 /* Define to 1 if you have the `explicit_memset' function. */
 /* #undef HAVE_EXPLICIT_MEMSET */
 
 /* Define to 1 if you have the `expm1' function. */
 #define HAVE_EXPM1 1
 
 /* Define to 1 if you have the `faccessat' function. */
 #define HAVE_FACCESSAT 1
 
 /* Define if you have the 'fchdir' function. */
-#define HAVE_FCHDIR 1
+/* #undef HAVE_FCHDIR */
 
 /* Define to 1 if you have the `fchmod' function. */
-#define HAVE_FCHMOD 1
+/* #undef HAVE_FCHMOD */
 
 /* Define to 1 if you have the `fchmodat' function. */
-#define HAVE_FCHMODAT 1
+/* #undef HAVE_FCHMODAT */
 
 /* Define to 1 if you have the `fchown' function. */
-#define HAVE_FCHOWN 1
+/* #undef HAVE_FCHOWN */
 
 /* Define to 1 if you have the `fchownat' function. */
-#define HAVE_FCHOWNAT 1
+/* #undef HAVE_FCHOWNAT */
 
 /* Define to 1 if you have the <fcntl.h> header file. */
 #define HAVE_FCNTL_H 1
 
 /* Define if you have the 'fdatasync' function. */
 #define HAVE_FDATASYNC 1
 
 /* Define to 1 if you have the `fdopendir' function. */
 #define HAVE_FDOPENDIR 1
 
 /* Define to 1 if you have the `fdwalk' function. */
 /* #undef HAVE_FDWALK */
 
 /* Define to 1 if you have the `fexecve' function. */
-#define HAVE_FEXECVE 1
+/* #undef HAVE_FEXECVE */
 
 /* Define to 1 if you have the `finite' function. */
 #define HAVE_FINITE 1
 
 /* Define to 1 if you have the `flock' function. */
-#define HAVE_FLOCK 1
+/* #undef HAVE_FLOCK */
 
 /* Define to 1 if you have the `fork' function. */
-#define HAVE_FORK 1
+/* #undef HAVE_FORK */
 
 /* Define to 1 if you have the `forkpty' function. */
-#define HAVE_FORKPTY 1
+/* #undef HAVE_FORKPTY */
 
 /* Define to 1 if you have the `fpathconf' function. */
 #define HAVE_FPATHCONF 1
 
 /* Define to 1 if you have the `fseek64' function. */
 /* #undef HAVE_FSEEK64 */
 
@@ -393,332 +391,332 @@
 /* Define to 1 if you have the `ftruncate' function. */
 #define HAVE_FTRUNCATE 1
 
 /* Define to 1 if you have the `futimens' function. */
 #define HAVE_FUTIMENS 1
 
 /* Define to 1 if you have the `futimes' function. */
-#define HAVE_FUTIMES 1
+/* #undef HAVE_FUTIMES */
 
 /* Define to 1 if you have the `futimesat' function. */
-#define HAVE_FUTIMESAT 1
+/* #undef HAVE_FUTIMESAT */
 
 /* Define to 1 if you have the `gai_strerror' function. */
-#define HAVE_GAI_STRERROR 1
+/* #undef HAVE_GAI_STRERROR */
 
 /* Define to 1 if you have the `gamma' function. */
-#define HAVE_GAMMA 1
+/* #undef HAVE_GAMMA */
 
 /* Define if we can use gcc inline assembler to get and set mc68881 fpcr */
 /* #undef HAVE_GCC_ASM_FOR_MC68881 */
 
 /* Define if we can use x64 gcc inline assembler */
-#define HAVE_GCC_ASM_FOR_X64 1
+/* #undef HAVE_GCC_ASM_FOR_X64 */
 
 /* Define if we can use gcc inline assembler to get and set x87 control word
-   */
-#define HAVE_GCC_ASM_FOR_X87 1
+ */
+/* #undef HAVE_GCC_ASM_FOR_X87 */
 
 /* Define if your compiler provides __uint128_t */
 #define HAVE_GCC_UINT128_T 1
 
 /* Define if you have the getaddrinfo function. */
-#define HAVE_GETADDRINFO 1
+/* #undef HAVE_GETADDRINFO */
 
 /* Define this if you have flockfile(), getc_unlocked(), and funlockfile() */
-#define HAVE_GETC_UNLOCKED 1
+/* #undef HAVE_GETC_UNLOCKED */
 
 /* Define to 1 if you have the `getentropy' function. */
 #define HAVE_GETENTROPY 1
 
 /* Define to 1 if you have the `getgrgid_r' function. */
-#define HAVE_GETGRGID_R 1
+/* #undef HAVE_GETGRGID_R */
 
 /* Define to 1 if you have the `getgrnam_r' function. */
-#define HAVE_GETGRNAM_R 1
+/* #undef HAVE_GETGRNAM_R */
 
 /* Define to 1 if you have the `getgrouplist' function. */
-#define HAVE_GETGROUPLIST 1
+/* #undef HAVE_GETGROUPLIST */
 
 /* Define to 1 if you have the `getgroups' function. */
-#define HAVE_GETGROUPS 1
+/* #undef HAVE_GETGROUPS */
 
 /* Define to 1 if you have the `gethostbyname' function. */
 /* #undef HAVE_GETHOSTBYNAME */
 
 /* Define this if you have some version of gethostbyname_r() */
-#define HAVE_GETHOSTBYNAME_R 1
+/* #undef HAVE_GETHOSTBYNAME_R */
 
 /* Define this if you have the 3-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_3_ARG */
 
 /* Define this if you have the 5-arg version of gethostbyname_r(). */
 /* #undef HAVE_GETHOSTBYNAME_R_5_ARG */
 
 /* Define this if you have the 6-arg version of gethostbyname_r(). */
-#define HAVE_GETHOSTBYNAME_R_6_ARG 1
+/* #undef HAVE_GETHOSTBYNAME_R_6_ARG */
 
 /* Define to 1 if you have the `getitimer' function. */
-#define HAVE_GETITIMER 1
+/* #undef HAVE_GETITIMER */
 
 /* Define to 1 if you have the `getloadavg' function. */
-#define HAVE_GETLOADAVG 1
+/* #undef HAVE_GETLOADAVG */
 
 /* Define to 1 if you have the `getlogin' function. */
-#define HAVE_GETLOGIN 1
+/* #undef HAVE_GETLOGIN */
 
 /* Define to 1 if you have the `getnameinfo' function. */
-#define HAVE_GETNAMEINFO 1
+/* #undef HAVE_GETNAMEINFO */
 
 /* Define if you have the 'getpagesize' function. */
-#define HAVE_GETPAGESIZE 1
+/* #undef HAVE_GETPAGESIZE */
 
 /* Define to 1 if you have the `getpeername' function. */
-#define HAVE_GETPEERNAME 1
+/* #undef HAVE_GETPEERNAME */
 
 /* Define to 1 if you have the `getpgid' function. */
-#define HAVE_GETPGID 1
+/* #undef HAVE_GETPGID */
 
 /* Define to 1 if you have the `getpgrp' function. */
-#define HAVE_GETPGRP 1
+/* #undef HAVE_GETPGRP */
 
 /* Define to 1 if you have the `getpid' function. */
-#define HAVE_GETPID 1
+/* #undef HAVE_GETPID */
 
 /* Define to 1 if you have the `getpriority' function. */
-#define HAVE_GETPRIORITY 1
+/* #undef HAVE_GETPRIORITY */
 
 /* Define to 1 if you have the `getpwent' function. */
-#define HAVE_GETPWENT 1
+/* #undef HAVE_GETPWENT */
 
 /* Define to 1 if you have the `getpwnam_r' function. */
-#define HAVE_GETPWNAM_R 1
+/* #undef HAVE_GETPWNAM_R */
 
 /* Define to 1 if you have the `getpwuid_r' function. */
-#define HAVE_GETPWUID_R 1
+/* #undef HAVE_GETPWUID_R */
 
 /* Define to 1 if the getrandom() function is available */
-#define HAVE_GETRANDOM 1
+/* #undef HAVE_GETRANDOM */
 
 /* Define to 1 if the Linux getrandom() syscall is available */
-#define HAVE_GETRANDOM_SYSCALL 1
+/* #undef HAVE_GETRANDOM_SYSCALL */
 
 /* Define to 1 if you have the `getresgid' function. */
-#define HAVE_GETRESGID 1
+/* #undef HAVE_GETRESGID */
 
 /* Define to 1 if you have the `getresuid' function. */
-#define HAVE_GETRESUID 1
+/* #undef HAVE_GETRESUID */
 
 /* Define to 1 if you have the `getsid' function. */
-#define HAVE_GETSID 1
+/* #undef HAVE_GETSID */
 
 /* Define to 1 if you have the `getspent' function. */
-#define HAVE_GETSPENT 1
+/* #undef HAVE_GETSPENT */
 
 /* Define to 1 if you have the `getspnam' function. */
-#define HAVE_GETSPNAM 1
+/* #undef HAVE_GETSPNAM */
 
 /* Define to 1 if you have the `getwd' function. */
-#define HAVE_GETWD 1
+/* #undef HAVE_GETWD */
 
 /* Define if glibc has incorrect _FORTIFY_SOURCE wrappers for memmove and
    bcopy. */
 /* #undef HAVE_GLIBC_MEMMOVE_BUG */
 
 /* Define to 1 if you have the <grp.h> header file. */
-#define HAVE_GRP_H 1
+/* #undef HAVE_GRP_H */
 
 /* Define if you have the 'hstrerror' function. */
-#define HAVE_HSTRERROR 1
+/* #undef HAVE_HSTRERROR */
 
 /* Define this if you have le64toh() */
 #define HAVE_HTOLE64 1
 
 /* Define to 1 if you have the `hypot' function. */
 #define HAVE_HYPOT 1
 
 /* Define to 1 if you have the <ieeefp.h> header file. */
 /* #undef HAVE_IEEEFP_H */
 
 /* Define to 1 if you have the `if_nameindex' function. */
-#define HAVE_IF_NAMEINDEX 1
+/* #undef HAVE_IF_NAMEINDEX */
 
 /* Define if you have the 'inet_aton' function. */
 #define HAVE_INET_ATON 1
 
 /* Define if you have the 'inet_pton' function. */
 #define HAVE_INET_PTON 1
 
 /* Define to 1 if you have the `initgroups' function. */
-#define HAVE_INITGROUPS 1
+/* #undef HAVE_INITGROUPS */
 
 /* Define to 1 if you have the <inttypes.h> header file. */
 #define HAVE_INTTYPES_H 1
 
 /* Define to 1 if you have the <io.h> header file. */
 /* #undef HAVE_IO_H */
 
 /* Define if gcc has the ipa-pure-const bug. */
 /* #undef HAVE_IPA_PURE_CONST_BUG */
 
 /* Define to 1 if you have the `kill' function. */
-#define HAVE_KILL 1
+/* #undef HAVE_KILL */
 
 /* Define to 1 if you have the `killpg' function. */
-#define HAVE_KILLPG 1
+/* #undef HAVE_KILLPG */
 
 /* Define if you have the 'kqueue' functions. */
 /* #undef HAVE_KQUEUE */
 
 /* Define to 1 if you have the <langinfo.h> header file. */
 #define HAVE_LANGINFO_H 1
 
 /* Defined to enable large file support when an off_t is bigger than a long
    and long long is at least as big as an off_t. You may need to add some
    flags for configuration and compilation to enable this mode. (For Solaris
    and Linux, the necessary defines are already defined.) */
-/* #undef HAVE_LARGEFILE_SUPPORT */
+#define HAVE_LARGEFILE_SUPPORT 1
 
 /* Define to 1 if you have the 'lchflags' function. */
 /* #undef HAVE_LCHFLAGS */
 
 /* Define to 1 if you have the `lchmod' function. */
 /* #undef HAVE_LCHMOD */
 
 /* Define to 1 if you have the `lchown' function. */
-#define HAVE_LCHOWN 1
+/* #undef HAVE_LCHOWN */
 
 /* Define to 1 if you have the `lgamma' function. */
 #define HAVE_LGAMMA 1
 
 /* Define to 1 if you have the `dl' library (-ldl). */
 #define HAVE_LIBDL 1
 
 /* Define to 1 if you have the `dld' library (-ldld). */
 /* #undef HAVE_LIBDLD */
 
 /* Define to 1 if you have the `ieee' library (-lieee). */
 /* #undef HAVE_LIBIEEE */
 
 /* Define to 1 if you have the <libintl.h> header file. */
-#define HAVE_LIBINTL_H 1
+/* #undef HAVE_LIBINTL_H */
 
 /* Define if you have the readline library (-lreadline). */
 /* #undef HAVE_LIBREADLINE */
 
 /* Define to 1 if you have the `resolv' library (-lresolv). */
-/* #undef HAVE_LIBRESOLV */
+#define HAVE_LIBRESOLV 1
 
 /* Define to 1 if you have the `sendfile' library (-lsendfile). */
 /* #undef HAVE_LIBSENDFILE */
 
 /* Define to 1 if you have the <libutil.h> header file. */
-/* #undef HAVE_LIBUTIL_H */
+#define HAVE_LIBUTIL_H 1
 
 /* Define to 1 if you have the `uuid' library (-luuid). */
 /* #undef HAVE_LIBUUID */
 
 /* Define if you have the 'link' function. */
 #define HAVE_LINK 1
 
 /* Define to 1 if you have the `linkat' function. */
 #define HAVE_LINKAT 1
 
 /* Define to 1 if you have the <linux/auxvec.h> header file. */
-#define HAVE_LINUX_AUXVEC_H 1
+/* #undef HAVE_LINUX_AUXVEC_H */
 
 /* Define to 1 if you have the <linux/can/bcm.h> header file. */
-#define HAVE_LINUX_CAN_BCM_H 1
+/* #undef HAVE_LINUX_CAN_BCM_H */
 
 /* Define to 1 if you have the <linux/can.h> header file. */
-#define HAVE_LINUX_CAN_H 1
+/* #undef HAVE_LINUX_CAN_H */
 
 /* Define to 1 if you have the <linux/can/j1939.h> header file. */
-#define HAVE_LINUX_CAN_J1939_H 1
+/* #undef HAVE_LINUX_CAN_J1939_H */
 
 /* Define if compiling using Linux 3.6 or later. */
-#define HAVE_LINUX_CAN_RAW_FD_FRAMES 1
+/* #undef HAVE_LINUX_CAN_RAW_FD_FRAMES */
 
 /* Define to 1 if you have the <linux/can/raw.h> header file. */
-#define HAVE_LINUX_CAN_RAW_H 1
+/* #undef HAVE_LINUX_CAN_RAW_H */
 
 /* Define if compiling using Linux 4.1 or later. */
-#define HAVE_LINUX_CAN_RAW_JOIN_FILTERS 1
+/* #undef HAVE_LINUX_CAN_RAW_JOIN_FILTERS */
 
 /* Define to 1 if you have the <linux/memfd.h> header file. */
-#define HAVE_LINUX_MEMFD_H 1
+/* #undef HAVE_LINUX_MEMFD_H */
 
 /* Define to 1 if you have the <linux/netlink.h> header file. */
-#define HAVE_LINUX_NETLINK_H 1
+/* #undef HAVE_LINUX_NETLINK_H */
 
 /* Define to 1 if you have the <linux/qrtr.h> header file. */
-#define HAVE_LINUX_QRTR_H 1
+/* #undef HAVE_LINUX_QRTR_H */
 
 /* Define to 1 if you have the <linux/random.h> header file. */
-#define HAVE_LINUX_RANDOM_H 1
+/* #undef HAVE_LINUX_RANDOM_H */
 
 /* Define to 1 if you have the <linux/tipc.h> header file. */
-#define HAVE_LINUX_TIPC_H 1
+/* #undef HAVE_LINUX_TIPC_H */
 
 /* Define to 1 if you have the <linux/vm_sockets.h> header file. */
-#define HAVE_LINUX_VM_SOCKETS_H 1
+/* #undef HAVE_LINUX_VM_SOCKETS_H */
 
 /* Define to 1 if you have the <linux/wait.h> header file. */
-#define HAVE_LINUX_WAIT_H 1
+/* #undef HAVE_LINUX_WAIT_H */
 
 /* Define to 1 if you have the `lockf' function. */
-#define HAVE_LOCKF 1
+/* #undef HAVE_LOCKF */
 
 /* Define to 1 if you have the `log1p' function. */
 #define HAVE_LOG1P 1
 
 /* Define to 1 if you have the `log2' function. */
 #define HAVE_LOG2 1
 
 /* Define to 1 if the system has the type `long double'. */
 #define HAVE_LONG_DOUBLE 1
 
 /* Define to 1 if you have the `lstat' function. */
 #define HAVE_LSTAT 1
 
 /* Define to 1 if you have the `lutimes' function. */
-#define HAVE_LUTIMES 1
+/* #undef HAVE_LUTIMES */
 
 /* Define to 1 if you have the `madvise' function. */
-#define HAVE_MADVISE 1
+/* #undef HAVE_MADVISE */
 
 /* Define this if you have the makedev macro. */
-#define HAVE_MAKEDEV 1
+/* #undef HAVE_MAKEDEV */
 
 /* Define to 1 if you have the `mbrtowc' function. */
 #define HAVE_MBRTOWC 1
 
 /* Define if you have the 'memfd_create' function. */
-#define HAVE_MEMFD_CREATE 1
+/* #undef HAVE_MEMFD_CREATE */
 
 /* Define to 1 if you have the <memory.h> header file. */
 #define HAVE_MEMORY_H 1
 
 /* Define to 1 if you have the `memrchr' function. */
 #define HAVE_MEMRCHR 1
 
 /* Define to 1 if you have the `mkdirat' function. */
 #define HAVE_MKDIRAT 1
 
 /* Define to 1 if you have the `mkfifo' function. */
-#define HAVE_MKFIFO 1
+/* #undef HAVE_MKFIFO */
 
 /* Define to 1 if you have the `mkfifoat' function. */
-#define HAVE_MKFIFOAT 1
+/* #undef HAVE_MKFIFOAT */
 
 /* Define to 1 if you have the `mknod' function. */
-#define HAVE_MKNOD 1
+/* #undef HAVE_MKNOD */
 
 /* Define to 1 if you have the `mknodat' function. */
-#define HAVE_MKNODAT 1
+/* #undef HAVE_MKNODAT */
 
 /* Define to 1 if you have the `mktime' function. */
 #define HAVE_MKTIME 1
 
 /* Define to 1 if you have the `mmap' function. */
 #define HAVE_MMAP 1
 
@@ -731,37 +729,37 @@
 /* Define to 1 if you have the <ndir.h> header file, and it defines `DIR'. */
 /* #undef HAVE_NDIR_H */
 
 /* Define to 1 if you have the <netpacket/packet.h> header file. */
 #define HAVE_NETPACKET_PACKET_H 1
 
 /* Define to 1 if you have the <net/if.h> header file. */
-#define HAVE_NET_IF_H 1
+/* #undef HAVE_NET_IF_H */
 
 /* Define to 1 if you have the `nice' function. */
-#define HAVE_NICE 1
+/* #undef HAVE_NICE */
 
 /* Define if the internal form of wchar_t in non-Unicode locales is not
    Unicode. */
 /* #undef HAVE_NON_UNICODE_WCHAR_T_REPRESENTATION */
 
 /* Define to 1 if you have the `openat' function. */
 #define HAVE_OPENAT 1
 
 /* Define to 1 if you have the `openpty' function. */
-#define HAVE_OPENPTY 1
+/* #undef HAVE_OPENPTY */
 
 /* Define to 1 if you have the `pathconf' function. */
 #define HAVE_PATHCONF 1
 
 /* Define to 1 if you have the `pause' function. */
-#define HAVE_PAUSE 1
+/* #undef HAVE_PAUSE */
 
 /* Define to 1 if you have the `pipe2' function. */
-#define HAVE_PIPE2 1
+/* #undef HAVE_PIPE2 */
 
 /* Define to 1 if you have the `plock' function. */
 /* #undef HAVE_PLOCK */
 
 /* Define to 1 if you have the `poll' function. */
 #define HAVE_POLL 1
 
@@ -771,30 +769,30 @@
 /* Define to 1 if you have the `posix_fadvise' function. */
 #define HAVE_POSIX_FADVISE 1
 
 /* Define to 1 if you have the `posix_fallocate' function. */
 #define HAVE_POSIX_FALLOCATE 1
 
 /* Define to 1 if you have the `posix_spawn' function. */
-#define HAVE_POSIX_SPAWN 1
+/* #undef HAVE_POSIX_SPAWN */
 
 /* Define to 1 if you have the `posix_spawnp' function. */
-#define HAVE_POSIX_SPAWNP 1
+/* #undef HAVE_POSIX_SPAWNP */
 
 /* Define to 1 if you have the `pread' function. */
 #define HAVE_PREAD 1
 
 /* Define to 1 if you have the `preadv' function. */
 #define HAVE_PREADV 1
 
 /* Define to 1 if you have the `preadv2' function. */
-#define HAVE_PREADV2 1
+/* #undef HAVE_PREADV2 */
 
 /* Define if you have the 'prlimit' functions. */
-#define HAVE_PRLIMIT 1
+/* #undef HAVE_PRLIMIT */
 
 /* Define to 1 if you have the <process.h> header file. */
 /* #undef HAVE_PROCESS_H */
 
 /* Define if your compiler supports function prototype */
 #define HAVE_PROTOTYPES 1
 
@@ -810,42 +808,42 @@
 /* Define to 1 if you have the <pthread.h> header file. */
 #define HAVE_PTHREAD_H 1
 
 /* Define to 1 if you have the `pthread_init' function. */
 /* #undef HAVE_PTHREAD_INIT */
 
 /* Define to 1 if you have the `pthread_kill' function. */
-#define HAVE_PTHREAD_KILL 1
+/* #undef HAVE_PTHREAD_KILL */
 
 /* Define to 1 if you have the `pthread_sigmask' function. */
-#define HAVE_PTHREAD_SIGMASK 1
+/* #undef HAVE_PTHREAD_SIGMASK */
 
 /* Define to 1 if you have the <pty.h> header file. */
-#define HAVE_PTY_H 1
+/* #undef HAVE_PTY_H */
 
 /* Define to 1 if you have the `pwrite' function. */
 #define HAVE_PWRITE 1
 
 /* Define to 1 if you have the `pwritev' function. */
 #define HAVE_PWRITEV 1
 
 /* Define to 1 if you have the `pwritev2' function. */
-#define HAVE_PWRITEV2 1
+/* #undef HAVE_PWRITEV2 */
 
 /* Define to 1 if you have the `readlink' function. */
 #define HAVE_READLINK 1
 
 /* Define to 1 if you have the `readlinkat' function. */
 #define HAVE_READLINKAT 1
 
 /* Define to 1 if you have the `readv' function. */
 #define HAVE_READV 1
 
 /* Define to 1 if you have the `realpath' function. */
-#define HAVE_REALPATH 1
+/* #undef HAVE_REALPATH */
 
 /* Define to 1 if you have the `renameat' function. */
 #define HAVE_RENAMEAT 1
 
 /* Define if readline supports append_history */
 /* #undef HAVE_RL_APPEND_HISTORY */
 
@@ -873,165 +871,165 @@
 /* Define to 1 if you have the `round' function. */
 #define HAVE_ROUND 1
 
 /* Define to 1 if you have the `rtpSpawn' function. */
 /* #undef HAVE_RTPSPAWN */
 
 /* Define to 1 if you have the `sched_get_priority_max' function. */
-#define HAVE_SCHED_GET_PRIORITY_MAX 1
+/* #undef HAVE_SCHED_GET_PRIORITY_MAX */
 
 /* Define to 1 if you have the <sched.h> header file. */
 #define HAVE_SCHED_H 1
 
 /* Define to 1 if you have the `sched_rr_get_interval' function. */
-#define HAVE_SCHED_RR_GET_INTERVAL 1
+/* #undef HAVE_SCHED_RR_GET_INTERVAL */
 
 /* Define to 1 if you have the `sched_setaffinity' function. */
-#define HAVE_SCHED_SETAFFINITY 1
+/* #undef HAVE_SCHED_SETAFFINITY */
 
 /* Define to 1 if you have the `sched_setparam' function. */
-#define HAVE_SCHED_SETPARAM 1
+/* #undef HAVE_SCHED_SETPARAM */
 
 /* Define to 1 if you have the `sched_setscheduler' function. */
-#define HAVE_SCHED_SETSCHEDULER 1
+/* #undef HAVE_SCHED_SETSCHEDULER */
 
 /* Define to 1 if you have the `sem_clockwait' function. */
-#define HAVE_SEM_CLOCKWAIT 1
+/* #undef HAVE_SEM_CLOCKWAIT */
 
 /* Define to 1 if you have the `sem_getvalue' function. */
-#define HAVE_SEM_GETVALUE 1
+/* #undef HAVE_SEM_GETVALUE */
 
 /* Define to 1 if you have the `sem_open' function. */
-#define HAVE_SEM_OPEN 1
+/* #undef HAVE_SEM_OPEN */
 
 /* Define to 1 if you have the `sem_timedwait' function. */
-#define HAVE_SEM_TIMEDWAIT 1
+/* #undef HAVE_SEM_TIMEDWAIT */
 
 /* Define to 1 if you have the `sem_unlink' function. */
-#define HAVE_SEM_UNLINK 1
+/* #undef HAVE_SEM_UNLINK */
 
 /* Define to 1 if you have the `sendfile' function. */
-#define HAVE_SENDFILE 1
+/* #undef HAVE_SENDFILE */
 
 /* Define to 1 if you have the `setegid' function. */
-#define HAVE_SETEGID 1
+/* #undef HAVE_SETEGID */
 
 /* Define to 1 if you have the `seteuid' function. */
-#define HAVE_SETEUID 1
+/* #undef HAVE_SETEUID */
 
 /* Define to 1 if you have the `setgid' function. */
-#define HAVE_SETGID 1
+/* #undef HAVE_SETGID */
 
 /* Define if you have the 'setgroups' function. */
-#define HAVE_SETGROUPS 1
+/* #undef HAVE_SETGROUPS */
 
 /* Define to 1 if you have the `sethostname' function. */
-#define HAVE_SETHOSTNAME 1
+/* #undef HAVE_SETHOSTNAME */
 
 /* Define to 1 if you have the `setitimer' function. */
-#define HAVE_SETITIMER 1
+/* #undef HAVE_SETITIMER */
 
 /* Define to 1 if you have the `setlocale' function. */
 #define HAVE_SETLOCALE 1
 
 /* Define to 1 if you have the `setpgid' function. */
-#define HAVE_SETPGID 1
+/* #undef HAVE_SETPGID */
 
 /* Define to 1 if you have the `setpgrp' function. */
-#define HAVE_SETPGRP 1
+/* #undef HAVE_SETPGRP */
 
 /* Define to 1 if you have the `setpriority' function. */
-#define HAVE_SETPRIORITY 1
+/* #undef HAVE_SETPRIORITY */
 
 /* Define to 1 if you have the `setregid' function. */
-#define HAVE_SETREGID 1
+/* #undef HAVE_SETREGID */
 
 /* Define to 1 if you have the `setresgid' function. */
-#define HAVE_SETRESGID 1
+/* #undef HAVE_SETRESGID */
 
 /* Define to 1 if you have the `setresuid' function. */
-#define HAVE_SETRESUID 1
+/* #undef HAVE_SETRESUID */
 
 /* Define to 1 if you have the `setreuid' function. */
-#define HAVE_SETREUID 1
+/* #undef HAVE_SETREUID */
 
 /* Define to 1 if you have the `setsid' function. */
-#define HAVE_SETSID 1
+/* #undef HAVE_SETSID */
 
 /* Define to 1 if you have the `setuid' function. */
-#define HAVE_SETUID 1
+/* #undef HAVE_SETUID */
 
 /* Define to 1 if you have the `setvbuf' function. */
 #define HAVE_SETVBUF 1
 
 /* Define to 1 if you have the <shadow.h> header file. */
-#define HAVE_SHADOW_H 1
+/* #undef HAVE_SHADOW_H */
 
 /* Define to 1 if you have the `shm_open' function. */
-#define HAVE_SHM_OPEN 1
+/* #undef HAVE_SHM_OPEN */
 
 /* Define to 1 if you have the `shm_unlink' function. */
-#define HAVE_SHM_UNLINK 1
+/* #undef HAVE_SHM_UNLINK */
 
 /* Define to 1 if you have the `sigaction' function. */
-#define HAVE_SIGACTION 1
+/* #undef HAVE_SIGACTION */
 
 /* Define to 1 if you have the `sigaltstack' function. */
-#define HAVE_SIGALTSTACK 1
+/* #undef HAVE_SIGALTSTACK */
 
 /* Define to 1 if you have the `sigfillset' function. */
-#define HAVE_SIGFILLSET 1
+/* #undef HAVE_SIGFILLSET */
 
 /* Define to 1 if `si_band' is a member of `siginfo_t'. */
-#define HAVE_SIGINFO_T_SI_BAND 1
+/* #undef HAVE_SIGINFO_T_SI_BAND */
 
 /* Define to 1 if you have the `siginterrupt' function. */
-#define HAVE_SIGINTERRUPT 1
+/* #undef HAVE_SIGINTERRUPT */
 
 /* Define to 1 if you have the <signal.h> header file. */
-#define HAVE_SIGNAL_H 1
+/* #undef HAVE_SIGNAL_H */
 
 /* Define to 1 if you have the `sigpending' function. */
-#define HAVE_SIGPENDING 1
+/* #undef HAVE_SIGPENDING */
 
 /* Define to 1 if you have the `sigrelse' function. */
-#define HAVE_SIGRELSE 1
+/* #undef HAVE_SIGRELSE */
 
 /* Define to 1 if you have the `sigtimedwait' function. */
-#define HAVE_SIGTIMEDWAIT 1
+/* #undef HAVE_SIGTIMEDWAIT */
 
 /* Define to 1 if you have the `sigwait' function. */
-#define HAVE_SIGWAIT 1
+/* #undef HAVE_SIGWAIT */
 
 /* Define to 1 if you have the `sigwaitinfo' function. */
-#define HAVE_SIGWAITINFO 1
+/* #undef HAVE_SIGWAITINFO */
 
 /* Define to 1 if you have the `snprintf' function. */
 #define HAVE_SNPRINTF 1
 
 /* struct sockaddr_alg (linux/if_alg.h) */
-#define HAVE_SOCKADDR_ALG 1
+/* #undef HAVE_SOCKADDR_ALG */
 
 /* Define if sockaddr has sa_len member */
 /* #undef HAVE_SOCKADDR_SA_LEN */
 
 /* struct sockaddr_storage (sys/socket.h) */
 #define HAVE_SOCKADDR_STORAGE 1
 
 /* Define if you have the 'socketpair' function. */
-#define HAVE_SOCKETPAIR 1
+/* #undef HAVE_SOCKETPAIR */
 
 /* Define to 1 if you have the <spawn.h> header file. */
-#define HAVE_SPAWN_H 1
+/* #undef HAVE_SPAWN_H */
 
 /* Define if your compiler provides ssize_t */
 #define HAVE_SSIZE_T 1
 
 /* Define to 1 if you have the `statvfs' function. */
-#define HAVE_STATVFS 1
+/* #undef HAVE_STATVFS */
 
 /* Define if you have struct stat.st_mtim.tv_nsec */
 #define HAVE_STAT_TV_NSEC 1
 
 /* Define if you have struct stat.st_mtimensec */
 /* #undef HAVE_STAT_TV_NSEC2 */
 
@@ -1057,27 +1055,27 @@
 /* Define to 1 if you have the <strings.h> header file. */
 #define HAVE_STRINGS_H 1
 
 /* Define to 1 if you have the <string.h> header file. */
 #define HAVE_STRING_H 1
 
 /* Define to 1 if you have the `strlcpy' function. */
-/* #undef HAVE_STRLCPY */
+#define HAVE_STRLCPY 1
 
 /* Define to 1 if you have the <stropts.h> header file. */
-/* #undef HAVE_STROPTS_H */
+#define HAVE_STROPTS_H 1
 
 /* Define to 1 if you have the `strsignal' function. */
-#define HAVE_STRSIGNAL 1
+/* #undef HAVE_STRSIGNAL */
 
 /* Define to 1 if `pw_gecos' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_GECOS 1
+/* #undef HAVE_STRUCT_PASSWD_PW_GECOS */
 
 /* Define to 1 if `pw_passwd' is a member of `struct passwd'. */
-#define HAVE_STRUCT_PASSWD_PW_PASSWD 1
+/* #undef HAVE_STRUCT_PASSWD_PW_PASSWD */
 
 /* Define to 1 if `st_birthtime' is a member of `struct stat'. */
 /* #undef HAVE_STRUCT_STAT_ST_BIRTHTIME */
 
 /* Define to 1 if `st_blksize' is a member of `struct stat'. */
 #define HAVE_STRUCT_STAT_ST_BLKSIZE 1
 
@@ -1099,43 +1097,43 @@
 /* Define if you have the 'symlink' function. */
 #define HAVE_SYMLINK 1
 
 /* Define to 1 if you have the `symlinkat' function. */
 #define HAVE_SYMLINKAT 1
 
 /* Define to 1 if you have the `sync' function. */
-#define HAVE_SYNC 1
+/* #undef HAVE_SYNC */
 
 /* Define to 1 if you have the `sysconf' function. */
 #define HAVE_SYSCONF 1
 
 /* Define to 1 if you have the <sysexits.h> header file. */
 #define HAVE_SYSEXITS_H 1
 
 /* Define to 1 if you have the <sys/audioio.h> header file. */
 /* #undef HAVE_SYS_AUDIOIO_H */
 
 /* Define to 1 if you have the <sys/auxv.h> header file. */
-#define HAVE_SYS_AUXV_H 1
+/* #undef HAVE_SYS_AUXV_H */
 
 /* Define to 1 if you have the <sys/bsdtty.h> header file. */
 /* #undef HAVE_SYS_BSDTTY_H */
 
 /* Define to 1 if you have the <sys/devpoll.h> header file. */
 /* #undef HAVE_SYS_DEVPOLL_H */
 
 /* Define to 1 if you have the <sys/dir.h> header file, and it defines `DIR'.
-   */
+ */
 /* #undef HAVE_SYS_DIR_H */
 
 /* Define to 1 if you have the <sys/endian.h> header file. */
 /* #undef HAVE_SYS_ENDIAN_H */
 
 /* Define to 1 if you have the <sys/epoll.h> header file. */
-#define HAVE_SYS_EPOLL_H 1
+/* #undef HAVE_SYS_EPOLL_H */
 
 /* Define to 1 if you have the <sys/event.h> header file. */
 /* #undef HAVE_SYS_EVENT_H */
 
 /* Define to 1 if you have the <sys/file.h> header file. */
 #define HAVE_SYS_FILE_H 1
 
@@ -1160,15 +1158,15 @@
 /* Define to 1 if you have the <sys/mman.h> header file. */
 #define HAVE_SYS_MMAN_H 1
 
 /* Define to 1 if you have the <sys/modem.h> header file. */
 /* #undef HAVE_SYS_MODEM_H */
 
 /* Define to 1 if you have the <sys/ndir.h> header file, and it defines `DIR'.
-   */
+ */
 /* #undef HAVE_SYS_NDIR_H */
 
 /* Define to 1 if you have the <sys/param.h> header file. */
 #define HAVE_SYS_PARAM_H 1
 
 /* Define to 1 if you have the <sys/poll.h> header file. */
 #define HAVE_SYS_POLL_H 1
@@ -1179,30 +1177,30 @@
 /* Define to 1 if you have the <sys/resource.h> header file. */
 #define HAVE_SYS_RESOURCE_H 1
 
 /* Define to 1 if you have the <sys/select.h> header file. */
 #define HAVE_SYS_SELECT_H 1
 
 /* Define to 1 if you have the <sys/sendfile.h> header file. */
-#define HAVE_SYS_SENDFILE_H 1
+/* #undef HAVE_SYS_SENDFILE_H */
 
 /* Define to 1 if you have the <sys/socket.h> header file. */
 #define HAVE_SYS_SOCKET_H 1
 
 /* Define to 1 if you have the <sys/statvfs.h> header file. */
-#define HAVE_SYS_STATVFS_H 1
+/* #undef HAVE_SYS_STATVFS_H */
 
 /* Define to 1 if you have the <sys/stat.h> header file. */
 #define HAVE_SYS_STAT_H 1
 
 /* Define to 1 if you have the <sys/syscall.h> header file. */
 #define HAVE_SYS_SYSCALL_H 1
 
 /* Define to 1 if you have the <sys/sysmacros.h> header file. */
-#define HAVE_SYS_SYSMACROS_H 1
+/* #undef HAVE_SYS_SYSMACROS_H */
 
 /* Define to 1 if you have the <sys/sys_domain.h> header file. */
 /* #undef HAVE_SYS_SYS_DOMAIN_H */
 
 /* Define to 1 if you have the <sys/termio.h> header file. */
 /* #undef HAVE_SYS_TERMIO_H */
 
@@ -1221,51 +1219,51 @@
 /* Define to 1 if you have the <sys/un.h> header file. */
 #define HAVE_SYS_UN_H 1
 
 /* Define to 1 if you have the <sys/utsname.h> header file. */
 #define HAVE_SYS_UTSNAME_H 1
 
 /* Define to 1 if you have the <sys/wait.h> header file. */
-#define HAVE_SYS_WAIT_H 1
+/* #undef HAVE_SYS_WAIT_H */
 
 /* Define to 1 if you have the <sys/xattr.h> header file. */
-#define HAVE_SYS_XATTR_H 1
+/* #undef HAVE_SYS_XATTR_H */
 
 /* Define to 1 if you have the `tcgetpgrp' function. */
-#define HAVE_TCGETPGRP 1
+/* #undef HAVE_TCGETPGRP */
 
 /* Define to 1 if you have the `tcsetpgrp' function. */
-#define HAVE_TCSETPGRP 1
+/* #undef HAVE_TCSETPGRP */
 
 /* Define to 1 if you have the `tempnam' function. */
-#define HAVE_TEMPNAM 1
+/* #undef HAVE_TEMPNAM */
 
 /* Define to 1 if you have the <termios.h> header file. */
-#define HAVE_TERMIOS_H 1
+/* #undef HAVE_TERMIOS_H */
 
 /* Define to 1 if you have the <term.h> header file. */
 /* #undef HAVE_TERM_H */
 
 /* Define to 1 if you have the `tgamma' function. */
 #define HAVE_TGAMMA 1
 
 /* Define to 1 if you have the `timegm' function. */
 #define HAVE_TIMEGM 1
 
 /* Define to 1 if you have the `times' function. */
 #define HAVE_TIMES 1
 
 /* Define to 1 if you have the `tmpfile' function. */
-#define HAVE_TMPFILE 1
+/* #undef HAVE_TMPFILE */
 
 /* Define to 1 if you have the `tmpnam' function. */
-#define HAVE_TMPNAM 1
+/* #undef HAVE_TMPNAM */
 
 /* Define to 1 if you have the `tmpnam_r' function. */
-#define HAVE_TMPNAM_R 1
+/* #undef HAVE_TMPNAM_R */
 
 /* Define to 1 if your `struct tm' has `tm_zone'. Deprecated, use
    `HAVE_STRUCT_TM_TM_ZONE' instead. */
 #define HAVE_TM_ZONE 1
 
 /* Define to 1 if you have the `truncate' function. */
 #define HAVE_TRUNCATE 1
@@ -1294,15 +1292,15 @@
 /* Define to 1 if you have the <util.h> header file. */
 /* #undef HAVE_UTIL_H */
 
 /* Define to 1 if you have the `utimensat' function. */
 #define HAVE_UTIMENSAT 1
 
 /* Define to 1 if you have the `utimes' function. */
-#define HAVE_UTIMES 1
+/* #undef HAVE_UTIMES */
 
 /* Define to 1 if you have the <utime.h> header file. */
 #define HAVE_UTIME_H 1
 
 /* Define if uuid_create() exists. */
 /* #undef HAVE_UUID_CREATE */
 
@@ -1315,24 +1313,24 @@
 /* Define to 1 if you have the <uuid.h> header file. */
 /* #undef HAVE_UUID_H */
 
 /* Define to 1 if you have the <uuid/uuid.h> header file. */
 /* #undef HAVE_UUID_UUID_H */
 
 /* Define to 1 if you have the `wait3' function. */
-#define HAVE_WAIT3 1
+/* #undef HAVE_WAIT3 */
 
 /* Define to 1 if you have the `wait4' function. */
-#define HAVE_WAIT4 1
+/* #undef HAVE_WAIT4 */
 
 /* Define to 1 if you have the `waitid' function. */
-#define HAVE_WAITID 1
+/* #undef HAVE_WAITID */
 
 /* Define to 1 if you have the `waitpid' function. */
-#define HAVE_WAITPID 1
+/* #undef HAVE_WAITPID */
 
 /* Define if the compiler provides a wchar.h header file. */
 #define HAVE_WCHAR_H 1
 
 /* Define to 1 if you have the `wcscoll' function. */
 #define HAVE_WCSCOLL 1
 
@@ -1342,36 +1340,36 @@
 /* Define to 1 if you have the `wcsxfrm' function. */
 #define HAVE_WCSXFRM 1
 
 /* Define to 1 if you have the `wmemcmp' function. */
 #define HAVE_WMEMCMP 1
 
 /* Define if tzset() actually switches the local timezone in a meaningful way.
-   */
-#define HAVE_WORKING_TZSET 1
+ */
+/* #undef HAVE_WORKING_TZSET */
 
 /* Define to 1 if you have the `writev' function. */
 #define HAVE_WRITEV 1
 
 /* Define if libssl has X509_VERIFY_PARAM_set1_host and related function */
 /* #undef HAVE_X509_VERIFY_PARAM_SET1_HOST */
 
 /* Define if the zlib library has inflateCopy */
-#define HAVE_ZLIB_COPY 1
+/* #undef HAVE_ZLIB_COPY */
 
 /* Define to 1 if you have the `_getpty' function. */
 /* #undef HAVE__GETPTY */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in <mkdev.h>.
-   */
+ */
 /* #undef MAJOR_IN_MKDEV */
 
 /* Define to 1 if `major', `minor', and `makedev' are declared in
    <sysmacros.h>. */
-#define MAJOR_IN_SYSMACROS 1
+/* #undef MAJOR_IN_SYSMACROS */
 
 /* Define if mvwdelch in curses.h is an expression. */
 /* #undef MVWDELCH_IS_EXPRESSION */
 
 /* Define to the address where bug reports for this package should be sent. */
 /* #undef PACKAGE_BUGREPORT */
 
@@ -1390,18 +1388,18 @@
 /* Define to the version of this package. */
 /* #undef PACKAGE_VERSION */
 
 /* Define if POSIX semaphores aren't enabled on your system */
 /* #undef POSIX_SEMAPHORES_NOT_ENABLED */
 
 /* Define if pthread_key_t is compatible with int. */
-#define PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT 1
+/* #undef PTHREAD_KEY_T_IS_COMPATIBLE_WITH_INT */
 
 /* Defined if PTHREAD_SCOPE_SYSTEM supported. */
-#define PTHREAD_SYSTEM_SCHED_SUPPORTED 1
+/* #undef PTHREAD_SYSTEM_SCHED_SUPPORTED */
 
 /* Define as the preferred size in bits of long digits */
 /* #undef PYLONG_BITS_IN_DIGIT */
 
 /* enabled builtin hash modules */
 #define PY_BUILTIN_HASHLIB_HASHES "md5,sha1,sha256,sha512,sha3,blake2"
 
@@ -1452,15 +1450,15 @@
 /* The size of `fpos_t', as computed by sizeof. */
 #define SIZEOF_FPOS_T 16
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
-#define SIZEOF_LONG 8
+#define SIZEOF_LONG 4
 
 /* The size of `long double', as computed by sizeof. */
 #define SIZEOF_LONG_DOUBLE 16
 
 /* The size of `long long', as computed by sizeof. */
 #define SIZEOF_LONG_LONG 8
 
@@ -1470,30 +1468,30 @@
 /* The size of `pid_t', as computed by sizeof. */
 #define SIZEOF_PID_T 4
 
 /* The size of `pthread_key_t', as computed by sizeof. */
 #define SIZEOF_PTHREAD_KEY_T 4
 
 /* The size of `pthread_t', as computed by sizeof. */
-#define SIZEOF_PTHREAD_T 8
+#define SIZEOF_PTHREAD_T 4
 
 /* The size of `short', as computed by sizeof. */
 #define SIZEOF_SHORT 2
 
 /* The size of `size_t', as computed by sizeof. */
 #define SIZEOF_SIZE_T 8
 
 /* The size of `time_t', as computed by sizeof. */
 #define SIZEOF_TIME_T 8
 
 /* The size of `uintptr_t', as computed by sizeof. */
-#define SIZEOF_UINTPTR_T 8
+#define SIZEOF_UINTPTR_T 4
 
 /* The size of `void *', as computed by sizeof. */
-#define SIZEOF_VOID_P 8
+#define SIZEOF_VOID_P 4
 
 /* The size of `wchar_t', as computed by sizeof. */
 #define SIZEOF_WCHAR_T 4
 
 /* The size of `_Bool', as computed by sizeof. */
 #define SIZEOF__BOOL 1
 
@@ -1514,34 +1512,33 @@
 /* #undef TM_IN_SYS_TIME */
 
 /* Define if you want to use computed gotos in ceval.c. */
 /* #undef USE_COMPUTED_GOTOS */
 
 /* Enable extensions on AIX 3, Interix.  */
 #ifndef _ALL_SOURCE
-# define _ALL_SOURCE 1
+#define _ALL_SOURCE 1
 #endif
 /* Enable GNU extensions on systems that have them.  */
 #ifndef _GNU_SOURCE
-# define _GNU_SOURCE 1
+#define _GNU_SOURCE 1
 #endif
 /* Enable threading extensions on Solaris.  */
 #ifndef _POSIX_PTHREAD_SEMANTICS
-# define _POSIX_PTHREAD_SEMANTICS 1
+#define _POSIX_PTHREAD_SEMANTICS 1
 #endif
 /* Enable extensions on HP NonStop.  */
 #ifndef _TANDEM_SOURCE
-# define _TANDEM_SOURCE 1
+#define _TANDEM_SOURCE 1
 #endif
 /* Enable general extensions on Solaris.  */
 #ifndef __EXTENSIONS__
-# define __EXTENSIONS__ 1
+#define __EXTENSIONS__ 1
 #endif
 
-
 /* Define if WINDOW in curses.h offers a field _flags. */
 /* #undef WINDOW_HAS_FLAGS */
 
 /* Define if you want build the _decimal module using a coroutine-local rather
    than a thread-local context */
 #define WITH_DECIMAL_CONTEXTVAR 1
 
@@ -1568,21 +1565,21 @@
 
 /* Define if you want pymalloc to be disabled when running under valgrind */
 /* #undef WITH_VALGRIND */
 
 /* Define WORDS_BIGENDIAN to 1 if your processor stores words with the most
    significant byte first (like Motorola and SPARC, unlike Intel). */
 #if defined AC_APPLE_UNIVERSAL_BUILD
-# if defined __BIG_ENDIAN__
-#  define WORDS_BIGENDIAN 1
-# endif
+#if defined __BIG_ENDIAN__
+#define WORDS_BIGENDIAN 1
+#endif
 #else
-# ifndef WORDS_BIGENDIAN
+#ifndef WORDS_BIGENDIAN
 /* #  undef WORDS_BIGENDIAN */
-# endif
+#endif
 #endif
 
 /* Define if arithmetic is subject to x87-style double rounding issue */
 /* #undef X87_DOUBLE_ROUNDING */
 
 /* Define on OpenBSD to activate all library features */
 /* #undef _BSD_SOURCE */
@@ -1665,15 +1662,13 @@
 
 /* Define to `int' if <sys/socket.h> does not define. */
 /* #undef socklen_t */
 
 /* Define to `int' if <sys/types.h> doesn't define. */
 /* #undef uid_t */
 
-
 /* Define the macros needed if on a UnixWare 7.x system. */
 #if defined(__USLC__) && defined(__SCO_VERSION__)
 #define STRICT_SYSV_CURSES /* Don't use ncurses extensions */
 #endif
 
 #endif /*Py_PYCONFIG_H*/
-
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyctype.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydebug.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.d` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyerrors.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyexpat.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pylifecycle.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacconfig.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacro.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymath.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymem.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyport.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pyport.h`

 * *Files 2% similar despite different names*

```diff
@@ -660,15 +660,15 @@
 
 #include "exports.h"
 
 /* only get special linkage if built as shared or platform is Cygwin */
 #if defined(Py_ENABLE_SHARED) || defined(__CYGWIN__)
 #       if defined(HAVE_DECLSPEC_DLL)
 #               if defined(Py_BUILD_CORE) && !defined(Py_BUILD_CORE_MODULE)
-#                       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#                       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #                       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
         /* module init functions inside the core need no external linkage */
         /* except for Cygwin to handle embedding */
 #                       if defined(__CYGWIN__)
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __CYGWIN__ */
 #                               define PyMODINIT_FUNC PyObject*
@@ -676,30 +676,30 @@
 #               else /* Py_BUILD_CORE */
         /* Building an extension module, or an embedded situation */
         /* public Python functions and data are imported */
         /* Under Cygwin, auto-import functions to prevent compilation */
         /* failures similar to those described at the bottom of 4.1: */
         /* http://docs.python.org/extending/windows.html#a-cookbook-approach */
 #                       if !defined(__CYGWIN__)
-#                               define PyAPI_FUNC(RTYPE) Py_IMPORTED_SYMBOL RTYPE
+#                               define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_IMPORTED_SYMBOL RTYPE
 #                       endif /* !__CYGWIN__ */
 #                       define PyAPI_DATA(RTYPE) extern Py_IMPORTED_SYMBOL RTYPE
         /* module init functions outside the core must be exported */
 #                       if defined(__cplusplus)
 #                               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
 #                       else /* __cplusplus */
 #                               define PyMODINIT_FUNC Py_EXPORTED_SYMBOL PyObject*
 #                       endif /* __cplusplus */
 #               endif /* Py_BUILD_CORE */
 #       endif /* HAVE_DECLSPEC_DLL */
 #endif /* Py_ENABLE_SHARED */
 
 /* If no external linkage macros defined by now, create defaults */
 #ifndef PyAPI_FUNC
-#       define PyAPI_FUNC(RTYPE) Py_EXPORTED_SYMBOL RTYPE
+#       define PyAPI_FUNC(RTYPE) __attribute__((import_module ("capi"))) Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyAPI_DATA
 #       define PyAPI_DATA(RTYPE) extern Py_EXPORTED_SYMBOL RTYPE
 #endif
 #ifndef PyMODINIT_FUNC
 #       if defined(__cplusplus)
 #               define PyMODINIT_FUNC extern "C" Py_EXPORTED_SYMBOL PyObject*
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystate.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrhex.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrtod.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythonrun.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythread.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pytime.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/rangeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/setobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/sliceobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/structmember.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/structseq.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/symtable.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/sysmodule.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/token.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/traceback.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/tracemalloc.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/tupleobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/typeslots.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ucnhash.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/unicodeobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/warnings.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build/include/cp39/weakrefobject.h` & `wasmpy-build-0.3.3/wasmpy_build/include/cp39/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.2/wasmpy_build.egg-info/PKG-INFO` & `wasmpy-build-0.3.3/wasmpy_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.3.2
+Version: 0.3.3
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wasmpy-build-0.3.2/wasmpy_build.egg-info/SOURCES.txt` & `wasmpy-build-0.3.3/wasmpy_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

