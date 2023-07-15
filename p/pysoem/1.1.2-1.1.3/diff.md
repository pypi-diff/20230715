# Comparing `tmp/pysoem-1.1.2.tar.gz` & `tmp/pysoem-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoem-1.1.2.tar", last modified: Mon Jul 10 18:33:13 2023, max compression
+gzip compressed data, was "pysoem-1.1.3.tar", last modified: Sat Jul 15 07:30:01 2023, max compression
```

## Comparing `pysoem-1.1.2.tar` & `pysoem-1.1.3.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.753751 pysoem-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 18:32:58.000000 pysoem-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 18:32:58.000000 pysoem-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-10 18:33:13.749751 pysoem-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-10 18:32:58.000000 pysoem-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.733750 pysoem-1.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/basic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/find_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/firmware_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/read_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/read_sdo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/write_foe.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 18:32:58.000000 pysoem-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/pysoem/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/cpysoem.pxd
--rw-r--r--   0 runner    (1001) docker     (123)  1335710 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem/pysoem.c
--rw-r--r--   0 runner    (1001) docker     (123)    42367 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/pysoem.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/pysoem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:33:13.753751 pysoem-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-10 18:32:58.000000 pysoem-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/erika/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/erika/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/erika/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/intime/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/intime/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/intime/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/linux/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/linux/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/linux/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/macosx/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/macosx/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/macosx/osal_defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/osal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/rtems/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtems/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtems/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/rtk/
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtk/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtk/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/vxworks/
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/vxworks/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/vxworks/osal_defs.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/win32/
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/inttypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal.c
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal_defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal_win32.h
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/stdint.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/oshw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/erika/
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/intime/
--rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/linux/
--rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/macosx/
--rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtems/
--rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/fec/
--rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.c
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/lw_mac/
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/lw_mac/lw_emac.c
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/lw_mac/lw_emac.h
--rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/vxworks/
--rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/nicdrv.c
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/nicdrv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/oshw.c
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/oshw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/oshw/win32/wpcap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Packet32.h
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Win32-Extensions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/bittypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/ip6_misc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bluetooth.h
--rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bpf.h
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/namedb.h
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/pcap.h
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/sll.h
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/usb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/vlan.h
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-bpf.h
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-namedb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-stdinc.h
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/remote-ext.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/soem/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercat.h
--rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatbase.c
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatbase.h
--rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatcoe.c
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatcoe.h
--rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfig.c
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfig.h
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfiglist.h
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatdc.c
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatdc.h
--rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercateoe.c
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercateoe.h
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatfoe.c
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatfoe.h
--rw-r--r--   0 runner    (1001) docker     (123)    75008 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatmain.c
--rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatmain.h
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatprint.c
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatprint.h
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatsoe.c
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatsoe.h
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercattype.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/intime/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/intime/ec_master/
--rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/intime/ec_master/ec_master.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/aliastool.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/ebox/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/ebox/ebox.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/eepromtool/
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/eepromtool/eepromtool.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/eoe_test/
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/eoe_test/eoe_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/firm_update/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/firm_update/firm_update.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/red_test/
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/red_test/red_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/simple_test/
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/simple_test/simple_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/slaveinfo/
--rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/slaveinfo/slaveinfo.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/rtk/
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/rtk/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/win32/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/ebox/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/ebox/ebox.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/eepromtool/
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/eepromtool/eepromtool.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/firm_update/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/firm_update/firm_update.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/red_test/
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/red_test/red_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/simple_test/
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/simple_test/simple_test.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/slaveinfo/
--rw-r--r--   0 runner    (1001) docker     (123)    22856 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/slaveinfo/slaveinfo.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-15 07:29:47.000000 pysoem-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 07:29:47.000000 pysoem-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-15 07:30:01.198075 pysoem-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-15 07:29:47.000000 pysoem-1.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.178075 pysoem-1.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/find_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/firmware_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/read_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/read_sdo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-15 07:29:47.000000 pysoem-1.1.3/examples/write_foe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-15 07:29:47.000000 pysoem-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/pysoem/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-15 07:29:47.000000 pysoem-1.1.3/pysoem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-15 07:29:47.000000 pysoem-1.1.3/pysoem/cpysoem.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  1343566 2023-07-15 07:30:00.000000 pysoem-1.1.3/pysoem/pysoem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43155 2023-07-15 07:29:47.000000 pysoem-1.1.3/pysoem/pysoem.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/pysoem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-15 07:30:01.000000 pysoem-1.1.3/pysoem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-15 07:30:01.000000 pysoem-1.1.3/pysoem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 07:30:01.000000 pysoem-1.1.3/pysoem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 07:30:01.000000 pysoem-1.1.3/pysoem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 07:30:01.198075 pysoem-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-15 07:29:47.000000 pysoem-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.174075 pysoem-1.1.3/soem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/soem/osal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/soem/osal/erika/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/erika/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/erika/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/soem/osal/intime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/intime/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/intime/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.182075 pysoem-1.1.3/soem/osal/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/linux/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/linux/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/osal/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/macosx/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/macosx/osal_defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/osal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/osal/rtems/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/rtems/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/rtems/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/osal/rtk/
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/rtk/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/rtk/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/osal/vxworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/vxworks/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/vxworks/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/osal/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/win32/inttypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/win32/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/win32/osal_defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/win32/osal_win32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/osal/win32/stdint.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.174075 pysoem-1.1.3/soem/oshw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/oshw/erika/
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/erika/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/erika/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/erika/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/erika/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/oshw/intime/
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/intime/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/intime/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/intime/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/intime/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.186075 pysoem-1.1.3/soem/oshw/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/linux/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/linux/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/linux/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/linux/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/macosx/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/macosx/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/macosx/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/macosx/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/rtems/
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtems/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtems/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtems/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtems/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/rtk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/rtk/fec/
+-rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/fec/fec_ecat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/fec/fec_ecat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/rtk/lw_mac/
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/lw_mac/lw_emac.c
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/lw_mac/lw_emac.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/rtk/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/vxworks/
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/vxworks/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/vxworks/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/vxworks/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/vxworks/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.190075 pysoem-1.1.3/soem/oshw/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.174075 pysoem-1.1.3/soem/oshw/win32/wpcap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.194075 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/Packet32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/Win32-Extensions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/bittypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/ip6_misc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.194075 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/bpf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/namedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/sll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/usb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/vlan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-bpf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-namedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-stdinc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/oshw/win32/wpcap/Include/remote-ext.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/soem/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatbase.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatcoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatcoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatconfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatconfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatconfiglist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatdc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatdc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercateoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercateoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatfoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatfoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    75008 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatmain.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatmain.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatprint.c
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatprint.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatsoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercatsoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/soem/ethercattype.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.174075 pysoem-1.1.3/soem/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.174075 pysoem-1.1.3/soem/test/intime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/intime/ec_master/
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/intime/ec_master/ec_master.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/aliastool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/ebox/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/ebox/ebox.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/eepromtool/
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/eepromtool/eepromtool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/eoe_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/eoe_test/eoe_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/firm_update/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/firm_update/firm_update.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/red_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/red_test/red_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/simple_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/simple_test/simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/linux/slaveinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/linux/slaveinfo/slaveinfo.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/rtk/
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/rtk/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.178075 pysoem-1.1.3/soem/test/win32/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/ebox/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/ebox/ebox.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/eepromtool/
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/eepromtool/eepromtool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/firm_update/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/firm_update/firm_update.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/red_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/red_test/red_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/simple_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/simple_test/simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 07:30:01.198075 pysoem-1.1.3/soem/test/win32/slaveinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)    22856 2023-07-15 07:29:49.000000 pysoem-1.1.3/soem/test/win32/slaveinfo/slaveinfo.c
```

### Comparing `pysoem-1.1.2/LICENSE` & `pysoem-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/PKG-INFO` & `pysoem-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoem
-Version: 1.1.2
+Version: 1.1.3
 Summary: Cython wrapper for the SOEM Library
 Home-page: https://github.com/bnjmnp/pysoem
 Author: Benjamin Partzsch
 Author-email: benjamin_partzsch@web.de
 License: MIT
 Project-URL: Documentation, https://pysoem.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,14 +86,18 @@
 Let's discuss any (major) API change, or large piles of new code first.
 Using `this pysoem chat room on gitter <https://gitter.im/pysoem/pysoem>`_ is one communication channel option.
 
 
 Changes
 -------
 
+v1.1.3
+^^^^^^^
+* Adds function ``_disable_complete_access()`` that stops config_map() from using "complete access" for SDO requests.
+
 v1.1.0
 ^^^^^^^
 * Changed the data type for the ``name`` attribute of SDO info CdefCoeObject and CdefCoeObjectEntry, they are of type bytes now instead of a regular Python 3 string.
 * Also changed the ``desc`` attribute of the ``find_adapters()`` list elements to ``bytes``.
 * Introduces the ``open()`` context manager function.
 * Adds the ``setup_func`` that will maybe later replace the ``config_func``.
```

### Comparing `pysoem-1.1.2/README.rst` & `pysoem-1.1.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 Let's discuss any (major) API change, or large piles of new code first.
 Using `this pysoem chat room on gitter <https://gitter.im/pysoem/pysoem>`_ is one communication channel option.
 
 
 Changes
 -------
 
+v1.1.3
+^^^^^^^
+* Adds function ``_disable_complete_access()`` that stops config_map() from using "complete access" for SDO requests.
+
 v1.1.0
 ^^^^^^^
 * Changed the data type for the ``name`` attribute of SDO info CdefCoeObject and CdefCoeObjectEntry, they are of type bytes now instead of a regular Python 3 string.
 * Also changed the ``desc`` attribute of the ``find_adapters()`` list elements to ``bytes``.
 * Introduces the ``open()`` context manager function.
 * Adds the ``setup_func`` that will maybe later replace the ``config_func``.
```

### Comparing `pysoem-1.1.2/examples/basic_example.py` & `pysoem-1.1.3/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/examples/firmware_update.py` & `pysoem-1.1.3/examples/firmware_update.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/examples/minimal_example.py` & `pysoem-1.1.3/examples/minimal_example.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/examples/read_eeprom.py` & `pysoem-1.1.3/examples/read_eeprom.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/examples/read_sdo_info.py` & `pysoem-1.1.3/examples/read_sdo_info.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/examples/write_foe.py` & `pysoem-1.1.3/examples/write_foe.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/pysoem/cpysoem.pxd` & `pysoem-1.1.3/pysoem/cpysoem.pxd`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/pysoem/pysoem.c` & `pysoem-1.1.3/pysoem/pysoem.c`

 * *Files 0% similar despite different names*

```diff
@@ -1015,15 +1015,15 @@
 struct __pyx_obj_6pysoem_6pysoem_CdefSlave;
 struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject;
 struct __pyx_obj_6pysoem_6pysoem_CdefCoeObjectEntry;
 struct __pyx_obj_6pysoem_6pysoem___pyx_scope_struct__open;
 struct __pyx_obj___Pyx_EnumMeta;
 struct __pyx_t_6pysoem_6pysoem_CdefMasterSettings;
 
-/* "pysoem/pysoem.pyx":45
+/* "pysoem/pysoem.pyx":52
  * 
  * 
  * cpdef enum ec_datatype:             # <<<<<<<<<<<<<<
  *     ECT_BOOLEAN         = 0x0001,
  *     ECT_INTEGER8        = 0x0002,
  */
 enum __pyx_t_6pysoem_6pysoem_ec_datatype {
@@ -1052,27 +1052,27 @@
   __pyx_e_6pysoem_6pysoem_ECT_BIT4 = 0x0033,
   __pyx_e_6pysoem_6pysoem_ECT_BIT5 = 0x0034,
   __pyx_e_6pysoem_6pysoem_ECT_BIT6 = 0x0035,
   __pyx_e_6pysoem_6pysoem_ECT_BIT7 = 0x0036,
   __pyx_e_6pysoem_6pysoem_ECT_BIT8 = 0x0037
 };
 
-/* "pysoem/pysoem.pyx":74
+/* "pysoem/pysoem.pyx":81
  *     ECT_BIT8            = 0x0037
  * 
  * cdef struct CdefMasterSettings:             # <<<<<<<<<<<<<<
  *     int* sdo_read_timeout
  *     int* sdo_write_timeout
  */
 struct __pyx_t_6pysoem_6pysoem_CdefMasterSettings {
   int *sdo_read_timeout;
   int *sdo_write_timeout;
 };
 
-/* "pysoem/pysoem.pyx":132
+/* "pysoem/pysoem.pyx":139
  * 
  * 
  * cdef class CdefMaster:             # <<<<<<<<<<<<<<
  *     """Representing a logical EtherCAT master device.
  * 
  */
 struct __pyx_obj_6pysoem_6pysoem_CdefMaster {
@@ -1097,15 +1097,15 @@
   char io_map[0x1000];
   struct __pyx_t_6pysoem_6pysoem_CdefMasterSettings _settings;
   int sdo_read_timeout;
   int sdo_write_timeout;
 };
 
 
-/* "pysoem/pysoem.pyx":554
+/* "pysoem/pysoem.pyx":561
  * 
  * 
  * cdef class _CallbackData:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object slave
  */
 struct __pyx_obj_6pysoem_6pysoem__CallbackData {
@@ -1113,15 +1113,15 @@
   PyObject *slave;
   PyObject *func;
   PyObject *exc_raised;
   PyObject *exc_info;
 };
 
 
-/* "pysoem/pysoem.pyx":575
+/* "pysoem/pysoem.pyx":582
  * 
  * 
  * cdef class CdefSlave:             # <<<<<<<<<<<<<<
  *     """Represents a slave device
  * 
  */
 struct __pyx_obj_6pysoem_6pysoem_CdefSlave {
@@ -1132,15 +1132,15 @@
   struct __pyx_t_6pysoem_6pysoem_CdefMasterSettings *_the_masters_settings;
   PyObject *_pos;
   struct __pyx_obj_6pysoem_6pysoem__CallbackData *_cd;
   ec_ODlistt _ex_odlist;
 };
 
 
-/* "pysoem/pysoem.pyx":1054
+/* "pysoem/pysoem.pyx":1074
  * 
  * 
  * cdef class CdefCoeObject:             # <<<<<<<<<<<<<<
  *     """Object info for objects in the object dictionary.
  * 
  */
 struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject {
@@ -1150,29 +1150,29 @@
   int _item;
   boolean _is_description_read;
   boolean _are_entries_read;
   ec_OElistt _ex_oelist;
 };
 
 
-/* "pysoem/pysoem.pyx":1144
+/* "pysoem/pysoem.pyx":1164
  * 
  * 
  * cdef class CdefCoeObjectEntry:             # <<<<<<<<<<<<<<
  *     cdef cpysoem.ec_OElistt* _ex_oelist
  *     cdef int _item
  */
 struct __pyx_obj_6pysoem_6pysoem_CdefCoeObjectEntry {
   PyObject_HEAD
   ec_OElistt *_ex_oelist;
   int _item;
 };
 
 
-/* "pysoem/pysoem.pyx":95
+/* "pysoem/pysoem.pyx":102
  * 
  * @contextlib.contextmanager
  * def open(ifname):             # <<<<<<<<<<<<<<
  *     """Context manager function to create a Master object.
  * 
  */
 struct __pyx_obj_6pysoem_6pysoem___pyx_scope_struct__open {
@@ -1191,15 +1191,15 @@
  */
 struct __pyx_obj___Pyx_EnumMeta {
   PyHeapTypeObject __pyx_base;
 };
 
 
 
-/* "pysoem/pysoem.pyx":575
+/* "pysoem/pysoem.pyx":582
  * 
  * 
  * cdef class CdefSlave:             # <<<<<<<<<<<<<<
  *     """Represents a slave device
  * 
  */
 
@@ -2291,14 +2291,15 @@
 static const char __pyx_k_get_al_status[] = "_get_al_status";
 static const char __pyx_k_get_data_type[] = "_get_data_type";
 static const char __pyx_k_pysoem_pysoem[] = "pysoem.pysoem";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_start_address[] = "start_address";
 static const char __pyx_k_AttributeError[] = "AttributeError";
 static const char __pyx_k_ConfigMapError[] = "ConfigMapError";
+static const char __pyx_k_ECT_COEDET_SDO[] = "ECT_COEDET_SDO";
 static const char __pyx_k_ECT_REG_WD_DIV[] = "ECT_REG_WD_DIV";
 static const char __pyx_k_ECT_UNSIGNED16[] = "ECT_UNSIGNED16";
 static const char __pyx_k_ECT_UNSIGNED24[] = "ECT_UNSIGNED24";
 static const char __pyx_k_ECT_UNSIGNED32[] = "ECT_UNSIGNED32";
 static const char __pyx_k_ECT_UNSIGNED64[] = "ECT_UNSIGNED64";
 static const char __pyx_k_contextmanager[] = "contextmanager";
 static const char __pyx_k_ecx_readODlist[] = "ecx_readODlist()";
@@ -2310,41 +2311,46 @@
 static const char __pyx_k_SdoError___init[] = "SdoError.__init__";
 static const char __pyx_k_WkcError___init[] = "WkcError.__init__";
 static const char __pyx_k_get_PO2SOconfig[] = "_get_PO2SOconfig";
 static const char __pyx_k_get_object_code[] = "_get_object_code";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_set_PO2SOconfig[] = "_set_PO2SOconfig";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_ECT_COEDET_SDOCA[] = "ECT_COEDET_SDOCA";
 static const char __pyx_k_ECT_OCTET_STRING[] = "ECT_OCTET_STRING";
 static const char __pyx_k_Emergency___init[] = "Emergency.__init__";
 static const char __pyx_k_get_expected_wkc[] = "_get_expected_wkc";
 static const char __pyx_k_read_description[] = "_read_description";
 static const char __pyx_k_sync0_cycle_time[] = "sync0_cycle_time";
 static const char __pyx_k_sync0_shift_time[] = "sync0_shift_time";
 static const char __pyx_k_sync1_cycle_time[] = "sync1_cycle_time";
 static const char __pyx_k_unexpected_error[] = "unexpected error";
+static const char __pyx_k_ECT_COEDET_UPLOAD[] = "ECT_COEDET_UPLOAD";
 static const char __pyx_k_UnboundLocalError[] = "UnboundLocalError";
 static const char __pyx_k_get_PO2SOconfigEx[] = "_get_PO2SOconfigEx";
 static const char __pyx_k_pysoem_pysoem_pyx[] = "pysoem/pysoem.pyx";
 static const char __pyx_k_set_PO2SOconfigEx[] = "_set_PO2SOconfigEx";
 static const char __pyx_k_CdefCoeObjectEntry[] = "CdefCoeObjectEntry";
+static const char __pyx_k_ECT_COEDET_SDOINFO[] = "ECT_COEDET_SDOINFO";
 static const char __pyx_k_ECT_UNICODE_STRING[] = "ECT_UNICODE_STRING";
 static const char __pyx_k_ECT_VISIBLE_STRING[] = "ECT_VISIBLE_STRING";
 static const char __pyx_k_EEPROM_write_error[] = "EEPROM write error";
 static const char __pyx_k_EepromError___init[] = "EepromError.__init__";
 static const char __pyx_k_PacketError___init[] = "PacketError.__init__";
 static const char __pyx_k_Pyx_EnumBase___new[] = "__Pyx_EnumBase.__new__";
 static const char __pyx_k_Pyx_EnumBase___str[] = "__Pyx_EnumBase.__str__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_ECT_REG_WD_TIME_PDI[] = "ECT_REG_WD_TIME_PDI";
 static const char __pyx_k_ECT_TIME_DIFFERENCE[] = "ECT_TIME_DIFFERENCE";
 static const char __pyx_k_MailboxError___init[] = "MailboxError.__init__";
 static const char __pyx_k_Pyx_EnumBase___repr[] = "__Pyx_EnumBase.__repr__";
 static const char __pyx_k_SdoInfoError___init[] = "SdoInfoError.__init__";
 static const char __pyx_k_manual_state_change[] = "manual_state_change";
+static const char __pyx_k_ECT_COEDET_PDOASSIGN[] = "ECT_COEDET_PDOASSIGN";
+static const char __pyx_k_ECT_COEDET_PDOCONFIG[] = "ECT_COEDET_PDOCONFIG";
 static const char __pyx_k_Unknown_enum_value_s[] = "Unknown enum value: '%s'";
 static const char __pyx_k_ConfigMapError___init[] = "ConfigMapError.__init__";
 static const char __pyx_k_PacketError__get_desc[] = "PacketError._get_desc";
 static const char __pyx_k_ecx_readODdescription[] = "ecx_readODdescription()";
 static const char __pyx_k_collect_mailbox_errors[] = "_collect_mailbox_errors";
 static const char __pyx_k_unexpected_error_Etype[] = "unexpected error, Etype: {}";
 static const char __pyx_k_get_manual_state_change[] = "_get_manual_state_change";
@@ -2397,14 +2403,20 @@
 static PyObject *__pyx_n_s_ECT_BIT3;
 static PyObject *__pyx_n_s_ECT_BIT4;
 static PyObject *__pyx_n_s_ECT_BIT5;
 static PyObject *__pyx_n_s_ECT_BIT6;
 static PyObject *__pyx_n_s_ECT_BIT7;
 static PyObject *__pyx_n_s_ECT_BIT8;
 static PyObject *__pyx_n_s_ECT_BOOLEAN;
+static PyObject *__pyx_n_s_ECT_COEDET_PDOASSIGN;
+static PyObject *__pyx_n_s_ECT_COEDET_PDOCONFIG;
+static PyObject *__pyx_n_s_ECT_COEDET_SDO;
+static PyObject *__pyx_n_s_ECT_COEDET_SDOCA;
+static PyObject *__pyx_n_s_ECT_COEDET_SDOINFO;
+static PyObject *__pyx_n_s_ECT_COEDET_UPLOAD;
 static PyObject *__pyx_n_s_ECT_DOMAIN;
 static PyObject *__pyx_n_s_ECT_INTEGER16;
 static PyObject *__pyx_n_s_ECT_INTEGER24;
 static PyObject *__pyx_n_s_ECT_INTEGER32;
 static PyObject *__pyx_n_s_ECT_INTEGER64;
 static PyObject *__pyx_n_s_ECT_INTEGER8;
 static PyObject *__pyx_n_s_ECT_OCTET_STRING;
@@ -2728,38 +2740,39 @@
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_16recover(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_timeout); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_18eeprom_read(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_word_address, PyObject *__pyx_v_timeout); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_20eeprom_write(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_word_address, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_22foe_write(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_password, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_24foe_read(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_password, PyObject *__pyx_v_size, PyObject *__pyx_v_timeout); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_26amend_mbx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_mailbox, PyObject *__pyx_v_start_address, PyObject *__pyx_v_size); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_28set_watchdog(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_wd_type, PyObject *__pyx_v_wd_time_ms); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_30_fprd(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, int __pyx_v_size, PyObject *__pyx_v_timeout_us); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fpwr(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout_us); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_34_get_name(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_eep_man(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_id(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_rev(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_46_set_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_50_get_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_52_set_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_54_get_input(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_58_set_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_60_get_al_status(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_64_set_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_66_get_od(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_30_disable_complete_access(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fprd(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, int __pyx_v_size, PyObject *__pyx_v_timeout_us); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_34_fpwr(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout_us); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_name(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_man(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_id(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_eep_rev(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_46_get_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_50_set_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_52_get_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_54_set_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_input(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_58_get_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_60_set_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_al_status(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_64_get_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_66_set_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_68_get_od(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_3_cd___get__(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
 static int __pyx_pf_6pysoem_6pysoem_9CdefSlave_3_cd_2__set__(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_6pysoem_6pysoem_9CdefSlave_3_cd_4__del__(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_68__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_70__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_70__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_72__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_6pysoem_6pysoem_13CdefCoeObject___init__(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self, int __pyx_v_item); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_2_read_description(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_4_read_entries(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_6_get_index(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_8_get_data_type(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_10_get_object_code(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6pysoem_6pysoem_13CdefCoeObject_12_get_name(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self); /* proto */
@@ -2794,22 +2807,25 @@
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_keys = {0, &__pyx_n_s_keys, 0, 0, 0};
 static PyObject *__pyx_float_1000000_0;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_3;
+static PyObject *__pyx_int_4;
 static PyObject *__pyx_int_8;
 static PyObject *__pyx_int_10;
 static PyObject *__pyx_int_11;
+static PyObject *__pyx_int_16;
 static PyObject *__pyx_int_20;
 static PyObject *__pyx_int_22;
 static PyObject *__pyx_int_24;
 static PyObject *__pyx_int_26;
 static PyObject *__pyx_int_28;
+static PyObject *__pyx_int_32;
 static PyObject *__pyx_int_40;
 static PyObject *__pyx_int_500;
 static PyObject *__pyx_int_1024;
 static PyObject *__pyx_int_1040;
 static PyObject *__pyx_int_1056;
 static PyObject *__pyx_int_2000;
 static PyObject *__pyx_int_2048;
@@ -2870,15 +2886,15 @@
 static PyObject *__pyx_codeobj__40;
 static PyObject *__pyx_codeobj__42;
 static PyObject *__pyx_codeobj__45;
 static PyObject *__pyx_codeobj__47;
 static PyObject *__pyx_codeobj__49;
 /* Late includes */
 
-/* "pysoem/pysoem.pyx":78
+/* "pysoem/pysoem.pyx":85
  *     int* sdo_write_timeout
  * 
  * def find_adapters():             # <<<<<<<<<<<<<<
  *     """Create a list of available network adapters.
  * 
  */
 
@@ -2915,36 +2931,36 @@
   int __pyx_t_10;
   ec_adaptert *__pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_adapters", 0);
 
-  /* "pysoem/pysoem.pyx":85
+  /* "pysoem/pysoem.pyx":92
  * 
  *     """
  *     cdef cpysoem.ec_adaptert* _ec_adapter = cpysoem.ec_find_adapters()             # <<<<<<<<<<<<<<
  *     Adapter = collections.namedtuple('Adapter', ['name', 'desc'])
  *     adapters = []
  */
   __pyx_v__ec_adapter = ec_find_adapters();
 
-  /* "pysoem/pysoem.pyx":86
+  /* "pysoem/pysoem.pyx":93
  *     """
  *     cdef cpysoem.ec_adaptert* _ec_adapter = cpysoem.ec_find_adapters()
  *     Adapter = collections.namedtuple('Adapter', ['name', 'desc'])             # <<<<<<<<<<<<<<
  *     adapters = []
  *     while not _ec_adapter == NULL:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_collections); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_collections); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_name);
   __Pyx_GIVEREF(__pyx_n_s_name);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_name);
   __Pyx_INCREF(__pyx_n_s_desc);
   __Pyx_GIVEREF(__pyx_n_s_desc);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_desc);
@@ -2959,83 +2975,83 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_s_Adapter, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_s_Adapter, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_s_Adapter);
     __Pyx_GIVEREF(__pyx_n_s_Adapter);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_n_s_Adapter);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_Adapter = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":87
+  /* "pysoem/pysoem.pyx":94
  *     cdef cpysoem.ec_adaptert* _ec_adapter = cpysoem.ec_find_adapters()
  *     Adapter = collections.namedtuple('Adapter', ['name', 'desc'])
  *     adapters = []             # <<<<<<<<<<<<<<
  *     while not _ec_adapter == NULL:
  *         adapters.append(Adapter(_ec_adapter.name.decode('utf8'), _ec_adapter.desc))
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_adapters = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":88
+  /* "pysoem/pysoem.pyx":95
  *     Adapter = collections.namedtuple('Adapter', ['name', 'desc'])
  *     adapters = []
  *     while not _ec_adapter == NULL:             # <<<<<<<<<<<<<<
  *         adapters.append(Adapter(_ec_adapter.name.decode('utf8'), _ec_adapter.desc))
  *         _ec_adapter = _ec_adapter.next
  */
   while (1) {
     __pyx_t_7 = ((!((__pyx_v__ec_adapter == NULL) != 0)) != 0);
     if (!__pyx_t_7) break;
 
-    /* "pysoem/pysoem.pyx":89
+    /* "pysoem/pysoem.pyx":96
  *     adapters = []
  *     while not _ec_adapter == NULL:
  *         adapters.append(Adapter(_ec_adapter.name.decode('utf8'), _ec_adapter.desc))             # <<<<<<<<<<<<<<
  *         _ec_adapter = _ec_adapter.next
  *     return adapters
  */
     __pyx_t_8 = __pyx_v__ec_adapter->name;
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_8, 0, strlen(__pyx_t_8), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_8, 0, strlen(__pyx_t_8), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v__ec_adapter->desc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v__ec_adapter->desc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_Adapter);
     __pyx_t_2 = __pyx_v_Adapter; __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
@@ -3045,76 +3061,76 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_5, __pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_5, __pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_adapters, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_adapters, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":90
+    /* "pysoem/pysoem.pyx":97
  *     while not _ec_adapter == NULL:
  *         adapters.append(Adapter(_ec_adapter.name.decode('utf8'), _ec_adapter.desc))
  *         _ec_adapter = _ec_adapter.next             # <<<<<<<<<<<<<<
  *     return adapters
  * 
  */
     __pyx_t_11 = __pyx_v__ec_adapter->next;
     __pyx_v__ec_adapter = __pyx_t_11;
   }
 
-  /* "pysoem/pysoem.pyx":91
+  /* "pysoem/pysoem.pyx":98
  *         adapters.append(Adapter(_ec_adapter.name.decode('utf8'), _ec_adapter.desc))
  *         _ec_adapter = _ec_adapter.next
  *     return adapters             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_adapters);
   __pyx_r = __pyx_v_adapters;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":78
+  /* "pysoem/pysoem.pyx":85
  *     int* sdo_write_timeout
  * 
  * def find_adapters():             # <<<<<<<<<<<<<<
  *     """Create a list of available network adapters.
  * 
  */
 
@@ -3133,15 +3149,15 @@
   __Pyx_XDECREF(__pyx_v_adapters);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6pysoem_6pysoem_4generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pysoem/pysoem.pyx":95
+/* "pysoem/pysoem.pyx":102
  * 
  * @contextlib.contextmanager
  * def open(ifname):             # <<<<<<<<<<<<<<
  *     """Context manager function to create a Master object.
  * 
  */
 
@@ -3168,23 +3184,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
   __pyx_cur_scope = (struct __pyx_obj_6pysoem_6pysoem___pyx_scope_struct__open *)__pyx_tp_new_6pysoem_6pysoem___pyx_scope_struct__open(__pyx_ptype_6pysoem_6pysoem___pyx_scope_struct__open, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6pysoem_6pysoem___pyx_scope_struct__open *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 95, __pyx_L1_error)
+    __PYX_ERR(0, 102, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_ifname = __pyx_v_ifname;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_ifname);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_ifname);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6pysoem_6pysoem_4generator, __pyx_codeobj_, (PyObject *) __pyx_cur_scope, __pyx_n_s_open, __pyx_n_s_open, __pyx_n_s_pysoem_pysoem); if (unlikely(!gen)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6pysoem_6pysoem_4generator, __pyx_codeobj_, (PyObject *) __pyx_cur_scope, __pyx_n_s_open, __pyx_n_s_open, __pyx_n_s_pysoem_pysoem); if (unlikely(!gen)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3212,71 +3228,71 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L4_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 102, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":100
+  /* "pysoem/pysoem.pyx":107
  *     .. versionadded:: 1.1.0
  *     """
  *     master = Master()             # <<<<<<<<<<<<<<
  *     master.open(ifname)
  *     yield master
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Master); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Master); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_master = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":101
+  /* "pysoem/pysoem.pyx":108
  *     """
  *     master = Master()
  *     master.open(ifname)             # <<<<<<<<<<<<<<
  *     yield master
  *     master.close()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_master, __pyx_n_s_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_master, __pyx_n_s_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_cur_scope->__pyx_v_ifname) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_cur_scope->__pyx_v_ifname);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":102
+  /* "pysoem/pysoem.pyx":109
  *     master = Master()
  *     master.open(ifname)
  *     yield master             # <<<<<<<<<<<<<<
  *     master.close()
  * 
  */
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_master);
@@ -3284,44 +3300,44 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   /* return from generator, yielding value */
   __pyx_generator->resume_label = 1;
   return __pyx_r;
   __pyx_L4_resume_from_yield:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 109, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":103
+  /* "pysoem/pysoem.pyx":110
  *     master.open(ifname)
  *     yield master
  *     master.close()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_master, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_master, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "pysoem/pysoem.pyx":95
+  /* "pysoem/pysoem.pyx":102
  * 
  * @contextlib.contextmanager
  * def open(ifname):             # <<<<<<<<<<<<<<
  *     """Context manager function to create a Master object.
  * 
  */
 
@@ -3340,15 +3356,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":106
+/* "pysoem/pysoem.pyx":113
  * 
  * 
  * def al_status_code_to_string(code):             # <<<<<<<<<<<<<<
  *     """Look up text string that belongs to AL status code.
  * 
  */
 
@@ -3374,32 +3390,32 @@
   char *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("al_status_code_to_string", 0);
 
-  /* "pysoem/pysoem.pyx":116
+  /* "pysoem/pysoem.pyx":123
  * 
  *     """
  *     return cpysoem.ec_ALstatuscode2string(code).decode('utf8');             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_code); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_code); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L1_error)
   __pyx_t_2 = ec_ALstatuscode2string(__pyx_t_1);
-  __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_2, 0, strlen(__pyx_t_2), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_decode_c_string(__pyx_t_2, 0, strlen(__pyx_t_2), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":106
+  /* "pysoem/pysoem.pyx":113
  * 
  * 
  * def al_status_code_to_string(code):             # <<<<<<<<<<<<<<
  *     """Look up text string that belongs to AL status code.
  * 
  */
 
@@ -3410,15 +3426,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":174
+/* "pysoem/pysoem.pyx":181
  *     manual_state_change = property(_get_manual_state_change, _set_manual_state_change)
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.port = &self._ecx_port
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]
  */
 
@@ -3443,252 +3459,252 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "pysoem/pysoem.pyx":175
+  /* "pysoem/pysoem.pyx":182
  * 
  *     def __cinit__(self):
  *         self._ecx_contextt.port = &self._ecx_port             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]
  *         self._ecx_contextt.slavecount = &self._ec_slavecount
  */
   __pyx_v_self->_ecx_contextt.port = (&__pyx_v_self->_ecx_port);
 
-  /* "pysoem/pysoem.pyx":176
+  /* "pysoem/pysoem.pyx":183
  *     def __cinit__(self):
  *         self._ecx_contextt.port = &self._ecx_port
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.slavecount = &self._ec_slavecount
  *         self._ecx_contextt.maxslave = EC_MAXSLAVE
  */
   __pyx_v_self->_ecx_contextt.slavelist = (&(__pyx_v_self->_ec_slave[0]));
 
-  /* "pysoem/pysoem.pyx":177
+  /* "pysoem/pysoem.pyx":184
  *         self._ecx_contextt.port = &self._ecx_port
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]
  *         self._ecx_contextt.slavecount = &self._ec_slavecount             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.maxslave = EC_MAXSLAVE
  *         self._ecx_contextt.grouplist = &self._ec_group[0]
  */
   __pyx_v_self->_ecx_contextt.slavecount = (&__pyx_v_self->_ec_slavecount);
 
-  /* "pysoem/pysoem.pyx":178
+  /* "pysoem/pysoem.pyx":185
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]
  *         self._ecx_contextt.slavecount = &self._ec_slavecount
  *         self._ecx_contextt.maxslave = EC_MAXSLAVE             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.grouplist = &self._ec_group[0]
  *         self._ecx_contextt.maxgroup = EC_MAXGROUP
  */
   __pyx_v_self->_ecx_contextt.maxslave = 0xC8;
 
-  /* "pysoem/pysoem.pyx":179
+  /* "pysoem/pysoem.pyx":186
  *         self._ecx_contextt.slavecount = &self._ec_slavecount
  *         self._ecx_contextt.maxslave = EC_MAXSLAVE
  *         self._ecx_contextt.grouplist = &self._ec_group[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.maxgroup = EC_MAXGROUP
  *         self._ecx_contextt.esibuf = &self._ec_esibuf[0]
  */
   __pyx_v_self->_ecx_contextt.grouplist = (&(__pyx_v_self->_ec_group[0]));
 
-  /* "pysoem/pysoem.pyx":180
+  /* "pysoem/pysoem.pyx":187
  *         self._ecx_contextt.maxslave = EC_MAXSLAVE
  *         self._ecx_contextt.grouplist = &self._ec_group[0]
  *         self._ecx_contextt.maxgroup = EC_MAXGROUP             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.esibuf = &self._ec_esibuf[0]
  *         self._ecx_contextt.esimap = &self._ec_esimap[0]
  */
   __pyx_v_self->_ecx_contextt.maxgroup = 1;
 
-  /* "pysoem/pysoem.pyx":181
+  /* "pysoem/pysoem.pyx":188
  *         self._ecx_contextt.grouplist = &self._ec_group[0]
  *         self._ecx_contextt.maxgroup = EC_MAXGROUP
  *         self._ecx_contextt.esibuf = &self._ec_esibuf[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.esimap = &self._ec_esimap[0]
  *         self._ecx_contextt.esislave = 0
  */
   __pyx_v_self->_ecx_contextt.esibuf = (&(__pyx_v_self->_ec_esibuf[0]));
 
-  /* "pysoem/pysoem.pyx":182
+  /* "pysoem/pysoem.pyx":189
  *         self._ecx_contextt.maxgroup = EC_MAXGROUP
  *         self._ecx_contextt.esibuf = &self._ec_esibuf[0]
  *         self._ecx_contextt.esimap = &self._ec_esimap[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.esislave = 0
  *         self._ecx_contextt.elist = &self._ec_elist
  */
   __pyx_v_self->_ecx_contextt.esimap = (&(__pyx_v_self->_ec_esimap[0]));
 
-  /* "pysoem/pysoem.pyx":183
+  /* "pysoem/pysoem.pyx":190
  *         self._ecx_contextt.esibuf = &self._ec_esibuf[0]
  *         self._ecx_contextt.esimap = &self._ec_esimap[0]
  *         self._ecx_contextt.esislave = 0             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.elist = &self._ec_elist
  *         self._ecx_contextt.idxstack = &self._ec_idxstack
  */
   __pyx_v_self->_ecx_contextt.esislave = 0;
 
-  /* "pysoem/pysoem.pyx":184
+  /* "pysoem/pysoem.pyx":191
  *         self._ecx_contextt.esimap = &self._ec_esimap[0]
  *         self._ecx_contextt.esislave = 0
  *         self._ecx_contextt.elist = &self._ec_elist             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.idxstack = &self._ec_idxstack
  *         self._EcatError = 0
  */
   __pyx_v_self->_ecx_contextt.elist = (&__pyx_v_self->_ec_elist);
 
-  /* "pysoem/pysoem.pyx":185
+  /* "pysoem/pysoem.pyx":192
  *         self._ecx_contextt.esislave = 0
  *         self._ecx_contextt.elist = &self._ec_elist
  *         self._ecx_contextt.idxstack = &self._ec_idxstack             # <<<<<<<<<<<<<<
  *         self._EcatError = 0
  *         self._ecx_contextt.ecaterror = &self._EcatError
  */
   __pyx_v_self->_ecx_contextt.idxstack = (&__pyx_v_self->_ec_idxstack);
 
-  /* "pysoem/pysoem.pyx":186
+  /* "pysoem/pysoem.pyx":193
  *         self._ecx_contextt.elist = &self._ec_elist
  *         self._ecx_contextt.idxstack = &self._ec_idxstack
  *         self._EcatError = 0             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.ecaterror = &self._EcatError
  *         self._ecx_contextt.DCtime = &self._ec_DCtime
  */
   __pyx_v_self->_EcatError = 0;
 
-  /* "pysoem/pysoem.pyx":187
+  /* "pysoem/pysoem.pyx":194
  *         self._ecx_contextt.idxstack = &self._ec_idxstack
  *         self._EcatError = 0
  *         self._ecx_contextt.ecaterror = &self._EcatError             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.DCtime = &self._ec_DCtime
  *         self._ecx_contextt.SMcommtype = &self._ec_SMcommtype[0]
  */
   __pyx_v_self->_ecx_contextt.ecaterror = (&__pyx_v_self->_EcatError);
 
-  /* "pysoem/pysoem.pyx":188
+  /* "pysoem/pysoem.pyx":195
  *         self._EcatError = 0
  *         self._ecx_contextt.ecaterror = &self._EcatError
  *         self._ecx_contextt.DCtime = &self._ec_DCtime             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.SMcommtype = &self._ec_SMcommtype[0]
  *         self._ecx_contextt.PDOassign = &self._ec_PDOassign[0]
  */
   __pyx_v_self->_ecx_contextt.DCtime = (&__pyx_v_self->_ec_DCtime);
 
-  /* "pysoem/pysoem.pyx":189
+  /* "pysoem/pysoem.pyx":196
  *         self._ecx_contextt.ecaterror = &self._EcatError
  *         self._ecx_contextt.DCtime = &self._ec_DCtime
  *         self._ecx_contextt.SMcommtype = &self._ec_SMcommtype[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.PDOassign = &self._ec_PDOassign[0]
  *         self._ecx_contextt.PDOdesc = &self._ec_PDOdesc[0]
  */
   __pyx_v_self->_ecx_contextt.SMcommtype = (&(__pyx_v_self->_ec_SMcommtype[0]));
 
-  /* "pysoem/pysoem.pyx":190
+  /* "pysoem/pysoem.pyx":197
  *         self._ecx_contextt.DCtime = &self._ec_DCtime
  *         self._ecx_contextt.SMcommtype = &self._ec_SMcommtype[0]
  *         self._ecx_contextt.PDOassign = &self._ec_PDOassign[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.PDOdesc = &self._ec_PDOdesc[0]
  *         self._ecx_contextt.eepSM = &self._ec_SM
  */
   __pyx_v_self->_ecx_contextt.PDOassign = (&(__pyx_v_self->_ec_PDOassign[0]));
 
-  /* "pysoem/pysoem.pyx":191
+  /* "pysoem/pysoem.pyx":198
  *         self._ecx_contextt.SMcommtype = &self._ec_SMcommtype[0]
  *         self._ecx_contextt.PDOassign = &self._ec_PDOassign[0]
  *         self._ecx_contextt.PDOdesc = &self._ec_PDOdesc[0]             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.eepSM = &self._ec_SM
  *         self._ecx_contextt.eepFMMU = &self._ec_FMMU
  */
   __pyx_v_self->_ecx_contextt.PDOdesc = (&(__pyx_v_self->_ec_PDOdesc[0]));
 
-  /* "pysoem/pysoem.pyx":192
+  /* "pysoem/pysoem.pyx":199
  *         self._ecx_contextt.PDOassign = &self._ec_PDOassign[0]
  *         self._ecx_contextt.PDOdesc = &self._ec_PDOdesc[0]
  *         self._ecx_contextt.eepSM = &self._ec_SM             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.eepFMMU = &self._ec_FMMU
  *         self._ecx_contextt.FOEhook = NULL
  */
   __pyx_v_self->_ecx_contextt.eepSM = (&__pyx_v_self->_ec_SM);
 
-  /* "pysoem/pysoem.pyx":193
+  /* "pysoem/pysoem.pyx":200
  *         self._ecx_contextt.PDOdesc = &self._ec_PDOdesc[0]
  *         self._ecx_contextt.eepSM = &self._ec_SM
  *         self._ecx_contextt.eepFMMU = &self._ec_FMMU             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.FOEhook = NULL
  *         self._ecx_contextt.manualstatechange = 0
  */
   __pyx_v_self->_ecx_contextt.eepFMMU = (&__pyx_v_self->_ec_FMMU);
 
-  /* "pysoem/pysoem.pyx":194
+  /* "pysoem/pysoem.pyx":201
  *         self._ecx_contextt.eepSM = &self._ec_SM
  *         self._ecx_contextt.eepFMMU = &self._ec_FMMU
  *         self._ecx_contextt.FOEhook = NULL             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.manualstatechange = 0
  * 
  */
   __pyx_v_self->_ecx_contextt.FOEhook = NULL;
 
-  /* "pysoem/pysoem.pyx":195
+  /* "pysoem/pysoem.pyx":202
  *         self._ecx_contextt.eepFMMU = &self._ec_FMMU
  *         self._ecx_contextt.FOEhook = NULL
  *         self._ecx_contextt.manualstatechange = 0             # <<<<<<<<<<<<<<
  * 
  *         self.slaves = []
  */
   __pyx_v_self->_ecx_contextt.manualstatechange = 0;
 
-  /* "pysoem/pysoem.pyx":197
+  /* "pysoem/pysoem.pyx":204
  *         self._ecx_contextt.manualstatechange = 0
  * 
  *         self.slaves = []             # <<<<<<<<<<<<<<
  *         self.sdo_read_timeout = 700000
  *         self.sdo_write_timeout = 700000
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves, __pyx_t_1) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":198
+  /* "pysoem/pysoem.pyx":205
  * 
  *         self.slaves = []
  *         self.sdo_read_timeout = 700000             # <<<<<<<<<<<<<<
  *         self.sdo_write_timeout = 700000
  *         self._settings.sdo_read_timeout = &self.sdo_read_timeout
  */
   __pyx_v_self->sdo_read_timeout = 0xAAE60;
 
-  /* "pysoem/pysoem.pyx":199
+  /* "pysoem/pysoem.pyx":206
  *         self.slaves = []
  *         self.sdo_read_timeout = 700000
  *         self.sdo_write_timeout = 700000             # <<<<<<<<<<<<<<
  *         self._settings.sdo_read_timeout = &self.sdo_read_timeout
  *         self._settings.sdo_write_timeout = &self.sdo_write_timeout
  */
   __pyx_v_self->sdo_write_timeout = 0xAAE60;
 
-  /* "pysoem/pysoem.pyx":200
+  /* "pysoem/pysoem.pyx":207
  *         self.sdo_read_timeout = 700000
  *         self.sdo_write_timeout = 700000
  *         self._settings.sdo_read_timeout = &self.sdo_read_timeout             # <<<<<<<<<<<<<<
  *         self._settings.sdo_write_timeout = &self.sdo_write_timeout
  * 
  */
   __pyx_v_self->_settings.sdo_read_timeout = (&__pyx_v_self->sdo_read_timeout);
 
-  /* "pysoem/pysoem.pyx":201
+  /* "pysoem/pysoem.pyx":208
  *         self.sdo_write_timeout = 700000
  *         self._settings.sdo_read_timeout = &self.sdo_read_timeout
  *         self._settings.sdo_write_timeout = &self.sdo_write_timeout             # <<<<<<<<<<<<<<
  * 
  *     def open(self, ifname):
  */
   __pyx_v_self->_settings.sdo_write_timeout = (&__pyx_v_self->sdo_write_timeout);
 
-  /* "pysoem/pysoem.pyx":174
+  /* "pysoem/pysoem.pyx":181
  *     manual_state_change = property(_get_manual_state_change, _set_manual_state_change)
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self._ecx_contextt.port = &self._ecx_port
  *         self._ecx_contextt.slavelist = &self._ec_slave[0]
  */
 
@@ -3700,15 +3716,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":203
+/* "pysoem/pysoem.pyx":210
  *         self._settings.sdo_write_timeout = &self.sdo_write_timeout
  * 
  *     def open(self, ifname):             # <<<<<<<<<<<<<<
  *         """Initialize and open network interface.
  * 
  */
 
@@ -3737,96 +3753,96 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "pysoem/pysoem.pyx":213
+  /* "pysoem/pysoem.pyx":220
  *                 you have no permission to open the interface
  *         """
  *         ret_val = cpysoem.ecx_init(&self._ecx_contextt, ifname.encode('utf8'))             # <<<<<<<<<<<<<<
  *         if ret_val == 0:
  *             raise ConnectionError('could not open interface {}'.format(ifname))
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ifname, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_ifname, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
   __pyx_v_ret_val = ecx_init((&__pyx_v_self->_ecx_contextt), __pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":214
+  /* "pysoem/pysoem.pyx":221
  *         """
  *         ret_val = cpysoem.ecx_init(&self._ecx_contextt, ifname.encode('utf8'))
  *         if ret_val == 0:             # <<<<<<<<<<<<<<
  *             raise ConnectionError('could not open interface {}'.format(ifname))
  * 
  */
   __pyx_t_5 = ((__pyx_v_ret_val == 0) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "pysoem/pysoem.pyx":215
+    /* "pysoem/pysoem.pyx":222
  *         ret_val = cpysoem.ecx_init(&self._ecx_contextt, ifname.encode('utf8'))
  *         if ret_val == 0:
  *             raise ConnectionError('could not open interface {}'.format(ifname))             # <<<<<<<<<<<<<<
  * 
  *     def config_init(self, usetable=False):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ConnectionError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ConnectionError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_could_not_open_interface, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_could_not_open_interface, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_ifname) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_ifname);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 215, __pyx_L1_error)
+    __PYX_ERR(0, 222, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":214
+    /* "pysoem/pysoem.pyx":221
  *         """
  *         ret_val = cpysoem.ecx_init(&self._ecx_contextt, ifname.encode('utf8'))
  *         if ret_val == 0:             # <<<<<<<<<<<<<<
  *             raise ConnectionError('could not open interface {}'.format(ifname))
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":203
+  /* "pysoem/pysoem.pyx":210
  *         self._settings.sdo_write_timeout = &self.sdo_write_timeout
  * 
  *     def open(self, ifname):             # <<<<<<<<<<<<<<
  *         """Initialize and open network interface.
  * 
  */
 
@@ -3842,15 +3858,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":217
+/* "pysoem/pysoem.pyx":224
  *             raise ConnectionError('could not open interface {}'.format(ifname))
  * 
  *     def config_init(self, usetable=False):             # <<<<<<<<<<<<<<
  *         """Enumerate and init all slaves.
  * 
  */
 
@@ -3883,29 +3899,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_usetable);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "config_init") < 0)) __PYX_ERR(0, 217, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "config_init") < 0)) __PYX_ERR(0, 224, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_usetable = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("config_init", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 217, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("config_init", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 224, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.config_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_10CdefMaster_4config_init(((struct __pyx_obj_6pysoem_6pysoem_CdefMaster *)__pyx_v_self), __pyx_v_usetable);
 
@@ -3931,104 +3947,104 @@
   PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("config_init", 0);
 
-  /* "pysoem/pysoem.pyx":226
+  /* "pysoem/pysoem.pyx":233
  *             int: Working counter of slave discover datagram = number of slaves found, -1 when no slave is connected
  *         """
  *         ret_val = cpysoem.ecx_config_init(&self._ecx_contextt, usetable)             # <<<<<<<<<<<<<<
  *         if ret_val > 0:
  *           for i in range(self._ec_slavecount):
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_usetable); if (unlikely((__pyx_t_1 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_usetable); if (unlikely((__pyx_t_1 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L1_error)
   __pyx_v_ret_val = ecx_config_init((&__pyx_v_self->_ecx_contextt), __pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":227
+  /* "pysoem/pysoem.pyx":234
  *         """
  *         ret_val = cpysoem.ecx_config_init(&self._ecx_contextt, usetable)
  *         if ret_val > 0:             # <<<<<<<<<<<<<<
  *           for i in range(self._ec_slavecount):
  *               self.slaves.append(self._get_slave(i))
  */
   __pyx_t_2 = ((__pyx_v_ret_val > 0) != 0);
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":228
+    /* "pysoem/pysoem.pyx":235
  *         ret_val = cpysoem.ecx_config_init(&self._ecx_contextt, usetable)
  *         if ret_val > 0:
  *           for i in range(self._ec_slavecount):             # <<<<<<<<<<<<<<
  *               self.slaves.append(self._get_slave(i))
  *         return ret_val
  */
     __pyx_t_3 = __pyx_v_self->_ec_slavecount;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "pysoem/pysoem.pyx":229
+      /* "pysoem/pysoem.pyx":236
  *         if ret_val > 0:
  *           for i in range(self._ec_slavecount):
  *               self.slaves.append(self._get_slave(i))             # <<<<<<<<<<<<<<
  *         return ret_val
  * 
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_slave); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_slave); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
       __pyx_t_7 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_10, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_9);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 229, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_11 = __Pyx_PyObject_Append(__pyx_t_6, __pyx_t_7); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_Append(__pyx_t_6, __pyx_t_7); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 236, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
 
-    /* "pysoem/pysoem.pyx":227
+    /* "pysoem/pysoem.pyx":234
  *         """
  *         ret_val = cpysoem.ecx_config_init(&self._ecx_contextt, usetable)
  *         if ret_val > 0:             # <<<<<<<<<<<<<<
  *           for i in range(self._ec_slavecount):
  *               self.slaves.append(self._get_slave(i))
  */
   }
 
-  /* "pysoem/pysoem.pyx":230
+  /* "pysoem/pysoem.pyx":237
  *           for i in range(self._ec_slavecount):
  *               self.slaves.append(self._get_slave(i))
  *         return ret_val             # <<<<<<<<<<<<<<
  * 
  *     def config_map(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":217
+  /* "pysoem/pysoem.pyx":224
  *             raise ConnectionError('could not open interface {}'.format(ifname))
  * 
  *     def config_init(self, usetable=False):             # <<<<<<<<<<<<<<
  *         """Enumerate and init all slaves.
  * 
  */
 
@@ -4043,15 +4059,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":232
+/* "pysoem/pysoem.pyx":239
  *         return ret_val
  * 
  *     def config_map(self):             # <<<<<<<<<<<<<<
  *         """Map all slaves PDOs in IO map.
  * 
  */
 
@@ -4086,166 +4102,166 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("config_map", 0);
 
-  /* "pysoem/pysoem.pyx":240
+  /* "pysoem/pysoem.pyx":247
  *         cdef _CallbackData cd
  *         # ecx_config_map_group returns the actual IO map size (not an error value), expect the value to be less than EC_IOMAPSIZE
  *         ret_val = cpysoem.ecx_config_map_group(&self._ecx_contextt, &self.io_map, 0)             # <<<<<<<<<<<<<<
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:
  */
   __pyx_v_ret_val = ecx_config_map_group((&__pyx_v_self->_ecx_contextt), (&__pyx_v_self->io_map), 0);
 
-  /* "pysoem/pysoem.pyx":242
+  /* "pysoem/pysoem.pyx":249
  *         ret_val = cpysoem.ecx_config_map_group(&self._ecx_contextt, &self.io_map, 0)
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:             # <<<<<<<<<<<<<<
  *             cd = slave._cd
  *             if cd.exc_raised:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 242, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 242, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 249, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 242, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 249, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 242, __pyx_L1_error)
+          else __PYX_ERR(0, 249, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_slave, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":243
+    /* "pysoem/pysoem.pyx":250
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:
  *             cd = slave._cd             # <<<<<<<<<<<<<<
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0], cd.exc_info[1], cd.exc_info[2]
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_slave, __pyx_n_s_cd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_slave, __pyx_n_s_cd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 243, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 250, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_cd, ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":244
+    /* "pysoem/pysoem.pyx":251
  *         for slave in self.slaves:
  *             cd = slave._cd
  *             if cd.exc_raised:             # <<<<<<<<<<<<<<
  *                 raise cd.exc_info[0], cd.exc_info[1], cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))
  */
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_cd->exc_raised); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 244, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_cd->exc_raised); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 251, __pyx_L1_error)
     if (unlikely(__pyx_t_5)) {
 
-      /* "pysoem/pysoem.pyx":245
+      /* "pysoem/pysoem.pyx":252
  *             cd = slave._cd
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0], cd.exc_info[1], cd.exc_info[2]             # <<<<<<<<<<<<<<
  *         logger.debug('io map size: {}'.format(ret_val))
  *         # raise an exception if one or more mailbox errors occured within ecx_config_map_group call
  */
-      __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 245, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 245, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_Raise(__pyx_t_1, __pyx_t_6, __pyx_t_7, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 245, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
 
-      /* "pysoem/pysoem.pyx":244
+      /* "pysoem/pysoem.pyx":251
  *         for slave in self.slaves:
  *             cd = slave._cd
  *             if cd.exc_raised:             # <<<<<<<<<<<<<<
  *                 raise cd.exc_info[0], cd.exc_info[1], cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))
  */
     }
 
-    /* "pysoem/pysoem.pyx":242
+    /* "pysoem/pysoem.pyx":249
  *         ret_val = cpysoem.ecx_config_map_group(&self._ecx_contextt, &self.io_map, 0)
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:             # <<<<<<<<<<<<<<
  *             cd = slave._cd
  *             if cd.exc_raised:
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":246
+  /* "pysoem/pysoem.pyx":253
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0], cd.exc_info[1], cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))             # <<<<<<<<<<<<<<
  *         # raise an exception if one or more mailbox errors occured within ecx_config_map_group call
  *         error_list = self._collect_mailbox_errors()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_io_map_size, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_io_map_size, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_9, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -4253,109 +4269,109 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":248
+  /* "pysoem/pysoem.pyx":255
  *         logger.debug('io map size: {}'.format(ret_val))
  *         # raise an exception if one or more mailbox errors occured within ecx_config_map_group call
  *         error_list = self._collect_mailbox_errors()             # <<<<<<<<<<<<<<
  *         if len(error_list) > 0:
  *             raise ConfigMapError(error_list)
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_collect_mailbox_errors); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_collect_mailbox_errors); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_error_list = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":249
+  /* "pysoem/pysoem.pyx":256
  *         # raise an exception if one or more mailbox errors occured within ecx_config_map_group call
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:             # <<<<<<<<<<<<<<
  *             raise ConfigMapError(error_list)
  *         return ret_val
  */
-  __pyx_t_3 = PyObject_Length(__pyx_v_error_list); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_v_error_list); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 256, __pyx_L1_error)
   __pyx_t_5 = ((__pyx_t_3 > 0) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "pysoem/pysoem.pyx":250
+    /* "pysoem/pysoem.pyx":257
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:
  *             raise ConfigMapError(error_list)             # <<<<<<<<<<<<<<
  *         return ret_val
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ConfigMapError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ConfigMapError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_v_error_list) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_error_list);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 250, __pyx_L1_error)
+    __PYX_ERR(0, 257, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":249
+    /* "pysoem/pysoem.pyx":256
  *         # raise an exception if one or more mailbox errors occured within ecx_config_map_group call
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:             # <<<<<<<<<<<<<<
  *             raise ConfigMapError(error_list)
  *         return ret_val
  */
   }
 
-  /* "pysoem/pysoem.pyx":251
+  /* "pysoem/pysoem.pyx":258
  *         if len(error_list) > 0:
  *             raise ConfigMapError(error_list)
  *         return ret_val             # <<<<<<<<<<<<<<
  * 
  *     def config_overlap_map(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":232
+  /* "pysoem/pysoem.pyx":239
  *         return ret_val
  * 
  *     def config_map(self):             # <<<<<<<<<<<<<<
  *         """Map all slaves PDOs in IO map.
  * 
  */
 
@@ -4374,15 +4390,15 @@
   __Pyx_XDECREF(__pyx_v_slave);
   __Pyx_XDECREF(__pyx_v_error_list);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":253
+/* "pysoem/pysoem.pyx":260
  *         return ret_val
  * 
  *     def config_overlap_map(self):             # <<<<<<<<<<<<<<
  *         """Map all slaves PDOs to overlapping IO map.
  * 
  */
 
@@ -4417,166 +4433,166 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("config_overlap_map", 0);
 
-  /* "pysoem/pysoem.pyx":261
+  /* "pysoem/pysoem.pyx":268
  *         cdef _CallbackData cd
  *         # ecx_config_map_group returns the actual IO map size (not an error value), expect the value to be less than EC_IOMAPSIZE
  *         ret_val = cpysoem.ecx_config_overlap_map_group(&self._ecx_contextt, &self.io_map, 0)             # <<<<<<<<<<<<<<
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:
  */
   __pyx_v_ret_val = ecx_config_overlap_map_group((&__pyx_v_self->_ecx_contextt), (&__pyx_v_self->io_map), 0);
 
-  /* "pysoem/pysoem.pyx":263
+  /* "pysoem/pysoem.pyx":270
  *         ret_val = cpysoem.ecx_config_overlap_map_group(&self._ecx_contextt, &self.io_map, 0)
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:             # <<<<<<<<<<<<<<
  *             cd = slave._cd
  *             if cd.exc_raised:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_slaves); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 263, __pyx_L1_error)
+          else __PYX_ERR(0, 270, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_slave, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":264
+    /* "pysoem/pysoem.pyx":271
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:
  *             cd = slave._cd             # <<<<<<<<<<<<<<
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0],cd.exc_info[1],cd.exc_info[2]
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_slave, __pyx_n_s_cd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_slave, __pyx_n_s_cd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 264, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_cd, ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":265
+    /* "pysoem/pysoem.pyx":272
  *         for slave in self.slaves:
  *             cd = slave._cd
  *             if cd.exc_raised:             # <<<<<<<<<<<<<<
  *                 raise cd.exc_info[0],cd.exc_info[1],cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))
  */
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_cd->exc_raised); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_cd->exc_raised); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 272, __pyx_L1_error)
     if (unlikely(__pyx_t_5)) {
 
-      /* "pysoem/pysoem.pyx":266
+      /* "pysoem/pysoem.pyx":273
  *             cd = slave._cd
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0],cd.exc_info[1],cd.exc_info[2]             # <<<<<<<<<<<<<<
  *         logger.debug('io map size: {}'.format(ret_val))
  *         # raise an exception if one or more mailbox errors occured within ecx_config_overlap_map_group call
  */
-      __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_cd->exc_info, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_Raise(__pyx_t_1, __pyx_t_6, __pyx_t_7, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 266, __pyx_L1_error)
+      __PYX_ERR(0, 273, __pyx_L1_error)
 
-      /* "pysoem/pysoem.pyx":265
+      /* "pysoem/pysoem.pyx":272
  *         for slave in self.slaves:
  *             cd = slave._cd
  *             if cd.exc_raised:             # <<<<<<<<<<<<<<
  *                 raise cd.exc_info[0],cd.exc_info[1],cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))
  */
     }
 
-    /* "pysoem/pysoem.pyx":263
+    /* "pysoem/pysoem.pyx":270
  *         ret_val = cpysoem.ecx_config_overlap_map_group(&self._ecx_contextt, &self.io_map, 0)
  *         # check for exceptions raised in the config functions
  *         for slave in self.slaves:             # <<<<<<<<<<<<<<
  *             cd = slave._cd
  *             if cd.exc_raised:
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":267
+  /* "pysoem/pysoem.pyx":274
  *             if cd.exc_raised:
  *                 raise cd.exc_info[0],cd.exc_info[1],cd.exc_info[2]
  *         logger.debug('io map size: {}'.format(ret_val))             # <<<<<<<<<<<<<<
  *         # raise an exception if one or more mailbox errors occured within ecx_config_overlap_map_group call
  *         error_list = self._collect_mailbox_errors()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logger); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_io_map_size, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_io_map_size, __pyx_n_s_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_9, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 267, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -4584,109 +4600,109 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":269
+  /* "pysoem/pysoem.pyx":276
  *         logger.debug('io map size: {}'.format(ret_val))
  *         # raise an exception if one or more mailbox errors occured within ecx_config_overlap_map_group call
  *         error_list = self._collect_mailbox_errors()             # <<<<<<<<<<<<<<
  *         if len(error_list) > 0:
  *             raise ConfigMapError(error_list)
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_collect_mailbox_errors); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_collect_mailbox_errors); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_error_list = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":270
+  /* "pysoem/pysoem.pyx":277
  *         # raise an exception if one or more mailbox errors occured within ecx_config_overlap_map_group call
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:             # <<<<<<<<<<<<<<
  *             raise ConfigMapError(error_list)
  * 
  */
-  __pyx_t_3 = PyObject_Length(__pyx_v_error_list); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 270, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_v_error_list); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 277, __pyx_L1_error)
   __pyx_t_5 = ((__pyx_t_3 > 0) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "pysoem/pysoem.pyx":271
+    /* "pysoem/pysoem.pyx":278
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:
  *             raise ConfigMapError(error_list)             # <<<<<<<<<<<<<<
  * 
  *         return ret_val
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ConfigMapError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ConfigMapError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_v_error_list) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_error_list);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 271, __pyx_L1_error)
+    __PYX_ERR(0, 278, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":270
+    /* "pysoem/pysoem.pyx":277
  *         # raise an exception if one or more mailbox errors occured within ecx_config_overlap_map_group call
  *         error_list = self._collect_mailbox_errors()
  *         if len(error_list) > 0:             # <<<<<<<<<<<<<<
  *             raise ConfigMapError(error_list)
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":273
+  /* "pysoem/pysoem.pyx":280
  *             raise ConfigMapError(error_list)
  * 
  *         return ret_val             # <<<<<<<<<<<<<<
  * 
  *     def _collect_mailbox_errors(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_ret_val); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":253
+  /* "pysoem/pysoem.pyx":260
  *         return ret_val
  * 
  *     def config_overlap_map(self):             # <<<<<<<<<<<<<<
  *         """Map all slaves PDOs to overlapping IO map.
  * 
  */
 
@@ -4705,15 +4721,15 @@
   __Pyx_XDECREF(__pyx_v_slave);
   __Pyx_XDECREF(__pyx_v_error_list);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":275
+/* "pysoem/pysoem.pyx":282
  *         return ret_val
  * 
  *     def _collect_mailbox_errors(self):             # <<<<<<<<<<<<<<
  *         # collect SDO or mailbox errors that occurred during PDO configuration read in ecx_config_map_group
  *         error_list = []
  */
 
@@ -4750,90 +4766,90 @@
   int __pyx_t_13;
   char *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_collect_mailbox_errors", 0);
 
-  /* "pysoem/pysoem.pyx":277
+  /* "pysoem/pysoem.pyx":284
  *     def _collect_mailbox_errors(self):
  *         # collect SDO or mailbox errors that occurred during PDO configuration read in ecx_config_map_group
  *         error_list = []             # <<<<<<<<<<<<<<
  *         cdef cpysoem.ec_errort err
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_error_list = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":279
+  /* "pysoem/pysoem.pyx":286
  *         error_list = []
  *         cdef cpysoem.ec_errort err
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *                 error_list.append(SdoError(err.Slave,
  */
   while (1) {
     __pyx_t_2 = (ecx_poperror((&__pyx_v_self->_ecx_contextt), (&__pyx_v_err)) != 0);
     if (!__pyx_t_2) break;
 
-    /* "pysoem/pysoem.pyx":280
+    /* "pysoem/pysoem.pyx":287
  *         cdef cpysoem.ec_errort err
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:             # <<<<<<<<<<<<<<
  *                 error_list.append(SdoError(err.Slave,
  *                                            err.Index,
  */
     switch (__pyx_v_err.Etype) {
       case EC_ERR_TYPE_SDO_ERROR:
 
-      /* "pysoem/pysoem.pyx":281
+      /* "pysoem/pysoem.pyx":288
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *                 error_list.append(SdoError(err.Slave,             # <<<<<<<<<<<<<<
  *                                            err.Index,
  *                                            err.SubIdx,
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SdoError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SdoError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 288, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "pysoem/pysoem.pyx":282
+      /* "pysoem/pysoem.pyx":289
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *                 error_list.append(SdoError(err.Slave,
  *                                            err.Index,             # <<<<<<<<<<<<<<
  *                                            err.SubIdx,
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))
  */
-      __pyx_t_5 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 282, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 289, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
 
-      /* "pysoem/pysoem.pyx":283
+      /* "pysoem/pysoem.pyx":290
  *                 error_list.append(SdoError(err.Slave,
  *                                            err.Index,
  *                                            err.SubIdx,             # <<<<<<<<<<<<<<
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  */
-      __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_v_err.SubIdx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_v_err.SubIdx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
 
-      /* "pysoem/pysoem.pyx":284
+      /* "pysoem/pysoem.pyx":291
  *                                            err.Index,
  *                                            err.SubIdx,
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))             # <<<<<<<<<<<<<<
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *                 error_list.append(MailboxError(err.Slave,
  */
-      __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_err.AbortCode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_err.AbortCode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = ec_sdoerror2string(__pyx_v_err.AbortCode);
-      __pyx_t_9 = __Pyx_decode_c_string(__pyx_t_8, 0, strlen(__pyx_t_8), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_decode_c_string(__pyx_t_8, 0, strlen(__pyx_t_8), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4842,39 +4858,39 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_9};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_9};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else
       #endif
       {
-        __pyx_t_12 = PyTuple_New(5+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(5+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 288, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (__pyx_t_10) {
           __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_5);
@@ -4887,71 +4903,71 @@
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_11, __pyx_t_9);
         __pyx_t_4 = 0;
         __pyx_t_5 = 0;
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "pysoem/pysoem.pyx":281
+      /* "pysoem/pysoem.pyx":288
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *                 error_list.append(SdoError(err.Slave,             # <<<<<<<<<<<<<<
  *                                            err.Index,
  *                                            err.SubIdx,
  */
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 288, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pysoem/pysoem.pyx":280
+      /* "pysoem/pysoem.pyx":287
  *         cdef cpysoem.ec_errort err
  *         while cpysoem.ecx_poperror(&self._ecx_contextt, &err):
  *             if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:             # <<<<<<<<<<<<<<
  *                 error_list.append(SdoError(err.Slave,
  *                                            err.Index,
  */
       break;
       case EC_ERR_TYPE_MBX_ERROR:
 
-      /* "pysoem/pysoem.pyx":286
+      /* "pysoem/pysoem.pyx":293
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *                 error_list.append(MailboxError(err.Slave,             # <<<<<<<<<<<<<<
  *                                                err.ErrorCode,
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_MailboxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_MailboxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_12 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 286, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 293, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
 
-      /* "pysoem/pysoem.pyx":287
+      /* "pysoem/pysoem.pyx":294
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *                 error_list.append(MailboxError(err.Slave,
  *                                                err.ErrorCode,             # <<<<<<<<<<<<<<
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  */
-      __pyx_t_9 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.ErrorCode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 287, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.ErrorCode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 294, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
 
-      /* "pysoem/pysoem.pyx":288
+      /* "pysoem/pysoem.pyx":295
  *                 error_list.append(MailboxError(err.Slave,
  *                                                err.ErrorCode,
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))             # <<<<<<<<<<<<<<
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *                 error_list.append(PacketError(err.Slave,
  */
       __pyx_t_14 = ec_mbxerror2string(__pyx_v_err.ErrorCode);
-      __pyx_t_7 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 288, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_6 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4960,95 +4976,95 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_12, __pyx_t_9, __pyx_t_7};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_12, __pyx_t_9, __pyx_t_7};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_5 = PyTuple_New(3+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(3+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         if (__pyx_t_6) {
           __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_12);
         PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_11, __pyx_t_12);
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_11, __pyx_t_9);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_11, __pyx_t_7);
         __pyx_t_12 = 0;
         __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "pysoem/pysoem.pyx":286
+      /* "pysoem/pysoem.pyx":293
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *                 error_list.append(MailboxError(err.Slave,             # <<<<<<<<<<<<<<
  *                                                err.ErrorCode,
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  */
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 286, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 293, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pysoem/pysoem.pyx":285
+      /* "pysoem/pysoem.pyx":292
  *                                            err.SubIdx,
  *                                            err.AbortCode, cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:             # <<<<<<<<<<<<<<
  *                 error_list.append(MailboxError(err.Slave,
  *                                                err.ErrorCode,
  */
       break;
       case EC_ERR_TYPE_PACKET_ERROR:
 
-      /* "pysoem/pysoem.pyx":290
+      /* "pysoem/pysoem.pyx":297
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *                 error_list.append(PacketError(err.Slave,             # <<<<<<<<<<<<<<
  *                                               err.ErrorCode))
  *             else:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PacketError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PacketError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
 
-      /* "pysoem/pysoem.pyx":291
+      /* "pysoem/pysoem.pyx":298
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *                 error_list.append(PacketError(err.Slave,
  *                                               err.ErrorCode))             # <<<<<<<<<<<<<<
  *             else:
  *                 error_list.append(Exception('unexpected error'))
  */
-      __pyx_t_7 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.ErrorCode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.ErrorCode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 298, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_9 = NULL;
       __pyx_t_11 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5057,97 +5073,97 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_5, __pyx_t_7};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_5, __pyx_t_7};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (__pyx_t_9) {
           __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_9); __pyx_t_9 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_5);
         PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_7);
         __pyx_t_5 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "pysoem/pysoem.pyx":290
+      /* "pysoem/pysoem.pyx":297
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *                 error_list.append(PacketError(err.Slave,             # <<<<<<<<<<<<<<
  *                                               err.ErrorCode))
  *             else:
  */
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 290, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pysoem/pysoem.pyx":289
+      /* "pysoem/pysoem.pyx":296
  *                                                err.ErrorCode,
  *                                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8')))
  *             elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:             # <<<<<<<<<<<<<<
  *                 error_list.append(PacketError(err.Slave,
  *                                               err.ErrorCode))
  */
       break;
       default:
 
-      /* "pysoem/pysoem.pyx":293
+      /* "pysoem/pysoem.pyx":300
  *                                               err.ErrorCode))
  *             else:
  *                 error_list.append(Exception('unexpected error'))             # <<<<<<<<<<<<<<
  *         return error_list
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 293, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_error_list, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 300, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       break;
     }
   }
 
-  /* "pysoem/pysoem.pyx":294
+  /* "pysoem/pysoem.pyx":301
  *             else:
  *                 error_list.append(Exception('unexpected error'))
  *         return error_list             # <<<<<<<<<<<<<<
  * 
  *     def config_dc(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_error_list);
   __pyx_r = __pyx_v_error_list;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":275
+  /* "pysoem/pysoem.pyx":282
  *         return ret_val
  * 
  *     def _collect_mailbox_errors(self):             # <<<<<<<<<<<<<<
  *         # collect SDO or mailbox errors that occurred during PDO configuration read in ecx_config_map_group
  *         error_list = []
  */
 
@@ -5167,15 +5183,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_error_list);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":296
+/* "pysoem/pysoem.pyx":303
  *         return error_list
  * 
  *     def config_dc(self):             # <<<<<<<<<<<<<<
  *         """Locate DC slaves, measure propagation delays.
  * 
  */
 
@@ -5198,29 +5214,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("config_dc", 0);
 
-  /* "pysoem/pysoem.pyx":302
+  /* "pysoem/pysoem.pyx":309
  *             bool: if slaves are found with DC
  *         """
  *         return cpysoem.ecx_configdc(&self._ecx_contextt)             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int8_t(ecx_configdc((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int8_t(ecx_configdc((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":296
+  /* "pysoem/pysoem.pyx":303
  *         return error_list
  * 
  *     def config_dc(self):             # <<<<<<<<<<<<<<
  *         """Locate DC slaves, measure propagation delays.
  * 
  */
 
@@ -5231,15 +5247,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":304
+/* "pysoem/pysoem.pyx":311
  *         return cpysoem.ecx_configdc(&self._ecx_contextt)
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Close the network interface.
  * 
  */
 
@@ -5258,39 +5274,39 @@
 }
 
 static PyObject *__pyx_pf_6pysoem_6pysoem_10CdefMaster_14close(struct __pyx_obj_6pysoem_6pysoem_CdefMaster *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pysoem/pysoem.pyx":309
+  /* "pysoem/pysoem.pyx":316
  *         """
  *         # ecx_close returns nothing
  *         cpysoem.ecx_close(&self._ecx_contextt)             # <<<<<<<<<<<<<<
  * 
  *     def read_state(self):
  */
   ecx_close((&__pyx_v_self->_ecx_contextt));
 
-  /* "pysoem/pysoem.pyx":304
+  /* "pysoem/pysoem.pyx":311
  *         return cpysoem.ecx_configdc(&self._ecx_contextt)
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Close the network interface.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":311
+/* "pysoem/pysoem.pyx":318
  *         cpysoem.ecx_close(&self._ecx_contextt)
  * 
  *     def read_state(self):             # <<<<<<<<<<<<<<
  *         """Read all slaves states.
  * 
  */
 
@@ -5313,29 +5329,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_state", 0);
 
-  /* "pysoem/pysoem.pyx":317
+  /* "pysoem/pysoem.pyx":324
  *             int: lowest state found
  *         """
  *         return cpysoem.ecx_readstate(&self._ecx_contextt)             # <<<<<<<<<<<<<<
  * 
  *     def write_state(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_readstate((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_readstate((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":311
+  /* "pysoem/pysoem.pyx":318
  *         cpysoem.ecx_close(&self._ecx_contextt)
  * 
  *     def read_state(self):             # <<<<<<<<<<<<<<
  *         """Read all slaves states.
  * 
  */
 
@@ -5346,15 +5362,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":319
+/* "pysoem/pysoem.pyx":326
  *         return cpysoem.ecx_readstate(&self._ecx_contextt)
  * 
  *     def write_state(self):             # <<<<<<<<<<<<<<
  *         """Write all slaves state.
  * 
  */
 
@@ -5377,29 +5393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_state", 0);
 
-  /* "pysoem/pysoem.pyx":327
+  /* "pysoem/pysoem.pyx":334
  *             int: Working counter or EC_NOFRAME
  *         """
  *         return cpysoem.ecx_writestate(&self._ecx_contextt, 0)             # <<<<<<<<<<<<<<
  * 
  *     def state_check(self, int expected_state, timeout=50000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_writestate((&__pyx_v_self->_ecx_contextt), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_writestate((&__pyx_v_self->_ecx_contextt), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":319
+  /* "pysoem/pysoem.pyx":326
  *         return cpysoem.ecx_readstate(&self._ecx_contextt)
  * 
  *     def write_state(self):             # <<<<<<<<<<<<<<
  *         """Write all slaves state.
  * 
  */
 
@@ -5410,15 +5426,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":329
+/* "pysoem/pysoem.pyx":336
  *         return cpysoem.ecx_writestate(&self._ecx_contextt, 0)
  * 
  *     def state_check(self, int expected_state, timeout=50000):             # <<<<<<<<<<<<<<
  *         """Check actual slave state.
  * 
  */
 
@@ -5458,31 +5474,31 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "state_check") < 0)) __PYX_ERR(0, 329, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "state_check") < 0)) __PYX_ERR(0, 336, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_expected_state = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_expected_state == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L3_error)
+    __pyx_v_expected_state = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_expected_state == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L3_error)
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("state_check", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 329, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("state_check", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 336, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.state_check", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_10CdefMaster_20state_check(((struct __pyx_obj_6pysoem_6pysoem_CdefMaster *)__pyx_v_self), __pyx_v_expected_state, __pyx_v_timeout);
 
@@ -5497,30 +5513,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("state_check", 0);
 
-  /* "pysoem/pysoem.pyx":342
+  /* "pysoem/pysoem.pyx":349
  *             int: Requested state, or found state after timeout
  *         """
  *         return cpysoem.ecx_statecheck(&self._ecx_contextt, 0, expected_state, timeout)             # <<<<<<<<<<<<<<
  * 
  *     def send_processdata(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(ecx_statecheck((&__pyx_v_self->_ecx_contextt), 0, __pyx_v_expected_state, __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(ecx_statecheck((&__pyx_v_self->_ecx_contextt), 0, __pyx_v_expected_state, __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":329
+  /* "pysoem/pysoem.pyx":336
  *         return cpysoem.ecx_writestate(&self._ecx_contextt, 0)
  * 
  *     def state_check(self, int expected_state, timeout=50000):             # <<<<<<<<<<<<<<
  *         """Check actual slave state.
  * 
  */
 
@@ -5531,15 +5547,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":344
+/* "pysoem/pysoem.pyx":351
  *         return cpysoem.ecx_statecheck(&self._ecx_contextt, 0, expected_state, timeout)
  * 
  *     def send_processdata(self):             # <<<<<<<<<<<<<<
  *         """Transmit processdata to slaves.
  * 
  */
 
@@ -5562,29 +5578,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_processdata", 0);
 
-  /* "pysoem/pysoem.pyx":358
+  /* "pysoem/pysoem.pyx":365
  *             int: >0 if processdata is transmitted, might only by 0 if config map is not configured properly
  *         """
  *         return cpysoem.ecx_send_processdata(&self._ecx_contextt)             # <<<<<<<<<<<<<<
  * 
  *     def send_overlap_processdata(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_send_processdata((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_send_processdata((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":344
+  /* "pysoem/pysoem.pyx":351
  *         return cpysoem.ecx_statecheck(&self._ecx_contextt, 0, expected_state, timeout)
  * 
  *     def send_processdata(self):             # <<<<<<<<<<<<<<
  *         """Transmit processdata to slaves.
  * 
  */
 
@@ -5595,15 +5611,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":360
+/* "pysoem/pysoem.pyx":367
  *         return cpysoem.ecx_send_processdata(&self._ecx_contextt)
  * 
  *     def send_overlap_processdata(self):             # <<<<<<<<<<<<<<
  *         """Transmit overlap processdata to slaves.
  * 
  */
 
@@ -5626,29 +5642,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_overlap_processdata", 0);
 
-  /* "pysoem/pysoem.pyx":366
+  /* "pysoem/pysoem.pyx":373
  *             int: >0 if processdata is transmitted, might only by 0 if config map is not configured properly
  *         """
  *         return cpysoem.ecx_send_overlap_processdata(&self._ecx_contextt)             # <<<<<<<<<<<<<<
  * 
  *     def receive_processdata(self, timeout=2000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_send_overlap_processdata((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(ecx_send_overlap_processdata((&__pyx_v_self->_ecx_contextt))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":360
+  /* "pysoem/pysoem.pyx":367
  *         return cpysoem.ecx_send_processdata(&self._ecx_contextt)
  * 
  *     def send_overlap_processdata(self):             # <<<<<<<<<<<<<<
  *         """Transmit overlap processdata to slaves.
  * 
  */
 
@@ -5659,15 +5675,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":368
+/* "pysoem/pysoem.pyx":375
  *         return cpysoem.ecx_send_overlap_processdata(&self._ecx_contextt)
  * 
  *     def receive_processdata(self, timeout=2000):             # <<<<<<<<<<<<<<
  *         """Receive processdata from slaves.
  * 
  */
 
@@ -5700,29 +5716,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "receive_processdata") < 0)) __PYX_ERR(0, 368, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "receive_processdata") < 0)) __PYX_ERR(0, 375, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("receive_processdata", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 368, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("receive_processdata", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 375, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.receive_processdata", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_10CdefMaster_26receive_processdata(((struct __pyx_obj_6pysoem_6pysoem_CdefMaster *)__pyx_v_self), __pyx_v_timeout);
 
@@ -5737,30 +5753,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("receive_processdata", 0);
 
-  /* "pysoem/pysoem.pyx":380
+  /* "pysoem/pysoem.pyx":387
  *             int: Working Counter
  *         """
  *         return cpysoem.ecx_receive_processdata(&self._ecx_contextt, timeout)             # <<<<<<<<<<<<<<
  * 
  *     def _get_slave(self, int pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 380, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(ecx_receive_processdata((&__pyx_v_self->_ecx_contextt), __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(ecx_receive_processdata((&__pyx_v_self->_ecx_contextt), __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":368
+  /* "pysoem/pysoem.pyx":375
  *         return cpysoem.ecx_send_overlap_processdata(&self._ecx_contextt)
  * 
  *     def receive_processdata(self, timeout=2000):             # <<<<<<<<<<<<<<
  *         """Receive processdata from slaves.
  * 
  */
 
@@ -5771,15 +5787,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":382
+/* "pysoem/pysoem.pyx":389
  *         return cpysoem.ecx_receive_processdata(&self._ecx_contextt, timeout)
  * 
  *     def _get_slave(self, int pos):             # <<<<<<<<<<<<<<
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')
  */
 
@@ -5790,15 +5806,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_slave (wrapper)", 0);
   assert(__pyx_arg_pos); {
-    __pyx_v_pos = __Pyx_PyInt_As_int(__pyx_arg_pos); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L3_error)
+    __pyx_v_pos = __Pyx_PyInt_As_int(__pyx_arg_pos); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster._get_slave", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -5817,133 +5833,133 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_slave", 0);
 
-  /* "pysoem/pysoem.pyx":383
+  /* "pysoem/pysoem.pyx":390
  * 
  *     def _get_slave(self, int pos):
  *         if pos < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError('requested slave device is not available')
  *         if pos >= self._ec_slavecount:
  */
   __pyx_t_1 = ((__pyx_v_pos < 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":384
+    /* "pysoem/pysoem.pyx":391
  *     def _get_slave(self, int pos):
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')             # <<<<<<<<<<<<<<
  *         if pos >= self._ec_slavecount:
  *             raise IndexError('requested slave device is not available')
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 384, __pyx_L1_error)
+    __PYX_ERR(0, 391, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":383
+    /* "pysoem/pysoem.pyx":390
  * 
  *     def _get_slave(self, int pos):
  *         if pos < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError('requested slave device is not available')
  *         if pos >= self._ec_slavecount:
  */
   }
 
-  /* "pysoem/pysoem.pyx":385
+  /* "pysoem/pysoem.pyx":392
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')
  *         if pos >= self._ec_slavecount:             # <<<<<<<<<<<<<<
  *             raise IndexError('requested slave device is not available')
  *         ethercat_slave = CdefSlave(pos+1)
  */
   __pyx_t_1 = ((__pyx_v_pos >= __pyx_v_self->_ec_slavecount) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":386
+    /* "pysoem/pysoem.pyx":393
  *             raise IndexError('requested slave device is not available')
  *         if pos >= self._ec_slavecount:
  *             raise IndexError('requested slave device is not available')             # <<<<<<<<<<<<<<
  *         ethercat_slave = CdefSlave(pos+1)
  *         ethercat_slave._ecx_contextt = &self._ecx_contextt
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 386, __pyx_L1_error)
+    __PYX_ERR(0, 393, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":385
+    /* "pysoem/pysoem.pyx":392
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')
  *         if pos >= self._ec_slavecount:             # <<<<<<<<<<<<<<
  *             raise IndexError('requested slave device is not available')
  *         ethercat_slave = CdefSlave(pos+1)
  */
   }
 
-  /* "pysoem/pysoem.pyx":387
+  /* "pysoem/pysoem.pyx":394
  *         if pos >= self._ec_slavecount:
  *             raise IndexError('requested slave device is not available')
  *         ethercat_slave = CdefSlave(pos+1)             # <<<<<<<<<<<<<<
  *         ethercat_slave._ecx_contextt = &self._ecx_contextt
  *         ethercat_slave._ec_slave = &self._ec_slave[pos+1] # +1 as _ec_slave[0] is reserved
  */
-  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_pos + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long((__pyx_v_pos + 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave), __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ethercat_slave = ((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":388
+  /* "pysoem/pysoem.pyx":395
  *             raise IndexError('requested slave device is not available')
  *         ethercat_slave = CdefSlave(pos+1)
  *         ethercat_slave._ecx_contextt = &self._ecx_contextt             # <<<<<<<<<<<<<<
  *         ethercat_slave._ec_slave = &self._ec_slave[pos+1] # +1 as _ec_slave[0] is reserved
  *         ethercat_slave._the_masters_settings = &self._settings
  */
   __pyx_v_ethercat_slave->_ecx_contextt = (&__pyx_v_self->_ecx_contextt);
 
-  /* "pysoem/pysoem.pyx":389
+  /* "pysoem/pysoem.pyx":396
  *         ethercat_slave = CdefSlave(pos+1)
  *         ethercat_slave._ecx_contextt = &self._ecx_contextt
  *         ethercat_slave._ec_slave = &self._ec_slave[pos+1] # +1 as _ec_slave[0] is reserved             # <<<<<<<<<<<<<<
  *         ethercat_slave._the_masters_settings = &self._settings
  *         return ethercat_slave
  */
   __pyx_v_ethercat_slave->_ec_slave = (&(__pyx_v_self->_ec_slave[(__pyx_v_pos + 1)]));
 
-  /* "pysoem/pysoem.pyx":390
+  /* "pysoem/pysoem.pyx":397
  *         ethercat_slave._ecx_contextt = &self._ecx_contextt
  *         ethercat_slave._ec_slave = &self._ec_slave[pos+1] # +1 as _ec_slave[0] is reserved
  *         ethercat_slave._the_masters_settings = &self._settings             # <<<<<<<<<<<<<<
  *         return ethercat_slave
  * 
  */
   __pyx_v_ethercat_slave->_the_masters_settings = (&__pyx_v_self->_settings);
 
-  /* "pysoem/pysoem.pyx":391
+  /* "pysoem/pysoem.pyx":398
  *         ethercat_slave._ec_slave = &self._ec_slave[pos+1] # +1 as _ec_slave[0] is reserved
  *         ethercat_slave._the_masters_settings = &self._settings
  *         return ethercat_slave             # <<<<<<<<<<<<<<
  * 
  *     def _get_state(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_ethercat_slave));
   __pyx_r = ((PyObject *)__pyx_v_ethercat_slave);
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":382
+  /* "pysoem/pysoem.pyx":389
  *         return cpysoem.ecx_receive_processdata(&self._ecx_contextt, timeout)
  * 
  *     def _get_slave(self, int pos):             # <<<<<<<<<<<<<<
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')
  */
 
@@ -5956,15 +5972,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_ethercat_slave);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":393
+/* "pysoem/pysoem.pyx":400
  *         return ethercat_slave
  * 
  *     def _get_state(self):             # <<<<<<<<<<<<<<
  *         """Can be used to check if all slaves are in Operational state, or to request a new state for all slaves.
  * 
  */
 
@@ -5987,29 +6003,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_state", 0);
 
-  /* "pysoem/pysoem.pyx":398
+  /* "pysoem/pysoem.pyx":405
  *         Make sure to call write_state(), once a new state for all slaves was set.
  *         """
  *         return self._ec_slave[0].state             # <<<<<<<<<<<<<<
  * 
  *     def _set_state(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ec_slave[0]).state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ec_slave[0]).state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":393
+  /* "pysoem/pysoem.pyx":400
  *         return ethercat_slave
  * 
  *     def _get_state(self):             # <<<<<<<<<<<<<<
  *         """Can be used to check if all slaves are in Operational state, or to request a new state for all slaves.
  * 
  */
 
@@ -6020,15 +6036,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":400
+/* "pysoem/pysoem.pyx":407
  *         return self._ec_slave[0].state
  * 
  *     def _set_state(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave[0].state = value
  * 
  */
 
@@ -6050,25 +6066,25 @@
   __Pyx_RefNannyDeclarations
   uint16 __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_state", 0);
 
-  /* "pysoem/pysoem.pyx":401
+  /* "pysoem/pysoem.pyx":408
  * 
  *     def _set_state(self, value):
  *         self._ec_slave[0].state = value             # <<<<<<<<<<<<<<
  * 
  *     def _get_expected_wkc(self):
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 408, __pyx_L1_error)
   (__pyx_v_self->_ec_slave[0]).state = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":400
+  /* "pysoem/pysoem.pyx":407
  *         return self._ec_slave[0].state
  * 
  *     def _set_state(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave[0].state = value
  * 
  */
 
@@ -6080,15 +6096,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":403
+/* "pysoem/pysoem.pyx":410
  *         self._ec_slave[0].state = value
  * 
  *     def _get_expected_wkc(self):             # <<<<<<<<<<<<<<
  *         """Calculates the expected Working Counter"""
  *         return (self._ec_group[0].outputsWKC * 2) + self._ec_group[0].inputsWKC
  */
 
@@ -6111,29 +6127,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_expected_wkc", 0);
 
-  /* "pysoem/pysoem.pyx":405
+  /* "pysoem/pysoem.pyx":412
  *     def _get_expected_wkc(self):
  *         """Calculates the expected Working Counter"""
  *         return (self._ec_group[0].outputsWKC * 2) + self._ec_group[0].inputsWKC             # <<<<<<<<<<<<<<
  * 
  *     def _get_dc_time(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long((((__pyx_v_self->_ec_group[0]).outputsWKC * 2) + (__pyx_v_self->_ec_group[0]).inputsWKC)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long((((__pyx_v_self->_ec_group[0]).outputsWKC * 2) + (__pyx_v_self->_ec_group[0]).inputsWKC)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":403
+  /* "pysoem/pysoem.pyx":410
  *         self._ec_slave[0].state = value
  * 
  *     def _get_expected_wkc(self):             # <<<<<<<<<<<<<<
  *         """Calculates the expected Working Counter"""
  *         return (self._ec_group[0].outputsWKC * 2) + self._ec_group[0].inputsWKC
  */
 
@@ -6144,15 +6160,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":407
+/* "pysoem/pysoem.pyx":414
  *         return (self._ec_group[0].outputsWKC * 2) + self._ec_group[0].inputsWKC
  * 
  *     def _get_dc_time(self):             # <<<<<<<<<<<<<<
  *         """DC time in ns required to synchronize the EtherCAT cycle with SYNC0 cycles.
  * 
  */
 
@@ -6175,29 +6191,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_dc_time", 0);
 
-  /* "pysoem/pysoem.pyx":411
+  /* "pysoem/pysoem.pyx":418
  * 
  *         Note EtherCAT cycle here means the call of send_processdata and receive_processdata."""
  *         return self._ec_DCtime             # <<<<<<<<<<<<<<
  * 
  *     def _set_manual_state_change(self, int manual_state_change):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int64_t(__pyx_v_self->_ec_DCtime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int64_t(__pyx_v_self->_ec_DCtime); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":407
+  /* "pysoem/pysoem.pyx":414
  *         return (self._ec_group[0].outputsWKC * 2) + self._ec_group[0].inputsWKC
  * 
  *     def _get_dc_time(self):             # <<<<<<<<<<<<<<
  *         """DC time in ns required to synchronize the EtherCAT cycle with SYNC0 cycles.
  * 
  */
 
@@ -6208,15 +6224,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":413
+/* "pysoem/pysoem.pyx":420
  *         return self._ec_DCtime
  * 
  *     def _set_manual_state_change(self, int manual_state_change):             # <<<<<<<<<<<<<<
  *         """Set manualstatechange variable in context.
  * 
  */
 
@@ -6228,15 +6244,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_manual_state_change (wrapper)", 0);
   assert(__pyx_arg_manual_state_change); {
-    __pyx_v_manual_state_change = __Pyx_PyInt_As_int(__pyx_arg_manual_state_change); if (unlikely((__pyx_v_manual_state_change == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L3_error)
+    __pyx_v_manual_state_change = __Pyx_PyInt_As_int(__pyx_arg_manual_state_change); if (unlikely((__pyx_v_manual_state_change == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 420, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster._set_manual_state_change", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -6248,39 +6264,39 @@
 }
 
 static PyObject *__pyx_pf_6pysoem_6pysoem_10CdefMaster_38_set_manual_state_change(struct __pyx_obj_6pysoem_6pysoem_CdefMaster *__pyx_v_self, int __pyx_v_manual_state_change) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_manual_state_change", 0);
 
-  /* "pysoem/pysoem.pyx":425
+  /* "pysoem/pysoem.pyx":432
  *         .. versionadded:: 1.0.5
  *         """
  *         self._ecx_contextt.manualstatechange = manual_state_change             # <<<<<<<<<<<<<<
  * 
  *     def _get_manual_state_change(self):
  */
   __pyx_v_self->_ecx_contextt.manualstatechange = __pyx_v_manual_state_change;
 
-  /* "pysoem/pysoem.pyx":413
+  /* "pysoem/pysoem.pyx":420
  *         return self._ec_DCtime
  * 
  *     def _set_manual_state_change(self, int manual_state_change):             # <<<<<<<<<<<<<<
  *         """Set manualstatechange variable in context.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":427
+/* "pysoem/pysoem.pyx":434
  *         self._ecx_contextt.manualstatechange = manual_state_change
  * 
  *     def _get_manual_state_change(self):             # <<<<<<<<<<<<<<
  *         return self._ecx_contextt.manualstatechange
  * 
  */
 
@@ -6302,29 +6318,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_manual_state_change", 0);
 
-  /* "pysoem/pysoem.pyx":428
+  /* "pysoem/pysoem.pyx":435
  * 
  *     def _get_manual_state_change(self):
  *         return self._ecx_contextt.manualstatechange             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_ecx_contextt.manualstatechange); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_ecx_contextt.manualstatechange); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":427
+  /* "pysoem/pysoem.pyx":434
  *         self._ecx_contextt.manualstatechange = manual_state_change
  * 
  *     def _get_manual_state_change(self):             # <<<<<<<<<<<<<<
  *         return self._ecx_contextt.manualstatechange
  * 
  */
 
@@ -6335,15 +6351,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":166
+/* "pysoem/pysoem.pyx":173
  *     cdef char io_map[EC_IOMAPSIZE]
  *     cdef CdefMasterSettings _settings
  *     cdef public int sdo_read_timeout             # <<<<<<<<<<<<<<
  *     cdef public int sdo_write_timeout
  * 
  */
 
@@ -6365,15 +6381,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sdo_read_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sdo_read_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6403,29 +6419,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
   __pyx_v_self->sdo_read_timeout = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.sdo_read_timeout.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":167
+/* "pysoem/pysoem.pyx":174
  *     cdef CdefMasterSettings _settings
  *     cdef public int sdo_read_timeout
  *     cdef public int sdo_write_timeout             # <<<<<<<<<<<<<<
  * 
  *     state = property(_get_state, _set_state)
  */
 
@@ -6447,15 +6463,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sdo_write_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sdo_write_timeout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6485,15 +6501,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L1_error)
   __pyx_v_self->sdo_write_timeout = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.sdo_write_timeout.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -6612,15 +6628,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefMaster.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":441
+/* "pysoem/pysoem.pyx":448
  *     """
  * 
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.index = index
  */
 
@@ -6667,43 +6683,43 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slave_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 1); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 1); __PYX_ERR(0, 448, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 2); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 2); __PYX_ERR(0, 448, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_subindex)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 3); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 3); __PYX_ERR(0, 448, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_abort_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 4); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 4); __PYX_ERR(0, 448, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_desc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 5); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, 5); __PYX_ERR(0, 448, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 448, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -6716,15 +6732,15 @@
     __pyx_v_index = values[2];
     __pyx_v_subindex = values[3];
     __pyx_v_abort_code = values[4];
     __pyx_v_desc = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 448, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.SdoError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_8SdoError___init__(__pyx_self, __pyx_v_self, __pyx_v_slave_pos, __pyx_v_index, __pyx_v_subindex, __pyx_v_abort_code, __pyx_v_desc);
 
@@ -6737,60 +6753,60 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":442
+  /* "pysoem/pysoem.pyx":449
  * 
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):
  *         self.slave_pos = slave_pos             # <<<<<<<<<<<<<<
  *         self.index = index
  *         self.subindex = subindex
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 442, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":443
+  /* "pysoem/pysoem.pyx":450
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):
  *         self.slave_pos = slave_pos
  *         self.index = index             # <<<<<<<<<<<<<<
  *         self.subindex = subindex
  *         self.abort_code = abort_code
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_v_index) < 0) __PYX_ERR(0, 443, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_v_index) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":444
+  /* "pysoem/pysoem.pyx":451
  *         self.slave_pos = slave_pos
  *         self.index = index
  *         self.subindex = subindex             # <<<<<<<<<<<<<<
  *         self.abort_code = abort_code
  *         self.desc = desc
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_subindex, __pyx_v_subindex) < 0) __PYX_ERR(0, 444, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_subindex, __pyx_v_subindex) < 0) __PYX_ERR(0, 451, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":445
+  /* "pysoem/pysoem.pyx":452
  *         self.index = index
  *         self.subindex = subindex
  *         self.abort_code = abort_code             # <<<<<<<<<<<<<<
  *         self.desc = desc
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_abort_code, __pyx_v_abort_code) < 0) __PYX_ERR(0, 445, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_abort_code, __pyx_v_abort_code) < 0) __PYX_ERR(0, 452, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":446
+  /* "pysoem/pysoem.pyx":453
  *         self.subindex = subindex
  *         self.abort_code = abort_code
  *         self.desc = desc             # <<<<<<<<<<<<<<
  * 
  * class Emergency(Exception):
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_desc, __pyx_v_desc) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_desc, __pyx_v_desc) < 0) __PYX_ERR(0, 453, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":441
+  /* "pysoem/pysoem.pyx":448
  *     """
  * 
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.index = index
  */
 
@@ -6802,15 +6818,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":460
+/* "pysoem/pysoem.pyx":467
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -6860,49 +6876,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slave_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 1); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 1); __PYX_ERR(0, 467, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 2); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 2); __PYX_ERR(0, 467, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_reg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 3); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 3); __PYX_ERR(0, 467, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 4); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 4); __PYX_ERR(0, 467, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_w1)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 5); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 5); __PYX_ERR(0, 467, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_w2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 6); __PYX_ERR(0, 460, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, 6); __PYX_ERR(0, 467, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 460, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 467, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 7) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -6917,15 +6933,15 @@
     __pyx_v_error_reg = values[3];
     __pyx_v_b1 = values[4];
     __pyx_v_w1 = values[5];
     __pyx_v_w2 = values[6];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 460, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 7, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 467, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.Emergency.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9Emergency___init__(__pyx_self, __pyx_v_self, __pyx_v_slave_pos, __pyx_v_error_code, __pyx_v_error_reg, __pyx_v_b1, __pyx_v_w1, __pyx_v_w2);
 
@@ -6938,69 +6954,69 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":461
+  /* "pysoem/pysoem.pyx":468
  * 
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):
  *         self.slave_pos = slave_pos             # <<<<<<<<<<<<<<
  *         self.error_code = error_code
  *         self.error_reg = error_reg
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 468, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":462
+  /* "pysoem/pysoem.pyx":469
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code             # <<<<<<<<<<<<<<
  *         self.error_reg = error_reg
  *         self.b1 = b1
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":463
+  /* "pysoem/pysoem.pyx":470
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  *         self.error_reg = error_reg             # <<<<<<<<<<<<<<
  *         self.b1 = b1
  *         self.w1 = w1
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_reg, __pyx_v_error_reg) < 0) __PYX_ERR(0, 463, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_reg, __pyx_v_error_reg) < 0) __PYX_ERR(0, 470, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":464
+  /* "pysoem/pysoem.pyx":471
  *         self.error_code = error_code
  *         self.error_reg = error_reg
  *         self.b1 = b1             # <<<<<<<<<<<<<<
  *         self.w1 = w1
  *         self.w2 = w2
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_b1, __pyx_v_b1) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_b1, __pyx_v_b1) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":465
+  /* "pysoem/pysoem.pyx":472
  *         self.error_reg = error_reg
  *         self.b1 = b1
  *         self.w1 = w1             # <<<<<<<<<<<<<<
  *         self.w2 = w2
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_w1, __pyx_v_w1) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_w1, __pyx_v_w1) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":466
+  /* "pysoem/pysoem.pyx":473
  *         self.b1 = b1
  *         self.w1 = w1
  *         self.w2 = w2             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_w2, __pyx_v_w2) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_w2, __pyx_v_w2) < 0) __PYX_ERR(0, 473, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":460
+  /* "pysoem/pysoem.pyx":467
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -7012,15 +7028,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":476
+/* "pysoem/pysoem.pyx":483
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -7055,32 +7071,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_message)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 476, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 483, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 476, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 483, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_message = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 476, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 483, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.SdoInfoError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_12SdoInfoError___init__(__pyx_self, __pyx_v_self, __pyx_v_message);
 
@@ -7093,24 +7109,24 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":477
+  /* "pysoem/pysoem.pyx":484
  * 
  *     def __init__(self, message):
  *         self.message = message             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 477, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":476
+  /* "pysoem/pysoem.pyx":483
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -7122,15 +7138,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":489
+/* "pysoem/pysoem.pyx":496
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -7171,31 +7187,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slave_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 1); __PYX_ERR(0, 489, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 1); __PYX_ERR(0, 496, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 2); __PYX_ERR(0, 489, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 2); __PYX_ERR(0, 496, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_desc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 3); __PYX_ERR(0, 489, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, 3); __PYX_ERR(0, 496, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 489, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 496, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7204,15 +7220,15 @@
     __pyx_v_self = values[0];
     __pyx_v_slave_pos = values[1];
     __pyx_v_error_code = values[2];
     __pyx_v_desc = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 489, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 496, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.MailboxError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_12MailboxError___init__(__pyx_self, __pyx_v_self, __pyx_v_slave_pos, __pyx_v_error_code, __pyx_v_desc);
 
@@ -7225,42 +7241,42 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":490
+  /* "pysoem/pysoem.pyx":497
  * 
  *     def __init__(self, slave_pos, error_code, desc):
  *         self.slave_pos = slave_pos             # <<<<<<<<<<<<<<
  *         self.error_code = error_code
  *         self.desc = desc
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 490, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 497, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":491
+  /* "pysoem/pysoem.pyx":498
  *     def __init__(self, slave_pos, error_code, desc):
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code             # <<<<<<<<<<<<<<
  *         self.desc = desc
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":492
+  /* "pysoem/pysoem.pyx":499
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  *         self.desc = desc             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_desc, __pyx_v_desc) < 0) __PYX_ERR(0, 492, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_desc, __pyx_v_desc) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":489
+  /* "pysoem/pysoem.pyx":496
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -7272,15 +7288,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":511
+/* "pysoem/pysoem.pyx":518
  *     }
  * 
  *     def __init__(self, slave_pos, error_code):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -7318,40 +7334,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_slave_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 511, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 518, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 511, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 518, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 511, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 518, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_slave_pos = values[1];
     __pyx_v_error_code = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 511, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 518, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.PacketError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_11PacketError___init__(__pyx_self, __pyx_v_self, __pyx_v_slave_pos, __pyx_v_error_code);
 
@@ -7364,33 +7380,33 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":512
+  /* "pysoem/pysoem.pyx":519
  * 
  *     def __init__(self, slave_pos, error_code):
  *         self.slave_pos = slave_pos             # <<<<<<<<<<<<<<
  *         self.error_code = error_code
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_slave_pos, __pyx_v_slave_pos) < 0) __PYX_ERR(0, 519, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":513
+  /* "pysoem/pysoem.pyx":520
  *     def __init__(self, slave_pos, error_code):
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code             # <<<<<<<<<<<<<<
  * 
  *     def _get_desc(self):
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 513, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_code, __pyx_v_error_code) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":511
+  /* "pysoem/pysoem.pyx":518
  *     }
  * 
  *     def __init__(self, slave_pos, error_code):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
 
@@ -7402,15 +7418,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":515
+/* "pysoem/pysoem.pyx":522
  *         self.error_code = error_code
  * 
  *     def _get_desc(self):             # <<<<<<<<<<<<<<
  *         return self._code_desc[self.error_code]
  * 
  */
 
@@ -7435,35 +7451,35 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_desc", 0);
 
-  /* "pysoem/pysoem.pyx":516
+  /* "pysoem/pysoem.pyx":523
  * 
  *     def _get_desc(self):
  *         return self._code_desc[self.error_code]             # <<<<<<<<<<<<<<
  * 
  *     desc = property(_get_desc)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code_desc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_code_desc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_error_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_error_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":515
+  /* "pysoem/pysoem.pyx":522
  *         self.error_code = error_code
  * 
  *     def _get_desc(self):             # <<<<<<<<<<<<<<
  *         return self._code_desc[self.error_code]
  * 
  */
 
@@ -7476,15 +7492,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":528
+/* "pysoem/pysoem.pyx":535
  *     """
  * 
  *     def __init__(self, error_list):             # <<<<<<<<<<<<<<
  *         self.error_list = error_list
  * 
  */
 
@@ -7519,32 +7535,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_list)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 528, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 535, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 528, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 535, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_error_list = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 528, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 535, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.ConfigMapError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_14ConfigMapError___init__(__pyx_self, __pyx_v_self, __pyx_v_error_list);
 
@@ -7557,24 +7573,24 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":529
+  /* "pysoem/pysoem.pyx":536
  * 
  *     def __init__(self, error_list):
  *         self.error_list = error_list             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_list, __pyx_v_error_list) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_error_list, __pyx_v_error_list) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":528
+  /* "pysoem/pysoem.pyx":535
  *     """
  * 
  *     def __init__(self, error_list):             # <<<<<<<<<<<<<<
  *         self.error_list = error_list
  * 
  */
 
@@ -7586,15 +7602,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":539
+/* "pysoem/pysoem.pyx":546
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -7629,32 +7645,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_message)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 539, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 546, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 539, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 546, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_message = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 539, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 546, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.EepromError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_11EepromError___init__(__pyx_self, __pyx_v_self, __pyx_v_message);
 
@@ -7667,24 +7683,24 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":540
+  /* "pysoem/pysoem.pyx":547
  * 
  *     def __init__(self, message):
  *         self.message = message             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 547, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":539
+  /* "pysoem/pysoem.pyx":546
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -7696,15 +7712,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":550
+/* "pysoem/pysoem.pyx":557
  *     """
  * 
  *     def __init__(self, message=None):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -7744,15 +7760,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_message);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 550, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 557, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -7760,15 +7776,15 @@
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_message = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 550, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 557, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.WkcError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_8WkcError___init__(__pyx_self, __pyx_v_self, __pyx_v_message);
 
@@ -7781,24 +7797,24 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":551
+  /* "pysoem/pysoem.pyx":558
  * 
  *     def __init__(self, message=None):
  *         self.message = message             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_message, __pyx_v_message) < 0) __PYX_ERR(0, 558, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":550
+  /* "pysoem/pysoem.pyx":557
  *     """
  * 
  *     def __init__(self, message=None):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
 
@@ -8137,15 +8153,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":606
+/* "pysoem/pysoem.pyx":613
  *     od = property(_get_od)
  * 
  *     def __init__(self, pos):             # <<<<<<<<<<<<<<
  *         self._pos = pos
  *         self._cd = _CallbackData()
  */
 
@@ -8174,26 +8190,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 606, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 613, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_pos = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 606, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 613, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave___init__(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_pos);
 
@@ -8207,56 +8223,56 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":607
+  /* "pysoem/pysoem.pyx":614
  * 
  *     def __init__(self, pos):
  *         self._pos = pos             # <<<<<<<<<<<<<<
  *         self._cd = _CallbackData()
  *         self._cd.slave = self
  */
   __Pyx_INCREF(__pyx_v_pos);
   __Pyx_GIVEREF(__pyx_v_pos);
   __Pyx_GOTREF(__pyx_v_self->_pos);
   __Pyx_DECREF(__pyx_v_self->_pos);
   __pyx_v_self->_pos = __pyx_v_pos;
 
-  /* "pysoem/pysoem.pyx":608
+  /* "pysoem/pysoem.pyx":615
  *     def __init__(self, pos):
  *         self._pos = pos
  *         self._cd = _CallbackData()             # <<<<<<<<<<<<<<
  *         self._cd.slave = self
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem__CallbackData)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem__CallbackData)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_cd);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_cd));
   __pyx_v_self->_cd = ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":609
+  /* "pysoem/pysoem.pyx":616
  *         self._pos = pos
  *         self._cd = _CallbackData()
  *         self._cd.slave = self             # <<<<<<<<<<<<<<
  * 
  *     def dc_sync(self, act, sync0_cycle_time, sync0_shift_time=0, sync1_cycle_time=None):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_self->_cd->slave);
   __Pyx_DECREF(__pyx_v_self->_cd->slave);
   __pyx_v_self->_cd->slave = ((PyObject *)__pyx_v_self);
 
-  /* "pysoem/pysoem.pyx":606
+  /* "pysoem/pysoem.pyx":613
  *     od = property(_get_od)
  * 
  *     def __init__(self, pos):             # <<<<<<<<<<<<<<
  *         self._pos = pos
  *         self._cd = _CallbackData()
  */
 
@@ -8268,15 +8284,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":611
+/* "pysoem/pysoem.pyx":618
  *         self._cd.slave = self
  * 
  *     def dc_sync(self, act, sync0_cycle_time, sync0_shift_time=0, sync1_cycle_time=None):             # <<<<<<<<<<<<<<
  *         """Activate or deactivate SYNC pulses at the slave.
  * 
  */
 
@@ -8319,15 +8335,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_act)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sync0_cycle_time)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("dc_sync", 0, 2, 4, 1); __PYX_ERR(0, 611, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dc_sync", 0, 2, 4, 1); __PYX_ERR(0, 618, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sync0_shift_time);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -8335,15 +8351,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sync1_cycle_time);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dc_sync") < 0)) __PYX_ERR(0, 611, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "dc_sync") < 0)) __PYX_ERR(0, 618, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -8356,15 +8372,15 @@
     __pyx_v_act = values[0];
     __pyx_v_sync0_cycle_time = values[1];
     __pyx_v_sync0_shift_time = values[2];
     __pyx_v_sync1_cycle_time = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dc_sync", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 611, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dc_sync", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 618, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.dc_sync", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_2dc_sync(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_act, __pyx_v_sync0_cycle_time, __pyx_v_sync0_shift_time, __pyx_v_sync1_cycle_time);
 
@@ -8384,66 +8400,66 @@
   int32 __pyx_t_6;
   uint32 __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dc_sync", 0);
 
-  /* "pysoem/pysoem.pyx":622
+  /* "pysoem/pysoem.pyx":629
  *         """
  * 
  *         if sync1_cycle_time is None:             # <<<<<<<<<<<<<<
  *             cpysoem.ecx_dcsync0(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync0_shift_time)
  *         else:
  */
   __pyx_t_1 = (__pyx_v_sync1_cycle_time == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":623
+    /* "pysoem/pysoem.pyx":630
  * 
  *         if sync1_cycle_time is None:
  *             cpysoem.ecx_dcsync0(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync0_shift_time)             # <<<<<<<<<<<<<<
  *         else:
  *             cpysoem.ecx_dcsync01(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync1_cycle_time, sync0_shift_time)
  */
-    __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 623, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_act); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 623, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync0_cycle_time); if (unlikely((__pyx_t_5 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 623, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyInt_As_int32_t(__pyx_v_sync0_shift_time); if (unlikely((__pyx_t_6 == ((int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 623, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_act); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync0_cycle_time); if (unlikely((__pyx_t_5 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int32_t(__pyx_v_sync0_shift_time); if (unlikely((__pyx_t_6 == ((int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
     ecx_dcsync0(__pyx_v_self->_ecx_contextt, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":622
+    /* "pysoem/pysoem.pyx":629
  *         """
  * 
  *         if sync1_cycle_time is None:             # <<<<<<<<<<<<<<
  *             cpysoem.ecx_dcsync0(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync0_shift_time)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pysoem/pysoem.pyx":625
+  /* "pysoem/pysoem.pyx":632
  *             cpysoem.ecx_dcsync0(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync0_shift_time)
  *         else:
  *             cpysoem.ecx_dcsync01(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync1_cycle_time, sync0_shift_time)             # <<<<<<<<<<<<<<
  * 
  *     def sdo_read(self, index, uint8_t subindex, int size=0, ca=False):
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_act); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync0_cycle_time); if (unlikely((__pyx_t_5 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync1_cycle_time); if (unlikely((__pyx_t_7 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyInt_As_int32_t(__pyx_v_sync0_shift_time); if (unlikely((__pyx_t_6 == ((int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_act); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync0_cycle_time); if (unlikely((__pyx_t_5 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_uint32_t(__pyx_v_sync1_cycle_time); if (unlikely((__pyx_t_7 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int32_t(__pyx_v_sync0_shift_time); if (unlikely((__pyx_t_6 == ((int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 632, __pyx_L1_error)
     ecx_dcsync01(__pyx_v_self->_ecx_contextt, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_7, __pyx_t_6);
   }
   __pyx_L3:;
 
-  /* "pysoem/pysoem.pyx":611
+  /* "pysoem/pysoem.pyx":618
  *         self._cd.slave = self
  * 
  *     def dc_sync(self, act, sync0_cycle_time, sync0_shift_time=0, sync1_cycle_time=None):             # <<<<<<<<<<<<<<
  *         """Activate or deactivate SYNC pulses at the slave.
  * 
  */
 
@@ -8455,15 +8471,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":627
+/* "pysoem/pysoem.pyx":634
  *             cpysoem.ecx_dcsync01(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync1_cycle_time, sync0_shift_time)
  * 
  *     def sdo_read(self, index, uint8_t subindex, int size=0, ca=False):             # <<<<<<<<<<<<<<
  *         """Read a CoE object.
  * 
  */
 
@@ -8505,15 +8521,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_subindex)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("sdo_read", 0, 2, 4, 1); __PYX_ERR(0, 627, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("sdo_read", 0, 2, 4, 1); __PYX_ERR(0, 634, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -8521,40 +8537,40 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ca);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sdo_read") < 0)) __PYX_ERR(0, 627, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sdo_read") < 0)) __PYX_ERR(0, 634, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_index = values[0];
-    __pyx_v_subindex = __Pyx_PyInt_As_uint8_t(values[1]); if (unlikely((__pyx_v_subindex == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 627, __pyx_L3_error)
+    __pyx_v_subindex = __Pyx_PyInt_As_uint8_t(values[1]); if (unlikely((__pyx_v_subindex == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 634, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_size = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 627, __pyx_L3_error)
+      __pyx_v_size = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 634, __pyx_L3_error)
     } else {
       __pyx_v_size = ((int)0);
     }
     __pyx_v_ca = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sdo_read", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 627, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("sdo_read", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 634, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.sdo_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_4sdo_read(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_index, __pyx_v_subindex, __pyx_v_size, __pyx_v_ca);
 
@@ -8587,258 +8603,258 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sdo_read", 0);
 
-  /* "pysoem/pysoem.pyx":647
+  /* "pysoem/pysoem.pyx":654
  *             PacketError: on packet level error
  *         """
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_ecx_contextt == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":648
+    /* "pysoem/pysoem.pyx":655
  *         """
  *         if self._ecx_contextt == NULL:
  *             raise UnboundLocalError()             # <<<<<<<<<<<<<<
  * 
  *         cdef unsigned char* pbuf
  */
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 655, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 648, __pyx_L1_error)
+    __PYX_ERR(0, 655, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":647
+    /* "pysoem/pysoem.pyx":654
  *             PacketError: on packet level error
  *         """
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":653
+  /* "pysoem/pysoem.pyx":660
  *         cdef uint8_t std_buffer[STATIC_SDO_READ_BUFFER_SIZE]
  *         cdef int size_inout
  *         if size == 0:             # <<<<<<<<<<<<<<
  *             pbuf = std_buffer
  *             size_inout = STATIC_SDO_READ_BUFFER_SIZE
  */
   __pyx_t_1 = ((__pyx_v_size == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":654
+    /* "pysoem/pysoem.pyx":661
  *         cdef int size_inout
  *         if size == 0:
  *             pbuf = std_buffer             # <<<<<<<<<<<<<<
  *             size_inout = STATIC_SDO_READ_BUFFER_SIZE
  *         else:
  */
     __pyx_v_pbuf = __pyx_v_std_buffer;
 
-    /* "pysoem/pysoem.pyx":655
+    /* "pysoem/pysoem.pyx":662
  *         if size == 0:
  *             pbuf = std_buffer
  *             size_inout = STATIC_SDO_READ_BUFFER_SIZE             # <<<<<<<<<<<<<<
  *         else:
  *             pbuf = <unsigned char*>PyMem_Malloc((size)*sizeof(unsigned char))
  */
     __pyx_v_size_inout = 0x100;
 
-    /* "pysoem/pysoem.pyx":653
+    /* "pysoem/pysoem.pyx":660
  *         cdef uint8_t std_buffer[STATIC_SDO_READ_BUFFER_SIZE]
  *         cdef int size_inout
  *         if size == 0:             # <<<<<<<<<<<<<<
  *             pbuf = std_buffer
  *             size_inout = STATIC_SDO_READ_BUFFER_SIZE
  */
     goto __pyx_L4;
   }
 
-  /* "pysoem/pysoem.pyx":657
+  /* "pysoem/pysoem.pyx":664
  *             size_inout = STATIC_SDO_READ_BUFFER_SIZE
  *         else:
  *             pbuf = <unsigned char*>PyMem_Malloc((size)*sizeof(unsigned char))             # <<<<<<<<<<<<<<
  *             size_inout = size
  * 
  */
   /*else*/ {
     __pyx_v_pbuf = ((unsigned char *)PyMem_Malloc((__pyx_v_size * (sizeof(unsigned char)))));
 
-    /* "pysoem/pysoem.pyx":658
+    /* "pysoem/pysoem.pyx":665
  *         else:
  *             pbuf = <unsigned char*>PyMem_Malloc((size)*sizeof(unsigned char))
  *             size_inout = size             # <<<<<<<<<<<<<<
  * 
  *         if pbuf == NULL:
  */
     __pyx_v_size_inout = __pyx_v_size;
   }
   __pyx_L4:;
 
-  /* "pysoem/pysoem.pyx":660
+  /* "pysoem/pysoem.pyx":667
  *             size_inout = size
  * 
  *         if pbuf == NULL:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_pbuf == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":661
+    /* "pysoem/pysoem.pyx":668
  * 
  *         if pbuf == NULL:
  *             raise MemoryError()             # <<<<<<<<<<<<<<
  * 
  *         cdef int result = cpysoem.ecx_SDOread(self._ecx_contextt, self._pos, index, subindex, ca,
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 661, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 668, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":660
+    /* "pysoem/pysoem.pyx":667
  *             size_inout = size
  * 
  *         if pbuf == NULL:             # <<<<<<<<<<<<<<
  *             raise MemoryError()
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":663
+  /* "pysoem/pysoem.pyx":670
  *             raise MemoryError()
  * 
  *         cdef int result = cpysoem.ecx_SDOread(self._ecx_contextt, self._pos, index, subindex, ca,             # <<<<<<<<<<<<<<
  *                                               &size_inout, pbuf, self._the_masters_settings.sdo_read_timeout[0])
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 663, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_index); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 663, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyInt_As_int8_t(__pyx_v_ca); if (unlikely((__pyx_t_5 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_index); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int8_t(__pyx_v_ca); if (unlikely((__pyx_t_5 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":664
+  /* "pysoem/pysoem.pyx":671
  * 
  *         cdef int result = cpysoem.ecx_SDOread(self._ecx_contextt, self._pos, index, subindex, ca,
  *                                               &size_inout, pbuf, self._the_masters_settings.sdo_read_timeout[0])             # <<<<<<<<<<<<<<
  * 
  *         cdef cpysoem.ec_errort err
  */
   __pyx_v_result = ecx_SDOread(__pyx_v_self->_ecx_contextt, __pyx_t_3, __pyx_t_4, __pyx_v_subindex, __pyx_t_5, (&__pyx_v_size_inout), __pyx_v_pbuf, (__pyx_v_self->_the_masters_settings->sdo_read_timeout[0]));
 
-  /* "pysoem/pysoem.pyx":667
+  /* "pysoem/pysoem.pyx":674
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)
  */
   __pyx_t_1 = (ecx_poperror(__pyx_v_self->_ecx_contextt, (&__pyx_v_err)) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":668
+    /* "pysoem/pysoem.pyx":675
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             if pbuf != std_buffer:             # <<<<<<<<<<<<<<
  *                 PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  */
     __pyx_t_1 = ((__pyx_v_pbuf != __pyx_v_std_buffer) != 0);
     if (__pyx_t_1) {
 
-      /* "pysoem/pysoem.pyx":669
+      /* "pysoem/pysoem.pyx":676
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)             # <<<<<<<<<<<<<<
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)
  */
       PyMem_Free(__pyx_v_pbuf);
 
-      /* "pysoem/pysoem.pyx":668
+      /* "pysoem/pysoem.pyx":675
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             if pbuf != std_buffer:             # <<<<<<<<<<<<<<
  *                 PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  */
     }
 
-    /* "pysoem/pysoem.pyx":670
+    /* "pysoem/pysoem.pyx":677
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)
  *             assert err.Slave == self._pos             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(__pyx_assertions_enabled())) {
-      __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 670, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 677, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = PyObject_RichCompare(__pyx_t_2, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 670, __pyx_L1_error)
+      __pyx_t_6 = PyObject_RichCompare(__pyx_t_2, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 677, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 670, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 677, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(!__pyx_t_1)) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 670, __pyx_L1_error)
+        __PYX_ERR(0, 677, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "pysoem/pysoem.pyx":671
+    /* "pysoem/pysoem.pyx":678
  *                 PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
-    __pyx_t_6 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 671, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 678, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pysoem/pysoem.pyx":667
+    /* "pysoem/pysoem.pyx":674
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)
  */
   }
 
-  /* "pysoem/pysoem.pyx":673
+  /* "pysoem/pysoem.pyx":680
  *             self._raise_exception(&err)
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  */
   /*try:*/ {
 
-    /* "pysoem/pysoem.pyx":674
+    /* "pysoem/pysoem.pyx":681
  * 
  *         try:
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)             # <<<<<<<<<<<<<<
  *         finally:
  *             if pbuf != std_buffer:
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)__pyx_v_pbuf), __pyx_v_size_inout); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 674, __pyx_L9_error)
+    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)__pyx_v_pbuf), __pyx_v_size_inout); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 681, __pyx_L9_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L8_return;
   }
 
-  /* "pysoem/pysoem.pyx":676
+  /* "pysoem/pysoem.pyx":683
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  *             if pbuf != std_buffer:             # <<<<<<<<<<<<<<
  *                 PyMem_Free(pbuf)
  * 
  */
   /*finally:*/ {
@@ -8858,24 +8874,24 @@
       __Pyx_XGOTREF(__pyx_t_14);
       __Pyx_XGOTREF(__pyx_t_15);
       __pyx_t_7 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
       {
         __pyx_t_1 = ((__pyx_v_pbuf != __pyx_v_std_buffer) != 0);
         if (__pyx_t_1) {
 
-          /* "pysoem/pysoem.pyx":677
+          /* "pysoem/pysoem.pyx":684
  *         finally:
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)             # <<<<<<<<<<<<<<
  * 
  *     def sdo_write(self, index, uint8_t subindex, bytes data, ca=False):
  */
           PyMem_Free(__pyx_v_pbuf);
 
-          /* "pysoem/pysoem.pyx":676
+          /* "pysoem/pysoem.pyx":683
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  *             if pbuf != std_buffer:             # <<<<<<<<<<<<<<
  *                 PyMem_Free(pbuf)
  * 
  */
         }
@@ -8896,38 +8912,38 @@
     }
     __pyx_L8_return: {
       __pyx_t_15 = __pyx_r;
       __pyx_r = 0;
       __pyx_t_1 = ((__pyx_v_pbuf != __pyx_v_std_buffer) != 0);
       if (__pyx_t_1) {
 
-        /* "pysoem/pysoem.pyx":677
+        /* "pysoem/pysoem.pyx":684
  *         finally:
  *             if pbuf != std_buffer:
  *                 PyMem_Free(pbuf)             # <<<<<<<<<<<<<<
  * 
  *     def sdo_write(self, index, uint8_t subindex, bytes data, ca=False):
  */
         PyMem_Free(__pyx_v_pbuf);
 
-        /* "pysoem/pysoem.pyx":676
+        /* "pysoem/pysoem.pyx":683
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  *             if pbuf != std_buffer:             # <<<<<<<<<<<<<<
  *                 PyMem_Free(pbuf)
  * 
  */
       }
       __pyx_r = __pyx_t_15;
       __pyx_t_15 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "pysoem/pysoem.pyx":627
+  /* "pysoem/pysoem.pyx":634
  *             cpysoem.ecx_dcsync01(self._ecx_contextt, self._pos, act, sync0_cycle_time, sync1_cycle_time, sync0_shift_time)
  * 
  *     def sdo_read(self, index, uint8_t subindex, int size=0, ca=False):             # <<<<<<<<<<<<<<
  *         """Read a CoE object.
  * 
  */
 
@@ -8939,15 +8955,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":679
+/* "pysoem/pysoem.pyx":686
  *                 PyMem_Free(pbuf)
  * 
  *     def sdo_write(self, index, uint8_t subindex, bytes data, ca=False):             # <<<<<<<<<<<<<<
  *         """Write to a CoE object.
  * 
  */
 
@@ -8989,57 +9005,57 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_subindex)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, 1); __PYX_ERR(0, 679, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, 1); __PYX_ERR(0, 686, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, 2); __PYX_ERR(0, 679, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, 2); __PYX_ERR(0, 686, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ca);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sdo_write") < 0)) __PYX_ERR(0, 679, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sdo_write") < 0)) __PYX_ERR(0, 686, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_index = values[0];
-    __pyx_v_subindex = __Pyx_PyInt_As_uint8_t(values[1]); if (unlikely((__pyx_v_subindex == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L3_error)
+    __pyx_v_subindex = __Pyx_PyInt_As_uint8_t(values[1]); if (unlikely((__pyx_v_subindex == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 686, __pyx_L3_error)
     __pyx_v_data = ((PyObject*)values[2]);
     __pyx_v_ca = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 679, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("sdo_write", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 686, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.sdo_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 686, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_6sdo_write(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_index, __pyx_v_subindex, __pyx_v_data, __pyx_v_ca);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9061,92 +9077,92 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sdo_write", 0);
 
-  /* "pysoem/pysoem.pyx":693
+  /* "pysoem/pysoem.pyx":700
  *             PacketError: on packet level error
  *         """
  *         cdef int size = len(data)             # <<<<<<<<<<<<<<
  *         cdef int result = cpysoem.ecx_SDOwrite(self._ecx_contextt, self._pos, index, subindex, ca,
  *                                                size, <unsigned char*>data, self._the_masters_settings.sdo_write_timeout[0])
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 693, __pyx_L1_error)
+    __PYX_ERR(0, 700, __pyx_L1_error)
   }
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 700, __pyx_L1_error)
   __pyx_v_size = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":694
+  /* "pysoem/pysoem.pyx":701
  *         """
  *         cdef int size = len(data)
  *         cdef int result = cpysoem.ecx_SDOwrite(self._ecx_contextt, self._pos, index, subindex, ca,             # <<<<<<<<<<<<<<
  *                                                size, <unsigned char*>data, self._the_masters_settings.sdo_write_timeout[0])
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_2 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_index); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_ca); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_2 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint16_t(__pyx_v_index); if (unlikely((__pyx_t_3 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int8_t(__pyx_v_ca); if (unlikely((__pyx_t_4 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 701, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":695
+  /* "pysoem/pysoem.pyx":702
  *         cdef int size = len(data)
  *         cdef int result = cpysoem.ecx_SDOwrite(self._ecx_contextt, self._pos, index, subindex, ca,
  *                                                size, <unsigned char*>data, self._the_masters_settings.sdo_write_timeout[0])             # <<<<<<<<<<<<<<
  * 
  *         cdef cpysoem.ec_errort err
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 695, __pyx_L1_error)
+    __PYX_ERR(0, 702, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 695, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 702, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":694
+  /* "pysoem/pysoem.pyx":701
  *         """
  *         cdef int size = len(data)
  *         cdef int result = cpysoem.ecx_SDOwrite(self._ecx_contextt, self._pos, index, subindex, ca,             # <<<<<<<<<<<<<<
  *                                                size, <unsigned char*>data, self._the_masters_settings.sdo_write_timeout[0])
  * 
  */
   __pyx_v_result = ecx_SDOwrite(__pyx_v_self->_ecx_contextt, __pyx_t_2, __pyx_t_3, __pyx_v_subindex, __pyx_t_4, __pyx_v_size, ((unsigned char *)__pyx_t_5), (__pyx_v_self->_the_masters_settings->sdo_write_timeout[0]));
 
-  /* "pysoem/pysoem.pyx":698
+  /* "pysoem/pysoem.pyx":705
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
   __pyx_t_6 = (ecx_poperror(__pyx_v_self->_ecx_contextt, (&__pyx_v_err)) != 0);
   if (__pyx_t_6) {
 
-    /* "pysoem/pysoem.pyx":699
+    /* "pysoem/pysoem.pyx":706
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             self._raise_exception(&err)             # <<<<<<<<<<<<<<
  * 
  *     def mbx_receive(self):
  */
-    __pyx_t_7 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 699, __pyx_L1_error)
+    __pyx_t_7 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 706, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pysoem/pysoem.pyx":698
+    /* "pysoem/pysoem.pyx":705
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":679
+  /* "pysoem/pysoem.pyx":686
  *                 PyMem_Free(pbuf)
  * 
  *     def sdo_write(self, index, uint8_t subindex, bytes data, ca=False):             # <<<<<<<<<<<<<<
  *         """Write to a CoE object.
  * 
  */
 
@@ -9159,15 +9175,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":701
+/* "pysoem/pysoem.pyx":708
  *             self._raise_exception(&err)
  * 
  *     def mbx_receive(self):             # <<<<<<<<<<<<<<
  *         """Read out the slaves out mailbox - to check for emergency messages.
  * 
  */
 
@@ -9195,78 +9211,78 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mbx_receive", 0);
 
-  /* "pysoem/pysoem.pyx":711
+  /* "pysoem/pysoem.pyx":718
  *         """
  *         cdef cpysoem.ec_mbxbuft buf
  *         cpysoem.ec_clearmbx(&buf)             # <<<<<<<<<<<<<<
  *         cdef int wkt = cpysoem.ecx_mbxreceive(self._ecx_contextt, self._pos, &buf, 0)
  * 
  */
   ec_clearmbx((&__pyx_v_buf));
 
-  /* "pysoem/pysoem.pyx":712
+  /* "pysoem/pysoem.pyx":719
  *         cdef cpysoem.ec_mbxbuft buf
  *         cpysoem.ec_clearmbx(&buf)
  *         cdef int wkt = cpysoem.ecx_mbxreceive(self._ecx_contextt, self._pos, &buf, 0)             # <<<<<<<<<<<<<<
  * 
  *         cdef cpysoem.ec_errort err
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 719, __pyx_L1_error)
   __pyx_v_wkt = ecx_mbxreceive(__pyx_v_self->_ecx_contextt, __pyx_t_1, (&__pyx_v_buf), 0);
 
-  /* "pysoem/pysoem.pyx":715
+  /* "pysoem/pysoem.pyx":722
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
   __pyx_t_2 = (ecx_poperror(__pyx_v_self->_ecx_contextt, (&__pyx_v_err)) != 0);
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":716
+    /* "pysoem/pysoem.pyx":723
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             self._raise_exception(&err)             # <<<<<<<<<<<<<<
  * 
  *         return wkt
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 716, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 723, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pysoem/pysoem.pyx":715
+    /* "pysoem/pysoem.pyx":722
  * 
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":718
+  /* "pysoem/pysoem.pyx":725
  *             self._raise_exception(&err)
  * 
  *         return wkt             # <<<<<<<<<<<<<<
  * 
  *     def write_state(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_wkt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_wkt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 725, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":701
+  /* "pysoem/pysoem.pyx":708
  *             self._raise_exception(&err)
  * 
  *     def mbx_receive(self):             # <<<<<<<<<<<<<<
  *         """Read out the slaves out mailbox - to check for emergency messages.
  * 
  */
 
@@ -9277,15 +9293,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":720
+/* "pysoem/pysoem.pyx":727
  *         return wkt
  * 
  *     def write_state(self):             # <<<<<<<<<<<<<<
  *         """Write slave state.
  * 
  */
 
@@ -9309,30 +9325,30 @@
   uint16 __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_state", 0);
 
-  /* "pysoem/pysoem.pyx":725
+  /* "pysoem/pysoem.pyx":732
  *         Note: The function does not check if the actual state is changed.
  *         """
  *         return cpysoem.ecx_writestate(self._ecx_contextt, self._pos)             # <<<<<<<<<<<<<<
  * 
  *     def state_check(self, int expected_state, timeout=2000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 725, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(ecx_writestate(__pyx_v_self->_ecx_contextt, __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 732, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(ecx_writestate(__pyx_v_self->_ecx_contextt, __pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":720
+  /* "pysoem/pysoem.pyx":727
  *         return wkt
  * 
  *     def write_state(self):             # <<<<<<<<<<<<<<
  *         """Write slave state.
  * 
  */
 
@@ -9343,15 +9359,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":727
+/* "pysoem/pysoem.pyx":734
  *         return cpysoem.ecx_writestate(self._ecx_contextt, self._pos)
  * 
  *     def state_check(self, int expected_state, timeout=2000):             # <<<<<<<<<<<<<<
  *         """Wait for the slave to reach the state that was requested."""
  *         return cpysoem.ecx_statecheck(self._ecx_contextt, self._pos, expected_state, timeout)
  */
 
@@ -9391,31 +9407,31 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "state_check") < 0)) __PYX_ERR(0, 727, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "state_check") < 0)) __PYX_ERR(0, 734, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_expected_state = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_expected_state == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 727, __pyx_L3_error)
+    __pyx_v_expected_state = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_expected_state == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 734, __pyx_L3_error)
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("state_check", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 727, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("state_check", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 734, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.state_check", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_12state_check(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_expected_state, __pyx_v_timeout);
 
@@ -9431,31 +9447,31 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("state_check", 0);
 
-  /* "pysoem/pysoem.pyx":729
+  /* "pysoem/pysoem.pyx":736
  *     def state_check(self, int expected_state, timeout=2000):
  *         """Wait for the slave to reach the state that was requested."""
  *         return cpysoem.ecx_statecheck(self._ecx_contextt, self._pos, expected_state, timeout)             # <<<<<<<<<<<<<<
  * 
  *     def reconfig(self, timeout=500):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 729, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 729, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_uint16_t(ecx_statecheck(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_v_expected_state, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 729, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint16_t(ecx_statecheck(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_v_expected_state, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":727
+  /* "pysoem/pysoem.pyx":734
  *         return cpysoem.ecx_writestate(self._ecx_contextt, self._pos)
  * 
  *     def state_check(self, int expected_state, timeout=2000):             # <<<<<<<<<<<<<<
  *         """Wait for the slave to reach the state that was requested."""
  *         return cpysoem.ecx_statecheck(self._ecx_contextt, self._pos, expected_state, timeout)
  */
 
@@ -9466,15 +9482,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":731
+/* "pysoem/pysoem.pyx":738
  *         return cpysoem.ecx_statecheck(self._ecx_contextt, self._pos, expected_state, timeout)
  * 
  *     def reconfig(self, timeout=500):             # <<<<<<<<<<<<<<
  *         """Reconfigure slave.
  * 
  */
 
@@ -9507,29 +9523,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reconfig") < 0)) __PYX_ERR(0, 731, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "reconfig") < 0)) __PYX_ERR(0, 738, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("reconfig", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 731, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("reconfig", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 738, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.reconfig", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_14reconfig(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_timeout);
 
@@ -9545,31 +9561,31 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("reconfig", 0);
 
-  /* "pysoem/pysoem.pyx":738
+  /* "pysoem/pysoem.pyx":745
  *         :rtype: int
  *         """
  *         return cpysoem.ecx_reconfig_slave(self._ecx_contextt, self._pos, timeout)             # <<<<<<<<<<<<<<
  * 
  *     def recover(self, timeout=500):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 738, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 738, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(ecx_reconfig_slave(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 738, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 745, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 745, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(ecx_reconfig_slave(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":731
+  /* "pysoem/pysoem.pyx":738
  *         return cpysoem.ecx_statecheck(self._ecx_contextt, self._pos, expected_state, timeout)
  * 
  *     def reconfig(self, timeout=500):             # <<<<<<<<<<<<<<
  *         """Reconfigure slave.
  * 
  */
 
@@ -9580,15 +9596,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":740
+/* "pysoem/pysoem.pyx":747
  *         return cpysoem.ecx_reconfig_slave(self._ecx_contextt, self._pos, timeout)
  * 
  *     def recover(self, timeout=500):             # <<<<<<<<<<<<<<
  *         """Recover slave.
  * 
  */
 
@@ -9621,29 +9637,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recover") < 0)) __PYX_ERR(0, 740, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "recover") < 0)) __PYX_ERR(0, 747, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_timeout = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("recover", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 740, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("recover", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 747, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.recover", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_16recover(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_timeout);
 
@@ -9659,31 +9675,31 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("recover", 0);
 
-  /* "pysoem/pysoem.pyx":747
+  /* "pysoem/pysoem.pyx":754
  *         :rtype: int
  *         """
  *         return cpysoem.ecx_recover_slave(self._ecx_contextt, self._pos, timeout)             # <<<<<<<<<<<<<<
  * 
  *     def eeprom_read(self, int word_address, timeout=20000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 747, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 747, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(ecx_recover_slave(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 747, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 754, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 754, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(ecx_recover_slave(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 754, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":740
+  /* "pysoem/pysoem.pyx":747
  *         return cpysoem.ecx_reconfig_slave(self._ecx_contextt, self._pos, timeout)
  * 
  *     def recover(self, timeout=500):             # <<<<<<<<<<<<<<
  *         """Recover slave.
  * 
  */
 
@@ -9694,15 +9710,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":749
+/* "pysoem/pysoem.pyx":756
  *         return cpysoem.ecx_recover_slave(self._ecx_contextt, self._pos, timeout)
  * 
  *     def eeprom_read(self, int word_address, timeout=20000):             # <<<<<<<<<<<<<<
  *         """Read 4 byte from EEPROM
  * 
  */
 
@@ -9742,31 +9758,31 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "eeprom_read") < 0)) __PYX_ERR(0, 749, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "eeprom_read") < 0)) __PYX_ERR(0, 756, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_word_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_word_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 749, __pyx_L3_error)
+    __pyx_v_word_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_word_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
     __pyx_v_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("eeprom_read", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 749, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("eeprom_read", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 756, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.eeprom_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_18eeprom_read(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_word_address, __pyx_v_timeout);
 
@@ -9783,40 +9799,40 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("eeprom_read", 0);
 
-  /* "pysoem/pysoem.pyx":761
+  /* "pysoem/pysoem.pyx":768
  *             bytes: EEPROM data
  *         """
  *         cdef uint32_t tmp = cpysoem.ecx_readeeprom(self._ecx_contextt, self._pos, word_address, timeout)             # <<<<<<<<<<<<<<
  *         return PyBytes_FromStringAndSize(<char*>&tmp, 4)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 768, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 768, __pyx_L1_error)
   __pyx_v_tmp = ecx_readeeprom(__pyx_v_self->_ecx_contextt, __pyx_t_1, __pyx_v_word_address, __pyx_t_2);
 
-  /* "pysoem/pysoem.pyx":762
+  /* "pysoem/pysoem.pyx":769
  *         """
  *         cdef uint32_t tmp = cpysoem.ecx_readeeprom(self._ecx_contextt, self._pos, word_address, timeout)
  *         return PyBytes_FromStringAndSize(<char*>&tmp, 4)             # <<<<<<<<<<<<<<
  * 
  *     def eeprom_write(self, int word_address, bytes data, timeout=20000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyBytes_FromStringAndSize(((char *)(&__pyx_v_tmp)), 4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_3 = PyBytes_FromStringAndSize(((char *)(&__pyx_v_tmp)), 4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 769, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":749
+  /* "pysoem/pysoem.pyx":756
  *         return cpysoem.ecx_recover_slave(self._ecx_contextt, self._pos, timeout)
  * 
  *     def eeprom_read(self, int word_address, timeout=20000):             # <<<<<<<<<<<<<<
  *         """Read 4 byte from EEPROM
  * 
  */
 
@@ -9827,15 +9843,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":764
+/* "pysoem/pysoem.pyx":771
  *         return PyBytes_FromStringAndSize(<char*>&tmp, 4)
  * 
  *     def eeprom_write(self, int word_address, bytes data, timeout=20000):             # <<<<<<<<<<<<<<
  *         """Write 2 byte (1 word) to EEPROM
  * 
  */
 
@@ -9874,49 +9890,49 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_word_address)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("eeprom_write", 0, 2, 3, 1); __PYX_ERR(0, 764, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("eeprom_write", 0, 2, 3, 1); __PYX_ERR(0, 771, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "eeprom_write") < 0)) __PYX_ERR(0, 764, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "eeprom_write") < 0)) __PYX_ERR(0, 771, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_word_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_word_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 764, __pyx_L3_error)
+    __pyx_v_word_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_word_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 771, __pyx_L3_error)
     __pyx_v_data = ((PyObject*)values[1]);
     __pyx_v_timeout = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("eeprom_write", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 764, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("eeprom_write", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 771, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.eeprom_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 764, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 771, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_20eeprom_write(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_word_address, __pyx_v_data, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9938,124 +9954,124 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("eeprom_write", 0);
 
-  /* "pysoem/pysoem.pyx":778
+  /* "pysoem/pysoem.pyx":785
  *             AttributeError: if data size is not 2
  *         """
  *         if not len(data) == 2:             # <<<<<<<<<<<<<<
  *             raise AttributeError()
  *         cdef uint16_t tmp
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 778, __pyx_L1_error)
+    __PYX_ERR(0, 785, __pyx_L1_error)
   }
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 778, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 785, __pyx_L1_error)
   __pyx_t_2 = ((!((__pyx_t_1 == 2) != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pysoem/pysoem.pyx":779
+    /* "pysoem/pysoem.pyx":786
  *         """
  *         if not len(data) == 2:
  *             raise AttributeError()             # <<<<<<<<<<<<<<
  *         cdef uint16_t tmp
  *         memcpy(<char*>&tmp, <unsigned char*>data, 2)
  */
-    __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 779, __pyx_L1_error)
+    __PYX_ERR(0, 786, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":778
+    /* "pysoem/pysoem.pyx":785
  *             AttributeError: if data size is not 2
  *         """
  *         if not len(data) == 2:             # <<<<<<<<<<<<<<
  *             raise AttributeError()
  *         cdef uint16_t tmp
  */
   }
 
-  /* "pysoem/pysoem.pyx":781
+  /* "pysoem/pysoem.pyx":788
  *             raise AttributeError()
  *         cdef uint16_t tmp
  *         memcpy(<char*>&tmp, <unsigned char*>data, 2)             # <<<<<<<<<<<<<<
  *         cdef int result = cpysoem.ecx_writeeeprom(self._ecx_contextt, self._pos, word_address, tmp, timeout)
  *         if not result > 0:
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 781, __pyx_L1_error)
+    __PYX_ERR(0, 788, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 781, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 788, __pyx_L1_error)
   (void)(memcpy(((char *)(&__pyx_v_tmp)), ((unsigned char *)__pyx_t_4), 2));
 
-  /* "pysoem/pysoem.pyx":782
+  /* "pysoem/pysoem.pyx":789
  *         cdef uint16_t tmp
  *         memcpy(<char*>&tmp, <unsigned char*>data, 2)
  *         cdef int result = cpysoem.ecx_writeeeprom(self._ecx_contextt, self._pos, word_address, tmp, timeout)             # <<<<<<<<<<<<<<
  *         if not result > 0:
  *             raise EepromError('EEPROM write error')
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 782, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 782, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 789, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 789, __pyx_L1_error)
   __pyx_v_result = ecx_writeeeprom(__pyx_v_self->_ecx_contextt, __pyx_t_5, __pyx_v_word_address, __pyx_v_tmp, __pyx_t_6);
 
-  /* "pysoem/pysoem.pyx":783
+  /* "pysoem/pysoem.pyx":790
  *         memcpy(<char*>&tmp, <unsigned char*>data, 2)
  *         cdef int result = cpysoem.ecx_writeeeprom(self._ecx_contextt, self._pos, word_address, tmp, timeout)
  *         if not result > 0:             # <<<<<<<<<<<<<<
  *             raise EepromError('EEPROM write error')
  * 
  */
   __pyx_t_2 = ((!((__pyx_v_result > 0) != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pysoem/pysoem.pyx":784
+    /* "pysoem/pysoem.pyx":791
  *         cdef int result = cpysoem.ecx_writeeeprom(self._ecx_contextt, self._pos, word_address, tmp, timeout)
  *         if not result > 0:
  *             raise EepromError('EEPROM write error')             # <<<<<<<<<<<<<<
  * 
  *     def foe_write(self, filename, password, bytes data, timeout = 200000):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_EepromError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 784, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_EepromError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_kp_s_EEPROM_write_error) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_s_EEPROM_write_error);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 784, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 784, __pyx_L1_error)
+    __PYX_ERR(0, 791, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":783
+    /* "pysoem/pysoem.pyx":790
  *         memcpy(<char*>&tmp, <unsigned char*>data, 2)
  *         cdef int result = cpysoem.ecx_writeeeprom(self._ecx_contextt, self._pos, word_address, tmp, timeout)
  *         if not result > 0:             # <<<<<<<<<<<<<<
  *             raise EepromError('EEPROM write error')
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":764
+  /* "pysoem/pysoem.pyx":771
  *         return PyBytes_FromStringAndSize(<char*>&tmp, 4)
  * 
  *     def eeprom_write(self, int word_address, bytes data, timeout=20000):             # <<<<<<<<<<<<<<
  *         """Write 2 byte (1 word) to EEPROM
  * 
  */
 
@@ -10070,15 +10086,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":786
+/* "pysoem/pysoem.pyx":793
  *             raise EepromError('EEPROM write error')
  * 
  *     def foe_write(self, filename, password, bytes data, timeout = 200000):             # <<<<<<<<<<<<<<
  *         """ Write given data to device using FoE
  * 
  */
 
@@ -10120,31 +10136,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_password)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, 1); __PYX_ERR(0, 786, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, 1); __PYX_ERR(0, 793, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, 2); __PYX_ERR(0, 786, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, 2); __PYX_ERR(0, 793, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "foe_write") < 0)) __PYX_ERR(0, 786, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "foe_write") < 0)) __PYX_ERR(0, 793, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -10156,21 +10172,21 @@
     __pyx_v_filename = values[0];
     __pyx_v_password = values[1];
     __pyx_v_data = ((PyObject*)values[2]);
     __pyx_v_timeout = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 786, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("foe_write", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 793, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.foe_write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 786, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 793, __pyx_L1_error)
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_22foe_write(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_filename, __pyx_v_password, __pyx_v_data, __pyx_v_timeout);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -10195,163 +10211,163 @@
   unsigned char *__pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("foe_write", 0);
 
-  /* "pysoem/pysoem.pyx":796
+  /* "pysoem/pysoem.pyx":803
  *         """
  *         # error handling
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_ecx_contextt == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":797
+    /* "pysoem/pysoem.pyx":804
  *         # error handling
  *         if self._ecx_contextt == NULL:
  *             raise UnboundLocalError()             # <<<<<<<<<<<<<<
  * 
  *         cdef int size = len(data)
  */
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 804, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 797, __pyx_L1_error)
+    __PYX_ERR(0, 804, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":796
+    /* "pysoem/pysoem.pyx":803
  *         """
  *         # error handling
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":799
+  /* "pysoem/pysoem.pyx":806
  *             raise UnboundLocalError()
  * 
  *         cdef int size = len(data)             # <<<<<<<<<<<<<<
  *         cdef int result = cpysoem.ecx_FOEwrite(self._ecx_contextt, self._pos, filename.encode('utf8'), password, size, <unsigned char*>data, timeout)
  * 
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 799, __pyx_L1_error)
+    __PYX_ERR(0, 806, __pyx_L1_error)
   }
-  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_3 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 806, __pyx_L1_error)
   __pyx_v_size = __pyx_t_3;
 
-  /* "pysoem/pysoem.pyx":800
+  /* "pysoem/pysoem.pyx":807
  * 
  *         cdef int size = len(data)
  *         cdef int result = cpysoem.ecx_FOEwrite(self._ecx_contextt, self._pos, filename.encode('utf8'), password, size, <unsigned char*>data, timeout)             # <<<<<<<<<<<<<<
  * 
  *         # error handling
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 807, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 800, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 807, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_uint32_t(__pyx_v_password); if (unlikely((__pyx_t_8 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 807, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint32_t(__pyx_v_password); if (unlikely((__pyx_t_8 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 807, __pyx_L1_error)
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 800, __pyx_L1_error)
+    __PYX_ERR(0, 807, __pyx_L1_error)
   }
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 807, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 807, __pyx_L1_error)
   __pyx_v_result = ecx_FOEwrite(__pyx_v_self->_ecx_contextt, __pyx_t_4, __pyx_t_7, __pyx_t_8, __pyx_v_size, ((unsigned char *)__pyx_t_9), __pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":804
+  /* "pysoem/pysoem.pyx":811
  *         # error handling
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)
  */
   __pyx_t_1 = (ecx_poperror(__pyx_v_self->_ecx_contextt, (&__pyx_v_err)) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":805
+    /* "pysoem/pysoem.pyx":812
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             assert err.Slave == self._pos             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(__pyx_assertions_enabled())) {
-      __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 805, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 812, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = PyObject_RichCompare(__pyx_t_2, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 805, __pyx_L1_error)
+      __pyx_t_5 = PyObject_RichCompare(__pyx_t_2, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 812, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 805, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 812, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_1)) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 805, __pyx_L1_error)
+        __PYX_ERR(0, 812, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "pysoem/pysoem.pyx":806
+    /* "pysoem/pysoem.pyx":813
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)             # <<<<<<<<<<<<<<
  * 
  *         return result
  */
-    __pyx_t_5 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 806, __pyx_L1_error)
+    __pyx_t_5 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pysoem/pysoem.pyx":804
+    /* "pysoem/pysoem.pyx":811
  *         # error handling
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)
  */
   }
 
-  /* "pysoem/pysoem.pyx":808
+  /* "pysoem/pysoem.pyx":815
  *             self._raise_exception(&err)
  * 
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     def foe_read(self, filename, password, size, timeout = 200000):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 808, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 815, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":786
+  /* "pysoem/pysoem.pyx":793
  *             raise EepromError('EEPROM write error')
  * 
  *     def foe_write(self, filename, password, bytes data, timeout = 200000):             # <<<<<<<<<<<<<<
  *         """ Write given data to device using FoE
  * 
  */
 
@@ -10364,15 +10380,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":810
+/* "pysoem/pysoem.pyx":817
  *         return result
  * 
  *     def foe_read(self, filename, password, size, timeout = 200000):             # <<<<<<<<<<<<<<
  *         """ Read given filename from device using FoE
  * 
  */
 
@@ -10414,31 +10430,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_password)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, 1); __PYX_ERR(0, 810, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, 1); __PYX_ERR(0, 817, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, 2); __PYX_ERR(0, 810, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, 2); __PYX_ERR(0, 817, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "foe_read") < 0)) __PYX_ERR(0, 810, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "foe_read") < 0)) __PYX_ERR(0, 817, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -10450,15 +10466,15 @@
     __pyx_v_filename = values[0];
     __pyx_v_password = values[1];
     __pyx_v_size = values[2];
     __pyx_v_timeout = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 810, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("foe_read", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 817, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.foe_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_24foe_read(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_filename, __pyx_v_password, __pyx_v_size, __pyx_v_timeout);
 
@@ -10492,189 +10508,189 @@
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("foe_read", 0);
 
-  /* "pysoem/pysoem.pyx":819
+  /* "pysoem/pysoem.pyx":826
  *             timeout (int): Timeout value in us
  *         """
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_ecx_contextt == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":820
+    /* "pysoem/pysoem.pyx":827
  *         """
  *         if self._ecx_contextt == NULL:
  *             raise UnboundLocalError()             # <<<<<<<<<<<<<<
  * 
  *         # prepare call of c function
  */
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 820, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_UnboundLocalError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 827, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 820, __pyx_L1_error)
+    __PYX_ERR(0, 827, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":819
+    /* "pysoem/pysoem.pyx":826
  *             timeout (int): Timeout value in us
  *         """
  *         if self._ecx_contextt == NULL:             # <<<<<<<<<<<<<<
  *             raise UnboundLocalError()
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":825
+  /* "pysoem/pysoem.pyx":832
  *         cdef unsigned char* pbuf
  *         cdef int size_inout
  *         pbuf = <unsigned char*>PyMem_Malloc((size)*sizeof(unsigned char))             # <<<<<<<<<<<<<<
  *         size_inout = size
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_FromSize_t((sizeof(unsigned char))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 825, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_FromSize_t((sizeof(unsigned char))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_v_size, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 825, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_v_size, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_4 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 825, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_4 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_pbuf = ((unsigned char *)PyMem_Malloc(__pyx_t_4));
 
-  /* "pysoem/pysoem.pyx":826
+  /* "pysoem/pysoem.pyx":833
  *         cdef int size_inout
  *         pbuf = <unsigned char*>PyMem_Malloc((size)*sizeof(unsigned char))
  *         size_inout = size             # <<<<<<<<<<<<<<
  * 
  *         cdef int result = cpysoem.ecx_FOEread(self._ecx_contextt, self._pos, filename.encode('utf8'), password, &size_inout, pbuf, timeout)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_size); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 826, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_size); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 833, __pyx_L1_error)
   __pyx_v_size_inout = __pyx_t_5;
 
-  /* "pysoem/pysoem.pyx":828
+  /* "pysoem/pysoem.pyx":835
  *         size_inout = size
  * 
  *         cdef int result = cpysoem.ecx_FOEread(self._ecx_contextt, self._pos, filename.encode('utf8'), password, &size_inout, pbuf, timeout)             # <<<<<<<<<<<<<<
  * 
  *         # error handling
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_6 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 828, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 828, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_6 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_n_s_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_utf8);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 828, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_password); if (unlikely((__pyx_t_9 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 828, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 828, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsWritableString(__pyx_t_3); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_password); if (unlikely((__pyx_t_9 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_timeout); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 835, __pyx_L1_error)
   __pyx_v_result = ecx_FOEread(__pyx_v_self->_ecx_contextt, __pyx_t_6, __pyx_t_8, __pyx_t_9, (&__pyx_v_size_inout), __pyx_v_pbuf, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":832
+  /* "pysoem/pysoem.pyx":839
  *         # error handling
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  */
   __pyx_t_1 = (ecx_poperror(__pyx_v_self->_ecx_contextt, (&__pyx_v_err)) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":833
+    /* "pysoem/pysoem.pyx":840
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             PyMem_Free(pbuf)             # <<<<<<<<<<<<<<
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)
  */
     PyMem_Free(__pyx_v_pbuf);
 
-    /* "pysoem/pysoem.pyx":834
+    /* "pysoem/pysoem.pyx":841
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):
  *             PyMem_Free(pbuf)
  *             assert err.Slave == self._pos             # <<<<<<<<<<<<<<
  *             self._raise_exception(&err)
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(__pyx_assertions_enabled())) {
-      __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 834, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err.Slave); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 834, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_t_3, __pyx_v_self->_pos, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 834, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 841, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (unlikely(!__pyx_t_1)) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 834, __pyx_L1_error)
+        __PYX_ERR(0, 841, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "pysoem/pysoem.pyx":835
+    /* "pysoem/pysoem.pyx":842
  *             PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  *             self._raise_exception(&err)             # <<<<<<<<<<<<<<
  * 
  *         # return data
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 835, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_6pysoem_6pysoem_CdefSlave *)__pyx_v_self->__pyx_vtab)->_raise_exception(__pyx_v_self, (&__pyx_v_err)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 842, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":832
+    /* "pysoem/pysoem.pyx":839
  *         # error handling
  *         cdef cpysoem.ec_errort err
  *         if cpysoem.ecx_poperror(self._ecx_contextt, &err):             # <<<<<<<<<<<<<<
  *             PyMem_Free(pbuf)
  *             assert err.Slave == self._pos
  */
   }
 
-  /* "pysoem/pysoem.pyx":838
+  /* "pysoem/pysoem.pyx":845
  * 
  *         # return data
  *         try:             # <<<<<<<<<<<<<<
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  */
   /*try:*/ {
 
-    /* "pysoem/pysoem.pyx":839
+    /* "pysoem/pysoem.pyx":846
  *         # return data
  *         try:
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)             # <<<<<<<<<<<<<<
  *         finally:
  *             PyMem_Free(pbuf)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyBytes_FromStringAndSize(((char *)__pyx_v_pbuf), __pyx_v_size_inout); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 839, __pyx_L6_error)
+    __pyx_t_2 = PyBytes_FromStringAndSize(((char *)__pyx_v_pbuf), __pyx_v_size_inout); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 846, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L5_return;
   }
 
-  /* "pysoem/pysoem.pyx":841
+  /* "pysoem/pysoem.pyx":848
  *             return PyBytes_FromStringAndSize(<char*>pbuf, size_inout)
  *         finally:
  *             PyMem_Free(pbuf)             # <<<<<<<<<<<<<<
  * 
  *     def amend_mbx(self, mailbox, start_address, size):
  */
   /*finally:*/ {
@@ -10718,15 +10734,15 @@
       PyMem_Free(__pyx_v_pbuf);
       __pyx_r = __pyx_t_17;
       __pyx_t_17 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "pysoem/pysoem.pyx":810
+  /* "pysoem/pysoem.pyx":817
  *         return result
  * 
  *     def foe_read(self, filename, password, size, timeout = 200000):             # <<<<<<<<<<<<<<
  *         """ Read given filename from device using FoE
  * 
  */
 
@@ -10739,15 +10755,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":843
+/* "pysoem/pysoem.pyx":850
  *             PyMem_Free(pbuf)
  * 
  *     def amend_mbx(self, mailbox, start_address, size):             # <<<<<<<<<<<<<<
  *         """Change the start address and size of a mailbox.
  * 
  */
 
@@ -10785,40 +10801,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mailbox)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start_address)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, 1); __PYX_ERR(0, 843, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, 1); __PYX_ERR(0, 850, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, 2); __PYX_ERR(0, 843, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, 2); __PYX_ERR(0, 850, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "amend_mbx") < 0)) __PYX_ERR(0, 843, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "amend_mbx") < 0)) __PYX_ERR(0, 850, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_mailbox = values[0];
     __pyx_v_start_address = values[1];
     __pyx_v_size = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 843, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("amend_mbx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 850, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.amend_mbx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_26amend_mbx(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_mailbox, __pyx_v_start_address, __pyx_v_size);
 
@@ -10842,47 +10858,47 @@
   uint16 __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("amend_mbx", 0);
 
-  /* "pysoem/pysoem.pyx":854
+  /* "pysoem/pysoem.pyx":861
  *         .. versionadded:: 1.0.6
  *         """
  *         fpwr_timeout_us = 4000             # <<<<<<<<<<<<<<
  *         if mailbox == 'out':
  *             # Clear the slaves mailbox configuration.
  */
   __pyx_v_fpwr_timeout_us = 0xFA0;
 
-  /* "pysoem/pysoem.pyx":855
+  /* "pysoem/pysoem.pyx":862
  *         """
  *         fpwr_timeout_us = 4000
  *         if mailbox == 'out':             # <<<<<<<<<<<<<<
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0, bytes(sizeof(self._ec_slave.SM[0])))
  */
-  __pyx_t_1 = (__Pyx_PyString_Equals(__pyx_v_mailbox, __pyx_n_s_out, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 855, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyString_Equals(__pyx_v_mailbox, __pyx_n_s_out, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 862, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":857
+    /* "pysoem/pysoem.pyx":864
  *         if mailbox == 'out':
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0, bytes(sizeof(self._ec_slave.SM[0])))             # <<<<<<<<<<<<<<
  *             self._ec_slave.SM[0].StartAddr = start_address
  *             self._ec_slave.SM[0].SMlength = size
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 857, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ECT_REG_SM0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 857, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ECT_REG_SM0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_FromSize_t((sizeof((__pyx_v_self->_ec_slave->SM[0])))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 857, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_FromSize_t((sizeof((__pyx_v_self->_ec_slave->SM[0])))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 857, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
@@ -10892,120 +10908,120 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 857, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 857, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 857, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 864, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 857, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":858
+    /* "pysoem/pysoem.pyx":865
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0, bytes(sizeof(self._ec_slave.SM[0])))
  *             self._ec_slave.SM[0].StartAddr = start_address             # <<<<<<<<<<<<<<
  *             self._ec_slave.SM[0].SMlength = size
  *             self._ec_slave.mbx_wo = start_address
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 858, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 865, __pyx_L1_error)
     (__pyx_v_self->_ec_slave->SM[0]).StartAddr = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":859
+    /* "pysoem/pysoem.pyx":866
  *             self._fpwr(ECT_REG_SM0, bytes(sizeof(self._ec_slave.SM[0])))
  *             self._ec_slave.SM[0].StartAddr = start_address
  *             self._ec_slave.SM[0].SMlength = size             # <<<<<<<<<<<<<<
  *             self._ec_slave.mbx_wo = start_address
  *             self._ec_slave.mbx_l = size
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 859, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 866, __pyx_L1_error)
     (__pyx_v_self->_ec_slave->SM[0]).SMlength = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":860
+    /* "pysoem/pysoem.pyx":867
  *             self._ec_slave.SM[0].StartAddr = start_address
  *             self._ec_slave.SM[0].SMlength = size
  *             self._ec_slave.mbx_wo = start_address             # <<<<<<<<<<<<<<
  *             self._ec_slave.mbx_l = size
  *             # Update the slaves mailbox configuration.
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 860, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 867, __pyx_L1_error)
     __pyx_v_self->_ec_slave->mbx_wo = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":861
+    /* "pysoem/pysoem.pyx":868
  *             self._ec_slave.SM[0].SMlength = size
  *             self._ec_slave.mbx_wo = start_address
  *             self._ec_slave.mbx_l = size             # <<<<<<<<<<<<<<
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0,
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 861, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 868, __pyx_L1_error)
     __pyx_v_self->_ec_slave->mbx_l = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":863
+    /* "pysoem/pysoem.pyx":870
  *             self._ec_slave.mbx_l = size
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0,             # <<<<<<<<<<<<<<
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[0], sizeof(self._ec_slave.SM[0])),
  *                        fpwr_timeout_us)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 863, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 870, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ECT_REG_SM0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 863, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ECT_REG_SM0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 870, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
 
-    /* "pysoem/pysoem.pyx":864
+    /* "pysoem/pysoem.pyx":871
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0,
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[0], sizeof(self._ec_slave.SM[0])),             # <<<<<<<<<<<<<<
  *                        fpwr_timeout_us)
  *         elif mailbox == 'in':
  */
-    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)(&(__pyx_v_self->_ec_slave->SM[0]))), (sizeof((__pyx_v_self->_ec_slave->SM[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 864, __pyx_L1_error)
+    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)(&(__pyx_v_self->_ec_slave->SM[0]))), (sizeof((__pyx_v_self->_ec_slave->SM[0])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 871, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":865
+    /* "pysoem/pysoem.pyx":872
  *             self._fpwr(ECT_REG_SM0,
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[0], sizeof(self._ec_slave.SM[0])),
  *                        fpwr_timeout_us)             # <<<<<<<<<<<<<<
  *         elif mailbox == 'in':
  *             # Clear the slaves mailbox configuration.
  */
-    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_fpwr_timeout_us); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 865, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_fpwr_timeout_us); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 872, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11014,89 +11030,89 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_8, __pyx_t_6, __pyx_t_4};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 863, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_8, __pyx_t_6, __pyx_t_4};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 863, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_10 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 863, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 870, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_7, __pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_7, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_7, __pyx_t_4);
       __pyx_t_8 = 0;
       __pyx_t_6 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 863, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":855
+    /* "pysoem/pysoem.pyx":862
  *         """
  *         fpwr_timeout_us = 4000
  *         if mailbox == 'out':             # <<<<<<<<<<<<<<
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM0, bytes(sizeof(self._ec_slave.SM[0])))
  */
     goto __pyx_L3;
   }
 
-  /* "pysoem/pysoem.pyx":866
+  /* "pysoem/pysoem.pyx":873
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[0], sizeof(self._ec_slave.SM[0])),
  *                        fpwr_timeout_us)
  *         elif mailbox == 'in':             # <<<<<<<<<<<<<<
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1, bytes(sizeof(self._ec_slave.SM[1])))
  */
-  __pyx_t_1 = (__Pyx_PyString_Equals(__pyx_v_mailbox, __pyx_n_s_in, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 866, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyString_Equals(__pyx_v_mailbox, __pyx_n_s_in, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 873, __pyx_L1_error)
   if (likely(__pyx_t_1)) {
 
-    /* "pysoem/pysoem.pyx":868
+    /* "pysoem/pysoem.pyx":875
  *         elif mailbox == 'in':
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1, bytes(sizeof(self._ec_slave.SM[1])))             # <<<<<<<<<<<<<<
  *             self._ec_slave.SM[1].StartAddr = start_address
  *             self._ec_slave.SM[1].SMlength = size
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 868, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 875, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_ECT_REG_SM1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 868, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_ECT_REG_SM1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 875, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t((sizeof((__pyx_v_self->_ec_slave->SM[1])))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 868, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t((sizeof((__pyx_v_self->_ec_slave->SM[1])))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 875, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 868, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 875, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -11106,120 +11122,120 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_10, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 868, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 875, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_10, __pyx_t_6};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 868, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 875, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 868, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 875, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_6);
       __pyx_t_10 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 868, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 875, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":869
+    /* "pysoem/pysoem.pyx":876
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1, bytes(sizeof(self._ec_slave.SM[1])))
  *             self._ec_slave.SM[1].StartAddr = start_address             # <<<<<<<<<<<<<<
  *             self._ec_slave.SM[1].SMlength = size
  *             self._ec_slave.mbx_ro = start_address
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 869, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 876, __pyx_L1_error)
     (__pyx_v_self->_ec_slave->SM[1]).StartAddr = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":870
+    /* "pysoem/pysoem.pyx":877
  *             self._fpwr(ECT_REG_SM1, bytes(sizeof(self._ec_slave.SM[1])))
  *             self._ec_slave.SM[1].StartAddr = start_address
  *             self._ec_slave.SM[1].SMlength = size             # <<<<<<<<<<<<<<
  *             self._ec_slave.mbx_ro = start_address
  *             self._ec_slave.mbx_rl = size
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 877, __pyx_L1_error)
     (__pyx_v_self->_ec_slave->SM[1]).SMlength = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":871
+    /* "pysoem/pysoem.pyx":878
  *             self._ec_slave.SM[1].StartAddr = start_address
  *             self._ec_slave.SM[1].SMlength = size
  *             self._ec_slave.mbx_ro = start_address             # <<<<<<<<<<<<<<
  *             self._ec_slave.mbx_rl = size
  *             # Update the slaves mailbox configuration.
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 871, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_start_address); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 878, __pyx_L1_error)
     __pyx_v_self->_ec_slave->mbx_ro = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":872
+    /* "pysoem/pysoem.pyx":879
  *             self._ec_slave.SM[1].SMlength = size
  *             self._ec_slave.mbx_ro = start_address
  *             self._ec_slave.mbx_rl = size             # <<<<<<<<<<<<<<
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1,
  */
-    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 872, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_uint16_t(__pyx_v_size); if (unlikely((__pyx_t_9 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 879, __pyx_L1_error)
     __pyx_v_self->_ec_slave->mbx_rl = __pyx_t_9;
 
-    /* "pysoem/pysoem.pyx":874
+    /* "pysoem/pysoem.pyx":881
  *             self._ec_slave.mbx_rl = size
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1,             # <<<<<<<<<<<<<<
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[1], sizeof(self._ec_slave.SM[1])),
  *                        fpwr_timeout_us)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 881, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ECT_REG_SM1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_ECT_REG_SM1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 881, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
 
-    /* "pysoem/pysoem.pyx":875
+    /* "pysoem/pysoem.pyx":882
  *             # Update the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1,
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[1], sizeof(self._ec_slave.SM[1])),             # <<<<<<<<<<<<<<
  *                        fpwr_timeout_us)
  *         else:
  */
-    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)(&(__pyx_v_self->_ec_slave->SM[1]))), (sizeof((__pyx_v_self->_ec_slave->SM[1])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 875, __pyx_L1_error)
+    __pyx_t_6 = PyBytes_FromStringAndSize(((char *)(&(__pyx_v_self->_ec_slave->SM[1]))), (sizeof((__pyx_v_self->_ec_slave->SM[1])))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 882, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":876
+    /* "pysoem/pysoem.pyx":883
  *             self._fpwr(ECT_REG_SM1,
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[1], sizeof(self._ec_slave.SM[1])),
  *                        fpwr_timeout_us)             # <<<<<<<<<<<<<<
  *         else:
  *             raise AttributeError()
  */
-    __pyx_t_10 = __Pyx_PyInt_From_long(__pyx_v_fpwr_timeout_us); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 876, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_long(__pyx_v_fpwr_timeout_us); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 883, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_4 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11228,82 +11244,82 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_8, __pyx_t_6, __pyx_t_10};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_t_8, __pyx_t_6, __pyx_t_10};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 874, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 881, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_10);
       PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_7, __pyx_t_10);
       __pyx_t_8 = 0;
       __pyx_t_6 = 0;
       __pyx_t_10 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":866
+    /* "pysoem/pysoem.pyx":873
  *                        PyBytes_FromStringAndSize(<char*>&self._ec_slave.SM[0], sizeof(self._ec_slave.SM[0])),
  *                        fpwr_timeout_us)
  *         elif mailbox == 'in':             # <<<<<<<<<<<<<<
  *             # Clear the slaves mailbox configuration.
  *             self._fpwr(ECT_REG_SM1, bytes(sizeof(self._ec_slave.SM[1])))
  */
     goto __pyx_L3;
   }
 
-  /* "pysoem/pysoem.pyx":878
+  /* "pysoem/pysoem.pyx":885
  *                        fpwr_timeout_us)
  *         else:
  *             raise AttributeError()             # <<<<<<<<<<<<<<
  * 
  *     def set_watchdog(self, wd_type, wd_time_ms):
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 878, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 878, __pyx_L1_error)
+    __PYX_ERR(0, 885, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pysoem/pysoem.pyx":843
+  /* "pysoem/pysoem.pyx":850
  *             PyMem_Free(pbuf)
  * 
  *     def amend_mbx(self, mailbox, start_address, size):             # <<<<<<<<<<<<<<
  *         """Change the start address and size of a mailbox.
  * 
  */
 
@@ -11322,15 +11338,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":880
+/* "pysoem/pysoem.pyx":887
  *             raise AttributeError()
  * 
  *     def set_watchdog(self, wd_type, wd_time_ms):             # <<<<<<<<<<<<<<
  *         """Change the watchdog time of the PDI or Process Data watchdog.
  * 
  */
 
@@ -11365,32 +11381,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_wd_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_wd_time_ms)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_watchdog", 1, 2, 2, 1); __PYX_ERR(0, 880, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_watchdog", 1, 2, 2, 1); __PYX_ERR(0, 887, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_watchdog") < 0)) __PYX_ERR(0, 880, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_watchdog") < 0)) __PYX_ERR(0, 887, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_wd_type = values[0];
     __pyx_v_wd_time_ms = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_watchdog", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 880, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_watchdog", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 887, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.set_watchdog", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_28set_watchdog(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_wd_type, __pyx_v_wd_time_ms);
 
@@ -11420,101 +11436,101 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_watchdog", 0);
 
-  /* "pysoem/pysoem.pyx":892
+  /* "pysoem/pysoem.pyx":899
  *         .. versionadded:: 1.0.6
  *         """
  *         fprd_fpwr_timeout_us = 4000             # <<<<<<<<<<<<<<
  *         wd_type_to_reg_map = {
  *             'pdi': ECT_REG_WD_TIME_PDI,
  */
   __pyx_v_fprd_fpwr_timeout_us = 0xFA0;
 
-  /* "pysoem/pysoem.pyx":894
+  /* "pysoem/pysoem.pyx":901
  *         fprd_fpwr_timeout_us = 4000
  *         wd_type_to_reg_map = {
  *             'pdi': ECT_REG_WD_TIME_PDI,             # <<<<<<<<<<<<<<
  *             'processdata': ECT_REG_WD_TIME_PROCESSDATA,
  *         }
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 894, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ECT_REG_WD_TIME_PDI); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 894, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ECT_REG_WD_TIME_PDI); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 901, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_pdi, __pyx_t_2) < 0) __PYX_ERR(0, 894, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_pdi, __pyx_t_2) < 0) __PYX_ERR(0, 901, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":895
+  /* "pysoem/pysoem.pyx":902
  *         wd_type_to_reg_map = {
  *             'pdi': ECT_REG_WD_TIME_PDI,
  *             'processdata': ECT_REG_WD_TIME_PROCESSDATA,             # <<<<<<<<<<<<<<
  *         }
  *         if wd_type not in wd_type_to_reg_map.keys():
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ECT_REG_WD_TIME_PROCESSDATA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 895, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ECT_REG_WD_TIME_PROCESSDATA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 902, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_processdata, __pyx_t_2) < 0) __PYX_ERR(0, 894, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_processdata, __pyx_t_2) < 0) __PYX_ERR(0, 901, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_wd_type_to_reg_map = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":897
+  /* "pysoem/pysoem.pyx":904
  *             'processdata': ECT_REG_WD_TIME_PROCESSDATA,
  *         }
  *         if wd_type not in wd_type_to_reg_map.keys():             # <<<<<<<<<<<<<<
  *             raise AttributeError()
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),
  */
-  __pyx_t_1 = __Pyx_PyDict_Keys(__pyx_v_wd_type_to_reg_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 897, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_Keys(__pyx_v_wd_type_to_reg_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 904, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_v_wd_type, __pyx_t_1, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 897, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_v_wd_type, __pyx_t_1, Py_NE)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 904, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pysoem/pysoem.pyx":898
+    /* "pysoem/pysoem.pyx":905
  *         }
  *         if wd_type not in wd_type_to_reg_map.keys():
  *             raise AttributeError()             # <<<<<<<<<<<<<<
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),
  *                                     byteorder='little',
  */
-    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 898, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_builtin_AttributeError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 905, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 898, __pyx_L1_error)
+    __PYX_ERR(0, 905, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":897
+    /* "pysoem/pysoem.pyx":904
  *             'processdata': ECT_REG_WD_TIME_PROCESSDATA,
  *         }
  *         if wd_type not in wd_type_to_reg_map.keys():             # <<<<<<<<<<<<<<
  *             raise AttributeError()
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),
  */
   }
 
-  /* "pysoem/pysoem.pyx":899
+  /* "pysoem/pysoem.pyx":906
  *         if wd_type not in wd_type_to_reg_map.keys():
  *             raise AttributeError()
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),             # <<<<<<<<<<<<<<
  *                                     byteorder='little',
  *                                     signed=False)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fprd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fprd); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ECT_REG_WD_DIV); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_ECT_REG_WD_DIV); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_fprd_fpwr_timeout_us); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_fprd_fpwr_timeout_us); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_8 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -11523,245 +11539,245 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_6, __pyx_int_2, __pyx_t_7};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 899, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_8, __pyx_t_6, __pyx_int_2, __pyx_t_7};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 899, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 899, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 906, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_6);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_int_2);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_9, __pyx_t_7);
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 899, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":900
+  /* "pysoem/pysoem.pyx":907
  *             raise AttributeError()
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),
  *                                     byteorder='little',             # <<<<<<<<<<<<<<
  *                                     signed=False)
  *         wd_div_ns = 40 * (wd_div_reg + 2)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 900, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 907, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 900, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 907, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":901
+  /* "pysoem/pysoem.pyx":908
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),
  *                                     byteorder='little',
  *                                     signed=False)             # <<<<<<<<<<<<<<
  *         wd_div_ns = 40 * (wd_div_reg + 2)
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 900, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 907, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":899
+  /* "pysoem/pysoem.pyx":906
  *         if wd_type not in wd_type_to_reg_map.keys():
  *             raise AttributeError()
  *         wd_div_reg = int.from_bytes(self._fprd(ECT_REG_WD_DIV, 2, fprd_fpwr_timeout_us),             # <<<<<<<<<<<<<<
  *                                     byteorder='little',
  *                                     signed=False)
  */
-  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 906, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_wd_div_reg = __pyx_t_10;
   __pyx_t_10 = 0;
 
-  /* "pysoem/pysoem.pyx":902
+  /* "pysoem/pysoem.pyx":909
  *                                     byteorder='little',
  *                                     signed=False)
  *         wd_div_ns = 40 * (wd_div_reg + 2)             # <<<<<<<<<<<<<<
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)
  *         if wd_time_reg > 0xFFFF:
  */
-  __pyx_t_10 = __Pyx_PyInt_AddObjC(__pyx_v_wd_div_reg, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 902, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_AddObjC(__pyx_v_wd_div_reg, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 909, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_int_40, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 902, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_int_40, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 909, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_wd_div_ns = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":903
+  /* "pysoem/pysoem.pyx":910
  *                                     signed=False)
  *         wd_div_ns = 40 * (wd_div_reg + 2)
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)             # <<<<<<<<<<<<<<
  *         if wd_time_reg > 0xFFFF:
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
  */
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_wd_time_ms, __pyx_float_1000000_0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 903, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_wd_time_ms, __pyx_float_1000000_0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 910, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_10 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 903, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 910, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 903, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 910, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_wd_time_reg = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":904
+  /* "pysoem/pysoem.pyx":911
  *         wd_div_ns = 40 * (wd_div_reg + 2)
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)
  *         if wd_time_reg > 0xFFFF:             # <<<<<<<<<<<<<<
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_wd_time_reg, __pyx_int_65535, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 904, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 904, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_wd_time_reg, __pyx_int_65535, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 911, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "pysoem/pysoem.pyx":905
+    /* "pysoem/pysoem.pyx":912
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)
  *         if wd_time_reg > 0xFFFF:
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0             # <<<<<<<<<<<<<<
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
  */
-    __pyx_t_2 = PyNumber_Multiply(__pyx_int_65535, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 905, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Multiply(__pyx_int_65535, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 912, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_10 = __Pyx_PyFloat_DivideObjC(__pyx_t_2, __pyx_float_1000000_0, 1000000.0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 905, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyFloat_DivideObjC(__pyx_t_2, __pyx_float_1000000_0, 1000000.0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 912, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_wd_time_ms_limit = __pyx_t_10;
     __pyx_t_10 = 0;
 
-    /* "pysoem/pysoem.pyx":906
+    /* "pysoem/pysoem.pyx":913
  *         if wd_time_reg > 0xFFFF:
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))             # <<<<<<<<<<<<<<
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
  *         self._fpwr(wd_type_to_reg_map[wd_type],
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_wd_time_ms_is_limited_to_ms, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_wd_time_ms_is_limited_to_ms, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 913, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_10 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_wd_time_ms_limit) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_wd_time_ms_limit);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 906, __pyx_L1_error)
+    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 913, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 906, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 913, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 906, __pyx_L1_error)
+    __PYX_ERR(0, 913, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":904
+    /* "pysoem/pysoem.pyx":911
  *         wd_div_ns = 40 * (wd_div_reg + 2)
  *         wd_time_reg = int((wd_time_ms*1000000.0) / wd_div_ns)
  *         if wd_time_reg > 0xFFFF:             # <<<<<<<<<<<<<<
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
  */
   }
 
-  /* "pysoem/pysoem.pyx":907
+  /* "pysoem/pysoem.pyx":914
  *             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0             # <<<<<<<<<<<<<<
  *         self._fpwr(wd_type_to_reg_map[wd_type],
  *                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),
  */
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_wd_time_reg, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 907, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_wd_time_reg, __pyx_v_wd_div_ns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 914, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_10 = __Pyx_PyFloat_DivideObjC(__pyx_t_2, __pyx_float_1000000_0, 1000000.0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 907, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyFloat_DivideObjC(__pyx_t_2, __pyx_float_1000000_0, 1000000.0, 0, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 914, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_actual_wd_time_ms = __pyx_t_10;
   __pyx_t_10 = 0;
 
-  /* "pysoem/pysoem.pyx":908
+  /* "pysoem/pysoem.pyx":915
  *             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
  *         self._fpwr(wd_type_to_reg_map[wd_type],             # <<<<<<<<<<<<<<
  *                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),
  *                    fprd_fpwr_timeout_us)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 908, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fpwr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 915, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_wd_type_to_reg_map, __pyx_v_wd_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 908, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_wd_type_to_reg_map, __pyx_v_wd_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 915, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "pysoem/pysoem.pyx":909
+  /* "pysoem/pysoem.pyx":916
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
  *         self._fpwr(wd_type_to_reg_map[wd_type],
  *                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),             # <<<<<<<<<<<<<<
  *                    fprd_fpwr_timeout_us)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wd_time_reg, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 909, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wd_time_reg, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 916, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 909, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 916, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 909, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 909, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__6, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 909, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_byteorder, __pyx_n_s_little) < 0) __PYX_ERR(0, 916, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 916, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__6, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 916, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pysoem/pysoem.pyx":910
+  /* "pysoem/pysoem.pyx":917
  *         self._fpwr(wd_type_to_reg_map[wd_type],
  *                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),
  *                    fprd_fpwr_timeout_us)             # <<<<<<<<<<<<<<
  * 
- *     def _fprd(self, int address, int size, timeout_us=2000):
+ *     def _disable_complete_access(self):
  */
-  __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_fprd_fpwr_timeout_us); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 910, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_fprd_fpwr_timeout_us); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 917, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_1 = NULL;
   __pyx_t_9 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -11770,56 +11786,56 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_9 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_1, __pyx_t_5, __pyx_t_6, __pyx_t_7};
-    __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 908, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 915, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_1, __pyx_t_5, __pyx_t_6, __pyx_t_7};
-    __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 908, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 915, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 908, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 915, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_1) {
       __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1); __pyx_t_1 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_9, __pyx_t_7);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 908, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 915, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "pysoem/pysoem.pyx":880
+  /* "pysoem/pysoem.pyx":887
  *             raise AttributeError()
  * 
  *     def set_watchdog(self, wd_type, wd_time_ms):             # <<<<<<<<<<<<<<
  *         """Change the watchdog time of the PDI or Process Data watchdog.
  * 
  */
 
@@ -11844,26 +11860,105 @@
   __Pyx_XDECREF(__pyx_v_wd_time_ms_limit);
   __Pyx_XDECREF(__pyx_v_actual_wd_time_ms);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":912
+/* "pysoem/pysoem.pyx":919
+ *                    fprd_fpwr_timeout_us)
+ * 
+ *     def _disable_complete_access(self):             # <<<<<<<<<<<<<<
+ *         """Helper function that stops config_map() from using "complete access" for SDO requests for this device.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_disable_complete_access(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_30_disable_complete_access[] = "Helper function that stops config_map() from using \"complete access\" for SDO requests for this device.\n\n        This should only be used if your device has issues handling complete access requests but the CoE details of the\n        SII tells that SDO complete access is supported by the device. If you need this function something is wrong\n        with your device and you should contact the manufacturer about this issue.\n\n        .. warning:: This is experimental.\n\n        .. versionadded:: 1.1.3\n        ";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_disable_complete_access(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("_disable_complete_access (wrapper)", 0);
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_30_disable_complete_access(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_30_disable_complete_access(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  uint8 __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_disable_complete_access", 0);
+
+  /* "pysoem/pysoem.pyx":930
+ *         .. versionadded:: 1.1.3
+ *         """
+ *         self._ec_slave.CoEdetails &= ~ECT_COEDET_SDOCA             # <<<<<<<<<<<<<<
+ * 
+ *     def _fprd(self, int address, int size, timeout_us=2000):
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->_ec_slave->CoEdetails); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 930, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ECT_COEDET_SDOCA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 930, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyNumber_Invert(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 930, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyNumber_InPlaceAnd(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 930, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_4 = __Pyx_PyInt_As_uint8_t(__pyx_t_2); if (unlikely((__pyx_t_4 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 930, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_self->_ec_slave->CoEdetails = __pyx_t_4;
+
+  /* "pysoem/pysoem.pyx":919
  *                    fprd_fpwr_timeout_us)
  * 
+ *     def _disable_complete_access(self):             # <<<<<<<<<<<<<<
+ *         """Helper function that stops config_map() from using "complete access" for SDO requests for this device.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("pysoem.pysoem.CdefSlave._disable_complete_access", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pysoem/pysoem.pyx":932
+ *         self._ec_slave.CoEdetails &= ~ECT_COEDET_SDOCA
+ * 
  *     def _fprd(self, int address, int size, timeout_us=2000):             # <<<<<<<<<<<<<<
  *         """Send and receive of the FPRD cmd primitive (Configured Address Physical Read)."""
  *         cdef unsigned char* data
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_fprd(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_30_fprd[] = "Send and receive of the FPRD cmd primitive (Configured Address Physical Read).";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_fprd(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fprd(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_32_fprd[] = "Send and receive of the FPRD cmd primitive (Configured Address Physical Read).";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fprd(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_address;
   int __pyx_v_size;
   PyObject *__pyx_v_timeout_us = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -11891,56 +11986,56 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_address)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fprd", 0, 2, 3, 1); __PYX_ERR(0, 912, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fprd", 0, 2, 3, 1); __PYX_ERR(0, 932, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout_us);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fprd") < 0)) __PYX_ERR(0, 912, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fprd") < 0)) __PYX_ERR(0, 932, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 912, __pyx_L3_error)
-    __pyx_v_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 912, __pyx_L3_error)
+    __pyx_v_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 932, __pyx_L3_error)
+    __pyx_v_size = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_size == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 932, __pyx_L3_error)
     __pyx_v_timeout_us = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_fprd", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 912, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_fprd", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 932, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave._fprd", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_30_fprd(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_address, __pyx_v_size, __pyx_v_timeout_us);
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fprd(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_address, __pyx_v_size, __pyx_v_timeout_us);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_30_fprd(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, int __pyx_v_size, PyObject *__pyx_v_timeout_us) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fprd(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, int __pyx_v_size, PyObject *__pyx_v_timeout_us) {
   unsigned char *__pyx_v_data;
   int __pyx_v_wkc;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -11955,114 +12050,114 @@
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fprd", 0);
 
-  /* "pysoem/pysoem.pyx":915
+  /* "pysoem/pysoem.pyx":935
  *         """Send and receive of the FPRD cmd primitive (Configured Address Physical Read)."""
  *         cdef unsigned char* data
  *         data = <unsigned char*>PyMem_Malloc(size)             # <<<<<<<<<<<<<<
  *         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)
  *         if wkc != 1:
  */
   __pyx_v_data = ((unsigned char *)PyMem_Malloc(__pyx_v_size));
 
-  /* "pysoem/pysoem.pyx":916
+  /* "pysoem/pysoem.pyx":936
  *         cdef unsigned char* data
  *         data = <unsigned char*>PyMem_Malloc(size)
  *         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)             # <<<<<<<<<<<<<<
  *         if wkc != 1:
  *             PyMem_Free(data)
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout_us); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 916, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_timeout_us); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 936, __pyx_L1_error)
   __pyx_v_wkc = ecx_FPRD(__pyx_v_self->_ecx_contextt->port, __pyx_v_self->_ec_slave->configadr, __pyx_v_address, __pyx_v_size, __pyx_v_data, __pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":917
+  /* "pysoem/pysoem.pyx":937
  *         data = <unsigned char*>PyMem_Malloc(size)
  *         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)
  *         if wkc != 1:             # <<<<<<<<<<<<<<
  *             PyMem_Free(data)
  *             raise WkcError()
  */
   __pyx_t_2 = ((__pyx_v_wkc != 1) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pysoem/pysoem.pyx":918
+    /* "pysoem/pysoem.pyx":938
  *         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)
  *         if wkc != 1:
  *             PyMem_Free(data)             # <<<<<<<<<<<<<<
  *             raise WkcError()
  *         try:
  */
     PyMem_Free(__pyx_v_data);
 
-    /* "pysoem/pysoem.pyx":919
+    /* "pysoem/pysoem.pyx":939
  *         if wkc != 1:
  *             PyMem_Free(data)
  *             raise WkcError()             # <<<<<<<<<<<<<<
  *         try:
  *             return PyBytes_FromStringAndSize(<char*>data, size)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_WkcError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 919, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_WkcError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 939, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 919, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 919, __pyx_L1_error)
+    __PYX_ERR(0, 939, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":917
+    /* "pysoem/pysoem.pyx":937
  *         data = <unsigned char*>PyMem_Malloc(size)
  *         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)
  *         if wkc != 1:             # <<<<<<<<<<<<<<
  *             PyMem_Free(data)
  *             raise WkcError()
  */
   }
 
-  /* "pysoem/pysoem.pyx":920
+  /* "pysoem/pysoem.pyx":940
  *             PyMem_Free(data)
  *             raise WkcError()
  *         try:             # <<<<<<<<<<<<<<
  *             return PyBytes_FromStringAndSize(<char*>data, size)
  *         finally:
  */
   /*try:*/ {
 
-    /* "pysoem/pysoem.pyx":921
+    /* "pysoem/pysoem.pyx":941
  *             raise WkcError()
  *         try:
  *             return PyBytes_FromStringAndSize(<char*>data, size)             # <<<<<<<<<<<<<<
  *         finally:
  *             PyMem_Free(data)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyBytes_FromStringAndSize(((char *)__pyx_v_data), __pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 921, __pyx_L5_error)
+    __pyx_t_3 = PyBytes_FromStringAndSize(((char *)__pyx_v_data), __pyx_v_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 941, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L4_return;
   }
 
-  /* "pysoem/pysoem.pyx":923
+  /* "pysoem/pysoem.pyx":943
  *             return PyBytes_FromStringAndSize(<char*>data, size)
  *         finally:
  *             PyMem_Free(data)             # <<<<<<<<<<<<<<
  * 
  *     def _fpwr(self, int address, bytes data, timeout_us=2000):
  */
   /*finally:*/ {
@@ -12106,16 +12201,16 @@
       PyMem_Free(__pyx_v_data);
       __pyx_r = __pyx_t_13;
       __pyx_t_13 = 0;
       goto __pyx_L0;
     }
   }
 
-  /* "pysoem/pysoem.pyx":912
- *                    fprd_fpwr_timeout_us)
+  /* "pysoem/pysoem.pyx":932
+ *         self._ec_slave.CoEdetails &= ~ECT_COEDET_SDOCA
  * 
  *     def _fprd(self, int address, int size, timeout_us=2000):             # <<<<<<<<<<<<<<
  *         """Send and receive of the FPRD cmd primitive (Configured Address Physical Read)."""
  *         cdef unsigned char* data
  */
 
   /* function exit code */
@@ -12127,26 +12222,26 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":925
+/* "pysoem/pysoem.pyx":945
  *             PyMem_Free(data)
  * 
  *     def _fpwr(self, int address, bytes data, timeout_us=2000):             # <<<<<<<<<<<<<<
  *         """Send and receive of the FPWR cmd primitive (Configured Address Physical Write)."""
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fpwr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_32_fpwr[] = "Send and receive of the FPWR cmd primitive (Configured Address Physical Write).";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fpwr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_fpwr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_34_fpwr[] = "Send and receive of the FPWR cmd primitive (Configured Address Physical Write).";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_fpwr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_address;
   PyObject *__pyx_v_data = 0;
   PyObject *__pyx_v_timeout_us = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -12174,61 +12269,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_address)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_fpwr", 0, 2, 3, 1); __PYX_ERR(0, 925, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_fpwr", 0, 2, 3, 1); __PYX_ERR(0, 945, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout_us);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fpwr") < 0)) __PYX_ERR(0, 925, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_fpwr") < 0)) __PYX_ERR(0, 945, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 925, __pyx_L3_error)
+    __pyx_v_address = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_address == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L3_error)
     __pyx_v_data = ((PyObject*)values[1]);
     __pyx_v_timeout_us = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_fpwr", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 925, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_fpwr", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 945, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave._fpwr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 925, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fpwr(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_address, __pyx_v_data, __pyx_v_timeout_us);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_data), (&PyBytes_Type), 1, "data", 1))) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_34_fpwr(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), __pyx_v_address, __pyx_v_data, __pyx_v_timeout_us);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_32_fpwr(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout_us) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_34_fpwr(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, int __pyx_v_address, PyObject *__pyx_v_data, PyObject *__pyx_v_timeout_us) {
   int __pyx_v_wkc;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   unsigned char *__pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
@@ -12236,82 +12331,82 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fpwr", 0);
 
-  /* "pysoem/pysoem.pyx":927
+  /* "pysoem/pysoem.pyx":947
  *     def _fpwr(self, int address, bytes data, timeout_us=2000):
  *         """Send and receive of the FPWR cmd primitive (Configured Address Physical Write)."""
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)             # <<<<<<<<<<<<<<
  *         if wkc != 1:
  *             raise WkcError()
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 927, __pyx_L1_error)
+    __PYX_ERR(0, 947, __pyx_L1_error)
   }
-  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_1 = PyBytes_GET_SIZE(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 947, __pyx_L1_error)
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 927, __pyx_L1_error)
+    __PYX_ERR(0, 947, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 927, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_timeout_us); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_timeout_us); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 947, __pyx_L1_error)
   __pyx_v_wkc = ecx_FPWR(__pyx_v_self->_ecx_contextt->port, __pyx_v_self->_ec_slave->configadr, __pyx_v_address, ((int)__pyx_t_1), ((unsigned char *)__pyx_t_2), __pyx_t_3);
 
-  /* "pysoem/pysoem.pyx":928
+  /* "pysoem/pysoem.pyx":948
  *         """Send and receive of the FPWR cmd primitive (Configured Address Physical Write)."""
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)
  *         if wkc != 1:             # <<<<<<<<<<<<<<
  *             raise WkcError()
  * 
  */
   __pyx_t_4 = ((__pyx_v_wkc != 1) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pysoem/pysoem.pyx":929
+    /* "pysoem/pysoem.pyx":949
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)
  *         if wkc != 1:
  *             raise WkcError()             # <<<<<<<<<<<<<<
  * 
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_WkcError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 929, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_WkcError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 949, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 929, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 949, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 929, __pyx_L1_error)
+    __PYX_ERR(0, 949, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":928
+    /* "pysoem/pysoem.pyx":948
  *         """Send and receive of the FPWR cmd primitive (Configured Address Physical Write)."""
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)
  *         if wkc != 1:             # <<<<<<<<<<<<<<
  *             raise WkcError()
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":925
+  /* "pysoem/pysoem.pyx":945
  *             PyMem_Free(data)
  * 
  *     def _fpwr(self, int address, bytes data, timeout_us=2000):             # <<<<<<<<<<<<<<
  *         """Send and receive of the FPWR cmd primitive (Configured Address Physical Write)."""
  *         cdef int wkc = cpysoem.ecx_FPWR(self._ecx_contextt.port, self._ec_slave.configadr, address, <int>len(data), <unsigned char*>data, timeout_us)
  */
 
@@ -12326,15 +12421,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":931
+/* "pysoem/pysoem.pyx":951
  *             raise WkcError()
  * 
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):             # <<<<<<<<<<<<<<
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *             raise SdoError(err.Slave,
  */
 
@@ -12355,75 +12450,75 @@
   PyObject *__pyx_t_12 = NULL;
   char *__pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_raise_exception", 0);
 
-  /* "pysoem/pysoem.pyx":932
+  /* "pysoem/pysoem.pyx":952
  * 
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:             # <<<<<<<<<<<<<<
  *             raise SdoError(err.Slave,
  *                            err.Index,
  */
   switch (__pyx_v_err->Etype) {
     case EC_ERR_TYPE_SDO_ERROR:
 
-    /* "pysoem/pysoem.pyx":933
+    /* "pysoem/pysoem.pyx":953
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *             raise SdoError(err.Slave,             # <<<<<<<<<<<<<<
  *                            err.Index,
  *                            err.SubIdx,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SdoError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 933, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_SdoError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 933, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 953, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "pysoem/pysoem.pyx":934
+    /* "pysoem/pysoem.pyx":954
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *             raise SdoError(err.Slave,
  *                            err.Index,             # <<<<<<<<<<<<<<
  *                            err.SubIdx,
  *                            err.AbortCode,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 934, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 954, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "pysoem/pysoem.pyx":935
+    /* "pysoem/pysoem.pyx":955
  *             raise SdoError(err.Slave,
  *                            err.Index,
  *                            err.SubIdx,             # <<<<<<<<<<<<<<
  *                            err.AbortCode,
  *                            cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8'))
  */
-    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->SubIdx); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 935, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->SubIdx); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 955, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "pysoem/pysoem.pyx":936
+    /* "pysoem/pysoem.pyx":956
  *                            err.Index,
  *                            err.SubIdx,
  *                            err.AbortCode,             # <<<<<<<<<<<<<<
  *                            cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_EMERGENCY:
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_err->AbortCode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 936, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_err->AbortCode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 956, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":937
+    /* "pysoem/pysoem.pyx":957
  *                            err.SubIdx,
  *                            err.AbortCode,
  *                            cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8'))             # <<<<<<<<<<<<<<
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_EMERGENCY:
  *             raise Emergency(err.Slave,
  */
     __pyx_t_7 = ec_sdoerror2string(__pyx_v_err->AbortCode);
-    __pyx_t_8 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 937, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_decode_c_string(__pyx_t_7, 0, strlen(__pyx_t_7), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 957, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12432,39 +12527,39 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_8};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 933, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_8};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 933, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 5+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     } else
     #endif
     {
-      __pyx_t_11 = PyTuple_New(5+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 933, __pyx_L1_error)
+      __pyx_t_11 = PyTuple_New(5+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 953, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       if (__pyx_t_9) {
         __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_9); __pyx_t_9 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_4);
@@ -12477,93 +12572,93 @@
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_11, 4+__pyx_t_10, __pyx_t_8);
       __pyx_t_3 = 0;
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 933, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 933, __pyx_L1_error)
+    __PYX_ERR(0, 953, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":932
+    /* "pysoem/pysoem.pyx":952
  * 
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:             # <<<<<<<<<<<<<<
  *             raise SdoError(err.Slave,
  *                            err.Index,
  */
     break;
     case EC_ERR_TYPE_EMERGENCY:
 
-    /* "pysoem/pysoem.pyx":939
+    /* "pysoem/pysoem.pyx":959
  *                            cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_EMERGENCY:
  *             raise Emergency(err.Slave,             # <<<<<<<<<<<<<<
  *                             err.ErrorCode,
  *                             err.ErrorReg,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Emergency); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 939, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Emergency); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 959, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 939, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 959, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
 
-    /* "pysoem/pysoem.pyx":940
+    /* "pysoem/pysoem.pyx":960
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_EMERGENCY:
  *             raise Emergency(err.Slave,
  *                             err.ErrorCode,             # <<<<<<<<<<<<<<
  *                             err.ErrorReg,
  *                             err.b1,
  */
-    __pyx_t_8 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 940, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 960, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
 
-    /* "pysoem/pysoem.pyx":941
+    /* "pysoem/pysoem.pyx":961
  *             raise Emergency(err.Slave,
  *                             err.ErrorCode,
  *                             err.ErrorReg,             # <<<<<<<<<<<<<<
  *                             err.b1,
  *                             err.w1,
  */
-    __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->ErrorReg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 941, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->ErrorReg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 961, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":942
+    /* "pysoem/pysoem.pyx":962
  *                             err.ErrorCode,
  *                             err.ErrorReg,
  *                             err.b1,             # <<<<<<<<<<<<<<
  *                             err.w1,
  *                             err.w2)
  */
-    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->b1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 942, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint8_t(__pyx_v_err->b1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 962, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "pysoem/pysoem.pyx":943
+    /* "pysoem/pysoem.pyx":963
  *                             err.ErrorReg,
  *                             err.b1,
  *                             err.w1,             # <<<<<<<<<<<<<<
  *                             err.w2)
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->w1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 943, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->w1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
-    /* "pysoem/pysoem.pyx":944
+    /* "pysoem/pysoem.pyx":964
  *                             err.b1,
  *                             err.w1,
  *                             err.w2)             # <<<<<<<<<<<<<<
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *             raise MailboxError(err.Slave,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->w2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 944, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->w2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 964, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_9 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12572,41 +12667,41 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[7] = {__pyx_t_9, __pyx_t_11, __pyx_t_8, __pyx_t_6, __pyx_t_5, __pyx_t_4, __pyx_t_3};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 959, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[7] = {__pyx_t_9, __pyx_t_11, __pyx_t_8, __pyx_t_6, __pyx_t_5, __pyx_t_4, __pyx_t_3};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 959, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     {
-      __pyx_t_12 = PyTuple_New(6+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 939, __pyx_L1_error)
+      __pyx_t_12 = PyTuple_New(6+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 959, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (__pyx_t_9) {
         __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_9); __pyx_t_9 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_11);
       PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, __pyx_t_11);
       __Pyx_GIVEREF(__pyx_t_8);
@@ -12621,64 +12716,64 @@
       PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_10, __pyx_t_3);
       __pyx_t_11 = 0;
       __pyx_t_8 = 0;
       __pyx_t_6 = 0;
       __pyx_t_5 = 0;
       __pyx_t_4 = 0;
       __pyx_t_3 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 959, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 939, __pyx_L1_error)
+    __PYX_ERR(0, 959, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":938
+    /* "pysoem/pysoem.pyx":958
  *                            err.AbortCode,
  *                            cpysoem.ec_sdoerror2string(err.AbortCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_EMERGENCY:             # <<<<<<<<<<<<<<
  *             raise Emergency(err.Slave,
  *                             err.ErrorCode,
  */
     break;
     case EC_ERR_TYPE_MBX_ERROR:
 
-    /* "pysoem/pysoem.pyx":946
+    /* "pysoem/pysoem.pyx":966
  *                             err.w2)
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *             raise MailboxError(err.Slave,             # <<<<<<<<<<<<<<
  *                                err.ErrorCode,
  *                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8'))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_MailboxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 946, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_MailboxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 966, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 946, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 966, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
 
-    /* "pysoem/pysoem.pyx":947
+    /* "pysoem/pysoem.pyx":967
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:
  *             raise MailboxError(err.Slave,
  *                                err.ErrorCode,             # <<<<<<<<<<<<<<
  *                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  */
-    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 967, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "pysoem/pysoem.pyx":948
+    /* "pysoem/pysoem.pyx":968
  *             raise MailboxError(err.Slave,
  *                                err.ErrorCode,
  *                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8'))             # <<<<<<<<<<<<<<
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *             raise PacketError(err.Slave,
  */
     __pyx_t_13 = ec_mbxerror2string(__pyx_v_err->ErrorCode);
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 948, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 968, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12687,88 +12782,88 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_12, __pyx_t_3, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 946, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 966, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_t_12, __pyx_t_3, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 946, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 3+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 966, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 946, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(3+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 966, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_12);
       PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_10, __pyx_t_12);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_10, __pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_10, __pyx_t_4);
       __pyx_t_12 = 0;
       __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 946, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 966, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 946, __pyx_L1_error)
+    __PYX_ERR(0, 966, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":945
+    /* "pysoem/pysoem.pyx":965
  *                             err.w1,
  *                             err.w2)
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_MBX_ERROR:             # <<<<<<<<<<<<<<
  *             raise MailboxError(err.Slave,
  *                                err.ErrorCode,
  */
     break;
     case EC_ERR_TYPE_PACKET_ERROR:
 
-    /* "pysoem/pysoem.pyx":950
+    /* "pysoem/pysoem.pyx":970
  *                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *             raise PacketError(err.Slave,             # <<<<<<<<<<<<<<
  *                               err.ErrorCode)
  *         else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PacketError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 950, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PacketError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 950, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->Slave); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 970, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pysoem/pysoem.pyx":951
+    /* "pysoem/pysoem.pyx":971
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:
  *             raise PacketError(err.Slave,
  *                               err.ErrorCode)             # <<<<<<<<<<<<<<
  *         else:
  *             raise Exception('unexpected error, Etype: {}'.format(err.Etype))
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 951, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_err->ErrorCode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 971, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = NULL;
     __pyx_t_10 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12777,99 +12872,99 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_10 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_6, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 950, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_6, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 950, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_12 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 950, __pyx_L1_error)
+      __pyx_t_12 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 970, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (__pyx_t_3) {
         __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_3); __pyx_t_3 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_10, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_10, __pyx_t_4);
       __pyx_t_6 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 950, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 950, __pyx_L1_error)
+    __PYX_ERR(0, 970, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":949
+    /* "pysoem/pysoem.pyx":969
  *                                err.ErrorCode,
  *                                cpysoem.ec_mbxerror2string(err.ErrorCode).decode('utf8'))
  *         elif err.Etype == cpysoem.EC_ERR_TYPE_PACKET_ERROR:             # <<<<<<<<<<<<<<
  *             raise PacketError(err.Slave,
  *                               err.ErrorCode)
  */
     break;
     default:
 
-    /* "pysoem/pysoem.pyx":953
+    /* "pysoem/pysoem.pyx":973
  *                               err.ErrorCode)
  *         else:
  *             raise Exception('unexpected error, Etype: {}'.format(err.Etype))             # <<<<<<<<<<<<<<
  * 
  *     def _get_name(self):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_unexpected_error_Etype, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_unexpected_error_Etype, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = __Pyx_PyInt_From_ec_err_type(__pyx_v_err->Etype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 953, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_From_ec_err_type(__pyx_v_err->Etype); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_12);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 953, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 953, __pyx_L1_error)
+    __PYX_ERR(0, 973, __pyx_L1_error)
     break;
   }
 
-  /* "pysoem/pysoem.pyx":931
+  /* "pysoem/pysoem.pyx":951
  *             raise WkcError()
  * 
  *     cdef _raise_exception(self, cpysoem.ec_errort* err):             # <<<<<<<<<<<<<<
  *         if err.Etype == cpysoem.EC_ERR_TYPE_SDO_ERROR:
  *             raise SdoError(err.Slave,
  */
 
@@ -12888,68 +12983,68 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave._raise_exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":955
+/* "pysoem/pysoem.pyx":975
  *             raise Exception('unexpected error, Etype: {}'.format(err.Etype))
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         """Name of the slave, read out from the slaves SII during config_init."""
  *         return (<bytes>self._ec_slave.name).decode('utf8')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_get_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_34_get_name[] = "Name of the slave, read out from the slaves SII during config_init.";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_get_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_36_get_name[] = "Name of the slave, read out from the slaves SII during config_init.";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_34_get_name(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_name(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_34_get_name(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_name(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_name", 0);
 
-  /* "pysoem/pysoem.pyx":957
+  /* "pysoem/pysoem.pyx":977
  *     def _get_name(self):
  *         """Name of the slave, read out from the slaves SII during config_init."""
  *         return (<bytes>self._ec_slave.name).decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     def _get_eep_man(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->_ec_slave->name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->_ec_slave->name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 977, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-    __PYX_ERR(0, 957, __pyx_L1_error)
+    __PYX_ERR(0, 977, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_bytes(((PyObject*)__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 977, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":955
+  /* "pysoem/pysoem.pyx":975
  *             raise Exception('unexpected error, Etype: {}'.format(err.Etype))
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         """Name of the slave, read out from the slaves SII during config_init."""
  *         return (<bytes>self._ec_slave.name).decode('utf8')
  */
 
@@ -12961,60 +13056,60 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":959
+/* "pysoem/pysoem.pyx":979
  *         return (<bytes>self._ec_slave.name).decode('utf8')
  * 
  *     def _get_eep_man(self):             # <<<<<<<<<<<<<<
  *         """Vendor ID of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_man
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_eep_man(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_36_get_eep_man[] = "Vendor ID of the slave, read out from the slaves SII during config_init.";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_eep_man(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_man(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_38_get_eep_man[] = "Vendor ID of the slave, read out from the slaves SII during config_init.";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_man(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_eep_man (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_eep_man(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_man(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_36_get_eep_man(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_man(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_eep_man", 0);
 
-  /* "pysoem/pysoem.pyx":961
+  /* "pysoem/pysoem.pyx":981
  *     def _get_eep_man(self):
  *         """Vendor ID of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_man             # <<<<<<<<<<<<<<
  * 
  *     def _get_eep_id(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_man); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_man); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 981, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":959
+  /* "pysoem/pysoem.pyx":979
  *         return (<bytes>self._ec_slave.name).decode('utf8')
  * 
  *     def _get_eep_man(self):             # <<<<<<<<<<<<<<
  *         """Vendor ID of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_man
  */
 
@@ -13025,60 +13120,60 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":963
+/* "pysoem/pysoem.pyx":983
  *         return self._ec_slave.eep_man
  * 
  *     def _get_eep_id(self):             # <<<<<<<<<<<<<<
  *         """Product Code of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_id
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_id(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_38_get_eep_id[] = "Product Code of the slave, read out from the slaves SII during config_init.";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_id(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_id(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_40_get_eep_id[] = "Product Code of the slave, read out from the slaves SII during config_init.";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_id(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_eep_id (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_id(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_id(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_38_get_eep_id(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_id(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_eep_id", 0);
 
-  /* "pysoem/pysoem.pyx":965
+  /* "pysoem/pysoem.pyx":985
  *     def _get_eep_id(self):
  *         """Product Code of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_id             # <<<<<<<<<<<<<<
  * 
  *     def _get_eep_rev(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 965, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":963
+  /* "pysoem/pysoem.pyx":983
  *         return self._ec_slave.eep_man
  * 
  *     def _get_eep_id(self):             # <<<<<<<<<<<<<<
  *         """Product Code of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_id
  */
 
@@ -13089,60 +13184,60 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":967
+/* "pysoem/pysoem.pyx":987
  *         return self._ec_slave.eep_id
  * 
  *     def _get_eep_rev(self):             # <<<<<<<<<<<<<<
  *         """Revision Number of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_rev
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_rev(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_40_get_eep_rev[] = "Revision Number of the slave, read out from the slaves SII during config_init.";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_rev(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_eep_rev(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_42_get_eep_rev[] = "Revision Number of the slave, read out from the slaves SII during config_init.";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_eep_rev(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_eep_rev (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_rev(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_eep_rev(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_40_get_eep_rev(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_eep_rev(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_eep_rev", 0);
 
-  /* "pysoem/pysoem.pyx":969
+  /* "pysoem/pysoem.pyx":989
  *     def _get_eep_rev(self):
  *         """Revision Number of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_rev             # <<<<<<<<<<<<<<
  * 
  *     def _get_PO2SOconfig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_rev); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 969, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_self->_ec_slave->eep_rev); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":967
+  /* "pysoem/pysoem.pyx":987
  *         return self._ec_slave.eep_id
  * 
  *     def _get_eep_rev(self):             # <<<<<<<<<<<<<<
  *         """Revision Number of the slave, read out from the slaves SII during config_init."""
  *         return self._ec_slave.eep_rev
  */
 
@@ -13153,382 +13248,382 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":971
+/* "pysoem/pysoem.pyx":991
  *         return self._ec_slave.eep_rev
  * 
  *     def _get_PO2SOconfig(self):             # <<<<<<<<<<<<<<
  *         """Slaves callback function that is called during config_map.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_PO2SOconfig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_42_get_PO2SOconfig[] = "Slaves callback function that is called during config_map.\n        \n        When the state changes from Pre-Operational state to Operational state.";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_PO2SOconfig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfig[] = "Slaves callback function that is called during config_map.\n        \n        When the state changes from Pre-Operational state to Operational state.";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfig(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_PO2SOconfig (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_PO2SOconfig(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfig(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_42_get_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_PO2SOconfig", 0);
 
-  /* "pysoem/pysoem.pyx":975
+  /* "pysoem/pysoem.pyx":995
  * 
  *         When the state changes from Pre-Operational state to Operational state."""
  *         return <object>self._ec_slave.user             # <<<<<<<<<<<<<<
  * 
  *     def _get_PO2SOconfigEx(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->_ec_slave->user));
   __pyx_r = ((PyObject *)__pyx_v_self->_ec_slave->user);
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":971
+  /* "pysoem/pysoem.pyx":991
  *         return self._ec_slave.eep_rev
  * 
  *     def _get_PO2SOconfig(self):             # <<<<<<<<<<<<<<
  *         """Slaves callback function that is called during config_map.
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":977
+/* "pysoem/pysoem.pyx":997
  *         return <object>self._ec_slave.user
  * 
  *     def _get_PO2SOconfigEx(self):             # <<<<<<<<<<<<<<
  *         """Alternative callback function that is called during config_map.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfigEx(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfigEx[] = "Alternative callback function that is called during config_map.\n\n        More precisely the function is called during the transition from Pre-Operational to Safe-Operational state.\n        Use this instead of the config_func. The difference is that the callbacks signature is fn(CdefSlave: slave).\n\n        .. versionadded:: 1.1.0\n        ";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfigEx(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_get_PO2SOconfigEx(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_46_get_PO2SOconfigEx[] = "Alternative callback function that is called during config_map.\n\n        More precisely the function is called during the transition from Pre-Operational to Safe-Operational state.\n        Use this instead of the config_func. The difference is that the callbacks signature is fn(CdefSlave: slave).\n\n        .. versionadded:: 1.1.0\n        ";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_get_PO2SOconfigEx(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_PO2SOconfigEx (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfigEx(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_46_get_PO2SOconfigEx(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_46_get_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_PO2SOconfigEx", 0);
 
-  /* "pysoem/pysoem.pyx":985
+  /* "pysoem/pysoem.pyx":1005
  *         .. versionadded:: 1.1.0
  *         """
  *         return <object>self._ec_slave.user             # <<<<<<<<<<<<<<
  * 
  *     def _set_PO2SOconfig(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->_ec_slave->user));
   __pyx_r = ((PyObject *)__pyx_v_self->_ec_slave->user);
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":977
+  /* "pysoem/pysoem.pyx":997
  *         return <object>self._ec_slave.user
  * 
  *     def _get_PO2SOconfigEx(self):             # <<<<<<<<<<<<<<
  *         """Alternative callback function that is called during config_map.
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":987
+/* "pysoem/pysoem.pyx":1007
  *         return <object>self._ec_slave.user
  * 
  *     def _set_PO2SOconfig(self, value):             # <<<<<<<<<<<<<<
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_set_PO2SOconfig(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_set_PO2SOconfig(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfig(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfig(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_PO2SOconfig (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_46_set_PO2SOconfig(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfig(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_46_set_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfig(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("_set_PO2SOconfig", 0);
 
-  /* "pysoem/pysoem.pyx":988
+  /* "pysoem/pysoem.pyx":1008
  * 
  *     def _set_PO2SOconfig(self, value):
  *         self._cd.func = value             # <<<<<<<<<<<<<<
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:
  */
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   __Pyx_GOTREF(__pyx_v_self->_cd->func);
   __Pyx_DECREF(__pyx_v_self->_cd->func);
   __pyx_v_self->_cd->func = __pyx_v_value;
 
-  /* "pysoem/pysoem.pyx":989
+  /* "pysoem/pysoem.pyx":1009
  *     def _set_PO2SOconfig(self, value):
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd             # <<<<<<<<<<<<<<
  *         if value is None:
  *             self._ec_slave.PO2SOconfig = NULL
  */
   __pyx_v_self->_ec_slave->user = ((void *)__pyx_v_self->_cd);
 
-  /* "pysoem/pysoem.pyx":990
+  /* "pysoem/pysoem.pyx":1010
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:             # <<<<<<<<<<<<<<
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  */
   __pyx_t_1 = (__pyx_v_value == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":991
+    /* "pysoem/pysoem.pyx":1011
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:
  *             self._ec_slave.PO2SOconfig = NULL             # <<<<<<<<<<<<<<
  *         else:
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfig
  */
     __pyx_v_self->_ec_slave->PO2SOconfig = NULL;
 
-    /* "pysoem/pysoem.pyx":990
+    /* "pysoem/pysoem.pyx":1010
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:             # <<<<<<<<<<<<<<
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pysoem/pysoem.pyx":993
+  /* "pysoem/pysoem.pyx":1013
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfig             # <<<<<<<<<<<<<<
  * 
  *     def _set_PO2SOconfigEx(self, value):
  */
   /*else*/ {
     __pyx_v_self->_ec_slave->PO2SOconfig = __pyx_f_6pysoem_6pysoem__xPO2SOconfig;
   }
   __pyx_L3:;
 
-  /* "pysoem/pysoem.pyx":987
+  /* "pysoem/pysoem.pyx":1007
  *         return <object>self._ec_slave.user
  * 
  *     def _set_PO2SOconfig(self, value):             # <<<<<<<<<<<<<<
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":995
+/* "pysoem/pysoem.pyx":1015
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfig
  * 
  *     def _set_PO2SOconfigEx(self, value):             # <<<<<<<<<<<<<<
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfigEx(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfigEx(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_set_PO2SOconfigEx(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_set_PO2SOconfigEx(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_PO2SOconfigEx (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfigEx(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_50_set_PO2SOconfigEx(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_48_set_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_50_set_PO2SOconfigEx(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("_set_PO2SOconfigEx", 0);
 
-  /* "pysoem/pysoem.pyx":996
+  /* "pysoem/pysoem.pyx":1016
  * 
  *     def _set_PO2SOconfigEx(self, value):
  *         self._cd.func = value             # <<<<<<<<<<<<<<
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:
  */
   __Pyx_INCREF(__pyx_v_value);
   __Pyx_GIVEREF(__pyx_v_value);
   __Pyx_GOTREF(__pyx_v_self->_cd->func);
   __Pyx_DECREF(__pyx_v_self->_cd->func);
   __pyx_v_self->_cd->func = __pyx_v_value;
 
-  /* "pysoem/pysoem.pyx":997
+  /* "pysoem/pysoem.pyx":1017
  *     def _set_PO2SOconfigEx(self, value):
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd             # <<<<<<<<<<<<<<
  *         if value is None:
  *             self._ec_slave.PO2SOconfig = NULL
  */
   __pyx_v_self->_ec_slave->user = ((void *)__pyx_v_self->_cd);
 
-  /* "pysoem/pysoem.pyx":998
+  /* "pysoem/pysoem.pyx":1018
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:             # <<<<<<<<<<<<<<
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  */
   __pyx_t_1 = (__pyx_v_value == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":999
+    /* "pysoem/pysoem.pyx":1019
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:
  *             self._ec_slave.PO2SOconfig = NULL             # <<<<<<<<<<<<<<
  *         else:
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfigEx
  */
     __pyx_v_self->_ec_slave->PO2SOconfig = NULL;
 
-    /* "pysoem/pysoem.pyx":998
+    /* "pysoem/pysoem.pyx":1018
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  *         if value is None:             # <<<<<<<<<<<<<<
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pysoem/pysoem.pyx":1001
+  /* "pysoem/pysoem.pyx":1021
  *             self._ec_slave.PO2SOconfig = NULL
  *         else:
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfigEx             # <<<<<<<<<<<<<<
  * 
  *     def _get_state(self):
  */
   /*else*/ {
     __pyx_v_self->_ec_slave->PO2SOconfig = __pyx_f_6pysoem_6pysoem__xPO2SOconfigEx;
   }
   __pyx_L3:;
 
-  /* "pysoem/pysoem.pyx":995
+  /* "pysoem/pysoem.pyx":1015
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfig
  * 
  *     def _set_PO2SOconfigEx(self, value):             # <<<<<<<<<<<<<<
  *         self._cd.func = value
  *         self._ec_slave.user = <void*>self._cd
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1003
+/* "pysoem/pysoem.pyx":1023
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfigEx
  * 
  *     def _get_state(self):             # <<<<<<<<<<<<<<
  *         """Request a new state.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_get_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_50_get_state[] = "Request a new state.\n\n        After a new state has been set, `write_state` must be called.\n        ";
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_get_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_get_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_6pysoem_6pysoem_9CdefSlave_52_get_state[] = "Request a new state.\n\n        After a new state has been set, `write_state` must be called.\n        ";
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_get_state(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_state (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_50_get_state(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_52_get_state(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_50_get_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_52_get_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_state", 0);
 
-  /* "pysoem/pysoem.pyx":1008
+  /* "pysoem/pysoem.pyx":1028
  *         After a new state has been set, `write_state` must be called.
  *         """
  *         return self._ec_slave.state             # <<<<<<<<<<<<<<
  * 
  *     def _set_state(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_self->_ec_slave->state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1008, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_self->_ec_slave->state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1028, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1003
+  /* "pysoem/pysoem.pyx":1023
  *             self._ec_slave.PO2SOconfig = _xPO2SOconfigEx
  * 
  *     def _get_state(self):             # <<<<<<<<<<<<<<
  *         """Request a new state.
  * 
  */
 
@@ -13539,55 +13634,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1010
+/* "pysoem/pysoem.pyx":1030
  *         return self._ec_slave.state
  * 
  *     def _set_state(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave.state = value
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_set_state(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_set_state(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_set_state(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_set_state(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_state (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_52_set_state(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_54_set_state(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_52_set_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_54_set_state(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   uint16 __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_state", 0);
 
-  /* "pysoem/pysoem.pyx":1011
+  /* "pysoem/pysoem.pyx":1031
  * 
  *     def _set_state(self, value):
  *         self._ec_slave.state = value             # <<<<<<<<<<<<<<
  * 
  *     def _get_input(self):
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1011, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1031, __pyx_L1_error)
   __pyx_v_self->_ec_slave->state = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":1010
+  /* "pysoem/pysoem.pyx":1030
  *         return self._ec_slave.state
  * 
  *     def _set_state(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave.state = value
  * 
  */
 
@@ -13599,59 +13694,59 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1013
+/* "pysoem/pysoem.pyx":1033
  *         self._ec_slave.state = value
  * 
  *     def _get_input(self):             # <<<<<<<<<<<<<<
  *         num_bytes = self._ec_slave.Ibytes
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_get_input(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_get_input(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_input(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_input(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_input (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_54_get_input(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_input(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_54_get_input(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_input(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   long __pyx_v_num_bytes;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   uint32 __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_input", 0);
 
-  /* "pysoem/pysoem.pyx":1014
+  /* "pysoem/pysoem.pyx":1034
  * 
  *     def _get_input(self):
  *         num_bytes = self._ec_slave.Ibytes             # <<<<<<<<<<<<<<
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):
  *             num_bytes = 1
  */
   __pyx_t_1 = __pyx_v_self->_ec_slave->Ibytes;
   __pyx_v_num_bytes = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":1015
+  /* "pysoem/pysoem.pyx":1035
  *     def _get_input(self):
  *         num_bytes = self._ec_slave.Ibytes
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):             # <<<<<<<<<<<<<<
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)
  */
   __pyx_t_3 = ((__pyx_v_self->_ec_slave->Ibytes == 0) != 0);
@@ -13661,47 +13756,47 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = ((__pyx_v_self->_ec_slave->Ibits > 0) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":1016
+    /* "pysoem/pysoem.pyx":1036
  *         num_bytes = self._ec_slave.Ibytes
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):
  *             num_bytes = 1             # <<<<<<<<<<<<<<
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)
  * 
  */
     __pyx_v_num_bytes = 1;
 
-    /* "pysoem/pysoem.pyx":1015
+    /* "pysoem/pysoem.pyx":1035
  *     def _get_input(self):
  *         num_bytes = self._ec_slave.Ibytes
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):             # <<<<<<<<<<<<<<
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)
  */
   }
 
-  /* "pysoem/pysoem.pyx":1017
+  /* "pysoem/pysoem.pyx":1037
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)             # <<<<<<<<<<<<<<
  * 
  *     def _get_output(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyBytes_FromStringAndSize(((char *)__pyx_v_self->_ec_slave->inputs), __pyx_v_num_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1017, __pyx_L1_error)
+  __pyx_t_4 = PyBytes_FromStringAndSize(((char *)__pyx_v_self->_ec_slave->inputs), __pyx_v_num_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1037, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1013
+  /* "pysoem/pysoem.pyx":1033
  *         self._ec_slave.state = value
  * 
  *     def _get_input(self):             # <<<<<<<<<<<<<<
  *         num_bytes = self._ec_slave.Ibytes
  *         if (self._ec_slave.Ibytes == 0 and self._ec_slave.Ibits > 0):
  */
 
@@ -13712,59 +13807,59 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1019
+/* "pysoem/pysoem.pyx":1039
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)
  * 
  *     def _get_output(self):             # <<<<<<<<<<<<<<
  *         num_bytes = self._ec_slave.Obytes
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_output(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_output(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_get_output(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_get_output(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_output (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_output(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_58_get_output(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_56_get_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_58_get_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   long __pyx_v_num_bytes;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   uint32 __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_output", 0);
 
-  /* "pysoem/pysoem.pyx":1020
+  /* "pysoem/pysoem.pyx":1040
  * 
  *     def _get_output(self):
  *         num_bytes = self._ec_slave.Obytes             # <<<<<<<<<<<<<<
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):
  *             num_bytes = 1
  */
   __pyx_t_1 = __pyx_v_self->_ec_slave->Obytes;
   __pyx_v_num_bytes = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":1021
+  /* "pysoem/pysoem.pyx":1041
  *     def _get_output(self):
  *         num_bytes = self._ec_slave.Obytes
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):             # <<<<<<<<<<<<<<
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)
  */
   __pyx_t_3 = ((__pyx_v_self->_ec_slave->Obytes == 0) != 0);
@@ -13774,47 +13869,47 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = ((__pyx_v_self->_ec_slave->Obits > 0) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "pysoem/pysoem.pyx":1022
+    /* "pysoem/pysoem.pyx":1042
  *         num_bytes = self._ec_slave.Obytes
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):
  *             num_bytes = 1             # <<<<<<<<<<<<<<
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)
  * 
  */
     __pyx_v_num_bytes = 1;
 
-    /* "pysoem/pysoem.pyx":1021
+    /* "pysoem/pysoem.pyx":1041
  *     def _get_output(self):
  *         num_bytes = self._ec_slave.Obytes
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):             # <<<<<<<<<<<<<<
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)
  */
   }
 
-  /* "pysoem/pysoem.pyx":1023
+  /* "pysoem/pysoem.pyx":1043
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):
  *             num_bytes = 1
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)             # <<<<<<<<<<<<<<
  * 
  *     def _set_output(self, bytes value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = PyBytes_FromStringAndSize(((char *)__pyx_v_self->_ec_slave->outputs), __pyx_v_num_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1023, __pyx_L1_error)
+  __pyx_t_4 = PyBytes_FromStringAndSize(((char *)__pyx_v_self->_ec_slave->outputs), __pyx_v_num_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1043, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1019
+  /* "pysoem/pysoem.pyx":1039
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.inputs, num_bytes)
  * 
  *     def _get_output(self):             # <<<<<<<<<<<<<<
  *         num_bytes = self._ec_slave.Obytes
  *         if (self._ec_slave.Obytes == 0 and self._ec_slave.Obits > 0):
  */
 
@@ -13825,73 +13920,73 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1025
+/* "pysoem/pysoem.pyx":1045
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)
  * 
  *     def _set_output(self, bytes value):             # <<<<<<<<<<<<<<
  *         memcpy(<char*>self._ec_slave.outputs, <char*>value, len(value))
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_set_output(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_set_output(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_set_output(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_set_output(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_output (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyBytes_Type), 1, "value", 1))) __PYX_ERR(0, 1025, __pyx_L1_error)
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_58_set_output(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject*)__pyx_v_value));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyBytes_Type), 1, "value", 1))) __PYX_ERR(0, 1045, __pyx_L1_error)
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_60_set_output(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject*)__pyx_v_value));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_58_set_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_60_set_output(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_output", 0);
 
-  /* "pysoem/pysoem.pyx":1026
+  /* "pysoem/pysoem.pyx":1046
  * 
  *     def _set_output(self, bytes value):
  *         memcpy(<char*>self._ec_slave.outputs, <char*>value, len(value))             # <<<<<<<<<<<<<<
  * 
  *     def _get_al_status(self):
  */
   if (unlikely(__pyx_v_value == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 1026, __pyx_L1_error)
+    __PYX_ERR(0, 1046, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyBytes_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 1026, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_AsWritableString(__pyx_v_value); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 1046, __pyx_L1_error)
   if (unlikely(__pyx_v_value == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 1026, __pyx_L1_error)
+    __PYX_ERR(0, 1046, __pyx_L1_error)
   }
-  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1026, __pyx_L1_error)
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_value); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1046, __pyx_L1_error)
   (void)(memcpy(((char *)__pyx_v_self->_ec_slave->outputs), ((char *)__pyx_t_1), __pyx_t_2));
 
-  /* "pysoem/pysoem.pyx":1025
+  /* "pysoem/pysoem.pyx":1045
  *         return PyBytes_FromStringAndSize(<char*>self._ec_slave.outputs, num_bytes)
  * 
  *     def _set_output(self, bytes value):             # <<<<<<<<<<<<<<
  *         memcpy(<char*>self._ec_slave.outputs, <char*>value, len(value))
  * 
  */
 
@@ -13903,59 +13998,59 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1028
+/* "pysoem/pysoem.pyx":1048
  *         memcpy(<char*>self._ec_slave.outputs, <char*>value, len(value))
  * 
  *     def _get_al_status(self):             # <<<<<<<<<<<<<<
  *         return self._ec_slave.ALstatuscode
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_get_al_status(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_get_al_status(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_al_status(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_al_status(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_al_status (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_60_get_al_status(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_al_status(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_60_get_al_status(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_al_status(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_al_status", 0);
 
-  /* "pysoem/pysoem.pyx":1029
+  /* "pysoem/pysoem.pyx":1049
  * 
  *     def _get_al_status(self):
  *         return self._ec_slave.ALstatuscode             # <<<<<<<<<<<<<<
  * 
  *     def _get_is_lost(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_self->_ec_slave->ALstatuscode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1029, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_self->_ec_slave->ALstatuscode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1049, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1028
+  /* "pysoem/pysoem.pyx":1048
  *         memcpy(<char*>self._ec_slave.outputs, <char*>value, len(value))
  * 
  *     def _get_al_status(self):             # <<<<<<<<<<<<<<
  *         return self._ec_slave.ALstatuscode
  * 
  */
 
@@ -13966,59 +14061,59 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1031
+/* "pysoem/pysoem.pyx":1051
  *         return self._ec_slave.ALstatuscode
  * 
  *     def _get_is_lost(self):             # <<<<<<<<<<<<<<
  *         return self._ec_slave.islost
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_is_lost(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_is_lost(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_get_is_lost(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_get_is_lost(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_is_lost (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_is_lost(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_64_get_is_lost(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_62_get_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_64_get_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_is_lost", 0);
 
-  /* "pysoem/pysoem.pyx":1032
+  /* "pysoem/pysoem.pyx":1052
  * 
  *     def _get_is_lost(self):
  *         return self._ec_slave.islost             # <<<<<<<<<<<<<<
  * 
  *     def _set_is_lost(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_ec_slave->islost); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int8_t(__pyx_v_self->_ec_slave->islost); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1052, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1031
+  /* "pysoem/pysoem.pyx":1051
  *         return self._ec_slave.ALstatuscode
  * 
  *     def _get_is_lost(self):             # <<<<<<<<<<<<<<
  *         return self._ec_slave.islost
  * 
  */
 
@@ -14029,55 +14124,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1034
+/* "pysoem/pysoem.pyx":1054
  *         return self._ec_slave.islost
  * 
  *     def _set_is_lost(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave.islost = value
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_set_is_lost(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_set_is_lost(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_set_is_lost(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_set_is_lost(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_set_is_lost (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_64_set_is_lost(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_66_set_is_lost(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_64_set_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_66_set_is_lost(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   boolean __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_is_lost", 0);
 
-  /* "pysoem/pysoem.pyx":1035
+  /* "pysoem/pysoem.pyx":1055
  * 
  *     def _set_is_lost(self, value):
  *         self._ec_slave.islost = value             # <<<<<<<<<<<<<<
  * 
  *     def _get_od(self):
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int8_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1035, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int8_t(__pyx_v_value); if (unlikely((__pyx_t_1 == ((boolean)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L1_error)
   __pyx_v_self->_ec_slave->islost = __pyx_t_1;
 
-  /* "pysoem/pysoem.pyx":1034
+  /* "pysoem/pysoem.pyx":1054
  *         return self._ec_slave.islost
  * 
  *     def _set_is_lost(self, value):             # <<<<<<<<<<<<<<
  *         self._ec_slave.islost = value
  * 
  */
 
@@ -14089,36 +14184,36 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1037
+/* "pysoem/pysoem.pyx":1057
  *         self._ec_slave.islost = value
  * 
  *     def _get_od(self):             # <<<<<<<<<<<<<<
  *         logger.debug('ecx_readODlist()')
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_get_od(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_get_od(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_69_get_od(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_69_get_od(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_od (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_66_get_od(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_68_get_od(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_66_get_od(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_68_get_od(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   int __pyx_v_result;
   PyObject *__pyx_v_coe_objects = NULL;
   uint16 __pyx_v_i;
   struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_coe_object = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -14131,181 +14226,181 @@
   ecx_contextt *__pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_od", 0);
 
-  /* "pysoem/pysoem.pyx":1038
+  /* "pysoem/pysoem.pyx":1058
  * 
  *     def _get_od(self):
  *         logger.debug('ecx_readODlist()')             # <<<<<<<<<<<<<<
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  *         if not result > 0:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1038, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1058, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1038, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1058, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_ecx_readODlist) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_ecx_readODlist);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1038, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1058, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1039
+  /* "pysoem/pysoem.pyx":1059
  *     def _get_od(self):
  *         logger.debug('ecx_readODlist()')
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)             # <<<<<<<<<<<<<<
  *         if not result > 0:
  *             raise SdoInfoError('Sdo List Info read failed')
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1039, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_self->_pos); if (unlikely((__pyx_t_4 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1059, __pyx_L1_error)
   __pyx_v_result = ecx_readODlist(__pyx_v_self->_ecx_contextt, __pyx_t_4, (&__pyx_v_self->_ex_odlist));
 
-  /* "pysoem/pysoem.pyx":1040
+  /* "pysoem/pysoem.pyx":1060
  *         logger.debug('ecx_readODlist()')
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  *         if not result > 0:             # <<<<<<<<<<<<<<
  *             raise SdoInfoError('Sdo List Info read failed')
  * 
  */
   __pyx_t_5 = ((!((__pyx_v_result > 0) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "pysoem/pysoem.pyx":1041
+    /* "pysoem/pysoem.pyx":1061
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  *         if not result > 0:
  *             raise SdoInfoError('Sdo List Info read failed')             # <<<<<<<<<<<<<<
  * 
  *         coe_objects = []
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1041, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1061, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_s_Sdo_List_Info_read_failed) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_s_Sdo_List_Info_read_failed);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1041, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1061, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 1041, __pyx_L1_error)
+    __PYX_ERR(0, 1061, __pyx_L1_error)
 
-    /* "pysoem/pysoem.pyx":1040
+    /* "pysoem/pysoem.pyx":1060
  *         logger.debug('ecx_readODlist()')
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  *         if not result > 0:             # <<<<<<<<<<<<<<
  *             raise SdoInfoError('Sdo List Info read failed')
  * 
  */
   }
 
-  /* "pysoem/pysoem.pyx":1043
+  /* "pysoem/pysoem.pyx":1063
  *             raise SdoInfoError('Sdo List Info read failed')
  * 
  *         coe_objects = []             # <<<<<<<<<<<<<<
  *         for i in range(self._ex_odlist.Entries):
  *             coe_object = CdefCoeObject(i)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1043, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1063, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_coe_objects = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1044
+  /* "pysoem/pysoem.pyx":1064
  * 
  *         coe_objects = []
  *         for i in range(self._ex_odlist.Entries):             # <<<<<<<<<<<<<<
  *             coe_object = CdefCoeObject(i)
  *             coe_object._ecx_context = self._ecx_contextt
  */
   __pyx_t_4 = __pyx_v_self->_ex_odlist.Entries;
   __pyx_t_6 = __pyx_t_4;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_i = __pyx_t_7;
 
-    /* "pysoem/pysoem.pyx":1045
+    /* "pysoem/pysoem.pyx":1065
  *         coe_objects = []
  *         for i in range(self._ex_odlist.Entries):
  *             coe_object = CdefCoeObject(i)             # <<<<<<<<<<<<<<
  *             coe_object._ecx_context = self._ecx_contextt
  *             coe_object._ex_odlist = &self._ex_odlist
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1045, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint16_t(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1065, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1045, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject), __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1065, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_coe_object, ((struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "pysoem/pysoem.pyx":1046
+    /* "pysoem/pysoem.pyx":1066
  *         for i in range(self._ex_odlist.Entries):
  *             coe_object = CdefCoeObject(i)
  *             coe_object._ecx_context = self._ecx_contextt             # <<<<<<<<<<<<<<
  *             coe_object._ex_odlist = &self._ex_odlist
  *             coe_objects.append(coe_object)
  */
     __pyx_t_8 = __pyx_v_self->_ecx_contextt;
     __pyx_v_coe_object->_ecx_context = __pyx_t_8;
 
-    /* "pysoem/pysoem.pyx":1047
+    /* "pysoem/pysoem.pyx":1067
  *             coe_object = CdefCoeObject(i)
  *             coe_object._ecx_context = self._ecx_contextt
  *             coe_object._ex_odlist = &self._ex_odlist             # <<<<<<<<<<<<<<
  *             coe_objects.append(coe_object)
  * 
  */
     __pyx_v_coe_object->_ex_odlist = (&__pyx_v_self->_ex_odlist);
 
-    /* "pysoem/pysoem.pyx":1048
+    /* "pysoem/pysoem.pyx":1068
  *             coe_object._ecx_context = self._ecx_contextt
  *             coe_object._ex_odlist = &self._ex_odlist
  *             coe_objects.append(coe_object)             # <<<<<<<<<<<<<<
  * 
  *         return coe_objects
  */
-    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_coe_objects, ((PyObject *)__pyx_v_coe_object)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 1048, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_coe_objects, ((PyObject *)__pyx_v_coe_object)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 1068, __pyx_L1_error)
   }
 
-  /* "pysoem/pysoem.pyx":1050
+  /* "pysoem/pysoem.pyx":1070
  *             coe_objects.append(coe_object)
  * 
  *         return coe_objects             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_coe_objects);
   __pyx_r = __pyx_v_coe_objects;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1037
+  /* "pysoem/pysoem.pyx":1057
  *         self._ec_slave.islost = value
  * 
  *     def _get_od(self):             # <<<<<<<<<<<<<<
  *         logger.debug('ecx_readODlist()')
  *         cdef int result = cpysoem.ecx_readODlist(self._ecx_contextt, self._pos, &self._ex_odlist)
  */
 
@@ -14320,15 +14415,15 @@
   __Pyx_XDECREF(__pyx_v_coe_objects);
   __Pyx_XDECREF((PyObject *)__pyx_v_coe_object);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":590
+/* "pysoem/pysoem.pyx":597
  *     cdef CdefMasterSettings* _the_masters_settings
  *     cdef _pos # keep in mind that first slave has pos 1
  *     cdef public _CallbackData _cd             # <<<<<<<<<<<<<<
  *     cdef cpysoem.ec_ODlistt _ex_odlist
  * 
  */
 
@@ -14378,15 +14473,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 590, __pyx_L1_error)
+  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 597, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_cd);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_cd));
   __pyx_v_self->_cd = ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -14435,27 +14530,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("self._ec_slave,self._ecx_contextt,self._ex_odlist,self._the_masters_settings cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_69__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_69__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_68__reduce_cython__(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_70__reduce_cython__(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_68__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_70__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -14492,27 +14587,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("self._ec_slave,self._ecx_contextt,self._ex_odlist,self._the_masters_settings cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("self._ec_slave,self._ecx_contextt,self._ex_odlist,self._the_masters_settings cannot be converted to a Python object for pickling")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_73__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_6pysoem_6pysoem_9CdefSlave_73__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_70__setstate_cython__(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_6pysoem_6pysoem_9CdefSlave_72__setstate_cython__(((struct __pyx_obj_6pysoem_6pysoem_CdefSlave *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_70__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_6pysoem_6pysoem_9CdefSlave_72__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6pysoem_6pysoem_CdefSlave *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -14541,15 +14636,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefSlave.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1074
+/* "pysoem/pysoem.pyx":1094
  *     obj_access = property(_get_obj_access)
  * 
  *     def __init__(self, int item):             # <<<<<<<<<<<<<<
  *         self._item = item
  *         self._is_description_read = False
  */
 
@@ -14578,26 +14673,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_item)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1074, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1094, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_item = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_item == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1074, __pyx_L3_error)
+    __pyx_v_item = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_item == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1094, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1074, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1094, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefCoeObject.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_13CdefCoeObject___init__(((struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *)__pyx_v_self), __pyx_v_item);
 
@@ -14607,56 +14702,56 @@
 }
 
 static int __pyx_pf_6pysoem_6pysoem_13CdefCoeObject___init__(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObject *__pyx_v_self, int __pyx_v_item) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":1075
+  /* "pysoem/pysoem.pyx":1095
  * 
  *     def __init__(self, int item):
  *         self._item = item             # <<<<<<<<<<<<<<
  *         self._is_description_read = False
  *         self._are_entries_read = False
  */
   __pyx_v_self->_item = __pyx_v_item;
 
-  /* "pysoem/pysoem.pyx":1076
+  /* "pysoem/pysoem.pyx":1096
  *     def __init__(self, int item):
  *         self._item = item
  *         self._is_description_read = False             # <<<<<<<<<<<<<<
  *         self._are_entries_read = False
  * 
  */
   __pyx_v_self->_is_description_read = 0;
 
-  /* "pysoem/pysoem.pyx":1077
+  /* "pysoem/pysoem.pyx":1097
  *         self._item = item
  *         self._is_description_read = False
  *         self._are_entries_read = False             # <<<<<<<<<<<<<<
  * 
  *     def _read_description(self):
  */
   __pyx_v_self->_are_entries_read = 0;
 
-  /* "pysoem/pysoem.pyx":1074
+  /* "pysoem/pysoem.pyx":1094
  *     obj_access = property(_get_obj_access)
  * 
  *     def __init__(self, int item):             # <<<<<<<<<<<<<<
  *         self._item = item
  *         self._is_description_read = False
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1079
+/* "pysoem/pysoem.pyx":1099
  *         self._are_entries_read = False
  * 
  *     def _read_description(self):             # <<<<<<<<<<<<<<
  *         cdef int result
  *         if not self._is_description_read:
  */
 
@@ -14682,128 +14777,128 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_read_description", 0);
 
-  /* "pysoem/pysoem.pyx":1081
+  /* "pysoem/pysoem.pyx":1101
  *     def _read_description(self):
  *         cdef int result
  *         if not self._is_description_read:             # <<<<<<<<<<<<<<
  *           logger.debug('ecx_readODdescription()')
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  */
   __pyx_t_1 = ((!(__pyx_v_self->_is_description_read != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":1082
+    /* "pysoem/pysoem.pyx":1102
  *         cdef int result
  *         if not self._is_description_read:
  *           logger.debug('ecx_readODdescription()')             # <<<<<<<<<<<<<<
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  *           if not result > 0:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1082, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_kp_s_ecx_readODdescription) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_ecx_readODdescription);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1082, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":1083
+    /* "pysoem/pysoem.pyx":1103
  *         if not self._is_description_read:
  *           logger.debug('ecx_readODdescription()')
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)             # <<<<<<<<<<<<<<
  *           if not result > 0:
  *               raise SdoInfoError('Sdo Object Info read failed')
  */
     __pyx_v_result = ecx_readODdescription(__pyx_v_self->_ecx_context, __pyx_v_self->_item, __pyx_v_self->_ex_odlist);
 
-    /* "pysoem/pysoem.pyx":1084
+    /* "pysoem/pysoem.pyx":1104
  *           logger.debug('ecx_readODdescription()')
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  *           if not result > 0:             # <<<<<<<<<<<<<<
  *               raise SdoInfoError('Sdo Object Info read failed')
  *           self._is_description_read = True
  */
     __pyx_t_1 = ((!((__pyx_v_result > 0) != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "pysoem/pysoem.pyx":1085
+      /* "pysoem/pysoem.pyx":1105
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  *           if not result > 0:
  *               raise SdoInfoError('Sdo Object Info read failed')             # <<<<<<<<<<<<<<
  *           self._is_description_read = True
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1085, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_kp_s_Sdo_Object_Info_read_failed) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Sdo_Object_Info_read_failed);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1085, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1105, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 1085, __pyx_L1_error)
+      __PYX_ERR(0, 1105, __pyx_L1_error)
 
-      /* "pysoem/pysoem.pyx":1084
+      /* "pysoem/pysoem.pyx":1104
  *           logger.debug('ecx_readODdescription()')
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  *           if not result > 0:             # <<<<<<<<<<<<<<
  *               raise SdoInfoError('Sdo Object Info read failed')
  *           self._is_description_read = True
  */
     }
 
-    /* "pysoem/pysoem.pyx":1086
+    /* "pysoem/pysoem.pyx":1106
  *           if not result > 0:
  *               raise SdoInfoError('Sdo Object Info read failed')
  *           self._is_description_read = True             # <<<<<<<<<<<<<<
  * 
  *     def _read_entries(self):
  */
     __pyx_v_self->_is_description_read = 1;
 
-    /* "pysoem/pysoem.pyx":1081
+    /* "pysoem/pysoem.pyx":1101
  *     def _read_description(self):
  *         cdef int result
  *         if not self._is_description_read:             # <<<<<<<<<<<<<<
  *           logger.debug('ecx_readODdescription()')
  *           result = cpysoem.ecx_readODdescription(self._ecx_context, self._item, self._ex_odlist)
  */
   }
 
-  /* "pysoem/pysoem.pyx":1079
+  /* "pysoem/pysoem.pyx":1099
  *         self._are_entries_read = False
  * 
  *     def _read_description(self):             # <<<<<<<<<<<<<<
  *         cdef int result
  *         if not self._is_description_read:
  */
 
@@ -14818,15 +14913,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1088
+/* "pysoem/pysoem.pyx":1108
  *           self._is_description_read = True
  * 
  *     def _read_entries(self):             # <<<<<<<<<<<<<<
  *         cdef int result
  *         if not self._are_entries_read:
  */
 
@@ -14852,128 +14947,128 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_read_entries", 0);
 
-  /* "pysoem/pysoem.pyx":1090
+  /* "pysoem/pysoem.pyx":1110
  *     def _read_entries(self):
  *         cdef int result
  *         if not self._are_entries_read:             # <<<<<<<<<<<<<<
  *             logger.debug('ecx_readOE()')
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  */
   __pyx_t_1 = ((!(__pyx_v_self->_are_entries_read != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":1091
+    /* "pysoem/pysoem.pyx":1111
  *         cdef int result
  *         if not self._are_entries_read:
  *             logger.debug('ecx_readOE()')             # <<<<<<<<<<<<<<
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  *             if not result > 0:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1091, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1091, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_kp_s_ecx_readOE) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_ecx_readOE);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1091, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pysoem/pysoem.pyx":1092
+    /* "pysoem/pysoem.pyx":1112
  *         if not self._are_entries_read:
  *             logger.debug('ecx_readOE()')
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)             # <<<<<<<<<<<<<<
  *             if not result > 0:
  *                 raise SdoInfoError('Sdo ObjectEntry Info read failed')
  */
     __pyx_v_result = ecx_readOE(__pyx_v_self->_ecx_context, __pyx_v_self->_item, __pyx_v_self->_ex_odlist, (&__pyx_v_self->_ex_oelist));
 
-    /* "pysoem/pysoem.pyx":1093
+    /* "pysoem/pysoem.pyx":1113
  *             logger.debug('ecx_readOE()')
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  *             if not result > 0:             # <<<<<<<<<<<<<<
  *                 raise SdoInfoError('Sdo ObjectEntry Info read failed')
  *             self._are_entries_read = True
  */
     __pyx_t_1 = ((!((__pyx_v_result > 0) != 0)) != 0);
     if (unlikely(__pyx_t_1)) {
 
-      /* "pysoem/pysoem.pyx":1094
+      /* "pysoem/pysoem.pyx":1114
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  *             if not result > 0:
  *                 raise SdoInfoError('Sdo ObjectEntry Info read failed')             # <<<<<<<<<<<<<<
  *             self._are_entries_read = True
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1094, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_SdoInfoError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_kp_s_Sdo_ObjectEntry_Info_read_failed) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_s_Sdo_ObjectEntry_Info_read_failed);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1094, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 1094, __pyx_L1_error)
+      __PYX_ERR(0, 1114, __pyx_L1_error)
 
-      /* "pysoem/pysoem.pyx":1093
+      /* "pysoem/pysoem.pyx":1113
  *             logger.debug('ecx_readOE()')
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  *             if not result > 0:             # <<<<<<<<<<<<<<
  *                 raise SdoInfoError('Sdo ObjectEntry Info read failed')
  *             self._are_entries_read = True
  */
     }
 
-    /* "pysoem/pysoem.pyx":1095
+    /* "pysoem/pysoem.pyx":1115
  *             if not result > 0:
  *                 raise SdoInfoError('Sdo ObjectEntry Info read failed')
  *             self._are_entries_read = True             # <<<<<<<<<<<<<<
  * 
  *     def _get_index(self):
  */
     __pyx_v_self->_are_entries_read = 1;
 
-    /* "pysoem/pysoem.pyx":1090
+    /* "pysoem/pysoem.pyx":1110
  *     def _read_entries(self):
  *         cdef int result
  *         if not self._are_entries_read:             # <<<<<<<<<<<<<<
  *             logger.debug('ecx_readOE()')
  *             result = cpysoem.ecx_readOE(self._ecx_context, self._item, self._ex_odlist, &self._ex_oelist)
  */
   }
 
-  /* "pysoem/pysoem.pyx":1088
+  /* "pysoem/pysoem.pyx":1108
  *           self._is_description_read = True
  * 
  *     def _read_entries(self):             # <<<<<<<<<<<<<<
  *         cdef int result
  *         if not self._are_entries_read:
  */
 
@@ -14988,15 +15083,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1097
+/* "pysoem/pysoem.pyx":1117
  *             self._are_entries_read = True
  * 
  *     def _get_index(self):             # <<<<<<<<<<<<<<
  *         return self._ex_odlist.Index[self._item]
  * 
  */
 
@@ -15018,29 +15113,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_index", 0);
 
-  /* "pysoem/pysoem.pyx":1098
+  /* "pysoem/pysoem.pyx":1118
  * 
  *     def _get_index(self):
  *         return self._ex_odlist.Index[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_data_type(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_odlist->Index[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1098, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_odlist->Index[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1097
+  /* "pysoem/pysoem.pyx":1117
  *             self._are_entries_read = True
  * 
  *     def _get_index(self):             # <<<<<<<<<<<<<<
  *         return self._ex_odlist.Index[self._item]
  * 
  */
 
@@ -15051,15 +15146,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1100
+/* "pysoem/pysoem.pyx":1120
  *         return self._ex_odlist.Index[self._item]
  * 
  *     def _get_data_type(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.DataType[self._item]
  */
 
@@ -15083,55 +15178,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_data_type", 0);
 
-  /* "pysoem/pysoem.pyx":1101
+  /* "pysoem/pysoem.pyx":1121
  * 
  *     def _get_data_type(self):
  *         self._read_description()             # <<<<<<<<<<<<<<
  *         return self._ex_odlist.DataType[self._item]
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1102
+  /* "pysoem/pysoem.pyx":1122
  *     def _get_data_type(self):
  *         self._read_description()
  *         return self._ex_odlist.DataType[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_object_code(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_odlist->DataType[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_odlist->DataType[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1100
+  /* "pysoem/pysoem.pyx":1120
  *         return self._ex_odlist.Index[self._item]
  * 
  *     def _get_data_type(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.DataType[self._item]
  */
 
@@ -15144,15 +15239,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1104
+/* "pysoem/pysoem.pyx":1124
  *         return self._ex_odlist.DataType[self._item]
  * 
  *     def _get_object_code(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.ObjectCode[self._item]
  */
 
@@ -15176,55 +15271,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_object_code", 0);
 
-  /* "pysoem/pysoem.pyx":1105
+  /* "pysoem/pysoem.pyx":1125
  * 
  *     def _get_object_code(self):
  *         self._read_description()             # <<<<<<<<<<<<<<
  *         return self._ex_odlist.ObjectCode[self._item]
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1105, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1106
+  /* "pysoem/pysoem.pyx":1126
  *     def _get_object_code(self):
  *         self._read_description()
  *         return self._ex_odlist.ObjectCode[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_name(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_self->_ex_odlist->ObjectCode[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t((__pyx_v_self->_ex_odlist->ObjectCode[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1104
+  /* "pysoem/pysoem.pyx":1124
  *         return self._ex_odlist.DataType[self._item]
  * 
  *     def _get_object_code(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.ObjectCode[self._item]
  */
 
@@ -15237,15 +15332,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1108
+/* "pysoem/pysoem.pyx":1128
  *         return self._ex_odlist.ObjectCode[self._item]
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.Name[self._item]
  */
 
@@ -15269,55 +15364,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_name", 0);
 
-  /* "pysoem/pysoem.pyx":1109
+  /* "pysoem/pysoem.pyx":1129
  * 
  *     def _get_name(self):
  *         self._read_description()             # <<<<<<<<<<<<<<
  *         return self._ex_odlist.Name[self._item]
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1109, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1109, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1110
+  /* "pysoem/pysoem.pyx":1130
  *     def _get_name(self):
  *         self._read_description()
  *         return self._ex_odlist.Name[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_entries(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_self->_ex_odlist->Name[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1110, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_self->_ex_odlist->Name[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1108
+  /* "pysoem/pysoem.pyx":1128
  *         return self._ex_odlist.ObjectCode[self._item]
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         return self._ex_odlist.Name[self._item]
  */
 
@@ -15330,15 +15425,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1112
+/* "pysoem/pysoem.pyx":1132
  *         return self._ex_odlist.Name[self._item]
  * 
  *     def _get_entries(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         self._read_entries()
  */
 
@@ -15370,172 +15465,172 @@
   long __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_entries", 0);
 
-  /* "pysoem/pysoem.pyx":1113
+  /* "pysoem/pysoem.pyx":1133
  * 
  *     def _get_entries(self):
  *         self._read_description()             # <<<<<<<<<<<<<<
  *         self._read_entries()
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1113, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1113, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1114
+  /* "pysoem/pysoem.pyx":1134
  *     def _get_entries(self):
  *         self._read_description()
  *         self._read_entries()             # <<<<<<<<<<<<<<
  * 
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1114, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1114, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1116
+  /* "pysoem/pysoem.pyx":1136
  *         self._read_entries()
  * 
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return []
  *         else:
  */
   __pyx_t_4 = (((__pyx_v_self->_ex_odlist->MaxSub[__pyx_v_self->_item]) == 0) != 0);
   if (__pyx_t_4) {
 
-    /* "pysoem/pysoem.pyx":1117
+    /* "pysoem/pysoem.pyx":1137
  * 
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return []             # <<<<<<<<<<<<<<
  *         else:
  *             entries = []
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1117, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pysoem/pysoem.pyx":1116
+    /* "pysoem/pysoem.pyx":1136
  *         self._read_entries()
  * 
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return []
  *         else:
  */
   }
 
-  /* "pysoem/pysoem.pyx":1119
+  /* "pysoem/pysoem.pyx":1139
  *             return []
  *         else:
  *             entries = []             # <<<<<<<<<<<<<<
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  *                 entry = CdefCoeObjectEntry(i)
  */
   /*else*/ {
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1119, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_entries = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pysoem/pysoem.pyx":1120
+    /* "pysoem/pysoem.pyx":1140
  *         else:
  *             entries = []
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):             # <<<<<<<<<<<<<<
  *                 entry = CdefCoeObjectEntry(i)
  *                 entry._ex_oelist = &self._ex_oelist
  */
     __pyx_t_5 = ((__pyx_v_self->_ex_odlist->MaxSub[__pyx_v_self->_item]) + 1);
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_v_i = __pyx_t_7;
 
-      /* "pysoem/pysoem.pyx":1121
+      /* "pysoem/pysoem.pyx":1141
  *             entries = []
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  *                 entry = CdefCoeObjectEntry(i)             # <<<<<<<<<<<<<<
  *                 entry._ex_oelist = &self._ex_oelist
  *                 entries.append(entry)
  */
-      __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1121, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1121, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1141, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF_SET(__pyx_v_entry, ((struct __pyx_obj_6pysoem_6pysoem_CdefCoeObjectEntry *)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "pysoem/pysoem.pyx":1122
+      /* "pysoem/pysoem.pyx":1142
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  *                 entry = CdefCoeObjectEntry(i)
  *                 entry._ex_oelist = &self._ex_oelist             # <<<<<<<<<<<<<<
  *                 entries.append(entry)
  *             return entries
  */
       __pyx_v_entry->_ex_oelist = (&__pyx_v_self->_ex_oelist);
 
-      /* "pysoem/pysoem.pyx":1123
+      /* "pysoem/pysoem.pyx":1143
  *                 entry = CdefCoeObjectEntry(i)
  *                 entry._ex_oelist = &self._ex_oelist
  *                 entries.append(entry)             # <<<<<<<<<<<<<<
  *             return entries
  * 
  */
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_entries, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 1123, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_entries, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 1143, __pyx_L1_error)
     }
 
-    /* "pysoem/pysoem.pyx":1124
+    /* "pysoem/pysoem.pyx":1144
  *                 entry._ex_oelist = &self._ex_oelist
  *                 entries.append(entry)
  *             return entries             # <<<<<<<<<<<<<<
  * 
  *     def _get_bit_length(self):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_entries);
     __pyx_r = __pyx_v_entries;
     goto __pyx_L0;
   }
 
-  /* "pysoem/pysoem.pyx":1112
+  /* "pysoem/pysoem.pyx":1132
  *         return self._ex_odlist.Name[self._item]
  * 
  *     def _get_entries(self):             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         self._read_entries()
  */
 
@@ -15550,15 +15645,15 @@
   __Pyx_XDECREF(__pyx_v_entries);
   __Pyx_XDECREF((PyObject *)__pyx_v_entry);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1126
+/* "pysoem/pysoem.pyx":1146
  *             return entries
  * 
  *     def _get_bit_length(self):             # <<<<<<<<<<<<<<
  *         cdef int sum = 0
  *         self._read_description()
  */
 
@@ -15588,147 +15683,147 @@
   long __pyx_t_6;
   long __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_bit_length", 0);
 
-  /* "pysoem/pysoem.pyx":1127
+  /* "pysoem/pysoem.pyx":1147
  * 
  *     def _get_bit_length(self):
  *         cdef int sum = 0             # <<<<<<<<<<<<<<
  *         self._read_description()
  *         self._read_entries()
  */
   __pyx_v_sum = 0;
 
-  /* "pysoem/pysoem.pyx":1128
+  /* "pysoem/pysoem.pyx":1148
  *     def _get_bit_length(self):
  *         cdef int sum = 0
  *         self._read_description()             # <<<<<<<<<<<<<<
  *         self._read_entries()
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1128, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_description); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1129
+  /* "pysoem/pysoem.pyx":1149
  *         cdef int sum = 0
  *         self._read_description()
  *         self._read_entries()             # <<<<<<<<<<<<<<
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return self._ex_oelist.BitLength[0]
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1129, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1129, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1130
+  /* "pysoem/pysoem.pyx":1150
  *         self._read_description()
  *         self._read_entries()
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return self._ex_oelist.BitLength[0]
  *         else:
  */
   __pyx_t_4 = (((__pyx_v_self->_ex_odlist->MaxSub[__pyx_v_self->_item]) == 0) != 0);
   if (__pyx_t_4) {
 
-    /* "pysoem/pysoem.pyx":1131
+    /* "pysoem/pysoem.pyx":1151
  *         self._read_entries()
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return self._ex_oelist.BitLength[0]             # <<<<<<<<<<<<<<
  *         else:
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist.BitLength[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1131, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist.BitLength[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pysoem/pysoem.pyx":1130
+    /* "pysoem/pysoem.pyx":1150
  *         self._read_description()
  *         self._read_entries()
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return self._ex_oelist.BitLength[0]
  *         else:
  */
   }
 
-  /* "pysoem/pysoem.pyx":1133
+  /* "pysoem/pysoem.pyx":1153
  *             return self._ex_oelist.BitLength[0]
  *         else:
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):             # <<<<<<<<<<<<<<
  *                 sum += self._ex_oelist.BitLength[i]
  *             return sum
  */
   /*else*/ {
     __pyx_t_5 = ((__pyx_v_self->_ex_odlist->MaxSub[__pyx_v_self->_item]) + 1);
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_v_i = __pyx_t_7;
 
-      /* "pysoem/pysoem.pyx":1134
+      /* "pysoem/pysoem.pyx":1154
  *         else:
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  *                 sum += self._ex_oelist.BitLength[i]             # <<<<<<<<<<<<<<
  *             return sum
  * 
  */
       __pyx_v_sum = (__pyx_v_sum + (__pyx_v_self->_ex_oelist.BitLength[__pyx_v_i]));
     }
 
-    /* "pysoem/pysoem.pyx":1135
+    /* "pysoem/pysoem.pyx":1155
  *             for i in range(self._ex_odlist.MaxSub[self._item]+1):
  *                 sum += self._ex_oelist.BitLength[i]
  *             return sum             # <<<<<<<<<<<<<<
  * 
  *     def _get_obj_access(self):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_sum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1135, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_sum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
   }
 
-  /* "pysoem/pysoem.pyx":1126
+  /* "pysoem/pysoem.pyx":1146
  *             return entries
  * 
  *     def _get_bit_length(self):             # <<<<<<<<<<<<<<
  *         cdef int sum = 0
  *         self._read_description()
  */
 
@@ -15741,15 +15836,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1137
+/* "pysoem/pysoem.pyx":1157
  *             return sum
  * 
  *     def _get_obj_access(self):             # <<<<<<<<<<<<<<
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return self._ex_oelist.ObjAccess[0]
  */
 
@@ -15772,62 +15867,62 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_obj_access", 0);
 
-  /* "pysoem/pysoem.pyx":1138
+  /* "pysoem/pysoem.pyx":1158
  * 
  *     def _get_obj_access(self):
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return self._ex_oelist.ObjAccess[0]
  *         else:
  */
   __pyx_t_1 = (((__pyx_v_self->_ex_odlist->MaxSub[__pyx_v_self->_item]) == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "pysoem/pysoem.pyx":1139
+    /* "pysoem/pysoem.pyx":1159
  *     def _get_obj_access(self):
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return self._ex_oelist.ObjAccess[0]             # <<<<<<<<<<<<<<
  *         else:
  *             return 0
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist.ObjAccess[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1139, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist.ObjAccess[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "pysoem/pysoem.pyx":1138
+    /* "pysoem/pysoem.pyx":1158
  * 
  *     def _get_obj_access(self):
  *         if self._ex_odlist.MaxSub[self._item] == 0:             # <<<<<<<<<<<<<<
  *             return self._ex_oelist.ObjAccess[0]
  *         else:
  */
   }
 
-  /* "pysoem/pysoem.pyx":1141
+  /* "pysoem/pysoem.pyx":1161
  *             return self._ex_oelist.ObjAccess[0]
  *         else:
  *             return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_int_0);
     __pyx_r = __pyx_int_0;
     goto __pyx_L0;
   }
 
-  /* "pysoem/pysoem.pyx":1137
+  /* "pysoem/pysoem.pyx":1157
  *             return sum
  * 
  *     def _get_obj_access(self):             # <<<<<<<<<<<<<<
  *         if self._ex_odlist.MaxSub[self._item] == 0:
  *             return self._ex_oelist.ObjAccess[0]
  */
 
@@ -15951,15 +16046,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefCoeObject.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1153
+/* "pysoem/pysoem.pyx":1173
  *     obj_access = property(_get_obj_access)
  * 
  *     def __init__(self, int item):             # <<<<<<<<<<<<<<
  *         self._item = item
  * 
  */
 
@@ -15988,26 +16083,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_item)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1153, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 1173, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_item = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_item == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1153, __pyx_L3_error)
+    __pyx_v_item = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_item == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1173, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1153, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1173, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pysoem.pysoem.CdefCoeObjectEntry.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6pysoem_6pysoem_18CdefCoeObjectEntry___init__(((struct __pyx_obj_6pysoem_6pysoem_CdefCoeObjectEntry *)__pyx_v_self), __pyx_v_item);
 
@@ -16017,38 +16112,38 @@
 }
 
 static int __pyx_pf_6pysoem_6pysoem_18CdefCoeObjectEntry___init__(struct __pyx_obj_6pysoem_6pysoem_CdefCoeObjectEntry *__pyx_v_self, int __pyx_v_item) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pysoem/pysoem.pyx":1154
+  /* "pysoem/pysoem.pyx":1174
  * 
  *     def __init__(self, int item):
  *         self._item = item             # <<<<<<<<<<<<<<
  * 
  *     def _get_name(self):
  */
   __pyx_v_self->_item = __pyx_v_item;
 
-  /* "pysoem/pysoem.pyx":1153
+  /* "pysoem/pysoem.pyx":1173
  *     obj_access = property(_get_obj_access)
  * 
  *     def __init__(self, int item):             # <<<<<<<<<<<<<<
  *         self._item = item
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1156
+/* "pysoem/pysoem.pyx":1176
  *         self._item = item
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.Name[self._item]
  * 
  */
 
@@ -16070,29 +16165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_name", 0);
 
-  /* "pysoem/pysoem.pyx":1157
+  /* "pysoem/pysoem.pyx":1177
  * 
  *     def _get_name(self):
  *         return self._ex_oelist.Name[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_data_type(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_self->_ex_oelist->Name[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1157, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_self->_ex_oelist->Name[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1156
+  /* "pysoem/pysoem.pyx":1176
  *         self._item = item
  * 
  *     def _get_name(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.Name[self._item]
  * 
  */
 
@@ -16103,15 +16198,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1159
+/* "pysoem/pysoem.pyx":1179
  *         return self._ex_oelist.Name[self._item]
  * 
  *     def _get_data_type(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.DataType[self._item]
  * 
  */
 
@@ -16133,29 +16228,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_data_type", 0);
 
-  /* "pysoem/pysoem.pyx":1160
+  /* "pysoem/pysoem.pyx":1180
  * 
  *     def _get_data_type(self):
  *         return self._ex_oelist.DataType[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_bit_length(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->DataType[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1160, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->DataType[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1159
+  /* "pysoem/pysoem.pyx":1179
  *         return self._ex_oelist.Name[self._item]
  * 
  *     def _get_data_type(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.DataType[self._item]
  * 
  */
 
@@ -16166,15 +16261,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1162
+/* "pysoem/pysoem.pyx":1182
  *         return self._ex_oelist.DataType[self._item]
  * 
  *     def _get_bit_length(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.BitLength[self._item]
  * 
  */
 
@@ -16196,29 +16291,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_bit_length", 0);
 
-  /* "pysoem/pysoem.pyx":1163
+  /* "pysoem/pysoem.pyx":1183
  * 
  *     def _get_bit_length(self):
  *         return self._ex_oelist.BitLength[self._item]             # <<<<<<<<<<<<<<
  * 
  *     def _get_obj_access(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->BitLength[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->BitLength[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1162
+  /* "pysoem/pysoem.pyx":1182
  *         return self._ex_oelist.DataType[self._item]
  * 
  *     def _get_bit_length(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.BitLength[self._item]
  * 
  */
 
@@ -16229,15 +16324,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1165
+/* "pysoem/pysoem.pyx":1185
  *         return self._ex_oelist.BitLength[self._item]
  * 
  *     def _get_obj_access(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.ObjAccess[self._item]
  * 
  */
 
@@ -16259,29 +16354,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_obj_access", 0);
 
-  /* "pysoem/pysoem.pyx":1166
+  /* "pysoem/pysoem.pyx":1186
  * 
  *     def _get_obj_access(self):
  *         return self._ex_oelist.ObjAccess[self._item]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->ObjAccess[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint16_t((__pyx_v_self->_ex_oelist->ObjAccess[__pyx_v_self->_item])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pysoem/pysoem.pyx":1165
+  /* "pysoem/pysoem.pyx":1185
  *         return self._ex_oelist.BitLength[self._item]
  * 
  *     def _get_obj_access(self):             # <<<<<<<<<<<<<<
  *         return self._ex_oelist.ObjAccess[self._item]
  * 
  */
 
@@ -16405,15 +16500,15 @@
   __Pyx_AddTraceback("pysoem.pysoem.CdefCoeObjectEntry.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1169
+/* "pysoem/pysoem.pyx":1189
  * 
  * 
  * cdef int _xPO2SOconfig(cpysoem.uint16 slave, void* user):             # <<<<<<<<<<<<<<
  *     cdef _CallbackData cd
  *     cd = <object>user
  */
 
@@ -16431,41 +16526,41 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_xPO2SOconfig", 0);
 
-  /* "pysoem/pysoem.pyx":1171
+  /* "pysoem/pysoem.pyx":1191
  * cdef int _xPO2SOconfig(cpysoem.uint16 slave, void* user):
  *     cdef _CallbackData cd
  *     cd = <object>user             # <<<<<<<<<<<<<<
  *     cd.exc_raised = False
  *     try:
  */
-  if (!(likely(((((PyObject *)__pyx_v_user)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user), __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 1171, __pyx_L1_error)
+  if (!(likely(((((PyObject *)__pyx_v_user)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user), __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 1191, __pyx_L1_error)
   __pyx_t_1 = ((PyObject *)__pyx_v_user);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cd = ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1172
+  /* "pysoem/pysoem.pyx":1192
  *     cdef _CallbackData cd
  *     cd = <object>user
  *     cd.exc_raised = False             # <<<<<<<<<<<<<<
  *     try:
  *         (<object>cd.func)(slave-1)
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_cd->exc_raised);
   __Pyx_DECREF(__pyx_v_cd->exc_raised);
   __pyx_v_cd->exc_raised = Py_False;
 
-  /* "pysoem/pysoem.pyx":1173
+  /* "pysoem/pysoem.pyx":1193
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(slave-1)
  *     except:
  */
   {
@@ -16473,22 +16568,22 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pysoem/pysoem.pyx":1174
+      /* "pysoem/pysoem.pyx":1194
  *     cd.exc_raised = False
  *     try:
  *         (<object>cd.func)(slave-1)             # <<<<<<<<<<<<<<
  *     except:
  *         cd.exc_raised = True
  */
-      __pyx_t_5 = __Pyx_PyInt_From_long((__pyx_v_slave - 1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1174, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyInt_From_long((__pyx_v_slave - 1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1194, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(((PyObject *)__pyx_v_cd->func));
       __pyx_t_6 = __pyx_v_cd->func; __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -16496,20 +16591,20 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1174, __pyx_L3_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1194, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pysoem/pysoem.pyx":1173
+      /* "pysoem/pysoem.pyx":1193
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(slave-1)
  *     except:
  */
     }
@@ -16519,81 +16614,81 @@
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pysoem/pysoem.pyx":1175
+    /* "pysoem/pysoem.pyx":1195
  *     try:
  *         (<object>cd.func)(slave-1)
  *     except:             # <<<<<<<<<<<<<<
  *         cd.exc_raised = True
  *         cd.exc_info = sys.exc_info()
  */
     /*except:*/ {
       __Pyx_AddTraceback("pysoem.pysoem._xPO2SOconfig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 1175, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 1195, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_5);
 
-      /* "pysoem/pysoem.pyx":1176
+      /* "pysoem/pysoem.pyx":1196
  *         (<object>cd.func)(slave-1)
  *     except:
  *         cd.exc_raised = True             # <<<<<<<<<<<<<<
  *         cd.exc_info = sys.exc_info()
  * 
  */
       __Pyx_INCREF(Py_True);
       __Pyx_GIVEREF(Py_True);
       __Pyx_GOTREF(__pyx_v_cd->exc_raised);
       __Pyx_DECREF(__pyx_v_cd->exc_raised);
       __pyx_v_cd->exc_raised = Py_True;
 
-      /* "pysoem/pysoem.pyx":1177
+      /* "pysoem/pysoem.pyx":1197
  *     except:
  *         cd.exc_raised = True
  *         cd.exc_info = sys.exc_info()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sys); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1177, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sys); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1197, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1177, __pyx_L5_except_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1197, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1177, __pyx_L5_except_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1197, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GIVEREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_v_cd->exc_info);
       __Pyx_DECREF(__pyx_v_cd->exc_info);
       __pyx_v_cd->exc_info = __pyx_t_7;
       __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L4_exception_handled;
     }
     __pyx_L5_except_error:;
 
-    /* "pysoem/pysoem.pyx":1173
+    /* "pysoem/pysoem.pyx":1193
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(slave-1)
  *     except:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -16605,15 +16700,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     __pyx_L8_try_end:;
   }
 
-  /* "pysoem/pysoem.pyx":1169
+  /* "pysoem/pysoem.pyx":1189
  * 
  * 
  * cdef int _xPO2SOconfig(cpysoem.uint16 slave, void* user):             # <<<<<<<<<<<<<<
  *     cdef _CallbackData cd
  *     cd = <object>user
  */
 
@@ -16631,15 +16726,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cd);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pysoem/pysoem.pyx":1180
+/* "pysoem/pysoem.pyx":1200
  * 
  * 
  * cdef int _xPO2SOconfigEx(cpysoem.uint16 slave, void* user):             # <<<<<<<<<<<<<<
  *     cdef _CallbackData cd
  *     cd = <object>user
  */
 
@@ -16657,41 +16752,41 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_xPO2SOconfigEx", 0);
 
-  /* "pysoem/pysoem.pyx":1182
+  /* "pysoem/pysoem.pyx":1202
  * cdef int _xPO2SOconfigEx(cpysoem.uint16 slave, void* user):
  *     cdef _CallbackData cd
  *     cd = <object>user             # <<<<<<<<<<<<<<
  *     cd.exc_raised = False
  *     try:
  */
-  if (!(likely(((((PyObject *)__pyx_v_user)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user), __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 1182, __pyx_L1_error)
+  if (!(likely(((((PyObject *)__pyx_v_user)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user), __pyx_ptype_6pysoem_6pysoem__CallbackData))))) __PYX_ERR(0, 1202, __pyx_L1_error)
   __pyx_t_1 = ((PyObject *)__pyx_v_user);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cd = ((struct __pyx_obj_6pysoem_6pysoem__CallbackData *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":1183
+  /* "pysoem/pysoem.pyx":1203
  *     cdef _CallbackData cd
  *     cd = <object>user
  *     cd.exc_raised = False             # <<<<<<<<<<<<<<
  *     try:
  *         (<object>cd.func)(cd.slave)
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_cd->exc_raised);
   __Pyx_DECREF(__pyx_v_cd->exc_raised);
   __pyx_v_cd->exc_raised = Py_False;
 
-  /* "pysoem/pysoem.pyx":1184
+  /* "pysoem/pysoem.pyx":1204
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(cd.slave)
  *     except:
  */
   {
@@ -16699,15 +16794,15 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pysoem/pysoem.pyx":1185
+      /* "pysoem/pysoem.pyx":1205
  *     cd.exc_raised = False
  *     try:
  *         (<object>cd.func)(cd.slave)             # <<<<<<<<<<<<<<
  *     except:
  *         cd.exc_raised = True
  */
       __Pyx_INCREF(((PyObject *)__pyx_v_cd->func));
@@ -16719,20 +16814,20 @@
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_cd->slave) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_cd->slave);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1185, __pyx_L3_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pysoem/pysoem.pyx":1184
+      /* "pysoem/pysoem.pyx":1204
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(cd.slave)
  *     except:
  */
     }
@@ -16741,78 +16836,78 @@
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pysoem/pysoem.pyx":1186
+    /* "pysoem/pysoem.pyx":1206
  *     try:
  *         (<object>cd.func)(cd.slave)
  *     except:             # <<<<<<<<<<<<<<
  *         cd.exc_raised = True
  *         cd.exc_info = sys.exc_info()
  */
     /*except:*/ {
       __Pyx_AddTraceback("pysoem.pysoem._xPO2SOconfigEx", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 1186, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 1206, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
 
-      /* "pysoem/pysoem.pyx":1187
+      /* "pysoem/pysoem.pyx":1207
  *         (<object>cd.func)(cd.slave)
  *     except:
  *         cd.exc_raised = True             # <<<<<<<<<<<<<<
  *         cd.exc_info = sys.exc_info()
  */
       __Pyx_INCREF(Py_True);
       __Pyx_GIVEREF(Py_True);
       __Pyx_GOTREF(__pyx_v_cd->exc_raised);
       __Pyx_DECREF(__pyx_v_cd->exc_raised);
       __pyx_v_cd->exc_raised = Py_True;
 
-      /* "pysoem/pysoem.pyx":1188
+      /* "pysoem/pysoem.pyx":1208
  *     except:
  *         cd.exc_raised = True
  *         cd.exc_info = sys.exc_info()             # <<<<<<<<<<<<<<
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sys); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1188, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sys); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1208, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1188, __pyx_L5_except_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1208, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_7 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1188, __pyx_L5_except_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1208, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GIVEREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_v_cd->exc_info);
       __Pyx_DECREF(__pyx_v_cd->exc_info);
       __pyx_v_cd->exc_info = __pyx_t_7;
       __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L4_exception_handled;
     }
     __pyx_L5_except_error:;
 
-    /* "pysoem/pysoem.pyx":1184
+    /* "pysoem/pysoem.pyx":1204
  *     cd = <object>user
  *     cd.exc_raised = False
  *     try:             # <<<<<<<<<<<<<<
  *         (<object>cd.func)(cd.slave)
  *     except:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -16824,15 +16919,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     __pyx_L8_try_end:;
   }
 
-  /* "pysoem/pysoem.pyx":1180
+  /* "pysoem/pysoem.pyx":1200
  * 
  * 
  * cdef int _xPO2SOconfigEx(cpysoem.uint16 slave, void* user):             # <<<<<<<<<<<<<<
  *     cdef _CallbackData cd
  *     cd = <object>user
  */
 
@@ -19231,35 +19326,36 @@
   {"recover", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_17recover, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_16recover},
   {"eeprom_read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_19eeprom_read, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_18eeprom_read},
   {"eeprom_write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_21eeprom_write, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_20eeprom_write},
   {"foe_write", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_23foe_write, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_22foe_write},
   {"foe_read", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_25foe_read, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_24foe_read},
   {"amend_mbx", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_27amend_mbx, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_26amend_mbx},
   {"set_watchdog", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_29set_watchdog, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_28set_watchdog},
-  {"_fprd", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_fprd, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_30_fprd},
-  {"_fpwr", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fpwr, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_32_fpwr},
-  {"_get_name", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_get_name, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_34_get_name},
-  {"_get_eep_man", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_eep_man, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_36_get_eep_man},
-  {"_get_eep_id", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_id, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_38_get_eep_id},
-  {"_get_eep_rev", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_rev, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_40_get_eep_rev},
-  {"_get_PO2SOconfig", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_PO2SOconfig, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_42_get_PO2SOconfig},
-  {"_get_PO2SOconfigEx", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfigEx, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfigEx},
-  {"_set_PO2SOconfig", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_set_PO2SOconfig, METH_O, 0},
-  {"_set_PO2SOconfigEx", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfigEx, METH_O, 0},
-  {"_get_state", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_get_state, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_50_get_state},
-  {"_set_state", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_set_state, METH_O, 0},
-  {"_get_input", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_get_input, METH_NOARGS, 0},
-  {"_get_output", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_output, METH_NOARGS, 0},
-  {"_set_output", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_set_output, METH_O, 0},
-  {"_get_al_status", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_get_al_status, METH_NOARGS, 0},
-  {"_get_is_lost", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_is_lost, METH_NOARGS, 0},
-  {"_set_is_lost", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_set_is_lost, METH_O, 0},
-  {"_get_od", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_get_od, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_69__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__setstate_cython__, METH_O, 0},
+  {"_disable_complete_access", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_31_disable_complete_access, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_30_disable_complete_access},
+  {"_fprd", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_33_fprd, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_32_fprd},
+  {"_fpwr", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6pysoem_6pysoem_9CdefSlave_35_fpwr, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_34_fpwr},
+  {"_get_name", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_37_get_name, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_36_get_name},
+  {"_get_eep_man", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_39_get_eep_man, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_38_get_eep_man},
+  {"_get_eep_id", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_41_get_eep_id, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_40_get_eep_id},
+  {"_get_eep_rev", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_43_get_eep_rev, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_42_get_eep_rev},
+  {"_get_PO2SOconfig", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_45_get_PO2SOconfig, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_44_get_PO2SOconfig},
+  {"_get_PO2SOconfigEx", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_47_get_PO2SOconfigEx, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_46_get_PO2SOconfigEx},
+  {"_set_PO2SOconfig", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_49_set_PO2SOconfig, METH_O, 0},
+  {"_set_PO2SOconfigEx", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_51_set_PO2SOconfigEx, METH_O, 0},
+  {"_get_state", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_53_get_state, METH_NOARGS, __pyx_doc_6pysoem_6pysoem_9CdefSlave_52_get_state},
+  {"_set_state", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_55_set_state, METH_O, 0},
+  {"_get_input", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_57_get_input, METH_NOARGS, 0},
+  {"_get_output", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_59_get_output, METH_NOARGS, 0},
+  {"_set_output", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_61_set_output, METH_O, 0},
+  {"_get_al_status", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_63_get_al_status, METH_NOARGS, 0},
+  {"_get_is_lost", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_65_get_is_lost, METH_NOARGS, 0},
+  {"_set_is_lost", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_67_set_is_lost, METH_O, 0},
+  {"_get_od", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_69_get_od, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_71__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_6pysoem_6pysoem_9CdefSlave_73__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_6pysoem_6pysoem_CdefSlave[] = {
   {(char *)"_cd", __pyx_getprop_6pysoem_6pysoem_9CdefSlave__cd, __pyx_setprop_6pysoem_6pysoem_9CdefSlave__cd, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -19855,14 +19951,20 @@
   {&__pyx_n_s_ECT_BIT3, __pyx_k_ECT_BIT3, sizeof(__pyx_k_ECT_BIT3), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BIT4, __pyx_k_ECT_BIT4, sizeof(__pyx_k_ECT_BIT4), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BIT5, __pyx_k_ECT_BIT5, sizeof(__pyx_k_ECT_BIT5), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BIT6, __pyx_k_ECT_BIT6, sizeof(__pyx_k_ECT_BIT6), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BIT7, __pyx_k_ECT_BIT7, sizeof(__pyx_k_ECT_BIT7), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BIT8, __pyx_k_ECT_BIT8, sizeof(__pyx_k_ECT_BIT8), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_BOOLEAN, __pyx_k_ECT_BOOLEAN, sizeof(__pyx_k_ECT_BOOLEAN), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_PDOASSIGN, __pyx_k_ECT_COEDET_PDOASSIGN, sizeof(__pyx_k_ECT_COEDET_PDOASSIGN), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_PDOCONFIG, __pyx_k_ECT_COEDET_PDOCONFIG, sizeof(__pyx_k_ECT_COEDET_PDOCONFIG), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_SDO, __pyx_k_ECT_COEDET_SDO, sizeof(__pyx_k_ECT_COEDET_SDO), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_SDOCA, __pyx_k_ECT_COEDET_SDOCA, sizeof(__pyx_k_ECT_COEDET_SDOCA), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_SDOINFO, __pyx_k_ECT_COEDET_SDOINFO, sizeof(__pyx_k_ECT_COEDET_SDOINFO), 0, 0, 1, 1},
+  {&__pyx_n_s_ECT_COEDET_UPLOAD, __pyx_k_ECT_COEDET_UPLOAD, sizeof(__pyx_k_ECT_COEDET_UPLOAD), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_DOMAIN, __pyx_k_ECT_DOMAIN, sizeof(__pyx_k_ECT_DOMAIN), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_INTEGER16, __pyx_k_ECT_INTEGER16, sizeof(__pyx_k_ECT_INTEGER16), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_INTEGER24, __pyx_k_ECT_INTEGER24, sizeof(__pyx_k_ECT_INTEGER24), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_INTEGER32, __pyx_k_ECT_INTEGER32, sizeof(__pyx_k_ECT_INTEGER32), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_INTEGER64, __pyx_k_ECT_INTEGER64, sizeof(__pyx_k_ECT_INTEGER64), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_INTEGER8, __pyx_k_ECT_INTEGER8, sizeof(__pyx_k_ECT_INTEGER8), 0, 0, 1, 1},
   {&__pyx_n_s_ECT_OCTET_STRING, __pyx_k_ECT_OCTET_STRING, sizeof(__pyx_k_ECT_OCTET_STRING), 0, 0, 1, 1},
@@ -20133,50 +20235,50 @@
   {&__pyx_n_s_wd_time_ms, __pyx_k_wd_time_ms, sizeof(__pyx_k_wd_time_ms), 0, 0, 1, 1},
   {&__pyx_kp_s_wd_time_ms_is_limited_to_ms, __pyx_k_wd_time_ms_is_limited_to_ms, sizeof(__pyx_k_wd_time_ms_is_limited_to_ms), 0, 0, 1, 0},
   {&__pyx_n_s_wd_type, __pyx_k_wd_type, sizeof(__pyx_k_wd_type), 0, 0, 1, 1},
   {&__pyx_n_s_word_address, __pyx_k_word_address, sizeof(__pyx_k_word_address), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 169, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 228, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 391, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_UnboundLocalError = __Pyx_GetBuiltinName(__pyx_n_s_UnboundLocalError); if (!__pyx_builtin_UnboundLocalError) __PYX_ERR(0, 648, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 661, __pyx_L1_error)
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 779, __pyx_L1_error)
+  __pyx_builtin_UnboundLocalError = __Pyx_GetBuiltinName(__pyx_n_s_UnboundLocalError); if (!__pyx_builtin_UnboundLocalError) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 786, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 33, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pysoem/pysoem.pyx":293
+  /* "pysoem/pysoem.pyx":300
  *                                               err.ErrorCode))
  *             else:
  *                 error_list.append(Exception('unexpected error'))             # <<<<<<<<<<<<<<
  *         return error_list
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_unexpected_error); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_unexpected_error); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "pysoem/pysoem.pyx":384
+  /* "pysoem/pysoem.pyx":391
  *     def _get_slave(self, int pos):
  *         if pos < 0:
  *             raise IndexError('requested slave device is not available')             # <<<<<<<<<<<<<<
  *         if pos >= self._ec_slavecount:
  *             raise IndexError('requested slave device is not available')
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_requested_slave_device_is_not_av); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_requested_slave_device_is_not_av); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20191,22 +20293,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "pysoem/pysoem.pyx":909
+  /* "pysoem/pysoem.pyx":916
  *         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
  *         self._fpwr(wd_type_to_reg_map[wd_type],
  *                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),             # <<<<<<<<<<<<<<
  *                    fprd_fpwr_timeout_us)
  * 
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 909, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_int_2); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 916, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._ec_slave,self._ecx_contextt,self._ex_odlist,self._the_masters_settings cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -20265,158 +20367,158 @@
   __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_169519306, __pyx_int_9788398, __pyx_int_58968170); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
   __pyx_tuple__14 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "pysoem/pysoem.pyx":78
+  /* "pysoem/pysoem.pyx":85
  *     int* sdo_write_timeout
  * 
  * def find_adapters():             # <<<<<<<<<<<<<<
  *     """Create a list of available network adapters.
  * 
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_ec_adapter, __pyx_n_s_Adapter, __pyx_n_s_adapters); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_ec_adapter, __pyx_n_s_Adapter, __pyx_n_s_adapters); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_find_adapters, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_find_adapters, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":95
+  /* "pysoem/pysoem.pyx":102
  * 
  * @contextlib.contextmanager
  * def open(ifname):             # <<<<<<<<<<<<<<
  *     """Context manager function to create a Master object.
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_ifname, __pyx_n_s_master); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_ifname, __pyx_n_s_master); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_open, 95, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_open, 102, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 102, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":106
+  /* "pysoem/pysoem.pyx":113
  * 
  * 
  * def al_status_code_to_string(code):             # <<<<<<<<<<<<<<
  *     """Look up text string that belongs to AL status code.
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_code); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_code); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_al_status_code_to_string, 106, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_al_status_code_to_string, 113, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 113, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":441
+  /* "pysoem/pysoem.pyx":448
  *     """
  * 
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.index = index
  */
-  __pyx_tuple__20 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_index, __pyx_n_s_subindex, __pyx_n_s_abort_code, __pyx_n_s_desc); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_index, __pyx_n_s_subindex, __pyx_n_s_abort_code, __pyx_n_s_desc); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 441, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 448, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 448, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":460
+  /* "pysoem/pysoem.pyx":467
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code, __pyx_n_s_error_reg, __pyx_n_s_b1, __pyx_n_s_w1, __pyx_n_s_w2); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code, __pyx_n_s_error_reg, __pyx_n_s_b1, __pyx_n_s_w1, __pyx_n_s_w2); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(7, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(7, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 467, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 467, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":476
+  /* "pysoem/pysoem.pyx":483
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 476, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 483, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 483, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":489
+  /* "pysoem/pysoem.pyx":496
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code, __pyx_n_s_desc); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code, __pyx_n_s_desc); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 489, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 496, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 496, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":511
+  /* "pysoem/pysoem.pyx":518
  *     }
  * 
  *     def __init__(self, slave_pos, error_code):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_slave_pos, __pyx_n_s_error_code); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 511, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 518, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 518, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":515
+  /* "pysoem/pysoem.pyx":522
  *         self.error_code = error_code
  * 
  *     def _get_desc(self):             # <<<<<<<<<<<<<<
  *         return self._code_desc[self.error_code]
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_get_desc, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_get_desc, 522, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 522, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":528
+  /* "pysoem/pysoem.pyx":535
  *     """
  * 
  *     def __init__(self, error_list):             # <<<<<<<<<<<<<<
  *         self.error_list = error_list
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_error_list); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_error_list); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 528, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 535, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 535, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":539
+  /* "pysoem/pysoem.pyx":546
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 539, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 546, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 546, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":550
+  /* "pysoem/pysoem.pyx":557
  *     """
  * 
  *     def __init__(self, message=None):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_message); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 550, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 550, __pyx_L1_error)
-  __pyx_tuple__38 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pysoem_pysoem_pyx, __pyx_n_s_init, 557, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle__CallbackData(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -20490,22 +20592,25 @@
   __pyx_umethod_PyDict_Type_keys.type = (PyObject*)&PyDict_Type;
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1000000_0 = PyFloat_FromDouble(1000000.0); if (unlikely(!__pyx_float_1000000_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_11 = PyInt_FromLong(11); if (unlikely(!__pyx_int_11)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_20 = PyInt_FromLong(20); if (unlikely(!__pyx_int_20)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_22 = PyInt_FromLong(22); if (unlikely(!__pyx_int_22)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_24 = PyInt_FromLong(24); if (unlikely(!__pyx_int_24)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_26 = PyInt_FromLong(26); if (unlikely(!__pyx_int_26)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_28 = PyInt_FromLong(28); if (unlikely(!__pyx_int_28)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_40 = PyInt_FromLong(40); if (unlikely(!__pyx_int_40)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_500 = PyInt_FromLong(500); if (unlikely(!__pyx_int_500)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1024 = PyInt_FromLong(1024); if (unlikely(!__pyx_int_1024)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1040 = PyInt_FromLong(1040); if (unlikely(!__pyx_int_1040)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1056 = PyInt_FromLong(1056); if (unlikely(!__pyx_int_1056)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2000 = PyInt_FromLong(2000); if (unlikely(!__pyx_int_2000)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2048 = PyInt_FromLong(2048); if (unlikely(!__pyx_int_2048)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20562,68 +20667,68 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem_CdefMaster.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem_CdefMaster.tp_dictoffset && __pyx_type_6pysoem_6pysoem_CdefMaster.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem_CdefMaster.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefMaster, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefMaster, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefMaster) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __pyx_ptype_6pysoem_6pysoem_CdefMaster = &__pyx_type_6pysoem_6pysoem_CdefMaster;
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem__CallbackData.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem__CallbackData.tp_dictoffset && __pyx_type_6pysoem_6pysoem__CallbackData.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem__CallbackData.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CallbackData, (PyObject *)&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 554, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CallbackData, (PyObject *)&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem__CallbackData) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
   __pyx_ptype_6pysoem_6pysoem__CallbackData = &__pyx_type_6pysoem_6pysoem__CallbackData;
   __pyx_vtabptr_6pysoem_6pysoem_CdefSlave = &__pyx_vtable_6pysoem_6pysoem_CdefSlave;
   __pyx_vtable_6pysoem_6pysoem_CdefSlave._raise_exception = (PyObject *(*)(struct __pyx_obj_6pysoem_6pysoem_CdefSlave *, ec_errort *))__pyx_f_6pysoem_6pysoem_9CdefSlave__raise_exception;
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem_CdefSlave.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem_CdefSlave.tp_dictoffset && __pyx_type_6pysoem_6pysoem_CdefSlave.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem_CdefSlave.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6pysoem_6pysoem_CdefSlave.tp_dict, __pyx_vtabptr_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefSlave, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6pysoem_6pysoem_CdefSlave.tp_dict, __pyx_vtabptr_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefSlave, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefSlave) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
   __pyx_ptype_6pysoem_6pysoem_CdefSlave = &__pyx_type_6pysoem_6pysoem_CdefSlave;
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1074, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem_CdefCoeObject.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem_CdefCoeObject.tp_dictoffset && __pyx_type_6pysoem_6pysoem_CdefCoeObject.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem_CdefCoeObject.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefCoeObject, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefCoeObject, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1074, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefCoeObject) < 0) __PYX_ERR(0, 1074, __pyx_L1_error)
   __pyx_ptype_6pysoem_6pysoem_CdefCoeObject = &__pyx_type_6pysoem_6pysoem_CdefCoeObject;
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1144, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1164, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry.tp_dictoffset && __pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefCoeObjectEntry, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1144, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1144, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CdefCoeObjectEntry, (PyObject *)&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1164, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry) < 0) __PYX_ERR(0, 1164, __pyx_L1_error)
   __pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry = &__pyx_type_6pysoem_6pysoem_CdefCoeObjectEntry;
-  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem___pyx_scope_struct__open) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6pysoem_6pysoem___pyx_scope_struct__open) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6pysoem_6pysoem___pyx_scope_struct__open.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6pysoem_6pysoem___pyx_scope_struct__open.tp_dictoffset && __pyx_type_6pysoem_6pysoem___pyx_scope_struct__open.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6pysoem_6pysoem___pyx_scope_struct__open.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6pysoem_6pysoem___pyx_scope_struct__open = &__pyx_type_6pysoem_6pysoem___pyx_scope_struct__open;
@@ -21128,1102 +21233,1156 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_REG_SM0, __pyx_int_2048) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
 
   /* "pysoem/pysoem.pyx":42
  * ECT_REG_WD_TIME_PROCESSDATA = 0x0420
  * ECT_REG_SM0 = 0x0800
  * ECT_REG_SM1 = ECT_REG_SM0 + 0x08             # <<<<<<<<<<<<<<
  * 
- * 
+ * ECT_COEDET_SDO       = 0x01
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ECT_REG_SM0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_8, 0x08, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_REG_SM1, __pyx_t_1) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":78
+  /* "pysoem/pysoem.pyx":44
+ * ECT_REG_SM1 = ECT_REG_SM0 + 0x08
+ * 
+ * ECT_COEDET_SDO       = 0x01             # <<<<<<<<<<<<<<
+ * ECT_COEDET_SDOINFO   = 0x02
+ * ECT_COEDET_PDOASSIGN = 0x04
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_SDO, __pyx_int_1) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":45
+ * 
+ * ECT_COEDET_SDO       = 0x01
+ * ECT_COEDET_SDOINFO   = 0x02             # <<<<<<<<<<<<<<
+ * ECT_COEDET_PDOASSIGN = 0x04
+ * ECT_COEDET_PDOCONFIG = 0x08
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_SDOINFO, __pyx_int_2) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":46
+ * ECT_COEDET_SDO       = 0x01
+ * ECT_COEDET_SDOINFO   = 0x02
+ * ECT_COEDET_PDOASSIGN = 0x04             # <<<<<<<<<<<<<<
+ * ECT_COEDET_PDOCONFIG = 0x08
+ * ECT_COEDET_UPLOAD    = 0x10
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_PDOASSIGN, __pyx_int_4) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":47
+ * ECT_COEDET_SDOINFO   = 0x02
+ * ECT_COEDET_PDOASSIGN = 0x04
+ * ECT_COEDET_PDOCONFIG = 0x08             # <<<<<<<<<<<<<<
+ * ECT_COEDET_UPLOAD    = 0x10
+ * ECT_COEDET_SDOCA     = 0x20
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_PDOCONFIG, __pyx_int_8) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":48
+ * ECT_COEDET_PDOASSIGN = 0x04
+ * ECT_COEDET_PDOCONFIG = 0x08
+ * ECT_COEDET_UPLOAD    = 0x10             # <<<<<<<<<<<<<<
+ * ECT_COEDET_SDOCA     = 0x20
+ * 
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_UPLOAD, __pyx_int_16) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":49
+ * ECT_COEDET_PDOCONFIG = 0x08
+ * ECT_COEDET_UPLOAD    = 0x10
+ * ECT_COEDET_SDOCA     = 0x20             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ECT_COEDET_SDOCA, __pyx_int_32) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+
+  /* "pysoem/pysoem.pyx":85
  *     int* sdo_write_timeout
  * 
  * def find_adapters():             # <<<<<<<<<<<<<<
  *     """Create a list of available network adapters.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_1find_adapters, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_1find_adapters, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_find_adapters, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_find_adapters, __pyx_t_1) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":94
+  /* "pysoem/pysoem.pyx":101
  * 
  * 
  * @contextlib.contextmanager             # <<<<<<<<<<<<<<
  * def open(ifname):
  *     """Context manager function to create a Master object.
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_contextlib); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_contextlib); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_contextmanager); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_contextmanager); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pysoem/pysoem.pyx":95
+  /* "pysoem/pysoem.pyx":102
  * 
  * @contextlib.contextmanager
  * def open(ifname):             # <<<<<<<<<<<<<<
  *     """Context manager function to create a Master object.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_3open, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_3open, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":94
+  /* "pysoem/pysoem.pyx":101
  * 
  * 
  * @contextlib.contextmanager             # <<<<<<<<<<<<<<
  * def open(ifname):
  *     """Context manager function to create a Master object.
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":106
+  /* "pysoem/pysoem.pyx":113
  * 
  * 
  * def al_status_code_to_string(code):             # <<<<<<<<<<<<<<
  *     """Look up text string that belongs to AL status code.
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_6al_status_code_to_string, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_6pysoem_6pysoem_6al_status_code_to_string, NULL, __pyx_n_s_pysoem_pysoem); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_al_status_code_to_string, __pyx_t_2) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_al_status_code_to_string, __pyx_t_2) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":119
+  /* "pysoem/pysoem.pyx":126
  * 
  * 
  * class Master(CdefMaster):             # <<<<<<<<<<<<<<
  *     """Representing a logical EtherCAT master device.
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster));
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_Master, __pyx_n_s_Master, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Representing_a_logical_EtherCAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_Master, __pyx_n_s_Master, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Representing_a_logical_EtherCAT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Master, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_Master, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Master, __pyx_t_4) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Master, __pyx_t_4) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pysoem/pysoem.pyx":169
+  /* "pysoem/pysoem.pyx":176
  *     cdef public int sdo_write_timeout
  * 
  *     state = property(_get_state, _set_state)             # <<<<<<<<<<<<<<
  *     expected_wkc  = property(_get_expected_wkc)
  *     dc_time = property(_get_dc_time)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_set_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_set_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_state, __pyx_t_1) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_state, __pyx_t_1) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefMaster);
 
-  /* "pysoem/pysoem.pyx":170
+  /* "pysoem/pysoem.pyx":177
  * 
  *     state = property(_get_state, _set_state)
  *     expected_wkc  = property(_get_expected_wkc)             # <<<<<<<<<<<<<<
  *     dc_time = property(_get_dc_time)
  *     manual_state_change = property(_get_manual_state_change, _set_manual_state_change)
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_expected_wkc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_expected_wkc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_expected_wkc, __pyx_t_3) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_expected_wkc, __pyx_t_3) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefMaster);
 
-  /* "pysoem/pysoem.pyx":171
+  /* "pysoem/pysoem.pyx":178
  *     state = property(_get_state, _set_state)
  *     expected_wkc  = property(_get_expected_wkc)
  *     dc_time = property(_get_dc_time)             # <<<<<<<<<<<<<<
  *     manual_state_change = property(_get_manual_state_change, _set_manual_state_change)
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_dc_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_dc_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_dc_time, __pyx_t_1) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_dc_time, __pyx_t_1) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefMaster);
 
-  /* "pysoem/pysoem.pyx":172
+  /* "pysoem/pysoem.pyx":179
  *     expected_wkc  = property(_get_expected_wkc)
  *     dc_time = property(_get_dc_time)
  *     manual_state_change = property(_get_manual_state_change, _set_manual_state_change)             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self):
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_manual_state_change); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_get_manual_state_change); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_set_manual_state_change); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster, __pyx_n_s_set_manual_state_change); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_manual_state_change, __pyx_t_3) < 0) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefMaster->tp_dict, __pyx_n_s_manual_state_change, __pyx_t_3) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefMaster);
 
-  /* "pysoem/pysoem.pyx":432
+  /* "pysoem/pysoem.pyx":439
  * 
  * 
  * class SdoError(Exception):             # <<<<<<<<<<<<<<
  *     """Sdo read or write abort
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_SdoError, __pyx_n_s_SdoError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Sdo_read_or_write_abort_Attribut); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_SdoError, __pyx_n_s_SdoError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Sdo_read_or_write_abort_Attribut); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":441
+  /* "pysoem/pysoem.pyx":448
  *     """
  * 
  *     def __init__(self, slave_pos, index, subindex, abort_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.index = index
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_8SdoError_1__init__, 0, __pyx_n_s_SdoError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_8SdoError_1__init__, 0, __pyx_n_s_SdoError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":432
+  /* "pysoem/pysoem.pyx":439
  * 
  * 
  * class SdoError(Exception):             # <<<<<<<<<<<<<<
  *     """Sdo read or write abort
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SdoError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SdoError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SdoError, __pyx_t_4) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SdoError, __pyx_t_4) < 0) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":448
+  /* "pysoem/pysoem.pyx":455
  *         self.desc = desc
  * 
  * class Emergency(Exception):             # <<<<<<<<<<<<<<
  *     """Sdo read or write abort
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_Emergency, __pyx_n_s_Emergency, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Sdo_read_or_write_abort_Attribut_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_Emergency, __pyx_n_s_Emergency, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Sdo_read_or_write_abort_Attribut_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":460
+  /* "pysoem/pysoem.pyx":467
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, error_reg, b1, w1, w2):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_9Emergency_1__init__, 0, __pyx_n_s_Emergency___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_9Emergency_1__init__, 0, __pyx_n_s_Emergency___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":448
+  /* "pysoem/pysoem.pyx":455
  *         self.desc = desc
  * 
  * class Emergency(Exception):             # <<<<<<<<<<<<<<
  *     """Sdo read or write abort
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_Emergency, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_Emergency, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Emergency, __pyx_t_4) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Emergency, __pyx_t_4) < 0) __PYX_ERR(0, 455, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":469
+  /* "pysoem/pysoem.pyx":476
  * 
  * 
  * class SdoInfoError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors during Object directory info read
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_SdoInfoError, __pyx_n_s_SdoInfoError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_during_Object_directory_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_SdoInfoError, __pyx_n_s_SdoInfoError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_during_Object_directory_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":476
+  /* "pysoem/pysoem.pyx":483
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_12SdoInfoError_1__init__, 0, __pyx_n_s_SdoInfoError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_12SdoInfoError_1__init__, 0, __pyx_n_s_SdoInfoError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":469
+  /* "pysoem/pysoem.pyx":476
  * 
  * 
  * class SdoInfoError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors during Object directory info read
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SdoInfoError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SdoInfoError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SdoInfoError, __pyx_t_4) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SdoInfoError, __pyx_t_4) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":480
+  /* "pysoem/pysoem.pyx":487
  * 
  * 
  * class MailboxError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors in mailbox communication
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_MailboxError, __pyx_n_s_MailboxError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_in_mailbox_communication); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_MailboxError, __pyx_n_s_MailboxError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_in_mailbox_communication); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":489
+  /* "pysoem/pysoem.pyx":496
  *     """
  * 
  *     def __init__(self, slave_pos, error_code, desc):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_12MailboxError_1__init__, 0, __pyx_n_s_MailboxError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_12MailboxError_1__init__, 0, __pyx_n_s_MailboxError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":480
+  /* "pysoem/pysoem.pyx":487
  * 
  * 
  * class MailboxError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors in mailbox communication
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_MailboxError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_MailboxError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MailboxError, __pyx_t_4) < 0) __PYX_ERR(0, 480, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MailboxError, __pyx_t_4) < 0) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":495
+  /* "pysoem/pysoem.pyx":502
  * 
  * 
  * class PacketError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors related to mailbox communication
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_PacketError, __pyx_n_s_PacketError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_related_to_mailbox_commun); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_PacketError, __pyx_n_s_PacketError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_related_to_mailbox_commun); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":507
+  /* "pysoem/pysoem.pyx":514
  *     # based on the comments in the soem code
  *     _code_desc = {
  *       1: 'Unexpected frame returned',             # <<<<<<<<<<<<<<
  *       3: 'Data container too small for type',
  *     }
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_int_1, __pyx_kp_s_Unexpected_frame_returned) < 0) __PYX_ERR(0, 507, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_int_3, __pyx_kp_s_Data_container_too_small_for_typ) < 0) __PYX_ERR(0, 507, __pyx_L1_error)
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_code_desc, __pyx_t_4) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_int_1, __pyx_kp_s_Unexpected_frame_returned) < 0) __PYX_ERR(0, 514, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_int_3, __pyx_kp_s_Data_container_too_small_for_typ) < 0) __PYX_ERR(0, 514, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_code_desc, __pyx_t_4) < 0) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":511
+  /* "pysoem/pysoem.pyx":518
  *     }
  * 
  *     def __init__(self, slave_pos, error_code):             # <<<<<<<<<<<<<<
  *         self.slave_pos = slave_pos
  *         self.error_code = error_code
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11PacketError_1__init__, 0, __pyx_n_s_PacketError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11PacketError_1__init__, 0, __pyx_n_s_PacketError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 511, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":515
+  /* "pysoem/pysoem.pyx":522
  *         self.error_code = error_code
  * 
  *     def _get_desc(self):             # <<<<<<<<<<<<<<
  *         return self._code_desc[self.error_code]
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11PacketError_3_get_desc, 0, __pyx_n_s_PacketError__get_desc, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11PacketError_3_get_desc, 0, __pyx_n_s_PacketError__get_desc, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_desc, __pyx_t_4) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_desc, __pyx_t_4) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pysoem/pysoem.pyx":518
+  /* "pysoem/pysoem.pyx":525
  *         return self._code_desc[self.error_code]
  * 
  *     desc = property(_get_desc)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = PyObject_GetItem(__pyx_t_1, __pyx_n_s_get_desc);
   if (unlikely(!__pyx_t_4)) {
     PyErr_Clear();
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_get_desc);
   }
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_desc, __pyx_t_5) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_desc, __pyx_t_5) < 0) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pysoem/pysoem.pyx":495
+  /* "pysoem/pysoem.pyx":502
  * 
  * 
  * class PacketError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors related to mailbox communication
  * 
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_PacketError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_PacketError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PacketError, __pyx_t_5) < 0) __PYX_ERR(0, 495, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PacketError, __pyx_t_5) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":521
+  /* "pysoem/pysoem.pyx":528
  * 
  * 
  * class ConfigMapError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors during Object directory info read
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_ConfigMapError, __pyx_n_s_ConfigMapError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_during_Object_directory_i_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_ConfigMapError, __pyx_n_s_ConfigMapError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Errors_during_Object_directory_i_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":528
+  /* "pysoem/pysoem.pyx":535
  *     """
  * 
  *     def __init__(self, error_list):             # <<<<<<<<<<<<<<
  *         self.error_list = error_list
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_14ConfigMapError_1__init__, 0, __pyx_n_s_ConfigMapError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_14ConfigMapError_1__init__, 0, __pyx_n_s_ConfigMapError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pysoem/pysoem.pyx":521
+  /* "pysoem/pysoem.pyx":528
  * 
  * 
  * class ConfigMapError(Exception):             # <<<<<<<<<<<<<<
  *     """Errors during Object directory info read
  * 
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_ConfigMapError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_ConfigMapError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ConfigMapError, __pyx_t_5) < 0) __PYX_ERR(0, 521, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ConfigMapError, __pyx_t_5) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":532
+  /* "pysoem/pysoem.pyx":539
  * 
  * 
  * class EepromError(Exception):             # <<<<<<<<<<<<<<
  *     """EEPROM access error
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_EepromError, __pyx_n_s_EepromError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_EEPROM_access_error_Attributes_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_EepromError, __pyx_n_s_EepromError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_EEPROM_access_error_Attributes_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":539
+  /* "pysoem/pysoem.pyx":546
  *     """
  * 
  *     def __init__(self, message):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11EepromError_1__init__, 0, __pyx_n_s_EepromError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_11EepromError_1__init__, 0, __pyx_n_s_EepromError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pysoem/pysoem.pyx":532
+  /* "pysoem/pysoem.pyx":539
  * 
  * 
  * class EepromError(Exception):             # <<<<<<<<<<<<<<
  *     """EEPROM access error
  * 
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_EepromError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_EepromError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EepromError, __pyx_t_5) < 0) __PYX_ERR(0, 532, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_EepromError, __pyx_t_5) < 0) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":543
+  /* "pysoem/pysoem.pyx":550
  * 
  * 
  * class WkcError(Exception):             # <<<<<<<<<<<<<<
  *     """Working counter error.
  * 
  */
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_WkcError, __pyx_n_s_WkcError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Working_counter_error_Attributes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_WkcError, __pyx_n_s_WkcError, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Working_counter_error_Attributes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pysoem/pysoem.pyx":550
+  /* "pysoem/pysoem.pyx":557
  *     """
  * 
  *     def __init__(self, message=None):             # <<<<<<<<<<<<<<
  *         self.message = message
  * 
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_8WkcError_1__init__, 0, __pyx_n_s_WkcError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6pysoem_6pysoem_8WkcError_1__init__, 0, __pyx_n_s_WkcError___init, NULL, __pyx_n_s_pysoem_pysoem, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__38);
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 550, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pysoem/pysoem.pyx":543
+  /* "pysoem/pysoem.pyx":550
  * 
  * 
  * class WkcError(Exception):             # <<<<<<<<<<<<<<
  *     """Working counter error.
  * 
  */
-  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_WkcError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_WkcError, __pyx_t_3, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WkcError, __pyx_t_5) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WkcError, __pyx_t_5) < 0) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":562
+  /* "pysoem/pysoem.pyx":569
  * 
  * 
  * class SiiOffset:             # <<<<<<<<<<<<<<
  *     """Item offsets in SII general section."""
  *     # Took it from ethercattype.h but no type was given.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SiiOffset, __pyx_n_s_SiiOffset, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Item_offsets_in_SII_general_sect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SiiOffset, __pyx_n_s_SiiOffset, (PyObject *) NULL, __pyx_n_s_pysoem_pysoem, __pyx_kp_s_Item_offsets_in_SII_general_sect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pysoem/pysoem.pyx":565
+  /* "pysoem/pysoem.pyx":572
  *     """Item offsets in SII general section."""
  *     # Took it from ethercattype.h but no type was given.
  *     MAN = 0x0008             # <<<<<<<<<<<<<<
  *     ID = 0x000A
  *     REV = 0x000B
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_MAN, __pyx_int_8) < 0) __PYX_ERR(0, 565, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_MAN, __pyx_int_8) < 0) __PYX_ERR(0, 572, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":566
+  /* "pysoem/pysoem.pyx":573
  *     # Took it from ethercattype.h but no type was given.
  *     MAN = 0x0008
  *     ID = 0x000A             # <<<<<<<<<<<<<<
  *     REV = 0x000B
  *     BOOT_RX_MBX = 0x0014
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_ID, __pyx_int_10) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_ID, __pyx_int_10) < 0) __PYX_ERR(0, 573, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":567
+  /* "pysoem/pysoem.pyx":574
  *     MAN = 0x0008
  *     ID = 0x000A
  *     REV = 0x000B             # <<<<<<<<<<<<<<
  *     BOOT_RX_MBX = 0x0014
  *     BOOT_TX_MBX = 0x0016
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_REV, __pyx_int_11) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_REV, __pyx_int_11) < 0) __PYX_ERR(0, 574, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":568
+  /* "pysoem/pysoem.pyx":575
  *     ID = 0x000A
  *     REV = 0x000B
  *     BOOT_RX_MBX = 0x0014             # <<<<<<<<<<<<<<
  *     BOOT_TX_MBX = 0x0016
  *     STD_RX_MBX = 0x0018
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_BOOT_RX_MBX, __pyx_int_20) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_BOOT_RX_MBX, __pyx_int_20) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":569
+  /* "pysoem/pysoem.pyx":576
  *     REV = 0x000B
  *     BOOT_RX_MBX = 0x0014
  *     BOOT_TX_MBX = 0x0016             # <<<<<<<<<<<<<<
  *     STD_RX_MBX = 0x0018
  *     STD_TX_MBX = 0x001A
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_BOOT_TX_MBX, __pyx_int_22) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_BOOT_TX_MBX, __pyx_int_22) < 0) __PYX_ERR(0, 576, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":570
+  /* "pysoem/pysoem.pyx":577
  *     BOOT_RX_MBX = 0x0014
  *     BOOT_TX_MBX = 0x0016
  *     STD_RX_MBX = 0x0018             # <<<<<<<<<<<<<<
  *     STD_TX_MBX = 0x001A
  *     MBX_PROTO = 0x001C
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_STD_RX_MBX, __pyx_int_24) < 0) __PYX_ERR(0, 570, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_STD_RX_MBX, __pyx_int_24) < 0) __PYX_ERR(0, 577, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":571
+  /* "pysoem/pysoem.pyx":578
  *     BOOT_TX_MBX = 0x0016
  *     STD_RX_MBX = 0x0018
  *     STD_TX_MBX = 0x001A             # <<<<<<<<<<<<<<
  *     MBX_PROTO = 0x001C
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_STD_TX_MBX, __pyx_int_26) < 0) __PYX_ERR(0, 571, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_STD_TX_MBX, __pyx_int_26) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":572
+  /* "pysoem/pysoem.pyx":579
  *     STD_RX_MBX = 0x0018
  *     STD_TX_MBX = 0x001A
  *     MBX_PROTO = 0x001C             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_MBX_PROTO, __pyx_int_28) < 0) __PYX_ERR(0, 572, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_MBX_PROTO, __pyx_int_28) < 0) __PYX_ERR(0, 579, __pyx_L1_error)
 
-  /* "pysoem/pysoem.pyx":562
+  /* "pysoem/pysoem.pyx":569
  * 
  * 
  * class SiiOffset:             # <<<<<<<<<<<<<<
  *     """Item offsets in SII general section."""
  *     # Took it from ethercattype.h but no type was given.
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SiiOffset, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_SiiOffset, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SiiOffset, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SiiOffset, __pyx_t_2) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pysoem/pysoem.pyx":593
+  /* "pysoem/pysoem.pyx":600
  *     cdef cpysoem.ec_ODlistt _ex_odlist
  * 
  *     name = property(_get_name)             # <<<<<<<<<<<<<<
  *     man = property(_get_eep_man)
  *     id = property(_get_eep_id)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 593, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":594
+  /* "pysoem/pysoem.pyx":601
  * 
  *     name = property(_get_name)
  *     man = property(_get_eep_man)             # <<<<<<<<<<<<<<
  *     id = property(_get_eep_id)
  *     rev = property(_get_eep_rev)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_man); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_man); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_man, __pyx_t_3) < 0) __PYX_ERR(0, 594, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_man, __pyx_t_3) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":595
+  /* "pysoem/pysoem.pyx":602
  *     name = property(_get_name)
  *     man = property(_get_eep_man)
  *     id = property(_get_eep_id)             # <<<<<<<<<<<<<<
  *     rev = property(_get_eep_rev)
  *     config_func = property(_get_PO2SOconfig, _set_PO2SOconfig)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_id, __pyx_t_2) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_id, __pyx_t_2) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":596
+  /* "pysoem/pysoem.pyx":603
  *     man = property(_get_eep_man)
  *     id = property(_get_eep_id)
  *     rev = property(_get_eep_rev)             # <<<<<<<<<<<<<<
  *     config_func = property(_get_PO2SOconfig, _set_PO2SOconfig)
  *     setup_func = property(_get_PO2SOconfigEx, _set_PO2SOconfigEx)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_rev); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_eep_rev); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_rev, __pyx_t_3) < 0) __PYX_ERR(0, 596, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_rev, __pyx_t_3) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":597
+  /* "pysoem/pysoem.pyx":604
  *     id = property(_get_eep_id)
  *     rev = property(_get_eep_rev)
  *     config_func = property(_get_PO2SOconfig, _set_PO2SOconfig)             # <<<<<<<<<<<<<<
  *     setup_func = property(_get_PO2SOconfigEx, _set_PO2SOconfigEx)
  *     state = property(_get_state, _set_state)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_PO2SOconfig); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_PO2SOconfig); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_PO2SOconfig); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_PO2SOconfig); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 597, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_config_func, __pyx_t_2) < 0) __PYX_ERR(0, 597, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_config_func, __pyx_t_2) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":598
+  /* "pysoem/pysoem.pyx":605
  *     rev = property(_get_eep_rev)
  *     config_func = property(_get_PO2SOconfig, _set_PO2SOconfig)
  *     setup_func = property(_get_PO2SOconfigEx, _set_PO2SOconfigEx)             # <<<<<<<<<<<<<<
  *     state = property(_get_state, _set_state)
  *     input = property(_get_input)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_PO2SOconfigEx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_PO2SOconfigEx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_PO2SOconfigEx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_PO2SOconfigEx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_setup_func, __pyx_t_1) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_setup_func, __pyx_t_1) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":599
+  /* "pysoem/pysoem.pyx":606
  *     config_func = property(_get_PO2SOconfig, _set_PO2SOconfig)
  *     setup_func = property(_get_PO2SOconfigEx, _set_PO2SOconfigEx)
  *     state = property(_get_state, _set_state)             # <<<<<<<<<<<<<<
  *     input = property(_get_input)
  *     output = property(_get_output, _set_output)
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":600
+  /* "pysoem/pysoem.pyx":607
  *     setup_func = property(_get_PO2SOconfigEx, _set_PO2SOconfigEx)
  *     state = property(_get_state, _set_state)
  *     input = property(_get_input)             # <<<<<<<<<<<<<<
  *     output = property(_get_output, _set_output)
  *     al_status = property(_get_al_status)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_input); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_input, __pyx_t_2) < 0) __PYX_ERR(0, 600, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_input, __pyx_t_2) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":601
+  /* "pysoem/pysoem.pyx":608
  *     state = property(_get_state, _set_state)
  *     input = property(_get_input)
  *     output = property(_get_output, _set_output)             # <<<<<<<<<<<<<<
  *     al_status = property(_get_al_status)
  *     is_lost = property(_get_is_lost, _set_is_lost)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_output); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_output); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_output); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_output); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_output, __pyx_t_3) < 0) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_output, __pyx_t_3) < 0) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":602
+  /* "pysoem/pysoem.pyx":609
  *     input = property(_get_input)
  *     output = property(_get_output, _set_output)
  *     al_status = property(_get_al_status)             # <<<<<<<<<<<<<<
  *     is_lost = property(_get_is_lost, _set_is_lost)
  *     od = property(_get_od)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_al_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_al_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_al_status, __pyx_t_1) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_al_status, __pyx_t_1) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":603
+  /* "pysoem/pysoem.pyx":610
  *     output = property(_get_output, _set_output)
  *     al_status = property(_get_al_status)
  *     is_lost = property(_get_is_lost, _set_is_lost)             # <<<<<<<<<<<<<<
  *     od = property(_get_od)
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_is_lost); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_is_lost); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_is_lost); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_set_is_lost); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_property, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_is_lost, __pyx_t_3) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_is_lost, __pyx_t_3) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":604
+  /* "pysoem/pysoem.pyx":611
  *     al_status = property(_get_al_status)
  *     is_lost = property(_get_is_lost, _set_is_lost)
  *     od = property(_get_od)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, pos):
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_od); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave, __pyx_n_s_get_od); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_od, __pyx_t_2) < 0) __PYX_ERR(0, 604, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefSlave->tp_dict, __pyx_n_s_od, __pyx_t_2) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefSlave);
 
-  /* "pysoem/pysoem.pyx":1066
+  /* "pysoem/pysoem.pyx":1086
  *     cdef cpysoem.ec_OElistt _ex_oelist
  * 
  *     index = property(_get_index)             # <<<<<<<<<<<<<<
  *     data_type = property(_get_data_type)
  *     name = property(_get_name)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1066, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1086, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1066, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1086, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_index, __pyx_t_3) < 0) __PYX_ERR(0, 1066, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_index, __pyx_t_3) < 0) __PYX_ERR(0, 1086, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1067
+  /* "pysoem/pysoem.pyx":1087
  * 
  *     index = property(_get_index)
  *     data_type = property(_get_data_type)             # <<<<<<<<<<<<<<
  *     name = property(_get_name)
  *     object_code = property(_get_object_code)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_data_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1067, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_data_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1087, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1067, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1087, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 1067, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 1087, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1068
+  /* "pysoem/pysoem.pyx":1088
  *     index = property(_get_index)
  *     data_type = property(_get_data_type)
  *     name = property(_get_name)             # <<<<<<<<<<<<<<
  *     object_code = property(_get_object_code)
  *     entries = property(_get_entries)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1068, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1068, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_name, __pyx_t_3) < 0) __PYX_ERR(0, 1068, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_name, __pyx_t_3) < 0) __PYX_ERR(0, 1088, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1069
+  /* "pysoem/pysoem.pyx":1089
  *     data_type = property(_get_data_type)
  *     name = property(_get_name)
  *     object_code = property(_get_object_code)             # <<<<<<<<<<<<<<
  *     entries = property(_get_entries)
  *     bit_length = property(_get_bit_length)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_object_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1069, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_object_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1089, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1069, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1089, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_object_code, __pyx_t_2) < 0) __PYX_ERR(0, 1069, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_object_code, __pyx_t_2) < 0) __PYX_ERR(0, 1089, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1070
+  /* "pysoem/pysoem.pyx":1090
  *     name = property(_get_name)
  *     object_code = property(_get_object_code)
  *     entries = property(_get_entries)             # <<<<<<<<<<<<<<
  *     bit_length = property(_get_bit_length)
  *     obj_access = property(_get_obj_access)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1070, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_entries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1070, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_entries, __pyx_t_3) < 0) __PYX_ERR(0, 1070, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_entries, __pyx_t_3) < 0) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1071
+  /* "pysoem/pysoem.pyx":1091
  *     object_code = property(_get_object_code)
  *     entries = property(_get_entries)
  *     bit_length = property(_get_bit_length)             # <<<<<<<<<<<<<<
  *     obj_access = property(_get_obj_access)
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_bit_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1071, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_bit_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1071, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_bit_length, __pyx_t_2) < 0) __PYX_ERR(0, 1071, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_bit_length, __pyx_t_2) < 0) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1072
+  /* "pysoem/pysoem.pyx":1092
  *     entries = property(_get_entries)
  *     bit_length = property(_get_bit_length)
  *     obj_access = property(_get_obj_access)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, int item):
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_obj_access); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1072, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject, __pyx_n_s_get_obj_access); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1092, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1072, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1092, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_obj_access, __pyx_t_3) < 0) __PYX_ERR(0, 1072, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObject->tp_dict, __pyx_n_s_obj_access, __pyx_t_3) < 0) __PYX_ERR(0, 1092, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObject);
 
-  /* "pysoem/pysoem.pyx":1148
+  /* "pysoem/pysoem.pyx":1168
  *     cdef int _item
  * 
  *     name = property(_get_name)             # <<<<<<<<<<<<<<
  *     data_type = property(_get_data_type)
  *     bit_length = property(_get_bit_length)
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1148, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 1148, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 1168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry);
 
-  /* "pysoem/pysoem.pyx":1149
+  /* "pysoem/pysoem.pyx":1169
  * 
  *     name = property(_get_name)
  *     data_type = property(_get_data_type)             # <<<<<<<<<<<<<<
  *     bit_length = property(_get_bit_length)
  *     obj_access = property(_get_obj_access)
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1149, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1149, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_data_type, __pyx_t_3) < 0) __PYX_ERR(0, 1149, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_data_type, __pyx_t_3) < 0) __PYX_ERR(0, 1169, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry);
 
-  /* "pysoem/pysoem.pyx":1150
+  /* "pysoem/pysoem.pyx":1170
  *     name = property(_get_name)
  *     data_type = property(_get_data_type)
  *     bit_length = property(_get_bit_length)             # <<<<<<<<<<<<<<
  *     obj_access = property(_get_obj_access)
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_bit_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1150, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_bit_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1150, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_bit_length, __pyx_t_2) < 0) __PYX_ERR(0, 1150, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_bit_length, __pyx_t_2) < 0) __PYX_ERR(0, 1170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry);
 
-  /* "pysoem/pysoem.pyx":1151
+  /* "pysoem/pysoem.pyx":1171
  *     data_type = property(_get_data_type)
  *     bit_length = property(_get_bit_length)
  *     obj_access = property(_get_obj_access)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, int item):
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_obj_access); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1151, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry, __pyx_n_s_get_obj_access); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1151, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_obj_access, __pyx_t_3) < 0) __PYX_ERR(0, 1151, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry->tp_dict, __pyx_n_s_obj_access, __pyx_t_3) < 0) __PYX_ERR(0, 1171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_6pysoem_6pysoem_CdefCoeObjectEntry);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle__CallbackData(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
```

### Comparing `pysoem-1.1.2/pysoem/pysoem.pyx` & `pysoem-1.1.3/pysoem/pysoem.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 
 ECT_REG_WD_DIV = 0x0400
 ECT_REG_WD_TIME_PDI = 0x0410
 ECT_REG_WD_TIME_PROCESSDATA = 0x0420
 ECT_REG_SM0 = 0x0800
 ECT_REG_SM1 = ECT_REG_SM0 + 0x08
 
+ECT_COEDET_SDO       = 0x01
+ECT_COEDET_SDOINFO   = 0x02
+ECT_COEDET_PDOASSIGN = 0x04
+ECT_COEDET_PDOCONFIG = 0x08
+ECT_COEDET_UPLOAD    = 0x10
+ECT_COEDET_SDOCA     = 0x20
+
 
 cpdef enum ec_datatype:
     ECT_BOOLEAN         = 0x0001,
     ECT_INTEGER8        = 0x0002,
     ECT_INTEGER16       = 0x0003,
     ECT_INTEGER32       = 0x0004,
     ECT_UNSIGNED8       = 0x0005,
@@ -905,14 +912,27 @@
             wd_time_ms_limit = 0xFFFF * wd_div_ns / 1000000.0
             raise AttributeError('wd_time_ms is limited to {} ms'.format(wd_time_ms_limit))
         actual_wd_time_ms = wd_time_reg * wd_div_ns / 1000000.0
         self._fpwr(wd_type_to_reg_map[wd_type],
                    wd_time_reg.to_bytes(2, byteorder='little', signed=False),
                    fprd_fpwr_timeout_us)
 
+    def _disable_complete_access(self):
+        """Helper function that stops config_map() from using "complete access" for SDO requests for this device.
+
+        This should only be used if your device has issues handling complete access requests but the CoE details of the
+        SII tells that SDO complete access is supported by the device. If you need this function something is wrong
+        with your device and you should contact the manufacturer about this issue.
+
+        .. warning:: This is experimental.
+
+        .. versionadded:: 1.1.3
+        """
+        self._ec_slave.CoEdetails &= ~ECT_COEDET_SDOCA
+
     def _fprd(self, int address, int size, timeout_us=2000):
         """Send and receive of the FPRD cmd primitive (Configured Address Physical Read)."""
         cdef unsigned char* data
         data = <unsigned char*>PyMem_Malloc(size)
         cdef int wkc = cpysoem.ecx_FPRD(self._ecx_contextt.port, self._ec_slave.configadr, address, size, data, timeout_us)
         if wkc != 1:
             PyMem_Free(data)
```

### Comparing `pysoem-1.1.2/pysoem.egg-info/PKG-INFO` & `pysoem-1.1.3/pysoem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoem
-Version: 1.1.2
+Version: 1.1.3
 Summary: Cython wrapper for the SOEM Library
 Home-page: https://github.com/bnjmnp/pysoem
 Author: Benjamin Partzsch
 Author-email: benjamin_partzsch@web.de
 License: MIT
 Project-URL: Documentation, https://pysoem.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,14 +86,18 @@
 Let's discuss any (major) API change, or large piles of new code first.
 Using `this pysoem chat room on gitter <https://gitter.im/pysoem/pysoem>`_ is one communication channel option.
 
 
 Changes
 -------
 
+v1.1.3
+^^^^^^^
+* Adds function ``_disable_complete_access()`` that stops config_map() from using "complete access" for SDO requests.
+
 v1.1.0
 ^^^^^^^
 * Changed the data type for the ``name`` attribute of SDO info CdefCoeObject and CdefCoeObjectEntry, they are of type bytes now instead of a regular Python 3 string.
 * Also changed the ``desc`` attribute of the ``find_adapters()`` list elements to ``bytes``.
 * Introduces the ``open()`` context manager function.
 * Adds the ``setup_func`` that will maybe later replace the ``config_func``.
```

### Comparing `pysoem-1.1.2/pysoem.egg-info/SOURCES.txt` & `pysoem-1.1.3/pysoem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/setup.py` & `pysoem-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/erika/osal.c` & `pysoem-1.1.3/soem/osal/erika/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/erika/osal_defs.h` & `pysoem-1.1.3/soem/osal/erika/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/intime/osal.c` & `pysoem-1.1.3/soem/osal/intime/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/intime/osal_defs.h` & `pysoem-1.1.3/soem/osal/intime/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/linux/osal.c` & `pysoem-1.1.3/soem/osal/linux/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/linux/osal_defs.h` & `pysoem-1.1.3/soem/osal/linux/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/macosx/osal.c` & `pysoem-1.1.3/soem/osal/macosx/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/macosx/osal_defs.h` & `pysoem-1.1.3/soem/osal/macosx/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/osal.h` & `pysoem-1.1.3/soem/osal/osal.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/rtems/osal.c` & `pysoem-1.1.3/soem/osal/rtems/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/rtems/osal_defs.h` & `pysoem-1.1.3/soem/osal/rtems/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/rtk/osal.c` & `pysoem-1.1.3/soem/osal/rtk/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/rtk/osal_defs.h` & `pysoem-1.1.3/soem/osal/rtk/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/vxworks/osal.c` & `pysoem-1.1.3/soem/osal/vxworks/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/vxworks/osal_defs.h` & `pysoem-1.1.3/soem/osal/vxworks/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/win32/inttypes.h` & `pysoem-1.1.3/soem/osal/win32/inttypes.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/win32/osal.c` & `pysoem-1.1.3/soem/osal/win32/osal.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/win32/osal_defs.h` & `pysoem-1.1.3/soem/osal/win32/osal_defs.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/win32/osal_win32.h` & `pysoem-1.1.3/soem/osal/win32/osal_win32.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/osal/win32/stdint.h` & `pysoem-1.1.3/soem/osal/win32/stdint.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/erika/nicdrv.c` & `pysoem-1.1.3/soem/oshw/erika/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/erika/nicdrv.h` & `pysoem-1.1.3/soem/oshw/erika/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/erika/oshw.c` & `pysoem-1.1.3/soem/oshw/erika/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/erika/oshw.h` & `pysoem-1.1.3/soem/oshw/erika/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/intime/nicdrv.c` & `pysoem-1.1.3/soem/oshw/intime/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/intime/nicdrv.h` & `pysoem-1.1.3/soem/oshw/intime/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/intime/oshw.c` & `pysoem-1.1.3/soem/oshw/intime/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/intime/oshw.h` & `pysoem-1.1.3/soem/oshw/intime/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/linux/nicdrv.c` & `pysoem-1.1.3/soem/oshw/linux/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/linux/nicdrv.h` & `pysoem-1.1.3/soem/oshw/linux/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/linux/oshw.c` & `pysoem-1.1.3/soem/oshw/linux/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/linux/oshw.h` & `pysoem-1.1.3/soem/oshw/linux/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/macosx/nicdrv.c` & `pysoem-1.1.3/soem/oshw/macosx/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/macosx/nicdrv.h` & `pysoem-1.1.3/soem/oshw/macosx/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/macosx/oshw.c` & `pysoem-1.1.3/soem/oshw/macosx/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/macosx/oshw.h` & `pysoem-1.1.3/soem/oshw/macosx/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtems/nicdrv.c` & `pysoem-1.1.3/soem/oshw/rtems/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtems/nicdrv.h` & `pysoem-1.1.3/soem/oshw/rtems/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtems/oshw.c` & `pysoem-1.1.3/soem/oshw/rtems/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtems/oshw.h` & `pysoem-1.1.3/soem/oshw/rtems/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.c` & `pysoem-1.1.3/soem/oshw/rtk/fec/fec_ecat.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.h` & `pysoem-1.1.3/soem/oshw/rtk/fec/fec_ecat.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/lw_mac/lw_emac.c` & `pysoem-1.1.3/soem/oshw/rtk/lw_mac/lw_emac.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/nicdrv.c` & `pysoem-1.1.3/soem/oshw/rtk/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/nicdrv.h` & `pysoem-1.1.3/soem/oshw/rtk/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/oshw.c` & `pysoem-1.1.3/soem/oshw/rtk/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/rtk/oshw.h` & `pysoem-1.1.3/soem/oshw/rtk/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/vxworks/nicdrv.c` & `pysoem-1.1.3/soem/oshw/vxworks/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/vxworks/nicdrv.h` & `pysoem-1.1.3/soem/oshw/vxworks/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/vxworks/oshw.c` & `pysoem-1.1.3/soem/oshw/vxworks/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/nicdrv.c` & `pysoem-1.1.3/soem/oshw/win32/nicdrv.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/nicdrv.h` & `pysoem-1.1.3/soem/oshw/win32/nicdrv.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/oshw.c` & `pysoem-1.1.3/soem/oshw/win32/oshw.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/oshw.h` & `pysoem-1.1.3/soem/oshw/win32/oshw.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Packet32.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/Packet32.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Win32-Extensions.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/Win32-Extensions.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/bittypes.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/bittypes.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/ip6_misc.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/ip6_misc.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bluetooth.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/bluetooth.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bpf.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/bpf.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/namedb.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/namedb.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/pcap.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/pcap.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/sll.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/sll.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/usb.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/usb.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/vlan.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap/vlan.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-bpf.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-bpf.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-namedb.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-namedb.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-stdinc.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap-stdinc.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/pcap.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/oshw/win32/wpcap/Include/remote-ext.h` & `pysoem-1.1.3/soem/oshw/win32/wpcap/Include/remote-ext.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercat.h` & `pysoem-1.1.3/soem/soem/ethercat.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatbase.c` & `pysoem-1.1.3/soem/soem/ethercatbase.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatbase.h` & `pysoem-1.1.3/soem/soem/ethercatbase.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatcoe.c` & `pysoem-1.1.3/soem/soem/ethercatcoe.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatcoe.h` & `pysoem-1.1.3/soem/soem/ethercatcoe.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatconfig.c` & `pysoem-1.1.3/soem/soem/ethercatconfig.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatconfig.h` & `pysoem-1.1.3/soem/soem/ethercatconfig.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatconfiglist.h` & `pysoem-1.1.3/soem/soem/ethercatconfiglist.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatdc.c` & `pysoem-1.1.3/soem/soem/ethercatdc.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatdc.h` & `pysoem-1.1.3/soem/soem/ethercatdc.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercateoe.c` & `pysoem-1.1.3/soem/soem/ethercateoe.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercateoe.h` & `pysoem-1.1.3/soem/soem/ethercateoe.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatfoe.c` & `pysoem-1.1.3/soem/soem/ethercatfoe.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatfoe.h` & `pysoem-1.1.3/soem/soem/ethercatfoe.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatmain.c` & `pysoem-1.1.3/soem/soem/ethercatmain.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatmain.h` & `pysoem-1.1.3/soem/soem/ethercatmain.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatprint.c` & `pysoem-1.1.3/soem/soem/ethercatprint.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatprint.h` & `pysoem-1.1.3/soem/soem/ethercatprint.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatsoe.c` & `pysoem-1.1.3/soem/soem/ethercatsoe.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercatsoe.h` & `pysoem-1.1.3/soem/soem/ethercatsoe.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/soem/ethercattype.h` & `pysoem-1.1.3/soem/soem/ethercattype.h`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/intime/ec_master/ec_master.c` & `pysoem-1.1.3/soem/test/intime/ec_master/ec_master.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/aliastool.c` & `pysoem-1.1.3/soem/test/linux/aliastool.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/ebox/ebox.c` & `pysoem-1.1.3/soem/test/linux/ebox/ebox.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/eepromtool/eepromtool.c` & `pysoem-1.1.3/soem/test/linux/eepromtool/eepromtool.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/eoe_test/eoe_test.c` & `pysoem-1.1.3/soem/test/linux/eoe_test/eoe_test.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/firm_update/firm_update.c` & `pysoem-1.1.3/soem/test/linux/firm_update/firm_update.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/red_test/red_test.c` & `pysoem-1.1.3/soem/test/linux/red_test/red_test.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/simple_test/simple_test.c` & `pysoem-1.1.3/soem/test/linux/simple_test/simple_test.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/linux/slaveinfo/slaveinfo.c` & `pysoem-1.1.3/soem/test/linux/slaveinfo/slaveinfo.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/rtk/main.c` & `pysoem-1.1.3/soem/test/rtk/main.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/ebox/ebox.c` & `pysoem-1.1.3/soem/test/win32/ebox/ebox.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/eepromtool/eepromtool.c` & `pysoem-1.1.3/soem/test/win32/eepromtool/eepromtool.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/firm_update/firm_update.c` & `pysoem-1.1.3/soem/test/win32/firm_update/firm_update.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/red_test/red_test.c` & `pysoem-1.1.3/soem/test/win32/red_test/red_test.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/simple_test/simple_test.c` & `pysoem-1.1.3/soem/test/win32/simple_test/simple_test.c`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.2/soem/test/win32/slaveinfo/slaveinfo.c` & `pysoem-1.1.3/soem/test/win32/slaveinfo/slaveinfo.c`

 * *Files identical despite different names*

