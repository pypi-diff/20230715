# Comparing `tmp/ork.build.tools-0.0.6.tar.gz` & `tmp/ork.build.tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ork.build.tools-0.0.6.tar", last modified: Fri Jul 14 20:53:09 2023, max compression
+gzip compressed data, was "ork.build.tools-0.0.7.tar", last modified: Fri Jul 14 21:16:02 2023, max compression
```

## Comparing `ork.build.tools-0.0.6.tar` & `ork.build.tools-0.0.7.tar`

### file list

```diff
@@ -1,402 +1,403 @@
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.571205 ork.build.tools-0.0.6/
--rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 20:53:09.570647 ork.build.tools-0.0.6/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    14749 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/README.md
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.392941 ork.build.tools-0.0.6/bin_priv/
--rw-r--r--   0 michael    (501) wheel        (0)        0 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/__init__.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      332 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.build.all.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1965 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1312 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.findtext.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1810 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3223 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.replacetext.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      206 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.require.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      840 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.shell.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2298 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.dep.status.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1612 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1107 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1240 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.kill.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2422 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      780 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1429 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.docker.method.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      708 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.ext.find.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1311 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.find.in.dep.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      649 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.find.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1099 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.host.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1839 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.installedacontainers.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       83 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.ix.udevrules.reload.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      977 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.litex.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1406 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.litex.zephyrriscv-sample.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       97 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.lsttys.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     6545 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.lsusbx.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       99 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.lsvideo.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.osx.macho.fixup.libs.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      359 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.osx.macho.showinstallname.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      350 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.osx.macho.showlibs.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      163 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.pip.install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1782 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.replace.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1377 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.sdk.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      955 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.sdk.install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1640 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.subspace.build.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.subspace.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      802 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.subspace.list.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.target.info.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2901 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.vivado.getsites.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2566 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.vivado.launch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2441 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_priv/obt.vscode.create.debug.task.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.398042 ork.build.tools-0.0.6/bin_pub/
--rwxr-xr-x   0 michael    (501) wheel        (0)     5555 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.create.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     8042 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.init.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      445 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.gentoo.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2951 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.linuxcnc.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3176 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      734 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/bin_pub/obt.osx.installdeps.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.365164 ork.build.tools-0.0.6/examples/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.398668 ork.build.tools-0.0.6/examples/dep-overrides/
--rw-r--r--   0 michael    (501) wheel        (0)     1530 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/dep-overrides/orkid.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.404033 ork.build.tools-0.0.6/examples/litex1/
--rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/bit2svf_nexysv.tcl
--rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/cmod_a7_platform.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/cmod_a7_target.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/nexys_video.py
--rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/nexysv.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      247 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/soc_arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex1/soc_nexysv.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.408410 ork.build.tools-0.0.6/examples/litex_zephyrtest/
--rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/CMakeLists.txt
--rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/LICENSE
--rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/README.rst
--rwxr-xr-x   0 michael    (501) wheel        (0)      315 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/build.py
--rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/main.c
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/prj.conf
--rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/sample.yaml
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.409042 ork.build.tools-0.0.6/examples/litex_zephyrtest/src/
--rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build.tools-0.0.6/examples/litex_zephyrtest/src/main.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.372811 ork.build.tools-0.0.6/modules/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.489345 ork.build.tools-0.0.6/modules/dep/
--rw-r--r--   0 michael    (501) wheel        (0)      718 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     8257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-05-09 20:23:50.000000 ork.build.tools-0.0.6/modules/dep/_nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1910 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/apitrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1776 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/arachnepnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1663 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/arm64_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1580 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/arm64_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/assimp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/astcencoder.py
--rw-r--r--   0 michael    (501) wheel        (0)     1675 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/audiofile.py
--rw-r--r--   0 michael    (501) wheel        (0)     1611 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/avr_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     2206 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/avr_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2209 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/avr_libc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1793 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/bazel.py
--rw-r--r--   0 michael    (501) wheel        (0)     1302 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/blosc.py
--rw-r--r--   0 michael    (501) wheel        (0)     9272 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/boost.py
--rw-r--r--   0 michael    (501) wheel        (0)     1248 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/bullet.py
--rw-r--r--   0 michael    (501) wheel        (0)     2004 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/calf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1541 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/cgal.py
--rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/clang.py
--rw-r--r--   0 michael    (501) wheel        (0)     1408 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/cmake.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/cpppeglib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1632 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/cppzmq.py
--rw-r--r--   0 michael    (501) wheel        (0)     1563 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/csvparser.py
--rw-r--r--   0 michael    (501) wheel        (0)     1257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1684 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/curlpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/cycles.py
--rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/depthaicore.py
--rw-r--r--   0 michael    (501) wheel        (0)      992 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/drawtext.py
--rw-r--r--   0 michael    (501) wheel        (0)     1491 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/easyprof.py
--rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-02-18 06:09:54.000000 ork.build.tools-0.0.6/modules/dep/eigen.py
--rw-r--r--   0 michael    (501) wheel        (0)     2047 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/embree.py
--rw-r--r--   0 michael    (501) wheel        (0)     1871 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/faust.py
--rw-r--r--   0 michael    (501) wheel        (0)     1577 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/fcollada.py
--rw-r--r--   0 michael    (501) wheel        (0)     1737 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ffmpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/flatcam.py
--rw-r--r--   0 michael    (501) wheel        (0)     1676 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/fltk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1891 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/fluidsynth.py
--rw-r--r--   0 michael    (501) wheel        (0)     1866 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/frameretrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1438 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/gcode_gpr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2148 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/giflib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1175 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/gitpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     2601 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/glfw.py
--rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-02-18 06:09:54.000000 ork.build.tools-0.0.6/modules/dep/glm.py
--rw-r--r--   0 michael    (501) wheel        (0)      894 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/gnutar.py
--rw-r--r--   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/houdini.py
--rw-r--r--   0 michael    (501) wheel        (0)     1731 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/icestorm.py
--rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-03-18 06:31:34.000000 ork.build.tools-0.0.6/modules/dep/igl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1767 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/irix65_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     6593 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/irix65_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1150 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/irrlicht.py
--rw-r--r--   0 michael    (501) wheel        (0)     3478 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ispc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2331 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ispctexc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/jpegturbo.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/klein.py
--rw-r--r--   0 michael    (501) wheel        (0)     1079 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/lapack.py
--rw-r--r--   0 michael    (501) wheel        (0)     1065 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/lemongraph.py
--rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-06-17 04:32:01.000000 ork.build.tools-0.0.6/modules/dep/lexertl14.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/libcurl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1701 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/libfive.py
--rw-r--r--   0 michael    (501) wheel        (0)     1490 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/libpqpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1425 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/libsocket.py
--rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-05-12 22:40:05.000000 ork.build.tools-0.0.6/modules/dep/libsurvive.py
--rw-r--r--   0 michael    (501) wheel        (0)     7892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/libtorch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1926 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/linuxcnc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/modules/dep/litex.py
--rw-r--r--   0 michael    (501) wheel        (0)     2529 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/llvm.py
--rw-r--r--   0 michael    (501) wheel        (0)     1339 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/lm32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1066 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/lm32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2937 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/lua.py
--rw-r--r--   0 michael    (501) wheel        (0)     2135 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/luajit.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/m68k_amiga_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1555 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/m68k_amiga_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     3841 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/minetest.py
--rw-r--r--   0 michael    (501) wheel        (0)     2009 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/moltenvk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1244 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/nextpnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2117 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ngc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-04-27 00:04:32.000000 ork.build.tools-0.0.6/modules/dep/nlohmannjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     1633 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/nss.py
--rw-r--r--   0 michael    (501) wheel        (0)     1464 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/nsync_cpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     3022 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/nvtt.py
--rw-r--r--   0 michael    (501) wheel        (0)     1562 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ocio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/oiio.py
--rw-r--r--   0 michael    (501) wheel        (0)     1738 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/oneapimkl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1406 2023-04-27 00:04:41.000000 ork.build.tools-0.0.6/modules/dep/openblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-04-25 17:02:18.000000 ork.build.tools-0.0.6/modules/dep/opencv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/opencv_contrib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1217 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/opendb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/openexr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1332 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/openjpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1270 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/openroad.py
--rw-r--r--   0 michael    (501) wheel        (0)     1791 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/opensubdiv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/openvdb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1376 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/openvr.py
--rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-06-23 17:21:13.000000 ork.build.tools-0.0.6/modules/dep/orkid.py
--rw-r--r--   0 michael    (501) wheel        (0)     1306 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/osgeolaszip.py
--rw-r--r--   0 michael    (501) wheel        (0)     1495 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/osgeoliblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/osgeoproj.py
--rw-r--r--   0 michael    (501) wheel        (0)     1543 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/osgeotiff.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/osl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/ozzanim.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pangolin.py
--rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/parsertl14.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.366790 ork.build.tools-0.0.6/modules/dep/patches/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.366002 ork.build.tools-0.0.6/modules/dep/patches/boost/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.491084 ork.build.tools-0.0.6/modules/dep/patches/boost/chg/
--rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/boost/chg/darwin.jam
--rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/boost/chg/project-config.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.491603 ork.build.tools-0.0.6/modules/dep/patches/boost/ori/
--rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/boost/ori/darwin.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.494999 ork.build.tools-0.0.6/modules/dep/patches/gcc/
--rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/gcc/gcc.sgifixes.patch
--rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
--rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
--rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/gcc/newlib.sgifixes.patch
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.366569 ork.build.tools-0.0.6/modules/dep/patches/giflib/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.495695 ork.build.tools-0.0.6/modules/dep/patches/giflib/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/giflib/chg/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.496347 ork.build.tools-0.0.6/modules/dep/patches/giflib/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/giflib/ori/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.367203 ork.build.tools-0.0.6/modules/dep/patches/pillar/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.496985 ork.build.tools-0.0.6/modules/dep/patches/pillar/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/pillar/chg/markdown.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.497532 ork.build.tools-0.0.6/modules/dep/patches/pillar/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/patches/pillar/ori/markdown.py
--rw-r--r--   0 michael    (501) wheel        (0)     1748 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pillar.py
--rw-r--r--   0 michael    (501) wheel        (0)     2152 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pkgconfig.py
--rw-r--r--   0 michael    (501) wheel        (0)     1362 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/portaudio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2133 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/postgresql.py
--rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-03-30 23:28:01.000000 ork.build.tools-0.0.6/modules/dep/premake.py
--rw-r--r--   0 michael    (501) wheel        (0)     1526 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ptex.py
--rw-r--r--   0 michael    (501) wheel        (0)     1298 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pugixml.py
--rw-r--r--   0 michael    (501) wheel        (0)     1488 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pybind11.py
--rw-r--r--   0 michael    (501) wheel        (0)     1459 2023-02-05 19:15:34.000000 ork.build.tools-0.0.6/modules/dep/pydefaults.py
--rw-r--r--   0 michael    (501) wheel        (0)      822 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pyopengl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1954 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pyqt5.py
--rw-r--r--   0 michael    (501) wheel        (0)      814 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/pyside2.py
--rw-r--r--   0 michael    (501) wheel        (0)     7450 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/python.py
--rw-r--r--   0 michael    (501) wheel        (0)     5932 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/qt5.py
--rw-r--r--   0 michael    (501) wheel        (0)     1781 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/qt5ct.py
--rw-r--r--   0 michael    (501) wheel        (0)     5913 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/qt5forpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-03-06 06:24:34.000000 ork.build.tools-0.0.6/modules/dep/rapidjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/realsense2.py
--rw-r--r--   0 michael    (501) wheel        (0)     1032 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/root.py
--rw-r--r--   0 michael    (501) wheel        (0)     1344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/rtmidi.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/rv32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1069 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/rv32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-03-30 23:28:01.000000 ork.build.tools-0.0.6/modules/dep/sigslot.py
--rw-r--r--   0 michael    (501) wheel        (0)     1215 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/simavr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/sse2neon.py
--rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/tbb.py
--rw-r--r--   0 michael    (501) wheel        (0)     6552 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/tflite.py
--rw-r--r--   0 michael    (501) wheel        (0)     3343 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ue5.py
--rw-r--r--   0 michael    (501) wheel        (0)     6344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/ue5_cesium.py
--rw-r--r--   0 michael    (501) wheel        (0)     1669 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/unittestpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     2361 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/usd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-03-30 23:28:01.000000 ork.build.tools-0.0.6/modules/dep/vhacd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/modules/dep/vivado.py
--rw-r--r--   0 michael    (501) wheel        (0)     2962 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/vpf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/vrx.py
--rw-r--r--   0 michael    (501) wheel        (0)     1972 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/vst3sdk.py
--rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/dep/vulkan.py
--rw-r--r--   0 michael    (501) wheel        (0)     2772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/wt4.py
--rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-03-30 23:28:01.000000 ork.build.tools-0.0.6/modules/dep/xatlas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1107 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/yarl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1887 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/yosys.py
--rw-r--r--   0 michael    (501) wheel        (0)     1922 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/zephyr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/dep/zmq.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.371478 ork.build.tools-0.0.6/modules/docker/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.498786 ork.build.tools-0.0.6/modules/docker/amigadev/
--rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/docker/amigadev/amigadev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.502632 ork.build.tools-0.0.6/modules/docker/amigadev/test1/
--rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.503130 ork.build.tools-0.0.6/modules/docker/amigadev/test1/S/
--rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/S/Startup-Sequence
--rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/_build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      527 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/build.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.504374 ork.build.tools-0.0.6/modules/docker/amigadev/test1/libs/
--rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
--rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
--rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/main.cpp
--rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/test_fsuae.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/amigadev/test1/test_vamos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.505989 ork.build.tools-0.0.6/modules/docker/androiddev/
--rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/androiddev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2071 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/androiddev/androiddev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.513049 ork.build.tools-0.0.6/modules/docker/cicd/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.520803 ork.build.tools-0.0.6/modules/docker/cicd/bin/
--rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/__init__.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/build_master_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      276 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/build_worker_android_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/build_worker_ub20_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/build_worker_ub22_image.py
--rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/ci_common.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/launch_attached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/launch_detached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/launch_testnossl.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/terminate.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_android.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_ub20.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_ub22.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.530318 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/
--rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/TODO.txt
--rw-r--r--   0 michael    (501) wheel        (0)     9906 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_masterimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     6829 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_watcher.py
--rw-r--r--   0 michael    (501) wheel        (0)     1087 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_workerimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_zmqssh.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.532482 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/
--rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
--rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/index.template
--rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/variant.template
--rw-r--r--   0 michael    (501) wheel        (0)     4134 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/badge.py
--rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/dummy.svg
--rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/httphandler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/master.py
--rw-r--r--   0 michael    (501) wheel        (0)     2597 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/orkbb.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/process_log.py
--rw-r--r--   0 michael    (501) wheel        (0)     7766 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/scheduler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/spin.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/start-master.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/start-worker.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker_build_branch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker_fetch_branch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1708 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/cicd.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.533744 ork.build.tools-0.0.6/modules/docker/cicd/conf/
--rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/conf/nginx_app.conf
--rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/conf/nginx_ssl.conf
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.537899 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
--rw-r--r--   0 michael    (501) wheel        (0)     2641 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
--rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/spin.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/start-master.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/start-worker.sh
--rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/worker.bashrc
--rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/worker.test.sh
--rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/docker-compose-nossl.yml
--rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/docker-compose.yml
--rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/master.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1037 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/master.json
--rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/readme.md
--rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/worker-android.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/worker-ub20.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/worker-ub22.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/worker20.json
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/cicd/worker22.json
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.541407 ork.build.tools-0.0.6/modules/docker/ps1dev/
--rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/Makefile.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/fetch.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2750 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/ps1dev.py
--rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/readme.md
--rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/setup.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.542026 ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/
--rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/project.mk
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.543268 ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/test1/
--rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/test1/Makefile
--rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/test1/test1.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.544518 ork.build.tools-0.0.6/modules/docker/realsense2/
--rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/docker/realsense2/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-02-05 19:12:10.000000 ork.build.tools-0.0.6/modules/docker/realsense2/realsense2.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.546737 ork.build.tools-0.0.6/modules/docker/sagemath/
--rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/sagemath/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/sagemath/docker-compose.yml
--rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/sagemath/entrypoint.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/sagemath/sagemath.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.550040 ork.build.tools-0.0.6/modules/docker/tflow2gpu/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/tflow2gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_mediapipe.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_multi_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_single_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/tflow2gpu/tflow2gpu.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.551481 ork.build.tools-0.0.6/modules/docker/ub-focal/
--rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ub-focal/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1702 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/docker/ub-focal/ub-focal.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.553511 ork.build.tools-0.0.6/modules/host/
--rw-r--r--   0 michael    (501) wheel        (0)     1181 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/host/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-03-06 06:24:34.000000 ork.build.tools-0.0.6/modules/host/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-05-09 20:23:50.000000 ork.build.tools-0.0.6/modules/host/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     2165 2023-04-05 23:31:27.000000 ork.build.tools-0.0.6/modules/host/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.556327 ork.build.tools-0.0.6/modules/sdk/
--rw-r--r--   0 michael    (501) wheel        (0)     4088 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/sdk/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)     1678 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/sdk/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      782 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/sdk/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/sdk/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)      618 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/sdk/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      625 2023-04-05 23:26:33.000000 ork.build.tools-0.0.6/modules/sdk/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.558217 ork.build.tools-0.0.6/modules/subspace/
--rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-06-24 23:47:10.000000 ork.build.tools-0.0.6/modules/subspace/conda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1227 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/subspace/host.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.558685 ork.build.tools-0.0.6/modules/subspace/nnsvs/
--rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-05-09 20:23:50.000000 ork.build.tools-0.0.6/modules/subspace/nnsvs/test.py
--rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-06-24 23:47:10.000000 ork.build.tools-0.0.6/modules/subspace/nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1187 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/subspace/yo.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.561444 ork.build.tools-0.0.6/modules/target/
--rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/modules/target/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.563241 ork.build.tools-0.0.6/ork.build.tools.egg-info/
--rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 20:53:09.000000 ork.build.tools-0.0.6/ork.build.tools.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    10884 2023-07-14 20:53:09.000000 ork.build.tools-0.0.6/ork.build.tools.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 20:53:09.000000 ork.build.tools-0.0.6/ork.build.tools.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) wheel        (0)        9 2023-07-14 20:53:09.000000 ork.build.tools-0.0.6/ork.build.tools.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-14 20:53:09.571326 ork.build.tools-0.0.6/setup.cfg
--rw-r--r--   0 michael    (501) wheel        (0)      997 2023-07-14 20:53:00.000000 ork.build.tools-0.0.6/setup.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.564139 ork.build.tools-0.0.6/tests/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.566425 ork.build.tools-0.0.6/tests/docker-gpu/
--rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu/launch_glmark.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu/launch_nvtopo.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.568813 ork.build.tools-0.0.6/tests/docker-gpu-tensorflow/
--rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu-tensorflow/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu-tensorflow/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu-tensorflow/launch_nvtopo.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/docker-gpu-tensorflow/launch_tf.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-14 17:52:14.000000 ork.build.tools-0.0.6/tests/litex1_nx4.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      178 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/osx_rpaths.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 20:53:09.569977 ork.build.tools-0.0.6/tests/pytorch/
--rwxr-xr-x   0 michael    (501) wheel        (0)      916 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/pytorch/install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2022-09-08 21:51:24.000000 ork.build.tools-0.0.6/tests/pytorch/training.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.218805 ork.build.tools-0.0.7/
+-rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 21:16:02.218249 ork.build.tools-0.0.7/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    14749 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/README.md
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.058156 ork.build.tools-0.0.7/bin_priv/
+-rw-r--r--   0 michael    (501) wheel        (0)        0 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/__init__.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      332 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.build.all.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1965 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1312 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.findtext.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1810 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3223 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.replacetext.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      206 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.require.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      840 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.shell.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2298 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.dep.status.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1612 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1107 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1240 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.kill.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2422 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      780 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1429 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.docker.method.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      708 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.ext.find.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1311 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.find.in.dep.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      649 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.find.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1099 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.host.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1839 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.installedacontainers.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       83 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.ix.udevrules.reload.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      977 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.litex.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      241 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.litex.zephyrriscv-env.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1406 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.litex.zephyrriscv-sample.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       97 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.lsttys.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     6545 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.lsusbx.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       99 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.lsvideo.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.osx.macho.fixup.libs.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      359 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.osx.macho.showinstallname.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      350 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.osx.macho.showlibs.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      163 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.pip.install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1782 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.replace.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1377 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.sdk.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      955 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.sdk.install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1640 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.subspace.build.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.subspace.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      802 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.subspace.list.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1262 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.target.info.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2901 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.vivado.getsites.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2566 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.vivado.launch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2441 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_priv/obt.vscode.create.debug.task.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.064813 ork.build.tools-0.0.7/bin_pub/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     5555 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.create.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     8042 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.init.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      445 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.gentoo.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2951 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.linuxcnc.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3176 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      734 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/bin_pub/obt.osx.installdeps.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.026483 ork.build.tools-0.0.7/examples/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.065283 ork.build.tools-0.0.7/examples/dep-overrides/
+-rw-r--r--   0 michael    (501) wheel        (0)     1530 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/dep-overrides/orkid.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.069278 ork.build.tools-0.0.7/examples/litex1/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/bit2svf_nexysv.tcl
+-rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/cmod_a7_platform.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/cmod_a7_target.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/nexys_video.py
+-rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/nexysv.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      247 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/soc_arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex1/soc_nexysv.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.072838 ork.build.tools-0.0.7/examples/litex_zephyrtest/
+-rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/CMakeLists.txt
+-rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/LICENSE
+-rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/README.rst
+-rwxr-xr-x   0 michael    (501) wheel        (0)      315 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/build.py
+-rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/main.c
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/prj.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/sample.yaml
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.073295 ork.build.tools-0.0.7/examples/litex_zephyrtest/src/
+-rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build.tools-0.0.7/examples/litex_zephyrtest/src/main.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.034460 ork.build.tools-0.0.7/modules/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.147069 ork.build.tools-0.0.7/modules/dep/
+-rw-r--r--   0 michael    (501) wheel        (0)      718 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-05-09 20:23:50.000000 ork.build.tools-0.0.7/modules/dep/_nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1910 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/apitrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1776 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/arachnepnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1663 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/arm64_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1580 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/arm64_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/assimp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/astcencoder.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1675 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/audiofile.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1611 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/avr_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2206 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/avr_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2209 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/avr_libc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1793 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/bazel.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1302 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/blosc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     9272 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/boost.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1248 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/bullet.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2004 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/calf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1541 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/cgal.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/clang.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1408 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/cmake.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/cpppeglib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1632 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/cppzmq.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1563 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/csvparser.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1684 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/curlpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/cycles.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/depthaicore.py
+-rw-r--r--   0 michael    (501) wheel        (0)      992 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/drawtext.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1491 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/easyprof.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-02-18 06:09:54.000000 ork.build.tools-0.0.7/modules/dep/eigen.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2047 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/embree.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1871 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/faust.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1577 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/fcollada.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1737 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ffmpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/flatcam.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1676 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/fltk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1891 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/fluidsynth.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1866 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/frameretrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1438 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/gcode_gpr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2148 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/giflib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1175 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/gitpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2601 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/glfw.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-02-18 06:09:54.000000 ork.build.tools-0.0.7/modules/dep/glm.py
+-rw-r--r--   0 michael    (501) wheel        (0)      894 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/gnutar.py
+-rw-r--r--   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/houdini.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1731 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/icestorm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-03-18 06:31:34.000000 ork.build.tools-0.0.7/modules/dep/igl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1767 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/irix65_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6593 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/irix65_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1150 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/irrlicht.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3478 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ispc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2331 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ispctexc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/jpegturbo.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/klein.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1079 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/lapack.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1065 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/lemongraph.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-06-17 04:32:01.000000 ork.build.tools-0.0.7/modules/dep/lexertl14.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/libcurl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1701 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/libfive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1490 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/libpqpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1425 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/libsocket.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-05-12 22:40:05.000000 ork.build.tools-0.0.7/modules/dep/libsurvive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/libtorch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1926 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/linuxcnc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/modules/dep/litex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2529 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/llvm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1339 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/lm32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1066 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/lm32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2937 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/lua.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2135 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/luajit.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/m68k_amiga_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1555 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/m68k_amiga_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3841 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/minetest.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2009 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/moltenvk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1244 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/nextpnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2117 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ngc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-04-27 00:04:32.000000 ork.build.tools-0.0.7/modules/dep/nlohmannjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1633 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/nss.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1464 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/nsync_cpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3022 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/nvtt.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1562 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ocio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/oiio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1738 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/oneapimkl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1406 2023-04-27 00:04:41.000000 ork.build.tools-0.0.7/modules/dep/openblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-04-25 17:02:18.000000 ork.build.tools-0.0.7/modules/dep/opencv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/opencv_contrib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1217 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/opendb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/openexr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1332 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/openjpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1270 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/openroad.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1791 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/opensubdiv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/openvdb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1376 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/openvr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-06-23 17:21:13.000000 ork.build.tools-0.0.7/modules/dep/orkid.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1306 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/osgeolaszip.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1495 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/osgeoliblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/osgeoproj.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1543 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/osgeotiff.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/osl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/ozzanim.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pangolin.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/parsertl14.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.028165 ork.build.tools-0.0.7/modules/dep/patches/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.027321 ork.build.tools-0.0.7/modules/dep/patches/boost/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.148159 ork.build.tools-0.0.7/modules/dep/patches/boost/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/boost/chg/darwin.jam
+-rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/boost/chg/project-config.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.148629 ork.build.tools-0.0.7/modules/dep/patches/boost/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/boost/ori/darwin.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.151071 ork.build.tools-0.0.7/modules/dep/patches/gcc/
+-rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/gcc/gcc.sgifixes.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/gcc/newlib.sgifixes.patch
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.027894 ork.build.tools-0.0.7/modules/dep/patches/giflib/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.151555 ork.build.tools-0.0.7/modules/dep/patches/giflib/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/giflib/chg/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.152048 ork.build.tools-0.0.7/modules/dep/patches/giflib/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/giflib/ori/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.028510 ork.build.tools-0.0.7/modules/dep/patches/pillar/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.152559 ork.build.tools-0.0.7/modules/dep/patches/pillar/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/pillar/chg/markdown.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.153162 ork.build.tools-0.0.7/modules/dep/patches/pillar/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/patches/pillar/ori/markdown.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1748 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pillar.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2152 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pkgconfig.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1362 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/portaudio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2133 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/postgresql.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-03-30 23:28:01.000000 ork.build.tools-0.0.7/modules/dep/premake.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1526 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ptex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1298 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pugixml.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1488 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pybind11.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1459 2023-02-05 19:15:34.000000 ork.build.tools-0.0.7/modules/dep/pydefaults.py
+-rw-r--r--   0 michael    (501) wheel        (0)      822 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pyopengl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1954 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pyqt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)      814 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/pyside2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7450 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/python.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5932 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/qt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1781 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/qt5ct.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5913 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/qt5forpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-03-06 06:24:34.000000 ork.build.tools-0.0.7/modules/dep/rapidjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/realsense2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1032 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/root.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/rtmidi.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/rv32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1069 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/rv32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-03-30 23:28:01.000000 ork.build.tools-0.0.7/modules/dep/sigslot.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1215 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/simavr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/sse2neon.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/tbb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6552 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/tflite.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3343 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ue5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/ue5_cesium.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1669 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/unittestpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2361 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/usd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-03-30 23:28:01.000000 ork.build.tools-0.0.7/modules/dep/vhacd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/modules/dep/vivado.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2962 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/vpf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/vrx.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1972 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/vst3sdk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/dep/vulkan.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/wt4.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-03-30 23:28:01.000000 ork.build.tools-0.0.7/modules/dep/xatlas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1107 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/yarl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1887 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/yosys.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1922 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/zephyr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/dep/zmq.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.033032 ork.build.tools-0.0.7/modules/docker/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.154202 ork.build.tools-0.0.7/modules/docker/amigadev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/docker/amigadev/amigadev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.157882 ork.build.tools-0.0.7/modules/docker/amigadev/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.158342 ork.build.tools-0.0.7/modules/docker/amigadev/test1/S/
+-rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/S/Startup-Sequence
+-rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/_build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      527 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/build.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.159385 ork.build.tools-0.0.7/modules/docker/amigadev/test1/libs/
+-rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
+-rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
+-rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/main.cpp
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/test_fsuae.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/amigadev/test1/test_vamos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.160324 ork.build.tools-0.0.7/modules/docker/androiddev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/androiddev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2071 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/androiddev/androiddev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.165591 ork.build.tools-0.0.7/modules/docker/cicd/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.171716 ork.build.tools-0.0.7/modules/docker/cicd/bin/
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/__init__.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/build_master_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      276 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/build_worker_android_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/build_worker_ub20_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/build_worker_ub22_image.py
+-rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/ci_common.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/launch_attached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/launch_detached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/launch_testnossl.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/terminate.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_android.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_ub20.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_ub22.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.180796 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/
+-rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/TODO.txt
+-rw-r--r--   0 michael    (501) wheel        (0)     9906 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_masterimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6829 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_watcher.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1087 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_workerimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_zmqssh.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.182391 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/
+-rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
+-rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/index.template
+-rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/variant.template
+-rw-r--r--   0 michael    (501) wheel        (0)     4134 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/badge.py
+-rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/dummy.svg
+-rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/httphandler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/master.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2597 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/orkbb.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/process_log.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7766 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/scheduler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/spin.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/start-master.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/start-worker.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker_build_branch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker_fetch_branch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1708 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/cicd.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.183378 ork.build.tools-0.0.7/modules/docker/cicd/conf/
+-rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/conf/nginx_app.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/conf/nginx_ssl.conf
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.186824 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2641 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
+-rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/spin.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/start-master.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/start-worker.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/worker.bashrc
+-rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/worker.test.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/docker-compose-nossl.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/docker-compose.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/master.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1037 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/master.json
+-rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/readme.md
+-rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/worker-android.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/worker-ub20.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/worker-ub22.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/worker20.json
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/cicd/worker22.json
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.189741 ork.build.tools-0.0.7/modules/docker/ps1dev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/Makefile.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/fetch.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2750 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/ps1dev.py
+-rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/readme.md
+-rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/setup.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.190317 ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/
+-rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/project.mk
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.191514 ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/test1/Makefile
+-rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/test1/test1.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.192473 ork.build.tools-0.0.7/modules/docker/realsense2/
+-rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/docker/realsense2/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-02-05 19:12:10.000000 ork.build.tools-0.0.7/modules/docker/realsense2/realsense2.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.194474 ork.build.tools-0.0.7/modules/docker/sagemath/
+-rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/sagemath/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/sagemath/docker-compose.yml
+-rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/sagemath/entrypoint.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/sagemath/sagemath.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.196849 ork.build.tools-0.0.7/modules/docker/tflow2gpu/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/tflow2gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_mediapipe.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_multi_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_single_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/tflow2gpu/tflow2gpu.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.197764 ork.build.tools-0.0.7/modules/docker/ub-focal/
+-rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ub-focal/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1702 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/docker/ub-focal/ub-focal.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.199562 ork.build.tools-0.0.7/modules/host/
+-rw-r--r--   0 michael    (501) wheel        (0)     1181 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/host/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-03-06 06:24:34.000000 ork.build.tools-0.0.7/modules/host/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-05-09 20:23:50.000000 ork.build.tools-0.0.7/modules/host/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2165 2023-04-05 23:31:27.000000 ork.build.tools-0.0.7/modules/host/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.202686 ork.build.tools-0.0.7/modules/sdk/
+-rw-r--r--   0 michael    (501) wheel        (0)     4088 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/sdk/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1678 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/sdk/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      782 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/sdk/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/sdk/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)      618 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/sdk/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      625 2023-04-05 23:26:33.000000 ork.build.tools-0.0.7/modules/sdk/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.204728 ork.build.tools-0.0.7/modules/subspace/
+-rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-06-24 23:47:10.000000 ork.build.tools-0.0.7/modules/subspace/conda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1227 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/subspace/host.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.205289 ork.build.tools-0.0.7/modules/subspace/nnsvs/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-05-09 20:23:50.000000 ork.build.tools-0.0.7/modules/subspace/nnsvs/test.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-06-24 23:47:10.000000 ork.build.tools-0.0.7/modules/subspace/nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1187 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/subspace/yo.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.209130 ork.build.tools-0.0.7/modules/target/
+-rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/modules/target/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.211850 ork.build.tools-0.0.7/ork.build.tools.egg-info/
+-rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 21:16:01.000000 ork.build.tools-0.0.7/ork.build.tools.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    12117 2023-07-14 21:16:02.000000 ork.build.tools-0.0.7/ork.build.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 21:16:01.000000 ork.build.tools-0.0.7/ork.build.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        9 2023-07-14 21:16:01.000000 ork.build.tools-0.0.7/ork.build.tools.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-14 21:16:02.218934 ork.build.tools-0.0.7/setup.cfg
+-rw-r--r--   0 michael    (501) wheel        (0)     1494 2023-07-14 21:15:58.000000 ork.build.tools-0.0.7/setup.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.212882 ork.build.tools-0.0.7/tests/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.214801 ork.build.tools-0.0.7/tests/docker-gpu/
+-rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu/launch_glmark.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu/launch_nvtopo.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.216686 ork.build.tools-0.0.7/tests/docker-gpu-tensorflow/
+-rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu-tensorflow/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu-tensorflow/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu-tensorflow/launch_nvtopo.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/docker-gpu-tensorflow/launch_tf.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-14 17:52:14.000000 ork.build.tools-0.0.7/tests/litex1_nx4.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      178 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/osx_rpaths.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 21:16:02.217595 ork.build.tools-0.0.7/tests/pytorch/
+-rwxr-xr-x   0 michael    (501) wheel        (0)      916 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/pytorch/install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2022-09-08 21:51:24.000000 ork.build.tools-0.0.7/tests/pytorch/training.py
```

### Comparing `ork.build.tools-0.0.6/PKG-INFO` & `ork.build.tools-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build.tools
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 
 # ORK.BUILD TOOLS (OBT)  
 
 ## [BuildStatus](https://www.orkid-engine.dev:4431)
 
 * Ubuntu 22.04 [![CISTATUS](https://www.orkid-engine.dev:4431/orkdotbuild-ix-ub2204/develop/status.svg)](https://www.orkid-engine.dev:4431)
```

### Comparing `ork.build.tools-0.0.6/README.md` & `ork.build.tools-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.build.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.findtext.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.findtext.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.info.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.info.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.list.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.list.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.replacetext.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.replacetext.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.shell.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.shell.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.dep.status.py` & `ork.build.tools-0.0.7/bin_priv/obt.dep.status.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.build.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.info.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.info.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.kill.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.kill.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.launch.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.list.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.list.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.docker.method.py` & `ork.build.tools-0.0.7/bin_priv/obt.docker.method.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.ext.find.py` & `ork.build.tools-0.0.7/bin_priv/obt.ext.find.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.find.in.dep.py` & `ork.build.tools-0.0.7/bin_priv/obt.find.in.dep.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.find.py` & `ork.build.tools-0.0.7/bin_priv/obt.find.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.host.info.py` & `ork.build.tools-0.0.7/bin_priv/obt.host.info.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.installedacontainers.py` & `ork.build.tools-0.0.7/bin_priv/obt.installedacontainers.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.litex.env.py` & `ork.build.tools-0.0.7/bin_priv/obt.litex.env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.litex.zephyrriscv-sample.py` & `ork.build.tools-0.0.7/bin_priv/obt.litex.zephyrriscv-sample.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.lsusbx.py` & `ork.build.tools-0.0.7/bin_priv/obt.lsusbx.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.osx.macho.fixup.libs.py` & `ork.build.tools-0.0.7/bin_priv/obt.osx.macho.fixup.libs.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.replace.py` & `ork.build.tools-0.0.7/bin_priv/obt.replace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.sdk.info.py` & `ork.build.tools-0.0.7/bin_priv/obt.sdk.info.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.sdk.install.py` & `ork.build.tools-0.0.7/bin_priv/obt.sdk.install.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.subspace.build.py` & `ork.build.tools-0.0.7/bin_priv/obt.subspace.build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.subspace.launch.py` & `ork.build.tools-0.0.7/bin_priv/obt.subspace.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.subspace.list.py` & `ork.build.tools-0.0.7/bin_priv/obt.subspace.list.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.target.info.py` & `ork.build.tools-0.0.7/bin_priv/obt.target.info.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.vivado.getsites.py` & `ork.build.tools-0.0.7/bin_priv/obt.vivado.getsites.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.vivado.launch.py` & `ork.build.tools-0.0.7/bin_priv/obt.vivado.launch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_priv/obt.vscode.create.debug.task.py` & `ork.build.tools-0.0.7/bin_priv/obt.vscode.create.debug.task.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.create.env.py` & `ork.build.tools-0.0.7/bin_pub/obt.create.env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.init.env.py` & `ork.build.tools-0.0.7/bin_pub/obt.init.env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.linuxcnc.py` & `ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py` & `ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py` & `ork.build.tools-0.0.7/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/bin_pub/obt.osx.installdeps.py` & `ork.build.tools-0.0.7/bin_pub/obt.osx.installdeps.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/dep-overrides/orkid.py` & `ork.build.tools-0.0.7/examples/dep-overrides/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/arty.py` & `ork.build.tools-0.0.7/examples/litex1/arty.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/cmod_a7_platform.py` & `ork.build.tools-0.0.7/examples/litex1/cmod_a7_platform.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/cmod_a7_target.py` & `ork.build.tools-0.0.7/examples/litex1/cmod_a7_target.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/nexys_video.py` & `ork.build.tools-0.0.7/examples/litex1/nexys_video.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/nexysv.cfg` & `ork.build.tools-0.0.7/examples/litex1/nexysv.cfg`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex1/soc_nexysv.py` & `ork.build.tools-0.0.7/examples/litex1/soc_nexysv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex_zephyrtest/LICENSE` & `ork.build.tools-0.0.7/examples/litex_zephyrtest/LICENSE`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex_zephyrtest/README.rst` & `ork.build.tools-0.0.7/examples/litex_zephyrtest/README.rst`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex_zephyrtest/sample.yaml` & `ork.build.tools-0.0.7/examples/litex_zephyrtest/sample.yaml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/examples/litex_zephyrtest/src/main.c` & `ork.build.tools-0.0.7/examples/litex_zephyrtest/src/main.c`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/_binutils.py` & `ork.build.tools-0.0.7/modules/dep/_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/_gcc.py` & `ork.build.tools-0.0.7/modules/dep/_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/_nnsvs.py` & `ork.build.tools-0.0.7/modules/dep/_nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/apitrace.py` & `ork.build.tools-0.0.7/modules/dep/apitrace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/arachnepnr.py` & `ork.build.tools-0.0.7/modules/dep/arachnepnr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/arm64_binutils.py` & `ork.build.tools-0.0.7/modules/dep/arm64_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/arm64_gcc.py` & `ork.build.tools-0.0.7/modules/dep/arm64_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/assimp.py` & `ork.build.tools-0.0.7/modules/dep/assimp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/astcencoder.py` & `ork.build.tools-0.0.7/modules/dep/astcencoder.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/audiofile.py` & `ork.build.tools-0.0.7/modules/dep/audiofile.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/avr_binutils.py` & `ork.build.tools-0.0.7/modules/dep/avr_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/avr_gcc.py` & `ork.build.tools-0.0.7/modules/dep/avr_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/avr_libc.py` & `ork.build.tools-0.0.7/modules/dep/avr_libc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/bazel.py` & `ork.build.tools-0.0.7/modules/dep/bazel.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/blosc.py` & `ork.build.tools-0.0.7/modules/dep/blosc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/boost.py` & `ork.build.tools-0.0.7/modules/dep/boost.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/bullet.py` & `ork.build.tools-0.0.7/modules/dep/bullet.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/calf.py` & `ork.build.tools-0.0.7/modules/dep/calf.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cgal.py` & `ork.build.tools-0.0.7/modules/dep/cgal.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/clang.py` & `ork.build.tools-0.0.7/modules/dep/clang.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cmake.py` & `ork.build.tools-0.0.7/modules/dep/cmake.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cpppeglib.py` & `ork.build.tools-0.0.7/modules/dep/cpppeglib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cppzmq.py` & `ork.build.tools-0.0.7/modules/dep/cppzmq.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/csvparser.py` & `ork.build.tools-0.0.7/modules/dep/csvparser.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cuda.py` & `ork.build.tools-0.0.7/modules/dep/cuda.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/curlpp.py` & `ork.build.tools-0.0.7/modules/dep/curlpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/cycles.py` & `ork.build.tools-0.0.7/modules/dep/cycles.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/depthaicore.py` & `ork.build.tools-0.0.7/modules/dep/depthaicore.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/drawtext.py` & `ork.build.tools-0.0.7/modules/dep/drawtext.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/easyprof.py` & `ork.build.tools-0.0.7/modules/dep/easyprof.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/eigen.py` & `ork.build.tools-0.0.7/modules/dep/eigen.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/embree.py` & `ork.build.tools-0.0.7/modules/dep/embree.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/faust.py` & `ork.build.tools-0.0.7/modules/dep/faust.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/fcollada.py` & `ork.build.tools-0.0.7/modules/dep/fcollada.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ffmpeg.py` & `ork.build.tools-0.0.7/modules/dep/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/flatcam.py` & `ork.build.tools-0.0.7/modules/dep/flatcam.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/fltk.py` & `ork.build.tools-0.0.7/modules/dep/fltk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/fluidsynth.py` & `ork.build.tools-0.0.7/modules/dep/fluidsynth.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/frameretrace.py` & `ork.build.tools-0.0.7/modules/dep/frameretrace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/gcode_gpr.py` & `ork.build.tools-0.0.7/modules/dep/gcode_gpr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/giflib.py` & `ork.build.tools-0.0.7/modules/dep/giflib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/gitpython.py` & `ork.build.tools-0.0.7/modules/dep/gitpython.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/glfw.py` & `ork.build.tools-0.0.7/modules/dep/glfw.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/glm.py` & `ork.build.tools-0.0.7/modules/dep/glm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/gnutar.py` & `ork.build.tools-0.0.7/modules/dep/gnutar.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/houdini.py` & `ork.build.tools-0.0.7/modules/dep/houdini.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/icestorm.py` & `ork.build.tools-0.0.7/modules/dep/icestorm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/igl.py` & `ork.build.tools-0.0.7/modules/dep/igl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/irix65_binutils.py` & `ork.build.tools-0.0.7/modules/dep/irix65_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/irix65_gcc.py` & `ork.build.tools-0.0.7/modules/dep/irix65_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/irrlicht.py` & `ork.build.tools-0.0.7/modules/dep/irrlicht.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ispc.py` & `ork.build.tools-0.0.7/modules/dep/ispc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ispctexc.py` & `ork.build.tools-0.0.7/modules/dep/ispctexc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/jpegturbo.py` & `ork.build.tools-0.0.7/modules/dep/jpegturbo.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/klein.py` & `ork.build.tools-0.0.7/modules/dep/klein.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lapack.py` & `ork.build.tools-0.0.7/modules/dep/lapack.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lemongraph.py` & `ork.build.tools-0.0.7/modules/dep/lemongraph.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lexertl14.py` & `ork.build.tools-0.0.7/modules/dep/lexertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libcurl.py` & `ork.build.tools-0.0.7/modules/dep/libcurl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libfive.py` & `ork.build.tools-0.0.7/modules/dep/libfive.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libpqpp.py` & `ork.build.tools-0.0.7/modules/dep/libpqpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libsocket.py` & `ork.build.tools-0.0.7/modules/dep/libsocket.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libsurvive.py` & `ork.build.tools-0.0.7/modules/dep/libsurvive.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/libtorch.py` & `ork.build.tools-0.0.7/modules/dep/libtorch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/linuxcnc.py` & `ork.build.tools-0.0.7/modules/dep/linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/litex.py` & `ork.build.tools-0.0.7/modules/dep/litex.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/llvm.py` & `ork.build.tools-0.0.7/modules/dep/llvm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lm32_binutils.py` & `ork.build.tools-0.0.7/modules/dep/lm32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lm32_gcc.py` & `ork.build.tools-0.0.7/modules/dep/lm32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/lua.py` & `ork.build.tools-0.0.7/modules/dep/lua.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/luajit.py` & `ork.build.tools-0.0.7/modules/dep/luajit.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/m68k_amiga_binutils.py` & `ork.build.tools-0.0.7/modules/dep/m68k_amiga_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/m68k_amiga_gcc.py` & `ork.build.tools-0.0.7/modules/dep/m68k_amiga_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/minetest.py` & `ork.build.tools-0.0.7/modules/dep/minetest.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/moltenvk.py` & `ork.build.tools-0.0.7/modules/dep/moltenvk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/nextpnr.py` & `ork.build.tools-0.0.7/modules/dep/nextpnr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ngc.py` & `ork.build.tools-0.0.7/modules/dep/ngc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/nlohmannjson.py` & `ork.build.tools-0.0.7/modules/dep/nlohmannjson.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/nss.py` & `ork.build.tools-0.0.7/modules/dep/nss.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/nsync_cpp.py` & `ork.build.tools-0.0.7/modules/dep/nsync_cpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/nvtt.py` & `ork.build.tools-0.0.7/modules/dep/nvtt.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ocio.py` & `ork.build.tools-0.0.7/modules/dep/ocio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/oiio.py` & `ork.build.tools-0.0.7/modules/dep/oiio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/oneapimkl.py` & `ork.build.tools-0.0.7/modules/dep/oneapimkl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openblas.py` & `ork.build.tools-0.0.7/modules/dep/openblas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/opencv.py` & `ork.build.tools-0.0.7/modules/dep/opencv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/opencv_contrib.py` & `ork.build.tools-0.0.7/modules/dep/opencv_contrib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/opendb.py` & `ork.build.tools-0.0.7/modules/dep/opendb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openexr.py` & `ork.build.tools-0.0.7/modules/dep/openexr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openjpeg.py` & `ork.build.tools-0.0.7/modules/dep/openjpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openroad.py` & `ork.build.tools-0.0.7/modules/dep/openroad.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/opensubdiv.py` & `ork.build.tools-0.0.7/modules/dep/opensubdiv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openvdb.py` & `ork.build.tools-0.0.7/modules/dep/openvdb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/openvr.py` & `ork.build.tools-0.0.7/modules/dep/openvr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/orkid.py` & `ork.build.tools-0.0.7/modules/dep/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/osgeolaszip.py` & `ork.build.tools-0.0.7/modules/dep/osgeolaszip.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/osgeoliblas.py` & `ork.build.tools-0.0.7/modules/dep/osgeoliblas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/osgeoproj.py` & `ork.build.tools-0.0.7/modules/dep/osgeoproj.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/osgeotiff.py` & `ork.build.tools-0.0.7/modules/dep/osgeotiff.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/osl.py` & `ork.build.tools-0.0.7/modules/dep/osl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ozzanim.py` & `ork.build.tools-0.0.7/modules/dep/ozzanim.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pangolin.py` & `ork.build.tools-0.0.7/modules/dep/pangolin.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/parsertl14.py` & `ork.build.tools-0.0.7/modules/dep/parsertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/boost/chg/darwin.jam` & `ork.build.tools-0.0.7/modules/dep/patches/boost/chg/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/boost/chg/project-config.jam` & `ork.build.tools-0.0.7/modules/dep/patches/boost/chg/project-config.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/boost/ori/darwin.jam` & `ork.build.tools-0.0.7/modules/dep/patches/boost/ori/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/gcc/gcc.sgifixes.patch` & `ork.build.tools-0.0.7/modules/dep/patches/gcc/gcc.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch` & `ork.build.tools-0.0.7/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/gcc/newlib.sgifixes.patch` & `ork.build.tools-0.0.7/modules/dep/patches/gcc/newlib.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/giflib/chg/Makefile` & `ork.build.tools-0.0.7/modules/dep/patches/giflib/chg/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/giflib/ori/Makefile` & `ork.build.tools-0.0.7/modules/dep/patches/giflib/ori/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/pillar/chg/markdown.py` & `ork.build.tools-0.0.7/modules/dep/patches/pillar/chg/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/patches/pillar/ori/markdown.py` & `ork.build.tools-0.0.7/modules/dep/patches/pillar/ori/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pillar.py` & `ork.build.tools-0.0.7/modules/dep/pillar.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pkgconfig.py` & `ork.build.tools-0.0.7/modules/dep/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/portaudio.py` & `ork.build.tools-0.0.7/modules/dep/portaudio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/postgresql.py` & `ork.build.tools-0.0.7/modules/dep/postgresql.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/premake.py` & `ork.build.tools-0.0.7/modules/dep/premake.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ptex.py` & `ork.build.tools-0.0.7/modules/dep/ptex.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pugixml.py` & `ork.build.tools-0.0.7/modules/dep/pugixml.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pybind11.py` & `ork.build.tools-0.0.7/modules/dep/pybind11.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pydefaults.py` & `ork.build.tools-0.0.7/modules/dep/pydefaults.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pyopengl.py` & `ork.build.tools-0.0.7/modules/dep/pyopengl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pyqt5.py` & `ork.build.tools-0.0.7/modules/dep/pyqt5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/pyside2.py` & `ork.build.tools-0.0.7/modules/dep/pyside2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/python.py` & `ork.build.tools-0.0.7/modules/dep/python.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/qt5.py` & `ork.build.tools-0.0.7/modules/dep/qt5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/qt5ct.py` & `ork.build.tools-0.0.7/modules/dep/qt5ct.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/qt5forpython.py` & `ork.build.tools-0.0.7/modules/dep/qt5forpython.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/rapidjson.py` & `ork.build.tools-0.0.7/modules/dep/rapidjson.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/realsense2.py` & `ork.build.tools-0.0.7/modules/dep/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/root.py` & `ork.build.tools-0.0.7/modules/dep/root.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/rtmidi.py` & `ork.build.tools-0.0.7/modules/dep/rtmidi.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/rv32_binutils.py` & `ork.build.tools-0.0.7/modules/dep/rv32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/rv32_gcc.py` & `ork.build.tools-0.0.7/modules/dep/rv32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/sigslot.py` & `ork.build.tools-0.0.7/modules/dep/sigslot.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/simavr.py` & `ork.build.tools-0.0.7/modules/dep/simavr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/sse2neon.py` & `ork.build.tools-0.0.7/modules/dep/sse2neon.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/tbb.py` & `ork.build.tools-0.0.7/modules/dep/tbb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/tflite.py` & `ork.build.tools-0.0.7/modules/dep/tflite.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ue5.py` & `ork.build.tools-0.0.7/modules/dep/ue5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/ue5_cesium.py` & `ork.build.tools-0.0.7/modules/dep/ue5_cesium.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/unittestpp.py` & `ork.build.tools-0.0.7/modules/dep/unittestpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/usd.py` & `ork.build.tools-0.0.7/modules/dep/usd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vhacd.py` & `ork.build.tools-0.0.7/modules/dep/vhacd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vivado.py` & `ork.build.tools-0.0.7/modules/dep/vivado.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vpf.py` & `ork.build.tools-0.0.7/modules/dep/vpf.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vrx.py` & `ork.build.tools-0.0.7/modules/dep/vrx.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vst3sdk.py` & `ork.build.tools-0.0.7/modules/dep/vst3sdk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/vulkan.py` & `ork.build.tools-0.0.7/modules/dep/vulkan.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/wt4.py` & `ork.build.tools-0.0.7/modules/dep/wt4.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/xatlas.py` & `ork.build.tools-0.0.7/modules/dep/xatlas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/yarl.py` & `ork.build.tools-0.0.7/modules/dep/yarl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/yosys.py` & `ork.build.tools-0.0.7/modules/dep/yosys.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/zephyr.py` & `ork.build.tools-0.0.7/modules/dep/zephyr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/dep/zmq.py` & `ork.build.tools-0.0.7/modules/dep/zmq.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/amigadev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/amigadev.py` & `ork.build.tools-0.0.7/modules/docker/amigadev/amigadev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/test1/build.py` & `ork.build.tools-0.0.7/modules/docker/amigadev/test1/build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/test1/libs/mathieeedoubbas.library` & `ork.build.tools-0.0.7/modules/docker/amigadev/test1/libs/mathieeedoubbas.library`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library` & `ork.build.tools-0.0.7/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/test1/main.cpp` & `ork.build.tools-0.0.7/modules/docker/amigadev/test1/main.cpp`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/amigadev/test1/test_fsuae.py` & `ork.build.tools-0.0.7/modules/docker/amigadev/test1/test_fsuae.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/androiddev/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/androiddev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/androiddev/androiddev.py` & `ork.build.tools-0.0.7/modules/docker/androiddev/androiddev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/bin/ci_common.py` & `ork.build.tools-0.0.7/modules/docker/cicd/bin/ci_common.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_android.py` & `ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_ub20.py` & `ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_ub20.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/bin/test_worker_ub22.py` & `ork.build.tools-0.0.7/modules/docker/cicd/bin/test_worker_ub22.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_masterimpl.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_masterimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_watcher.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_watcher.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_workerimpl.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_workerimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/_zmqssh.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/_zmqssh.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/OrkidLogo.png` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/OrkidLogo.png`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/index.template` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/index.template`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/assets/variant.template` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/assets/variant.template`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/badge.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/badge.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/httphandler.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/httphandler.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/master.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/master.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/orkbb.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/orkbb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/process_log.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/process_log.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/scheduler.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/scheduler.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker_build_branch.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker_build_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/ci_impl/worker_fetch_branch.py` & `ork.build.tools-0.0.7/modules/docker/cicd/ci_impl/worker_fetch_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/cicd.py` & `ork.build.tools-0.0.7/modules/docker/cicd/cicd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/conf/nginx_ssl.conf` & `ork.build.tools-0.0.7/modules/docker/cicd/conf/nginx_ssl.conf`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py` & `ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py` & `ork.build.tools-0.0.7/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/docker-compose-nossl.yml` & `ork.build.tools-0.0.7/modules/docker/cicd/docker-compose-nossl.yml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/docker-compose.yml` & `ork.build.tools-0.0.7/modules/docker/cicd/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/master.dockerfile` & `ork.build.tools-0.0.7/modules/docker/cicd/master.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/master.json` & `ork.build.tools-0.0.7/modules/docker/cicd/master.json`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/worker-android.dockerfile` & `ork.build.tools-0.0.7/modules/docker/cicd/worker-android.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/worker-ub20.dockerfile` & `ork.build.tools-0.0.7/modules/docker/cicd/worker-ub20.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/cicd/worker-ub22.dockerfile` & `ork.build.tools-0.0.7/modules/docker/cicd/worker-ub22.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/ps1dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/Makefile.cfg` & `ork.build.tools-0.0.7/modules/docker/ps1dev/Makefile.cfg`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/ps1dev.py` & `ork.build.tools-0.0.7/modules/docker/ps1dev/ps1dev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/setup.sh` & `ork.build.tools-0.0.7/modules/docker/ps1dev/setup.sh`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/project.mk` & `ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/project.mk`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ps1dev/testprograms/test1/test1.c` & `ork.build.tools-0.0.7/modules/docker/ps1dev/testprograms/test1/test1.c`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/realsense2/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/realsense2/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/realsense2/realsense2.py` & `ork.build.tools-0.0.7/modules/docker/realsense2/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/sagemath/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/sagemath/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/sagemath/sagemath.py` & `ork.build.tools-0.0.7/modules/docker/sagemath/sagemath.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/tflow2gpu/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/tflow2gpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_mediapipe.sh` & `ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_mediapipe.sh`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_multi_gpu.py` & `ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_multi_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/tflow2gpu/test_single_gpu.py` & `ork.build.tools-0.0.7/modules/docker/tflow2gpu/test_single_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/tflow2gpu/tflow2gpu.py` & `ork.build.tools-0.0.7/modules/docker/tflow2gpu/tflow2gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ub-focal/Dockerfile` & `ork.build.tools-0.0.7/modules/docker/ub-focal/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/docker/ub-focal/ub-focal.py` & `ork.build.tools-0.0.7/modules/docker/ub-focal/ub-focal.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/host/aarch64-linux.py` & `ork.build.tools-0.0.7/modules/host/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/host/aarch64-macos.py` & `ork.build.tools-0.0.7/modules/host/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/host/x86_64-linux.py` & `ork.build.tools-0.0.7/modules/host/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/host/x86_64-macos.py` & `ork.build.tools-0.0.7/modules/host/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/sdk/aarch64-android.py` & `ork.build.tools-0.0.7/modules/sdk/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/sdk/aarch64-ios.py` & `ork.build.tools-0.0.7/modules/sdk/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/sdk/aarch64-macos.py` & `ork.build.tools-0.0.7/modules/sdk/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/sdk/x86_64-linux.py` & `ork.build.tools-0.0.7/modules/sdk/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/sdk/x86_64-macos.py` & `ork.build.tools-0.0.7/modules/sdk/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/subspace/conda.py` & `ork.build.tools-0.0.7/modules/subspace/conda.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/subspace/host.py` & `ork.build.tools-0.0.7/modules/subspace/host.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/subspace/nnsvs/test.py` & `ork.build.tools-0.0.7/modules/subspace/nnsvs/test.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/subspace/nnsvs.py` & `ork.build.tools-0.0.7/modules/subspace/nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/subspace/yo.py` & `ork.build.tools-0.0.7/modules/subspace/yo.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/aarch64-android.py` & `ork.build.tools-0.0.7/modules/target/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/aarch64-ios.py` & `ork.build.tools-0.0.7/modules/target/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/aarch64-linux.py` & `ork.build.tools-0.0.7/modules/target/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/aarch64-macos.py` & `ork.build.tools-0.0.7/modules/target/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/x86_64-linux.py` & `ork.build.tools-0.0.7/modules/target/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/modules/target/x86_64-macos.py` & `ork.build.tools-0.0.7/modules/target/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/ork.build.tools.egg-info/PKG-INFO` & `ork.build.tools-0.0.7/ork.build.tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build.tools
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 
 # ORK.BUILD TOOLS (OBT)  
 
 ## [BuildStatus](https://www.orkid-engine.dev:4431)
 
 * Ubuntu 22.04 [![CISTATUS](https://www.orkid-engine.dev:4431/orkdotbuild-ix-ub2204/develop/status.svg)](https://www.orkid-engine.dev:4431)
```

### Comparing `ork.build.tools-0.0.6/ork.build.tools.egg-info/SOURCES.txt` & `ork.build.tools-0.0.7/ork.build.tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -37,14 +37,56 @@
 ./bin_priv/obt.subspace.build.py
 ./bin_priv/obt.subspace.launch.py
 ./bin_priv/obt.subspace.list.py
 ./bin_priv/obt.target.info.py
 ./bin_priv/obt.vivado.getsites.py
 ./bin_priv/obt.vivado.launch.py
 ./bin_priv/obt.vscode.create.debug.task.py
+bin_priv/__init__.py
+bin_priv/obt.dep.build.all.py
+bin_priv/obt.dep.build.py
+bin_priv/obt.dep.findtext.py
+bin_priv/obt.dep.info.py
+bin_priv/obt.dep.list.py
+bin_priv/obt.dep.replacetext.py
+bin_priv/obt.dep.require.py
+bin_priv/obt.dep.shell.py
+bin_priv/obt.dep.status.py
+bin_priv/obt.docker.build.py
+bin_priv/obt.docker.info.py
+bin_priv/obt.docker.kill.py
+bin_priv/obt.docker.launch.py
+bin_priv/obt.docker.list.py
+bin_priv/obt.docker.method.py
+bin_priv/obt.ext.find.py
+bin_priv/obt.find.in.dep.py
+bin_priv/obt.find.py
+bin_priv/obt.host.info.py
+bin_priv/obt.installedacontainers.py
+bin_priv/obt.ix.udevrules.reload.py
+bin_priv/obt.litex.env.py
+bin_priv/obt.litex.zephyrriscv-env.sh
+bin_priv/obt.litex.zephyrriscv-sample.py
+bin_priv/obt.lsttys.py
+bin_priv/obt.lsusbx.py
+bin_priv/obt.lsvideo.py
+bin_priv/obt.osx.macho.fixup.libs.py
+bin_priv/obt.osx.macho.showinstallname.py
+bin_priv/obt.osx.macho.showlibs.py
+bin_priv/obt.pip.install.py
+bin_priv/obt.replace.py
+bin_priv/obt.sdk.info.py
+bin_priv/obt.sdk.install.py
+bin_priv/obt.subspace.build.py
+bin_priv/obt.subspace.launch.py
+bin_priv/obt.subspace.list.py
+bin_priv/obt.target.info.py
+bin_priv/obt.vivado.getsites.py
+bin_priv/obt.vivado.launch.py
+bin_priv/obt.vscode.create.debug.task.py
 bin_pub/obt.create.env.py
 bin_pub/obt.init.env.py
 bin_pub/obt.ix.installdeps.gentoo.py
 bin_pub/obt.ix.installdeps.linuxcnc.py
 bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
 bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
 bin_pub/obt.osx.installdeps.py
```

### Comparing `ork.build.tools-0.0.6/tests/litex1_nx4.py` & `ork.build.tools-0.0.7/tests/litex1_nx4.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/tests/pytorch/install.py` & `ork.build.tools-0.0.7/tests/pytorch/install.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.6/tests/pytorch/training.py` & `ork.build.tools-0.0.7/tests/pytorch/training.py`

 * *Files identical despite different names*

