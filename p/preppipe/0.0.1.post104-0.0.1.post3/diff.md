# Comparing `tmp/preppipe-0.0.1.post104.tar.gz` & `tmp/preppipe-0.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preppipe-0.0.1.post104.tar", last modified: Sat Jul 15 12:38:02 2023, max compression
+gzip compressed data, was "preppipe-0.0.1.post3.tar", last modified: Sat Dec 25 09:30:24 2021, max compression
```

## Comparing `preppipe-0.0.1.post104.tar` & `preppipe-0.0.1.post3.tar`

### file list

```diff
@@ -1,132 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/
--rw-r--r--   0 runner    (1001) docker     (123)    20765 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/develop_bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.480864 preppipe-0.0.1.post104/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   112854 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.480864 preppipe-0.0.1.post104/docs/image/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4639 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/docs/image/logo.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   109431 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/preppipe.ico
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/preppipe_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.476864 preppipe-0.0.1.post104/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.480864 preppipe-0.0.1.post104/src/preppipe/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/assetusage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/icfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/timemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/analysis/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/analysis/vnmodel/vnsaydump.py
--rw-r--r--   0 runner    (1001) docker     (123)    38167 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/commontypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/deprecated/documentimport/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/documentimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/documentimport/opendocument.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/documentmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/renpy_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/visualnovelmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/deprecated/vnexport/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnexport/renpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe/deprecated/vnimport/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnimport/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.488864 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnasset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnconstant.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    23107 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vninstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnnamespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    16692 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vnstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel/vntype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/deprecated/vnmodel_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.488864 preppipe-0.0.1.post104/src/preppipe/enginesupport/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/enginesupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25594 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/enginesupport/enginesupport.py
--rw-r--r--   0 runner    (1001) docker     (123)    24889 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/enginesupport/renpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.488864 preppipe-0.0.1.post104/src/preppipe/frontend/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/CommandParse.g4
--rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/CommandScan.g4
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.488864 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandParseLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandParseListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandParseParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandParseVisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandScanLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandScanListener.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/CommandScanParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/_antlr_generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37804 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/commandsemantics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/commandsyntaxparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/opendocument.py
--rw-r--r--   0 runner    (1001) docker     (123)    46566 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/SayScan.g4
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)    39050 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/vnast.py
--rw-r--r--   0 runner    (1001) docker     (123)   100958 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/vncodegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    60923 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/vnparser_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/vnsayscan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/frontend/vnmodel/vnutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/imageexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/inputmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)   142727 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/irbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/irdataop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/nameresolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29560 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/pipeline_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/src/preppipe/renpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25334 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    49497 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    20701 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/renpy/preppipert.rpy
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/src/preppipe/transform/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/passes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/src/preppipe/transform/vnmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/vnmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/vnmodel/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/vnmodel/vnentryinference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/transform/vnmodel/vnlongsaysplitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.492864 preppipe-0.0.1.post104/src/preppipe/util/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/antlr4util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/graphtrait.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/nameconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/typo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/util/versioning.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    66482 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/vnmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    66331 2023-07-15 12:37:41.000000 preppipe-0.0.1.post104/src/preppipe/vnmodel_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:38:02.484864 preppipe-0.0.1.post104/src/preppipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 12:38:02.000000 preppipe-0.0.1.post104/src/preppipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.760685 preppipe-0.0.1.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2543 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/commontypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/documentimport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9105 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentimport/opendocument.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7795 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/documentmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/enginesupport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6485 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/enginesupport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31191 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/enginesupport/renpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3177 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/visualnovelmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/vnexport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnexport/renpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe/vnimport/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnimport/document.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    34366 2021-12-25 09:29:45.000000 preppipe-0.0.1.post3/src/preppipe/vnmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-25 09:30:24.764685 preppipe-0.0.1.post3/src/preppipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-25 09:30:24.000000 preppipe-0.0.1.post3/src/preppipe.egg-info/top_level.txt
```

### Comparing `preppipe-0.0.1.post104/LICENSE` & `preppipe-0.0.1.post3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 PrepPipe's Contributors
+   Copyright [yyyy] [name of copyright owner]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `preppipe-0.0.1.post104/PKG-INFO` & `preppipe-0.0.1.post3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: preppipe
-Version: 0.0.1.post104
+Version: 0.0.1.post3
 Summary: Document to Visual Novel generator
 Home-page: https://github.com/PrepPipe/preppipe-python
 Author: Shengjie Xu
 Author-email: xsj617603321@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PrepPipe/preppipe-python/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PrepPipe
 
 Document TODO
 
 Experimental project. Do not use for production (for now).
 
+
+
```

### Comparing `preppipe-0.0.1.post104/setup.cfg` & `preppipe-0.0.1.post3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,24 @@
 project_urls = 
 	Bug Tracker = https://github.com/PrepPipe/preppipe-python/issues
 license = Apache-2.0
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
-	Development Status :: 1 - Planning
 
 [options]
-include_package_data = True
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.6
 install_requires = 
-	llist
-	odfpy
 	pillow
+	odfpy
 	pydub
-	numpy
-	ghostscript
-	editdistance
-	bidict
-	pypinyin
-	graphviz
-	antlr4-python3-runtime >= 4.10
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/documentimport/opendocument.py` & `preppipe-0.0.1.post3/src/preppipe/documentimport/opendocument.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io, sys, os
 import typing
 from warnings import warn
 import PIL.Image
 
 import odf.opendocument
 
-import preppipe.deprecated.documentmodel as documentmodel
+import preppipe.documentmodel as documentmodel
 import preppipe.commontypes
 
 
 def import_odf(fileData : io.BufferedReader, filePath: str) -> documentmodel.DocumentModel:
   """Import an ODF document and return a document model"""
 
   odfhandle = odf.opendocument.load(fileData)
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/documentmodel.py` & `preppipe-0.0.1.post3/src/preppipe/documentmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# SPDX-FileCopyrightText: 2022 PrepPipe's Contributors
-# SPDX-License-Identifier: Apache-2.0
+#!/usr/bin/env python3
 
 import typing
 import PIL.Image
 import importlib
 import hashlib
 from enum import Enum
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/renpy_old.py` & `preppipe-0.0.1.post3/src/preppipe/enginesupport/renpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,28 +967,28 @@
         bb = bb_worklist.popleft()
         bb_label = bb_name_map[bb]
         rpybb = EMBasicBlock(bb_label)
         bb_map[bb] = rpybb
         rpybb_list.append(rpybb)
         
         for instr in bb.get_instruction_list():
-          if isinstance(instr, VNUpdateBackgroundInst):
+          if isinstance(instr, VNUpdateBackground):
             background = instr.get_background()
             background_expr = materialize_background_image(background)
             operand = background_expr
             if isinstance(background_expr, list):
               operand = " ".join(background_expr)
             sceneinstr = EMInstruction(_RenpyInstrOpcode.RO_Scene)
             sceneinstr.set_operand_list([operand])
             rpybb.add_instruction(sceneinstr)
-          elif isinstance(instr, VNSayerDeclInst):
+          elif isinstance(instr, VNSayerDeclInstr):
             handle_sayer_update(instr)
-          elif isinstance(instr, VNSayerUpdateInst):
+          elif isinstance(instr, VNSayerUpdateInstr):
             handle_sayer_update(instr)
-          elif isinstance(instr, VNUpdateBGMInst):
+          elif isinstance(instr, VNUpdateBGMInstr):
             bgm = instr.get_first_bgm()
             bgm_expr = materialize_audio(bgm, "bgm")
             bgminstr = EMInstruction(_RenpyInstrOpcode.RO_PlayMusic)
             bgminstr.add_operand(quote(bgm_expr))
             rpybb.add_instruction(bgminstr)
           elif isinstance(instr, VNSayInst):
             voice = instr.get_voice()
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/visualnovelmodel.py` & `preppipe-0.0.1.post3/src/preppipe/visualnovelmodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# SPDX-FileCopyrightText: 2022 PrepPipe's Contributors
-# SPDX-License-Identifier: Apache-2.0
+#!/usr/bin/env python3
 
 import typing
 import PIL.Image
 from enum import Enum
 import preppipe.commontypes
 
 class VNContext:
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/vnexport/renpy.py` & `preppipe-0.0.1.post3/src/preppipe/vnexport/renpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 from io import UnsupportedOperation
 from warnings import warn
 import os, sys, typing
-import preppipe.deprecated.visualnovelmodel as visualnovelmodel
+import preppipe.visualnovelmodel as visualnovelmodel
 
 def renpy_sanitize(text: str) -> str:
   result = ""
   for ch in text:
     if ch == '[':
       result += "[["
     elif ch == '{':
```

### Comparing `preppipe-0.0.1.post104/src/preppipe/deprecated/vnimport/document.py` & `preppipe-0.0.1.post3/src/preppipe/vnimport/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import io, sys
 import typing
 
-import preppipe.deprecated.documentmodel as documentmodel
-import preppipe.deprecated.visualnovelmodel as visualnovelmodel
+import preppipe.documentmodel as documentmodel
+import preppipe.visualnovelmodel as visualnovelmodel
 
 def get_visual_novel_model_from_document(doc : documentmodel.DocumentModel) -> visualnovelmodel.VisualNovelModel:
   """Convert a DocumentModel into a VisualNovelModel
   This function makes best effort in converting all information, even if there are errors
   """
   result = visualnovelmodel.VisualNovelModel()
   # TODO import all images
```

### Comparing `preppipe-0.0.1.post104/src/preppipe.egg-info/PKG-INFO` & `preppipe-0.0.1.post3/src/preppipe.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: preppipe
-Version: 0.0.1.post104
+Version: 0.0.1.post3
 Summary: Document to Visual Novel generator
 Home-page: https://github.com/PrepPipe/preppipe-python
 Author: Shengjie Xu
 Author-email: xsj617603321@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/PrepPipe/preppipe-python/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PrepPipe
 
 Document TODO
 
 Experimental project. Do not use for production (for now).
 
+
+
```

