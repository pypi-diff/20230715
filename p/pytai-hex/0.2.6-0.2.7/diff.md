# Comparing `tmp/pytai-hex-0.2.6.tar.gz` & `tmp/pytai-hex-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytai-hex-0.2.6.tar", last modified: Fri Jul 22 11:53:48 2022, max compression
+gzip compressed data, was "pytai-hex-0.2.7.tar", last modified: Sat Jul 15 17:39:15 2023, max compression
```

## Comparing `pytai-hex-0.2.6.tar` & `pytai-hex-0.2.7.tar`

### file list

```diff
@@ -1,249 +1,251 @@
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.795738 pytai-hex-0.2.6/
--rwxrwxrwx   0 owner     (1000) owner     (1000)      171 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/.editorconfig
--rwxrwxrwx   0 owner     (1000) owner     (1000)     2219 2022-07-22 11:25:31.000000 pytai-hex-0.2.6/.gitignore
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25727 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/LICENSE
--rwxrwxrwx   0 owner     (1000) owner     (1000)       26 2022-05-27 21:02:32.000000 pytai-hex-0.2.6/MANIFEST.in
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7586 2022-07-22 11:53:48.790715 pytai-hex-0.2.6/PKG-INFO
--rwxrwxrwx   0 owner     (1000) owner     (1000)     6982 2022-06-12 18:45:13.000000 pytai-hex-0.2.6/README.md
--rwxrwxrwx   0 owner     (1000) owner     (1000)     1678 2022-05-27 21:39:57.000000 pytai-hex-0.2.6/__main__.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:46.537367 pytai-hex-0.2.6/docs/
--rwxrwxrwx   0 owner     (1000) owner     (1000)     1779 2022-07-22 11:51:30.000000 pytai-hex-0.2.6/docs/Release_process.md
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:46.581906 pytai-hex-0.2.6/docs/images/
--rwxrwxrwx   0 owner     (1000) owner     (1000)    93738 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/docs/images/mark1.png
--rwxrwxrwx   0 owner     (1000) owner     (1000)    94479 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/docs/images/mark2.png
--rwxrwxrwx   0 owner     (1000) owner     (1000)   102940 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/docs/images/meta.png
--rwxrwxrwx   0 owner     (1000) owner     (1000)    90409 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/docs/images/pytai.png
--rwxrwxrwx   0 owner     (1000) owner     (1000)    83711 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/docs/images/xref.gif
--rwxrwxrwx   0 owner     (1000) owner     (1000)     1180 2022-05-27 21:51:55.000000 pytai-hex-0.2.6/pyproject.toml
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:46.616840 pytai-hex-0.2.6/pytai/
--rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/__init__.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     3071 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/pytai/__main__.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14108 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/application.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     1964 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/common.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:46.632390 pytai-hex-0.2.6/pytai/kaitai/
--rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/kaitai/__init__.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.503053 pytai-hex-0.2.6/pytai/kaitai/formats/
--rwxrwxrwx   0 owner     (1000) owner     (1000)      158 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/README.md
--rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/__init__.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12438 2022-07-22 10:09:37.000000 pytai-hex-0.2.6/pytai/kaitai/formats/aix_utmp.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23433 2022-07-22 10:09:19.000000 pytai-hex-0.2.6/pytai/kaitai/formats/allegro_dat.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10318 2022-07-22 10:09:16.000000 pytai-hex-0.2.6/pytai/kaitai/formats/andes_firmware.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12539 2022-07-22 10:08:51.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_asus.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15589 2022-07-22 10:08:51.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_huawei.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    19266 2022-07-22 10:08:52.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_qcom.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13685 2022-07-22 10:08:52.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_dto.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    20040 2022-07-22 10:08:53.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_img.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14901 2022-07-22 10:09:04.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_nanoapp_header.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18365 2022-07-22 10:09:44.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_opengl_shaders_cache.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18473 2022-07-22 10:08:53.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_sparse.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    29843 2022-07-22 10:09:09.000000 pytai-hex-0.2.6/pytai/kaitai/formats/android_super.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16896 2022-07-22 10:09:10.000000 pytai-hex-0.2.6/pytai/kaitai/formats/apm_partition_table.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14988 2022-07-22 10:09:10.000000 pytai-hex-0.2.6/pytai/kaitai/formats/apple_single_double.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16731 2022-07-22 10:10:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/asn1_der.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12487 2022-07-22 10:09:45.000000 pytai-hex-0.2.6/pytai/kaitai/formats/au.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13012 2022-07-22 10:10:05.000000 pytai-hex-0.2.6/pytai/kaitai/formats/avantes_roh60.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    20839 2022-07-22 10:09:45.000000 pytai-hex-0.2.6/pytai/kaitai/formats/avi.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12621 2022-07-22 10:08:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/bcd.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11800 2022-07-22 10:09:53.000000 pytai-hex-0.2.6/pytai/kaitai/formats/bitcoin_transaction.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23047 2022-07-22 10:09:45.000000 pytai-hex-0.2.6/pytai/kaitai/formats/blender_blend.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    43300 2022-07-22 10:09:28.000000 pytai-hex-0.2.6/pytai/kaitai/formats/bmp.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    26357 2022-07-22 10:10:07.000000 pytai-hex-0.2.6/pytai/kaitai/formats/bson.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    21855 2022-07-22 10:09:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/btrfs_stream.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     2138 2022-07-22 10:08:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/bytes_with_io.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15369 2022-07-22 10:10:08.000000 pytai-hex-0.2.6/pytai/kaitai/formats/chrome_pak.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25021 2022-07-22 10:09:40.000000 pytai-hex-0.2.6/pytai/kaitai/formats/code_6502.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12320 2022-07-22 10:09:40.000000 pytai-hex-0.2.6/pytai/kaitai/formats/compressed_resource.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15223 2022-07-22 10:08:54.000000 pytai-hex-0.2.6/pytai/kaitai/formats/cpio_old_le.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14641 2022-07-22 10:09:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/cramfs.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    22405 2022-07-22 10:09:46.000000 pytai-hex-0.2.6/pytai/kaitai/formats/creative_voice_file.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18886 2022-07-22 10:09:02.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dbf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    34552 2022-07-22 10:09:42.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_0.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    20397 2022-07-22 10:09:43.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_1.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18715 2022-07-22 10:09:43.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_2.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     3651 2022-07-22 10:09:44.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_variable_length_integer.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    59075 2022-07-22 10:09:05.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dex.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)   198109 2022-07-22 10:09:29.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dicom.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16888 2022-07-22 10:09:53.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dime_message.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    30623 2022-07-22 10:09:53.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dns_packet.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    37276 2022-07-22 10:09:19.000000 pytai-hex-0.2.6/pytai/kaitai/formats/doom_wad.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15366 2022-07-22 10:09:00.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dos_datetime.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15322 2022-07-22 10:09:05.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dos_mz.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25258 2022-07-22 10:09:41.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ds_store.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    21032 2022-07-22 10:09:27.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dtb.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11803 2022-07-22 10:09:20.000000 pytai-hex-0.2.6/pytai/kaitai/formats/dune_2_pak.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    28733 2022-07-22 10:09:27.000000 pytai-hex-0.2.6/pytai/kaitai/formats/edid.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    22219 2022-07-22 10:10:06.000000 pytai-hex-0.2.6/pytai/kaitai/formats/efivar_signature_list.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)   110046 2022-07-22 10:09:06.000000 pytai-hex-0.2.6/pytai/kaitai/formats/elf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12320 2022-07-22 10:09:54.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ethernet_frame.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    37278 2022-07-22 10:09:30.000000 pytai-hex-0.2.6/pytai/kaitai/formats/exif.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    33729 2022-07-22 10:09:12.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ext2.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14672 2022-07-22 10:09:20.000000 pytai-hex-0.2.6/pytai/kaitai/formats/fallout2_dat.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14280 2022-07-22 10:09:21.000000 pytai-hex-0.2.6/pytai/kaitai/formats/fallout_dat.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31728 2022-07-22 10:09:52.000000 pytai-hex-0.2.6/pytai/kaitai/formats/fasttracker_xm_module.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10941 2022-07-22 10:09:21.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ftl_dat.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14646 2022-07-22 10:09:46.000000 pytai-hex-0.2.6/pytai/kaitai/formats/genmidi_op2.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    24228 2022-07-22 10:09:03.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gettext_mo.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    28806 2022-07-22 10:09:30.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gif.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18169 2022-07-22 10:09:31.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gimp_brush.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12173 2022-07-22 10:09:37.000000 pytai-hex-0.2.6/pytai/kaitai/formats/glibc_utmp.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     6553 2022-07-22 10:08:51.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gltf_binary.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7614 2022-07-22 10:10:08.000000 pytai-hex-0.2.6/pytai/kaitai/formats/google_protobuf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15337 2022-07-22 10:09:12.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gpt_partition_table.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13151 2022-07-22 10:09:22.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gran_turismo_vol.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    22534 2022-07-22 10:09:17.000000 pytai-hex-0.2.6/pytai/kaitai/formats/grub2_font.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17430 2022-07-22 10:08:54.000000 pytai-hex-0.2.6/pytai/kaitai/formats/gzip.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10130 2022-07-22 10:09:37.000000 pytai-hex-0.2.6/pytai/kaitai/formats/hashcat_restore.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     5996 2022-07-22 10:09:54.000000 pytai-hex-0.2.6/pytai/kaitai/formats/hccap.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     6451 2022-07-22 10:09:55.000000 pytai-hex-0.2.6/pytai/kaitai/formats/hccapx.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9352 2022-07-22 10:09:22.000000 pytai-hex-0.2.6/pytai/kaitai/formats/heaps_pak.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12129 2022-07-22 10:09:22.000000 pytai-hex-0.2.6/pytai/kaitai/formats/heroes_of_might_and_magic_agg.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     8751 2022-07-22 10:09:23.000000 pytai-hex-0.2.6/pytai/kaitai/formats/heroes_of_might_and_magic_bmp.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13279 2022-07-22 10:09:55.000000 pytai-hex-0.2.6/pytai/kaitai/formats/icmp_packet.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13015 2022-07-22 10:09:32.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ico.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14613 2022-07-22 10:09:47.000000 pytai-hex-0.2.6/pytai/kaitai/formats/id3v1_1.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    21643 2022-07-22 10:09:47.000000 pytai-hex-0.2.6/pytai/kaitai/formats/id3v2_3.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    27572 2022-07-22 10:09:48.000000 pytai-hex-0.2.6/pytai/kaitai/formats/id3v2_4.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13249 2022-07-22 10:09:16.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ines.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13681 2022-07-22 10:09:56.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ipv4_packet.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10063 2022-07-22 10:09:56.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ipv6_packet.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    34715 2022-07-22 10:09:13.000000 pytai-hex-0.2.6/pytai/kaitai/formats/iso9660.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    51617 2022-07-22 10:09:06.000000 pytai-hex-0.2.6/pytai/kaitai/formats/java_class.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23440 2022-07-22 10:09:32.000000 pytai-hex-0.2.6/pytai/kaitai/formats/jpeg.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15429 2022-07-22 10:09:13.000000 pytai-hex-0.2.6/pytai/kaitai/formats/luks.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14818 2022-07-22 10:08:55.000000 pytai-hex-0.2.6/pytai/kaitai/formats/lzh.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23827 2022-07-22 10:09:41.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mac_os_resource_snd.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)   145656 2022-07-22 10:09:07.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mach_o.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17981 2022-07-22 10:09:48.000000 pytai-hex-0.2.6/pytai/kaitai/formats/magicavoxel_vox.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12609 2022-07-22 10:09:14.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mbr_partition_table.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    59017 2022-07-22 10:09:38.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mcap.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    21196 2022-07-22 10:10:09.000000 pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_cfb.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    19538 2022-07-22 10:09:57.000000 pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_network_monitor_v2.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    45274 2022-07-22 10:09:08.000000 pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_pe.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31274 2022-07-22 10:09:28.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mifare_classic.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    28231 2022-07-22 10:09:23.000000 pytai-hex-0.2.6/pytai/kaitai/formats/minecraft_nbt.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10114 2022-07-22 10:08:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/monomakh_sapr_chg.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18319 2022-07-22 10:08:55.000000 pytai-hex-0.2.6/pytai/kaitai/formats/mozilla_mar.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23455 2022-07-22 10:10:09.000000 pytai-hex-0.2.6/pytai/kaitai/formats/msgpack.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    69504 2022-07-22 10:09:33.000000 pytai-hex-0.2.6/pytai/kaitai/formats/nitf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     8709 2022-07-22 10:10:04.000000 pytai-hex-0.2.6/pytai/kaitai/formats/nt_mdt_pal.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13415 2022-07-22 10:09:49.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ogg.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    47234 2022-07-22 10:10:06.000000 pytai-hex-0.2.6/pytai/kaitai/formats/openpgp_message.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    30564 2022-07-22 10:09:57.000000 pytai-hex-0.2.6/pytai/kaitai/formats/packet_ppi.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16672 2022-07-22 10:09:58.000000 pytai-hex-0.2.6/pytai/kaitai/formats/pcap.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    32294 2022-07-22 10:09:18.000000 pytai-hex-0.2.6/pytai/kaitai/formats/pcf_font.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16482 2022-07-22 10:09:33.000000 pytai-hex-0.2.6/pytai/kaitai/formats/pcx.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10370 2022-07-22 10:09:34.000000 pytai-hex-0.2.6/pytai/kaitai/formats/pcx_dcx.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    26021 2022-07-22 10:08:56.000000 pytai-hex-0.2.6/pytai/kaitai/formats/phar_without_stub.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31559 2022-07-22 10:10:10.000000 pytai-hex-0.2.6/pytai/kaitai/formats/php_serialized_value.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    39417 2022-07-22 10:09:34.000000 pytai-hex-0.2.6/pytai/kaitai/formats/png.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14926 2022-07-22 10:09:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/protocol_body.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11177 2022-07-22 10:09:35.000000 pytai-hex-0.2.6/pytai/kaitai/formats/psx_tim.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    37629 2022-07-22 10:10:10.000000 pytai-hex-0.2.6/pytai/kaitai/formats/python_pickle.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    27747 2022-07-22 10:09:08.000000 pytai-hex-0.2.6/pytai/kaitai/formats/python_pyc_27.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25124 2022-07-22 10:09:24.000000 pytai-hex-0.2.6/pytai/kaitai/formats/quake_mdl.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11812 2022-07-22 10:09:24.000000 pytai-hex-0.2.6/pytai/kaitai/formats/quake_pak.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31982 2022-07-22 10:09:49.000000 pytai-hex-0.2.6/pytai/kaitai/formats/quicktime_mov.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18807 2022-07-22 10:08:56.000000 pytai-hex-0.2.6/pytai/kaitai/formats/rar.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    36883 2022-07-22 10:10:12.000000 pytai-hex-0.2.6/pytai/kaitai/formats/regf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    33073 2022-07-22 10:09:42.000000 pytai-hex-0.2.6/pytai/kaitai/formats/resource_fork.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    24213 2022-07-22 10:09:00.000000 pytai-hex-0.2.6/pytai/kaitai/formats/riff.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    44380 2022-07-22 10:08:57.000000 pytai-hex-0.2.6/pytai/kaitai/formats/rpm.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31966 2022-07-22 10:09:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/rtcp_payload.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7293 2022-07-22 10:10:00.000000 pytai-hex-0.2.6/pytai/kaitai/formats/rtp_packet.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     6762 2022-07-22 10:09:59.000000 pytai-hex-0.2.6/pytai/kaitai/formats/rtpdump.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25711 2022-07-22 10:10:11.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ruby_marshal.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    30589 2022-07-22 10:09:52.000000 pytai-hex-0.2.6/pytai/kaitai/formats/s3m.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12204 2022-07-22 10:09:25.000000 pytai-hex-0.2.6/pytai/kaitai/formats/saints_row_2_vpp_pc.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15671 2022-07-22 10:09:26.000000 pytai-hex-0.2.6/pytai/kaitai/formats/shapefile_index.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    51912 2022-07-22 10:09:26.000000 pytai-hex-0.2.6/pytai/kaitai/formats/shapefile_main.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16858 2022-07-22 10:10:02.000000 pytai-hex-0.2.6/pytai/kaitai/formats/some_ip.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     8824 2022-07-22 10:10:03.000000 pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_container.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11427 2022-07-22 10:10:03.000000 pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15193 2022-07-22 10:10:03.000000 pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd_entries.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25768 2022-07-22 10:10:04.000000 pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd_options.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    19800 2022-07-22 10:10:05.000000 pytai-hex-0.2.6/pytai/kaitai/formats/specpr.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    29158 2022-07-22 10:09:03.000000 pytai-hex-0.2.6/pytai/kaitai/formats/sqlite3.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17749 2022-07-22 10:10:07.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ssh_public_key.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23595 2022-07-22 10:09:50.000000 pytai-hex-0.2.6/pytai/kaitai/formats/standard_midi_file.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12051 2022-07-22 10:09:50.000000 pytai-hex-0.2.6/pytai/kaitai/formats/stl.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16143 2022-07-22 10:09:38.000000 pytai-hex-0.2.6/pytai/kaitai/formats/sudoers_ts.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    25103 2022-07-22 10:09:09.000000 pytai-hex-0.2.6/pytai/kaitai/formats/swf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    24601 2022-07-22 10:09:39.000000 pytai-hex-0.2.6/pytai/kaitai/formats/systemd_journal.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9996 2022-07-22 10:10:00.000000 pytai-hex-0.2.6/pytai/kaitai/formats/tcp_segment.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17870 2022-07-22 10:09:35.000000 pytai-hex-0.2.6/pytai/kaitai/formats/tga.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    13866 2022-07-22 10:10:01.000000 pytai-hex-0.2.6/pytai/kaitai/formats/tls_client_hello.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    21892 2022-07-22 10:09:14.000000 pytai-hex-0.2.6/pytai/kaitai/formats/tr_dos_image.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9969 2022-07-22 10:09:04.000000 pytai-hex-0.2.6/pytai/kaitai/formats/tsm.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)   104811 2022-07-22 10:09:18.000000 pytai-hex-0.2.6/pytai/kaitai/formats/ttf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9201 2022-07-22 10:10:01.000000 pytai-hex-0.2.6/pytai/kaitai/formats/udp_datagram.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18386 2022-07-22 10:09:09.000000 pytai-hex-0.2.6/pytai/kaitai/formats/uefi_te.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14000 2022-07-22 10:09:17.000000 pytai-hex-0.2.6/pytai/kaitai/formats/uimage.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12848 2022-07-22 10:09:01.000000 pytai-hex-0.2.6/pytai/kaitai/formats/utf8_string.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    27741 2022-07-22 10:09:15.000000 pytai-hex-0.2.6/pytai/kaitai/formats/vfat.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    11472 2022-07-22 10:09:01.000000 pytai-hex-0.2.6/pytai/kaitai/formats/vlq_base128_be.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12469 2022-07-22 10:09:02.000000 pytai-hex-0.2.6/pytai/kaitai/formats/vlq_base128_le.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15682 2022-07-22 10:09:15.000000 pytai-hex-0.2.6/pytai/kaitai/formats/vmware_vmdk.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    12460 2022-07-22 10:09:50.000000 pytai-hex-0.2.6/pytai/kaitai/formats/vp8_ivf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23900 2022-07-22 10:09:25.000000 pytai-hex-0.2.6/pytai/kaitai/formats/warcraft_2_pud.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    42578 2022-07-22 10:45:45.000000 pytai-hex-0.2.6/pytai/kaitai/formats/wav.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14876 2022-07-22 10:10:02.000000 pytai-hex-0.2.6/pytai/kaitai/formats/websocket.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    22122 2022-07-22 10:09:39.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_evt_log.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    31022 2022-07-22 10:10:12.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_lnk_file.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    34138 2022-07-22 10:10:13.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_minidump.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17555 2022-07-22 10:10:13.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_resource_file.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15107 2022-07-22 10:10:14.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_shell_items.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9590 2022-07-22 10:10:14.000000 pytai-hex-0.2.6/pytai/kaitai/formats/windows_systemtime.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    27342 2022-07-22 10:09:36.000000 pytai-hex-0.2.6/pytai/kaitai/formats/wmf.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16073 2022-07-22 10:08:57.000000 pytai-hex-0.2.6/pytai/kaitai/formats/xar.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    17088 2022-07-22 10:09:36.000000 pytai-hex-0.2.6/pytai/kaitai/formats/xwd.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    40971 2022-07-22 10:08:58.000000 pytai-hex-0.2.6/pytai/kaitai/formats/zip.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14426 2022-07-22 10:08:58.000000 pytai-hex-0.2.6/pytai/kaitai/formats/zisofs.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    15488 2022-07-22 10:09:15.000000 pytai-hex-0.2.6/pytai/kaitai/formats/zx_spectrum_tap.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    18757 2022-07-22 10:26:16.000000 pytai-hex-0.2.6/pytai/kaitai/kaitaistruct.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    23493 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/model.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.528157 pytai-hex-0.2.6/pytai/tests/
--rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 21:08:01.000000 pytai-hex-0.2.6/pytai/tests/__init__.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     6687 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/tests/kaitai_to_xml.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     3771 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/tests/xml_utils.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7876 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/utils.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.598879 pytai-hex-0.2.6/pytai/view/
--rwxrwxrwx   0 owner     (1000) owner     (1000)       56 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/__init__.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.629341 pytai-hex-0.2.6/pytai/view/assets/
--rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/assets/__init__.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)      133 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/assets/pytai.gif
--rwxrwxrwx   0 owner     (1000) owner     (1000)    32988 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/assets/pytai.ico
--rwxrwxrwx   0 owner     (1000) owner     (1000)     2619 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/bars.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     2249 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/events.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    14608 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/hex_area.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    10793 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/main.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7025 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/menus.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     8928 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/tree_area.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     2115 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/widgets.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16258 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/pytai/view/windows.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.670577 pytai-hex-0.2.6/pytai_hex.egg-info/
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7586 2022-07-22 11:53:38.000000 pytai-hex-0.2.6/pytai_hex.egg-info/PKG-INFO
--rwxrwxrwx   0 owner     (1000) owner     (1000)     7565 2022-07-22 11:53:46.000000 pytai-hex-0.2.6/pytai_hex.egg-info/SOURCES.txt
--rwxrwxrwx   0 owner     (1000) owner     (1000)        1 2022-07-22 11:53:38.000000 pytai-hex-0.2.6/pytai_hex.egg-info/dependency_links.txt
--rwxrwxrwx   0 owner     (1000) owner     (1000)       46 2022-07-22 11:53:38.000000 pytai-hex-0.2.6/pytai_hex.egg-info/entry_points.txt
--rwxrwxrwx   0 owner     (1000) owner     (1000)       18 2022-07-22 11:53:38.000000 pytai-hex-0.2.6/pytai_hex.egg-info/requires.txt
--rwxrwxrwx   0 owner     (1000) owner     (1000)        6 2022-07-22 11:53:38.000000 pytai-hex-0.2.6/pytai_hex.egg-info/top_level.txt
--rwxrwxrwx   0 owner     (1000) owner     (1000)        1 2022-07-22 11:53:29.000000 pytai-hex-0.2.6/pytai_hex.egg-info/zip-safe
--rwxrwxrwx   0 owner     (1000) owner     (1000)       38 2022-07-22 11:53:48.795738 pytai-hex-0.2.6/setup.cfg
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.679588 pytai-hex-0.2.6/tests/
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.760637 pytai-hex-0.2.6/tests/resources/
--rwxrwxrwx   0 owner     (1000) owner     (1000)      130 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/bmp.bmp
--rwxrwxrwx   0 owner     (1000) owner     (1000)     9602 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/bmp.xml
--rwxrwxrwx   0 owner     (1000) owner     (1000)    16608 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/elf.elf
--rwxrwxrwx   0 owner     (1000) owner     (1000)   419730 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/elf.xml
--rwxrwxrwx   0 owner     (1000) owner     (1000)      149 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/png.png
--rwxrwxrwx   0 owner     (1000) owner     (1000)     5452 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/png.xml
--rwxrwxrwx   0 owner     (1000) owner     (1000)   140682 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/wav.wav
--rwxrwxrwx   0 owner     (1000) owner     (1000)     4683 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/wav.xml
--rwxrwxrwx   0 owner     (1000) owner     (1000)    19404 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/zip.xml
--rwxrwxrwx   0 owner     (1000) owner     (1000)      162 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/resources/zip.zip
--rwxrwxrwx   0 owner     (1000) owner     (1000)     3665 2022-05-27 19:10:58.000000 pytai-hex-0.2.6/tests/test_application.py
-drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-07-22 11:53:48.784704 pytai-hex-0.2.6/utils/
--rwxrwxrwx   0 owner     (1000) owner     (1000)      897 2022-07-22 10:53:18.000000 pytai-hex-0.2.6/utils/Dockerfile
--rwxrwxrwx   0 owner     (1000) owner     (1000)      382 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/utils/README.md
--rwxrwxrwx   0 owner     (1000) owner     (1000)    29405 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/utils/compile_kaitai_formats.py
--rwxrwxrwx   0 owner     (1000) owner     (1000)     1867 2022-05-27 19:04:11.000000 pytai-hex-0.2.6/utils/packer.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.954307 pytai-hex-0.2.7/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      171 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/.editorconfig
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2219 2022-07-22 11:25:31.000000 pytai-hex-0.2.7/.gitignore
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25727 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/LICENSE
+-rwxrwxrwx   0 owner     (1000) owner     (1000)       26 2022-05-27 21:02:32.000000 pytai-hex-0.2.7/MANIFEST.in
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7586 2023-07-15 17:39:15.952803 pytai-hex-0.2.7/PKG-INFO
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6982 2022-06-12 18:45:13.000000 pytai-hex-0.2.7/README.md
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     1678 2022-05-27 21:39:57.000000 pytai-hex-0.2.7/__main__.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:08.209861 pytai-hex-0.2.7/docs/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     1916 2022-07-23 12:13:20.000000 pytai-hex-0.2.7/docs/Release_process.md
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:08.314035 pytai-hex-0.2.7/docs/images/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    93738 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/docs/images/mark1.png
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    94479 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/docs/images/mark2.png
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   102940 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/docs/images/meta.png
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    90409 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/docs/images/pytai.png
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    83711 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/docs/images/xref.gif
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     1180 2022-05-27 21:51:55.000000 pytai-hex-0.2.7/pyproject.toml
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:08.411586 pytai-hex-0.2.7/pytai/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/__init__.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     3212 2022-07-23 12:42:26.000000 pytai-hex-0.2.7/pytai/__main__.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16581 2023-07-01 16:56:25.000000 pytai-hex-0.2.7/pytai/application.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     4100 2023-07-01 17:01:28.000000 pytai-hex-0.2.7/pytai/common.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:08.467516 pytai-hex-0.2.7/pytai/kaitai/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/kaitai/__init__.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.060814 pytai-hex-0.2.7/pytai/kaitai/formats/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      158 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/kaitai/formats/README.md
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/kaitai/formats/__init__.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12410 2023-04-05 06:43:22.000000 pytai-hex-0.2.7/pytai/kaitai/formats/aix_utmp.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23433 2023-04-05 06:43:05.000000 pytai-hex-0.2.7/pytai/kaitai/formats/allegro_dat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10318 2023-04-05 06:43:02.000000 pytai-hex-0.2.7/pytai/kaitai/formats/andes_firmware.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12539 2023-04-05 06:42:36.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_asus.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15589 2023-04-05 06:42:36.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_huawei.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    19266 2023-04-05 06:42:37.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_qcom.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13687 2023-04-05 06:42:37.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_dto.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    20055 2023-04-05 06:42:38.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_img.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14901 2023-04-05 06:42:49.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_nanoapp_header.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18365 2023-04-05 06:43:30.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_opengl_shaders_cache.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18516 2023-04-05 06:42:38.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_sparse.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    29840 2023-04-05 06:42:55.000000 pytai-hex-0.2.7/pytai/kaitai/formats/android_super.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16896 2023-04-05 06:42:56.000000 pytai-hex-0.2.7/pytai/kaitai/formats/apm_partition_table.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14988 2023-04-05 06:42:56.000000 pytai-hex-0.2.7/pytai/kaitai/formats/apple_single_double.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16736 2023-04-05 06:43:57.000000 pytai-hex-0.2.7/pytai/kaitai/formats/asn1_der.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12489 2023-04-05 06:43:30.000000 pytai-hex-0.2.7/pytai/kaitai/formats/au.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13012 2023-04-05 06:43:51.000000 pytai-hex-0.2.7/pytai/kaitai/formats/avantes_roh60.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    20842 2023-04-05 06:43:31.000000 pytai-hex-0.2.7/pytai/kaitai/formats/avi.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12621 2023-04-05 06:42:44.000000 pytai-hex-0.2.7/pytai/kaitai/formats/bcd.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11800 2023-04-05 06:43:38.000000 pytai-hex-0.2.7/pytai/kaitai/formats/bitcoin_transaction.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23058 2023-04-05 06:43:31.000000 pytai-hex-0.2.7/pytai/kaitai/formats/blender_blend.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    43329 2023-04-05 06:43:14.000000 pytai-hex-0.2.7/pytai/kaitai/formats/bmp.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    26411 2023-04-05 06:43:53.000000 pytai-hex-0.2.7/pytai/kaitai/formats/bson.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    21887 2023-04-05 06:42:57.000000 pytai-hex-0.2.7/pytai/kaitai/formats/btrfs_stream.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2138 2023-04-05 06:42:45.000000 pytai-hex-0.2.7/pytai/kaitai/formats/bytes_with_io.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15412 2023-04-05 06:43:54.000000 pytai-hex-0.2.7/pytai/kaitai/formats/chrome_pak.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25021 2023-04-05 06:43:26.000000 pytai-hex-0.2.7/pytai/kaitai/formats/code_6502.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12320 2023-04-05 06:43:26.000000 pytai-hex-0.2.7/pytai/kaitai/formats/compressed_resource.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15223 2023-04-05 06:42:39.000000 pytai-hex-0.2.7/pytai/kaitai/formats/cpio_old_le.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14641 2023-04-05 06:42:57.000000 pytai-hex-0.2.7/pytai/kaitai/formats/cramfs.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    22405 2023-04-05 06:43:32.000000 pytai-hex-0.2.7/pytai/kaitai/formats/creative_voice_file.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    20840 2023-04-05 06:42:47.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dbf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    34552 2023-04-05 06:43:28.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_0.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    20397 2023-04-05 06:43:29.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_1.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18715 2023-04-05 06:43:29.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_2.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     3651 2023-04-05 06:43:30.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_variable_length_integer.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    59073 2023-04-05 06:42:50.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dex.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   198112 2023-04-05 06:43:15.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dicom.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16899 2023-04-05 06:43:39.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dime_message.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    30623 2023-04-05 06:43:39.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dns_packet.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    37293 2023-04-05 06:43:05.000000 pytai-hex-0.2.7/pytai/kaitai/formats/doom_wad.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15372 2023-04-05 06:42:45.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dos_datetime.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15322 2023-04-05 06:42:50.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dos_mz.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25324 2023-04-05 06:43:27.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ds_store.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    21032 2023-04-05 06:43:13.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dtb.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11805 2023-04-05 06:43:06.000000 pytai-hex-0.2.7/pytai/kaitai/formats/dune_2_pak.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    28733 2023-04-05 06:43:13.000000 pytai-hex-0.2.7/pytai/kaitai/formats/edid.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    22219 2023-04-05 06:43:52.000000 pytai-hex-0.2.7/pytai/kaitai/formats/efivar_signature_list.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   110381 2023-04-05 06:42:51.000000 pytai-hex-0.2.7/pytai/kaitai/formats/elf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12320 2023-04-05 06:43:40.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ethernet_frame.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    37278 2023-04-05 06:43:15.000000 pytai-hex-0.2.7/pytai/kaitai/formats/exif.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    33729 2023-04-05 06:42:58.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ext2.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14672 2023-04-05 06:43:06.000000 pytai-hex-0.2.7/pytai/kaitai/formats/fallout2_dat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14280 2023-04-05 06:43:07.000000 pytai-hex-0.2.7/pytai/kaitai/formats/fallout_dat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    31728 2023-04-05 06:43:38.000000 pytai-hex-0.2.7/pytai/kaitai/formats/fasttracker_xm_module.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10941 2023-04-05 06:43:07.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ftl_dat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14650 2023-04-05 06:43:32.000000 pytai-hex-0.2.7/pytai/kaitai/formats/genmidi_op2.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    24228 2023-04-05 06:42:48.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gettext_mo.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    28806 2023-04-05 06:43:16.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gif.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18165 2023-04-05 06:43:16.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gimp_brush.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12173 2023-04-05 06:43:23.000000 pytai-hex-0.2.7/pytai/kaitai/formats/glibc_utmp.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6553 2023-04-05 06:42:35.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gltf_binary.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7603 2023-04-05 06:43:54.000000 pytai-hex-0.2.7/pytai/kaitai/formats/google_protobuf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15337 2023-04-05 06:42:58.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gpt_partition_table.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13151 2023-04-05 06:43:08.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gran_turismo_vol.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    22534 2023-04-05 06:43:03.000000 pytai-hex-0.2.7/pytai/kaitai/formats/grub2_font.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17433 2023-04-05 06:42:39.000000 pytai-hex-0.2.7/pytai/kaitai/formats/gzip.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10130 2023-04-05 06:43:23.000000 pytai-hex-0.2.7/pytai/kaitai/formats/hashcat_restore.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6002 2023-04-05 06:43:40.000000 pytai-hex-0.2.7/pytai/kaitai/formats/hccap.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6451 2023-04-05 06:43:41.000000 pytai-hex-0.2.7/pytai/kaitai/formats/hccapx.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9352 2023-04-05 06:43:08.000000 pytai-hex-0.2.7/pytai/kaitai/formats/heaps_pak.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12129 2023-04-05 06:43:08.000000 pytai-hex-0.2.7/pytai/kaitai/formats/heroes_of_might_and_magic_agg.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     8751 2023-04-05 06:43:09.000000 pytai-hex-0.2.7/pytai/kaitai/formats/heroes_of_might_and_magic_bmp.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13279 2023-04-05 06:43:41.000000 pytai-hex-0.2.7/pytai/kaitai/formats/icmp_packet.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13016 2023-04-05 06:43:18.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ico.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14613 2023-04-05 06:43:33.000000 pytai-hex-0.2.7/pytai/kaitai/formats/id3v1_1.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    21643 2023-04-05 06:43:33.000000 pytai-hex-0.2.7/pytai/kaitai/formats/id3v2_3.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    27572 2023-04-05 06:43:34.000000 pytai-hex-0.2.7/pytai/kaitai/formats/id3v2_4.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13194 2023-04-05 06:43:02.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ines.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13681 2023-04-05 06:43:42.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ipv4_packet.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10063 2023-04-05 06:43:42.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ipv6_packet.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    34718 2023-04-05 06:42:59.000000 pytai-hex-0.2.7/pytai/kaitai/formats/iso9660.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    58209 2023-04-05 06:42:52.000000 pytai-hex-0.2.7/pytai/kaitai/formats/java_class.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23440 2023-04-05 06:43:18.000000 pytai-hex-0.2.7/pytai/kaitai/formats/jpeg.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15431 2023-04-05 06:42:59.000000 pytai-hex-0.2.7/pytai/kaitai/formats/luks.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14818 2023-04-05 06:42:40.000000 pytai-hex-0.2.7/pytai/kaitai/formats/lzh.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23827 2023-04-05 06:43:27.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mac_os_resource_snd.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   146435 2023-04-05 06:42:52.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mach_o.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11513 2023-04-05 06:42:53.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mach_o_fat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17981 2023-04-05 06:43:34.000000 pytai-hex-0.2.7/pytai/kaitai/formats/magicavoxel_vox.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12609 2023-04-05 06:43:00.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mbr_partition_table.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    59017 2023-04-05 06:43:24.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mcap.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    21196 2023-04-05 06:43:55.000000 pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_cfb.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    19540 2023-04-05 06:43:43.000000 pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_network_monitor_v2.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    45338 2023-04-05 06:42:53.000000 pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_pe.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    31283 2023-04-05 06:43:14.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mifare_classic.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    28243 2023-04-05 06:43:09.000000 pytai-hex-0.2.7/pytai/kaitai/formats/minecraft_nbt.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10105 2023-04-05 06:42:44.000000 pytai-hex-0.2.7/pytai/kaitai/formats/monomakh_sapr_chg.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18319 2023-04-05 06:42:40.000000 pytai-hex-0.2.7/pytai/kaitai/formats/mozilla_mar.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23455 2023-04-05 06:43:55.000000 pytai-hex-0.2.7/pytai/kaitai/formats/msgpack.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    69509 2023-04-05 06:43:19.000000 pytai-hex-0.2.7/pytai/kaitai/formats/nitf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     8709 2023-04-05 06:43:51.000000 pytai-hex-0.2.7/pytai/kaitai/formats/nt_mdt_pal.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13415 2023-04-05 06:43:35.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ogg.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    47237 2023-04-05 06:43:52.000000 pytai-hex-0.2.7/pytai/kaitai/formats/openpgp_message.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    30564 2023-04-05 06:43:43.000000 pytai-hex-0.2.7/pytai/kaitai/formats/packet_ppi.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18661 2023-04-05 06:43:44.000000 pytai-hex-0.2.7/pytai/kaitai/formats/pcap.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    32294 2023-04-05 06:43:04.000000 pytai-hex-0.2.7/pytai/kaitai/formats/pcf_font.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16482 2023-04-05 06:43:19.000000 pytai-hex-0.2.7/pytai/kaitai/formats/pcx.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    10370 2023-04-05 06:43:20.000000 pytai-hex-0.2.7/pytai/kaitai/formats/pcx_dcx.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    26021 2023-04-05 06:42:41.000000 pytai-hex-0.2.7/pytai/kaitai/formats/phar_without_stub.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    31559 2023-04-05 06:43:56.000000 pytai-hex-0.2.7/pytai/kaitai/formats/php_serialized_value.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    39417 2023-04-05 06:43:20.000000 pytai-hex-0.2.7/pytai/kaitai/formats/png.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14926 2023-04-05 06:43:45.000000 pytai-hex-0.2.7/pytai/kaitai/formats/protocol_body.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11178 2023-04-05 06:43:21.000000 pytai-hex-0.2.7/pytai/kaitai/formats/psx_tim.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    37649 2023-04-05 06:43:56.000000 pytai-hex-0.2.7/pytai/kaitai/formats/python_pickle.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    27747 2023-04-05 06:42:54.000000 pytai-hex-0.2.7/pytai/kaitai/formats/python_pyc_27.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    27941 2023-04-05 06:43:10.000000 pytai-hex-0.2.7/pytai/kaitai/formats/quake_mdl.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11812 2023-04-05 06:43:10.000000 pytai-hex-0.2.7/pytai/kaitai/formats/quake_pak.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    32320 2023-04-05 06:43:35.000000 pytai-hex-0.2.7/pytai/kaitai/formats/quicktime_mov.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18807 2023-04-05 06:42:41.000000 pytai-hex-0.2.7/pytai/kaitai/formats/rar.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    36881 2023-04-05 06:43:58.000000 pytai-hex-0.2.7/pytai/kaitai/formats/regf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    33074 2023-04-05 06:43:28.000000 pytai-hex-0.2.7/pytai/kaitai/formats/resource_fork.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9841 2023-04-05 06:42:41.000000 pytai-hex-0.2.7/pytai/kaitai/formats/respack.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    24213 2023-04-05 06:42:46.000000 pytai-hex-0.2.7/pytai/kaitai/formats/riff.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    44717 2023-04-05 06:42:42.000000 pytai-hex-0.2.7/pytai/kaitai/formats/rpm.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    31969 2023-04-05 06:43:45.000000 pytai-hex-0.2.7/pytai/kaitai/formats/rtcp_payload.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7293 2023-04-05 06:43:46.000000 pytai-hex-0.2.7/pytai/kaitai/formats/rtp_packet.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6762 2023-04-05 06:43:46.000000 pytai-hex-0.2.7/pytai/kaitai/formats/rtpdump.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25725 2023-04-05 06:43:57.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ruby_marshal.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    30589 2023-04-05 06:43:38.000000 pytai-hex-0.2.7/pytai/kaitai/formats/s3m.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12204 2023-04-05 06:43:11.000000 pytai-hex-0.2.7/pytai/kaitai/formats/saints_row_2_vpp_pc.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15671 2023-04-05 06:43:12.000000 pytai-hex-0.2.7/pytai/kaitai/formats/shapefile_index.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    51912 2023-04-05 06:43:12.000000 pytai-hex-0.2.7/pytai/kaitai/formats/shapefile_main.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16846 2023-04-05 06:43:48.000000 pytai-hex-0.2.7/pytai/kaitai/formats/some_ip.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     8824 2023-04-05 06:43:49.000000 pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_container.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11415 2023-04-05 06:43:49.000000 pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15181 2023-04-05 06:43:50.000000 pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd_entries.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25756 2023-04-05 06:43:50.000000 pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd_options.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    19800 2023-04-05 06:43:51.000000 pytai-hex-0.2.7/pytai/kaitai/formats/specpr.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    29158 2023-04-05 06:42:48.000000 pytai-hex-0.2.7/pytai/kaitai/formats/sqlite3.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17769 2023-04-05 06:43:53.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ssh_public_key.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23595 2023-04-05 06:43:36.000000 pytai-hex-0.2.7/pytai/kaitai/formats/standard_midi_file.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12051 2023-04-05 06:43:36.000000 pytai-hex-0.2.7/pytai/kaitai/formats/stl.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16144 2023-04-05 06:43:24.000000 pytai-hex-0.2.7/pytai/kaitai/formats/sudoers_ts.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    25078 2023-04-05 06:42:54.000000 pytai-hex-0.2.7/pytai/kaitai/formats/swf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    24601 2023-04-05 06:43:25.000000 pytai-hex-0.2.7/pytai/kaitai/formats/systemd_journal.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9996 2023-04-05 06:43:46.000000 pytai-hex-0.2.7/pytai/kaitai/formats/tcp_segment.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17870 2023-04-05 06:43:21.000000 pytai-hex-0.2.7/pytai/kaitai/formats/tga.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    13866 2023-04-05 06:43:47.000000 pytai-hex-0.2.7/pytai/kaitai/formats/tls_client_hello.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    21892 2023-04-05 06:43:00.000000 pytai-hex-0.2.7/pytai/kaitai/formats/tr_dos_image.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9969 2023-04-05 06:42:49.000000 pytai-hex-0.2.7/pytai/kaitai/formats/tsm.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   104854 2023-04-05 06:43:04.000000 pytai-hex-0.2.7/pytai/kaitai/formats/ttf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9201 2023-04-05 06:43:47.000000 pytai-hex-0.2.7/pytai/kaitai/formats/udp_datagram.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18386 2023-04-05 06:42:55.000000 pytai-hex-0.2.7/pytai/kaitai/formats/uefi_te.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14003 2023-04-05 06:43:03.000000 pytai-hex-0.2.7/pytai/kaitai/formats/uimage.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12848 2023-04-05 06:42:46.000000 pytai-hex-0.2.7/pytai/kaitai/formats/utf8_string.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    27741 2023-04-05 06:43:01.000000 pytai-hex-0.2.7/pytai/kaitai/formats/vfat.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11474 2023-04-05 06:42:47.000000 pytai-hex-0.2.7/pytai/kaitai/formats/vlq_base128_be.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12463 2023-04-05 06:42:47.000000 pytai-hex-0.2.7/pytai/kaitai/formats/vlq_base128_le.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15678 2023-04-05 06:43:01.000000 pytai-hex-0.2.7/pytai/kaitai/formats/vmware_vmdk.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    12462 2023-04-05 06:43:36.000000 pytai-hex-0.2.7/pytai/kaitai/formats/vp8_ivf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    23900 2023-04-05 06:43:11.000000 pytai-hex-0.2.7/pytai/kaitai/formats/warcraft_2_pud.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    42579 2023-04-05 06:45:34.000000 pytai-hex-0.2.7/pytai/kaitai/formats/wav.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14876 2023-04-05 06:43:48.000000 pytai-hex-0.2.7/pytai/kaitai/formats/websocket.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    22117 2023-04-05 06:43:25.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_evt_log.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    31022 2023-04-05 06:43:58.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_lnk_file.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    34150 2023-04-05 06:43:59.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_minidump.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17556 2023-04-05 06:43:59.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_resource_file.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15099 2023-04-05 06:44:00.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_shell_items.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9591 2023-04-05 06:44:00.000000 pytai-hex-0.2.7/pytai/kaitai/formats/windows_systemtime.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    27348 2023-04-05 06:43:22.000000 pytai-hex-0.2.7/pytai/kaitai/formats/wmf.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16073 2023-04-05 06:42:43.000000 pytai-hex-0.2.7/pytai/kaitai/formats/xar.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    17088 2023-04-05 06:43:22.000000 pytai-hex-0.2.7/pytai/kaitai/formats/xwd.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    40971 2023-04-05 06:42:43.000000 pytai-hex-0.2.7/pytai/kaitai/formats/zip.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    14426 2023-04-05 06:42:44.000000 pytai-hex-0.2.7/pytai/kaitai/formats/zisofs.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    15494 2023-04-05 06:43:01.000000 pytai-hex-0.2.7/pytai/kaitai/formats/zx_spectrum_tap.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    18757 2022-07-22 10:26:16.000000 pytai-hex-0.2.7/pytai/kaitai/kaitaistruct.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    28348 2023-07-01 17:24:08.000000 pytai-hex-0.2.7/pytai/model.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.139176 pytai-hex-0.2.7/pytai/tests/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 21:08:01.000000 pytai-hex-0.2.7/pytai/tests/__init__.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     6687 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/tests/kaitai_to_xml.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     3771 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/tests/xml_utils.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7876 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/utils.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.391937 pytai-hex-0.2.7/pytai/view/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)       56 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/__init__.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.494909 pytai-hex-0.2.7/pytai/view/assets/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        0 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/assets/__init__.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      133 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/assets/pytai.gif
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    32988 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/assets/pytai.ico
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2619 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/bars.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2631 2023-07-01 17:25:09.000000 pytai-hex-0.2.7/pytai/view/events.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16852 2023-07-01 17:26:06.000000 pytai-hex-0.2.7/pytai/view/hex_area.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11261 2023-07-01 17:26:56.000000 pytai-hex-0.2.7/pytai/view/main.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11709 2023-07-01 19:33:37.000000 pytai-hex-0.2.7/pytai/view/menus.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    11401 2023-07-01 19:30:36.000000 pytai-hex-0.2.7/pytai/view/tree_area.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2115 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/pytai/view/widgets.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16647 2022-07-23 12:39:39.000000 pytai-hex-0.2.7/pytai/view/windows.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.618491 pytai-hex-0.2.7/pytai_hex.egg-info/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7586 2023-07-15 17:38:42.000000 pytai-hex-0.2.7/pytai_hex.egg-info/PKG-INFO
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     7632 2023-07-15 17:39:08.000000 pytai-hex-0.2.7/pytai_hex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        1 2023-07-15 17:38:42.000000 pytai-hex-0.2.7/pytai_hex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 owner     (1000) owner     (1000)       46 2023-07-15 17:38:42.000000 pytai-hex-0.2.7/pytai_hex.egg-info/entry_points.txt
+-rwxrwxrwx   0 owner     (1000) owner     (1000)       18 2023-07-15 17:38:42.000000 pytai-hex-0.2.7/pytai_hex.egg-info/requires.txt
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        6 2023-07-15 17:38:42.000000 pytai-hex-0.2.7/pytai_hex.egg-info/top_level.txt
+-rwxrwxrwx   0 owner     (1000) owner     (1000)        1 2023-07-15 17:38:14.000000 pytai-hex-0.2.7/pytai_hex.egg-info/zip-safe
+-rwxrwxrwx   0 owner     (1000) owner     (1000)       38 2023-07-15 17:39:15.955287 pytai-hex-0.2.7/setup.cfg
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.630679 pytai-hex-0.2.7/tests/
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.864614 pytai-hex-0.2.7/tests/resources/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      130 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/bmp.bmp
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     9602 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/bmp.xml
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    16608 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/elf.elf
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   419730 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/elf.xml
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      149 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/png.png
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     5452 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/png.xml
+-rwxrwxrwx   0 owner     (1000) owner     (1000)   140682 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/wav.wav
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     4683 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/wav.xml
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    19404 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/zip.xml
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      162 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/resources/zip.zip
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     3665 2022-05-27 19:10:58.000000 pytai-hex-0.2.7/tests/test_application.py
+drwxrwxrwx   0 owner     (1000) owner     (1000)        0 2023-07-15 17:39:15.935673 pytai-hex-0.2.7/utils/
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      902 2022-07-23 12:53:03.000000 pytai-hex-0.2.7/utils/Dockerfile
+-rwxrwxrwx   0 owner     (1000) owner     (1000)      382 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/utils/README.md
+-rwxrwxrwx   0 owner     (1000) owner     (1000)    29405 2022-05-27 19:04:11.000000 pytai-hex-0.2.7/utils/compile_kaitai_formats.py
+-rwxrwxrwx   0 owner     (1000) owner     (1000)     2429 2022-07-23 12:23:40.000000 pytai-hex-0.2.7/utils/packer.py
```

### Comparing `pytai-hex-0.2.6/.gitignore` & `pytai-hex-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/LICENSE` & `pytai-hex-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/PKG-INFO` & `pytai-hex-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytai-hex
-Version: 0.2.6
+Version: 0.2.7
 Summary: Kaitai Struct: Visualizer and Hex Viewer GUI in Python
 Author: Dvd848
 License: MIT
 Project-URL: Homepage, https://github.com/Dvd848/pytai
 Keywords: pytai,python,kaitai,gui
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pytai-hex-0.2.6/README.md` & `pytai-hex-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/__main__.py` & `pytai-hex-0.2.7/__main__.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/docs/Release_process.md` & `pytai-hex-0.2.7/docs/Release_process.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,30 @@
       ```
 
    1. Remove "`dist`" directory if it exists
       ```
       rm -rf dist
       ```
 
-   1. Ensure that all changes are committed:
+   1. Ensure that all changes are committed and pushed to GitHub:
       ```
       git status
       ```
 
    1. Create new tag: 
       ```
       git tag
       git tag vX.Y.Z
       ```
 
+   1. Pack release:
+      ```
+      python3 packer.py
+      ```
+
    1. Create Python Virtual Environment:
       ```
       python3 -m venv pytai-env
       source pytai-env/bin/activate
       ```
 
    1. Install `pypi`-related packages:
@@ -49,14 +54,19 @@
       ```
 
    1. Install new release from `testpypi`:
       ```
       pip install --index-url https://test.pypi.org/simple/ --no-deps pytai-hex
       ```
 
+   1. Test release:
+      ```
+      pytai
+      ```
+
    1. Uninstall release:
       ```
       pip uninstall pytai-hex
       ```
 
    1. Upload to `pypi`:
       ```
@@ -64,14 +74,19 @@
       ```
 
    1. Install new release from `pypi`:
       ```
       pip install pytai-hex
       ```
 
+   1. Test release:
+      ```
+      pytai
+      ```
+
    1. Deactivate virtual environment:
       ```
       deactivate
       ```
 
    1. Remove virtual environment:
       ```
@@ -85,13 +100,8 @@
       ```
 
    1. Push tag:
       ```
       git push origin --tags
       ```
 
-   1. Pack release:
-      ```
-      python3 packer.py
-      ```
-
    1. Upload `pytai.pyz` to GitHub
```

### Comparing `pytai-hex-0.2.6/docs/images/mark1.png` & `pytai-hex-0.2.7/docs/images/mark1.png`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/docs/images/mark2.png` & `pytai-hex-0.2.7/docs/images/mark2.png`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/docs/images/meta.png` & `pytai-hex-0.2.7/docs/images/meta.png`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/docs/images/pytai.png` & `pytai-hex-0.2.7/docs/images/pytai.png`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/docs/images/xref.gif` & `pytai-hex-0.2.7/docs/images/xref.gif`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pyproject.toml` & `pytai-hex-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/__main__.py` & `pytai-hex-0.2.7/pytai/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     allowed_formats = kaitai_formats()
     parser = argparse.ArgumentParser(description='pytai: A Python-based Kaitai Struct Visualizer and HEX Viewer')
     parser.add_argument('file', action="store", nargs='?', default = None, help='Path to binary file')
     parser.add_argument('-kf', '--kaitai-format', action="store", 
                         choices = allowed_formats, metavar="FORMAT", 
                         help='Kaitai Format to use when parsing the file. '
                              f'Current formats found under "{SUBFOLDER_KAITAI}/{SUBFOLDER_FORMATS}" are: {", ".join(allowed_formats)}')
+    parser.add_argument('--version', action='version',
+                        version='%(prog)s {version}'.format(version=get_version()))
     args = parser.parse_args()
 
     
 
     if args.file is not None:
         if args.kaitai_format is None:
             args.kaitai_format = get_kaitai_format(args.file)
```

### Comparing `pytai-hex-0.2.6/pytai/application.py` & `pytai-hex-0.2.7/pytai/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,32 +49,38 @@
         POPULATE_HEX_AREA  = enum.auto()
 
     def __init__(self, file: Optional[str], format: Dict[str, Optional[str]], *args, **kwargs):
 
         # These callbacks are used to notify the application
         #  of events from the view
         callbacks = {
-            v.Events.REFRESH:             self.cb_refresh,
-            v.Events.STRUCTURE_SELECTED:  self.cb_structure_selected,
-            v.Events.GOTO:                self.cb_goto,
-            v.Events.OPEN:                self.cb_open,
-            v.Events.GET_CWD:             self.cb_get_cwd,
-            v.Events.CANCEL_LOAD:         self.cb_cancel_load,
-            v.Events.SEARCH:              self.cb_search,
-            v.Events.FIND_NEXT:           self.cb_find_next,
-            v.Events.FIND_PREV:           lambda: self.cb_find_next(reverse = True),
-            v.Events.GET_XREF:            self.cb_get_xref,
+            v.Events.REFRESH:                self.cb_refresh,
+            v.Events.STRUCTURE_SELECTED:     self.cb_structure_selected,
+            v.Events.GOTO:                   self.cb_goto,
+            v.Events.OPEN:                   self.cb_open,
+            v.Events.GET_CWD:                self.cb_get_cwd,
+            v.Events.CANCEL_LOAD:            self.cb_cancel_load,
+            v.Events.SEARCH:                 self.cb_search,
+            v.Events.FIND_NEXT:              self.cb_find_next,
+            v.Events.FIND_PREV:              lambda: self.cb_find_next(reverse = True),
+            v.Events.GET_XREF:               self.cb_get_xref,
+            v.Events.COPY_SELECTION:         self.cb_copy_selection,
+            v.Events.GET_SELECTION:          self.cb_get_selection,
+            v.Events.HIGHLIGHT_SELECTION:    self.cb_highlight_selection,
+            v.Events.GET_HIGHLIGHTED_COLORS: self.cb_get_highlighted_colors,
         }
 
         self.current_file_path = None
         self.format = None
 
         self.view = v.View(title = APP_NAME, callbacks = callbacks)
         self.model = m.Model()
 
+        self.highlight_context = {ht: set() for ht in HighlightType if HighlightType.is_custom(ht)}
+
         self.work_item = utils.WorkItem()
 
         if (file is not None):
             # Need to run populate_view in the View context, *after* the View mainloop is in action 
             self.view.schedule_function(time_ms = 100, callback = lambda: self.populate_view(file, format))
 
     def run(self) -> None:
@@ -255,17 +261,56 @@
         self.view.reset()
         self.view.set_status("Refreshing...")
         if self.current_file_path is not None:
             self.populate_view(self.current_file_path, self.format)
 
     def cb_structure_selected(self, path: str, start_offset: int, end_offset: int) -> None:
         """Callback for an event where the user selects a structure from the tree."""
-        self.view.mark_range(start_offset, end_offset)
+        self.view.mark_range(None, None, mark = False, highlight_type = HighlightType.DEFAULT)
+        self.view.mark_range(start_offset, end_offset, mark = True, highlight_type = HighlightType.DEFAULT)
         self.view.make_visible(start_offset)
 
+    def cb_copy_selection(self, path: str, start_offset: int, end_offset: int, byte_representation: ByteRepresentation) -> None:
+        """Callback for an event where the user wants to copy the contents of a tree item."""
+        byte_array = self.model.get_byte_range(self.file_mmap, start_offset, end_offset, byte_representation)
+        self.view.clipboard_clear()
+        self.view.clipboard_append(byte_array)
+
+    def cb_get_selection(self, path: str, start_offset: int, end_offset: int) -> None:
+        """Callback for an event where the user wants to return the contents of a tree item as a byte array."""
+        return self.model.get_byte_range(self.file_mmap, start_offset, end_offset, ByteRepresentation.RAW_BYTES)
+    
+    def cb_highlight_selection(self, path: str, start_offset: int, end_offset: int, highlight_type: HighlightType, mark: bool) -> None:
+        """Callback for an event where the user wants to highlight/un-highlight the selection.
+        
+        Args:
+            path:
+                Path to the selection.
+            
+            start_offset:
+                Start offset of the selection
+
+            end_offset:
+                End offset of the selection
+
+            highlight_type:
+                The type of the highlighter to use
+
+            mark:
+                True if the request is to highlight the selection, False if to un-highlight
+
+        """
+
+        if self.model.process_highlight(start_offset, end_offset, mark, highlight_type):
+            self.view.mark_range(start_offset, end_offset, mark, highlight_type)
+
+    def cb_get_highlighted_colors(self, path: str, start_offset: int, end_offset: int) -> Dict[HighlightType, HighlightDetails]:
+        """Returns details for which highlighters are used in this selection."""
+        return self.model.get_highlighted_colors(start_offset, end_offset)
+
     def cb_goto(self, offset: int) -> None:
         """Callback for an event where the user wants to jump to a given offset."""
         if offset < 0 or offset >= len(self.file_mmap):
             raise ValueError("Offset out of range")
         self.view.make_visible(offset, highlight = True)
         self.view.set_status(f"Jumping to offset {hex(offset)} ({offset})")
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/aix_utmp.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/aix_utmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class AixUtmp(KaitaiStruct):
     """This spec can be used to parse utmp, wtmp and other similar as created by IBM AIX.
     
     .. seealso::
-       Source - https://www.ibm.com/support/knowledgecenter/en/ssw_aix_71/com.ibm.aix.files/utmp.h.htm
+       Source - https://www.ibm.com/docs/en/aix/7.1?topic=files-utmph-file
     """
 
     class EntryType(Enum):
         empty = 0
         run_lvl = 1
         boot_time = 2
         old_time = 3
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/allegro_dat.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/allegro_dat.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/andes_firmware.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/andes_firmware.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_asus.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_asus.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_huawei.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_huawei.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_bootldr_qcom.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_bootldr_qcom.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_dto.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     (dtb, dtbo) on an android device to organize device tree files.
     The format consists of a header with info about size and number
     of device tree entries and the entries themselves. This format
     description could be used to extract device tree entries from a
     partition images and decompile them with dtc (device tree compiler).
     
     .. seealso::
-       Source - https://source.android.com/devices/architecture/dto/partitions
+       Source - https://source.android.com/docs/core/architecture/dto/partitions
     
     
     .. seealso::
        Source - https://android.googlesource.com/platform/system/libufdt/+/refs/tags/android-10.0.0_r47
     """
     SEQ_FIELDS = ["header", "entries"]
     def __init__(self, _io, _parent=None, _root=None):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_img.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_img.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class AndroidImg(KaitaiStruct):
     """
     .. seealso::
-       Source - https://source.android.com/devices/bootloader/boot-image-header
+       Source - https://source.android.com/docs/core/architecture/bootloader/boot-image-header
     """
     SEQ_FIELDS = ["magic", "kernel", "ramdisk", "second", "tags_load", "page_size", "header_version", "os_version", "name", "cmdline", "sha", "extra_cmdline", "recovery_dtbo", "boot_header_size", "dtb"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_nanoapp_header.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_nanoapp_header.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_opengl_shaders_cache.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_opengl_shaders_cache.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_sparse.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     Note: this is not the same as the Android sparse data image format.
     
     .. seealso::
        Source - https://android.googlesource.com/platform/system/core/+/e8d02c50d7/libsparse/sparse_format.h
     
     
     .. seealso::
-       Source - https://source.android.com/devices/bootloader/images#sparse-image-format
+       Source - https://web.archive.org/web/20220322054458/https://source.android.com/devices/bootloader/images#sparse-image-format
     """
 
     class ChunkTypes(Enum):
         raw = 51905
         fill = 51906
         dont_care = 51907
         crc32 = 51908
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/android_super.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/android_super.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     """The metadata stored by Android at the beginning of a "super" partition, which
     is what it calls a disk partition that holds one or more Dynamic Partitions.
     Dynamic Partitions do more or less the same thing that LVM does on Linux,
     allowing Android to map ranges of non-contiguous extents to a single logical
     device. This metadata holds that mapping.
     
     .. seealso::
-       Source - https://source.android.com/devices/tech/ota/dynamic_partitions
+       Source - https://source.android.com/docs/core/ota/dynamic_partitions
     
     
     .. seealso::
        Source - https://android.googlesource.com/platform/system/core/+/refs/tags/android-11.0.0_r8/fs_mgr/liblp/include/liblp/metadata_format.h
     """
     SEQ_FIELDS = []
     def __init__(self, _io, _parent=None, _root=None):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/apm_partition_table.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/apm_partition_table.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/apple_single_double.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/apple_single_double.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/asn1_der.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/asn1_der.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,17 @@
     This spec allows full parsing of format syntax, but to understand
     the semantics, one would typically require a dictionary of Object
     Identifiers (OIDs), to match OID bodies against some human-readable
     list of constants. OIDs are covered by many different standards,
     so typically it's simpler to use a pre-compiled list of them, such
     as:
     
-    * https://www.cs.auckland.ac.nz/~pgut001/dumpasn1.cfg
-    * http://oid-info.com/
-    * https://www.alvestrand.no/objectid/top.html
+    * <https://www.cs.auckland.ac.nz/~pgut001/dumpasn1.cfg>
+    * <http://oid-info.com/>
+    * <https://www.alvestrand.no/objectid/top.html>
     
     .. seealso::
        Source - https://www.itu.int/itu-t/recommendations/rec.aspx?rec=12483&lang=en
     """
 
     class TypeTag(Enum):
         end_of_content = 0
@@ -273,15 +273,15 @@
             self.str = (self._io.read_bytes_full()).decode(u"UTF-8")
             self._debug['str']['end'] = self._io.pos()
 
 
     class BodyObjectId(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/desktop/SecCertEnroll/about-object-identifier
+           Source - https://learn.microsoft.com/en-us/windows/win32/seccertenroll/about-object-identifier
         """
         SEQ_FIELDS = ["first_and_second", "rest"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/au.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/au.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,18 +138,18 @@
 class Au(KaitaiStruct):
     """The NeXT/Sun audio file format.
     
     Sample files:
     
     * <https://github.com/python/cpython/tree/b8a7daf077da/Lib/test/sndhdrdata>
     * <ftp://ftp-ccrma.stanford.edu/pub/Lisp/sf.tar.gz>
-    * <http://www-mmsp.ece.mcgill.ca/Documents/AudioFormats/AU/Samples.html>
+    * <https://www.mmsp.ece.mcgill.ca/Documents/AudioFormats/AU/Samples.html>
     
     .. seealso::
-       Source - http://www-mmsp.ece.mcgill.ca/Documents/AudioFormats/AU/AU.html
+       Source - https://www.mmsp.ece.mcgill.ca/Documents/AudioFormats/AU/AU.html
     
     
     .. seealso::
        Source - http://soundfile.sapp.org/doc/NextFormat/
     
     
     .. seealso::
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/avantes_roh60.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/avantes_roh60.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/avi.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/avi.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Avi(KaitaiStruct):
     """
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/previous-versions/ms779636(v=vs.85)
+       Source - https://learn.microsoft.com/en-us/previous-versions/ms779636(v=vs.85)
     """
 
     class ChunkType(Enum):
         idx1 = 829973609
         junk = 1263424842
         info = 1330007625
         isft = 1413894985
@@ -260,15 +260,15 @@
             self._debug['entries']['end'] = self._io.pos()
 
 
     class AvihBody(KaitaiStruct):
         """Main header of an AVI file, defined as AVIMAINHEADER structure.
         
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/previous-versions/ms779632(v=vs.85)
+           Source - https://learn.microsoft.com/en-us/previous-versions/ms779632(v=vs.85)
         """
         SEQ_FIELDS = ["micro_sec_per_frame", "max_bytes_per_sec", "padding_granularity", "flags", "total_frames", "initial_frames", "streams", "suggested_buffer_size", "width", "height", "reserved"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -346,15 +346,15 @@
             self._debug['data']['end'] = self._io.pos()
 
 
     class StrhBody(KaitaiStruct):
         """Stream header (one header per stream), defined as AVISTREAMHEADER structure.
         
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/previous-versions/ms779638(v=vs.85)
+           Source - https://learn.microsoft.com/en-us/previous-versions/ms779638(v=vs.85)
         """
         SEQ_FIELDS = ["fcc_type", "fcc_handler", "flags", "priority", "language", "initial_frames", "scale", "rate", "start", "length", "suggested_buffer_size", "quality", "sample_size", "frame"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/bcd.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/bcd.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/bitcoin_transaction.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/bitcoin_transaction.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/blender_blend.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/blender_blend.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         * a sequence of "names" (strings which represent field names)
         * a sequence of "types" (strings which represent type name)
         * a sequence of "type lengths"
         * a sequence of "structs" (which describe contents of every
           structure, referring to types and names by index)
         
         .. seealso::
-           Source - https://en.blender.org/index.php/Dev:Source/Architecture/File_Format#Structure_DNA
+           Source - https://archive.blender.org/wiki/index.php/Dev:Source/Architecture/File_Format/#Structure_DNA
         """
         SEQ_FIELDS = ["id", "name_magic", "num_names", "names", "padding_1", "type_magic", "num_types", "types", "padding_2", "tlen_magic", "lengths", "padding_3", "strc_magic", "num_structs", "structs"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/bmp.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/bmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     
     ![Bitmap headers overview](
       https://web.archive.org/web/20190527043845/https://forums.adobe.com/servlet/JiveServlet/showImage/2-3273299-47801/BMP_Headers.png
     )
     
     ## Specs
      * [Bitmap Storage (Windows Dev Center)](
-         https://docs.microsoft.com/en-us/windows/win32/gdi/bitmap-storage
+         https://learn.microsoft.com/en-us/windows/win32/gdi/bitmap-storage
        )
         * BITMAPFILEHEADER
         * BITMAPINFOHEADER
         * BITMAPV4HEADER
         * BITMAPV5HEADER
      * [OS/2 Bitmap File Format](
           https://www.fileformat.info/format/os2bmp/egff.htm
@@ -276,15 +276,15 @@
         self.bitmap = Bmp.Bitmap(_io__raw_bitmap, self, self._root)
         self.bitmap._read()
         self._debug['bitmap']['end'] = self._io.pos()
 
     class CieXyz(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-ciexyz
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-ciexyz
         """
         SEQ_FIELDS = ["x", "y", "z"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -329,15 +329,15 @@
                 self._debug['reserved']['end'] = self._io.pos()
 
 
 
     class BitmapV5Extension(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapv5header
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapv5header
         """
         SEQ_FIELDS = ["intent", "ofs_profile", "len_profile", "reserved"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -364,15 +364,15 @@
             self._m_has_profile =  ((self._parent.bitmap_v4_ext.color_space_type == Bmp.ColorSpace.profile_linked) or (self._parent.bitmap_v4_ext.color_space_type == Bmp.ColorSpace.profile_embedded)) 
             return getattr(self, '_m_has_profile', None)
 
         @property
         def profile_data(self):
             """
             .. seealso::
-               "If the profile is embedded, profile data is the actual profile, and if it is linked, the profile data is the null-terminated file name of the profile. This cannot be a Unicode string. It must be composed exclusively of characters from the Windows character set (code page 1252)." - https://docs.microsoft.com/en-us/windows/win32/wcs/using-structures-in-wcs-1-0
+               "If the profile is embedded, profile data is the actual profile, and if it is linked, the profile data is the null-terminated file name of the profile. This cannot be a Unicode string. It must be composed exclusively of characters from the Windows character set (code page 1252)." - https://learn.microsoft.com/en-us/windows/win32/wcs/using-structures-in-wcs-1-0
             """
             if hasattr(self, '_m_profile_data'):
                 return self._m_profile_data
 
             if self.has_profile:
                 io = self._root._io
                 _pos = io.pos()
@@ -414,15 +414,15 @@
                 self._debug['alpha_mask']['end'] = self._io.pos()
 
 
 
     class BitmapV4Extension(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapv4header
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapv4header
         """
         SEQ_FIELDS = ["color_space_type", "endpoint_red", "endpoint_green", "endpoint_blue", "gamma_red", "gamma_blue", "gamma_green"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -456,15 +456,15 @@
             self.gamma_green._read()
             self._debug['gamma_green']['end'] = self._io.pos()
 
 
     class BitmapInfoExtension(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/previous-versions/dd183376(v=vs.85)
+           Source - https://learn.microsoft.com/en-us/previous-versions/dd183376(v=vs.85)
         """
         SEQ_FIELDS = ["compression", "os2_compression", "len_image", "x_resolution", "y_resolution", "num_colors_used", "num_colors_important"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -516,18 +516,20 @@
                 return self._m_value
 
             self._m_value = ((self.raw + 0.0) / (1 << 30))
             return getattr(self, '_m_value', None)
 
 
     class Bitmap(KaitaiStruct):
-        """Replace with an opaque type if you care about the pixels.
-        You can look at an example of a JavaScript implementation: https://github.com/generalmimon/bmptool/blob/master/src/Bitmap.js
+        """Replace with an opaque type if you care about the pixels. You can look at
+        an example of a JavaScript implementation:
+        <https://github.com/generalmimon/bmptool/blob/master/src/Bitmap.js>
         
-        There is a proposal for adding bitmap data type to Kaitai Struct: https://github.com/kaitai-io/kaitai_struct/issues/188
+        There is a proposal for adding bitmap data type to Kaitai Struct:
+        <https://github.com/kaitai-io/kaitai_struct/issues/188>
         """
         SEQ_FIELDS = []
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -535,15 +537,15 @@
         def _read(self):
             pass
 
 
     class BitmapHeader(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapcoreheader
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapcoreheader
         
         
         .. seealso::
            Source - https://www.fileformat.info/format/os2bmp/egff.htm#OS2BMP-DMYID.3.1
         """
         SEQ_FIELDS = ["image_width", "image_height_raw", "num_planes", "bits_per_pixel", "bitmap_info_ext", "color_mask", "os2_2x_bitmap_ext", "bitmap_v4_ext", "bitmap_v5_ext"]
         def __init__(self, len_header, _io, _parent=None, _root=None):
@@ -771,15 +773,15 @@
             self._m_num_colors_present = self._io.size() // (4 if self.has_reserved_field else 3)
             return getattr(self, '_m_num_colors_present', None)
 
 
     class FileHeader(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapfileheader
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapfileheader
         """
         SEQ_FIELDS = ["file_type", "len_file", "reserved1", "reserved2", "ofs_bitmap"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -803,15 +805,15 @@
             self.ofs_bitmap = self._io.read_s4le()
             self._debug['ofs_bitmap']['end'] = self._io.pos()
 
 
     class BitmapInfo(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapinfo
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-bitmapinfo
         """
         SEQ_FIELDS = ["len_header", "header", "color_mask", "color_table"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/bson.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/bson.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,15 +482,18 @@
             self._io.align_to_byte()
             self._debug['significand_lo']['start'] = self._io.pos()
             self.significand_lo = self._io.read_u8le()
             self._debug['significand_lo']['end'] = self._io.pos()
 
 
     class ObjectId(KaitaiStruct):
-        """https://docs.mongodb.com/manual/reference/method/ObjectId/."""
+        """
+        .. seealso::
+           Source - https://www.mongodb.com/docs/manual/reference/method/ObjectId/
+        """
         SEQ_FIELDS = ["epoch_time", "machine_id", "process_id", "counter"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/btrfs_stream.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/btrfs_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     using the `btrfs send` command that can be replayed later by using `btrfs receive`, possibly on a
     different Btrfs file system. The `btrfs send` command creates a set of data modifications required
     for converting one subvolume into another.
     This spec can be used to disassemble the binary diff created by the `btrfs send` command.
     If you want a text representation you may want to checkout `btrfs receive --dump` instead.
     
     .. seealso::
-       Source - https://btrfs.wiki.kernel.org/index.php/Design_notes_on_Send/Receive
+       Source - https://archive.kernel.org/oldwiki/btrfs.wiki.kernel.org/index.php/Design_notes_on_Send/Receive.html
     """
 
     class Command(Enum):
         unspec = 0
         subvol = 1
         snapshot = 2
         mkfile = 3
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/bytes_with_io.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/bytes_with_io.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/chrome_pak.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/chrome_pak.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class ChromePak(KaitaiStruct):
     """Format mostly used by Google Chrome and various Android apps to store
     resources such as translated strings, help messages and images.
     
     .. seealso::
-       Source - https://dev.chromium.org/developers/design-documents/linuxresourcesandlocalizedstrings
+       Source - https://web.archive.org/web/20220126211447/https://dev.chromium.org/developers/design-documents/linuxresourcesandlocalizedstrings
     
     
     .. seealso::
        Source - https://chromium.googlesource.com/chromium/src/tools/grit/+/3c36f27/grit/format/data_pack.py
     
     
     .. seealso::
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/code_6502.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/code_6502.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/compressed_resource.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/compressed_resource.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/cpio_old_le.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/cpio_old_le.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/cramfs.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/cramfs.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/creative_voice_file.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/creative_voice_file.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dbf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dbf.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 # https://github.com/kaitai-io/kaitai_struct_formats
 
 
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
+from enum import Enum
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Dbf(KaitaiStruct):
@@ -140,39 +141,53 @@
     
     One .dbf file corresponds to one table and contains a series of headers,
     specification of fields, and a number of fixed-size records.
     
     .. seealso::
        Source - http://www.dbase.com/Knowledgebase/INT/db7_file_fmt.htm
     """
-    SEQ_FIELDS = ["header1", "header2", "records"]
+
+    class DeleteState(Enum):
+        false = 32
+        true = 42
+    SEQ_FIELDS = ["header1", "header2", "header_terminator", "records"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
         self._debug['header1']['start'] = self._io.pos()
         self.header1 = Dbf.Header1(self._io, self, self._root)
         self.header1._read()
         self._debug['header1']['end'] = self._io.pos()
         self._debug['header2']['start'] = self._io.pos()
-        self._raw_header2 = self._io.read_bytes((self.header1.len_header - 12))
+        self._raw_header2 = self._io.read_bytes(((self.header1.len_header - 12) - 1))
         _io__raw_header2 = KaitaiStream(BytesIO(self._raw_header2))
         self.header2 = Dbf.Header2(_io__raw_header2, self, self._root)
         self.header2._read()
         self._debug['header2']['end'] = self._io.pos()
+        self._debug['header_terminator']['start'] = self._io.pos()
+        self.header_terminator = self._io.read_bytes(1)
+        self._debug['header_terminator']['end'] = self._io.pos()
+        if not self.header_terminator == b"\x0D":
+            raise kaitaistruct.ValidationNotEqualError(b"\x0D", self.header_terminator, self._io, u"/seq/2")
         self._debug['records']['start'] = self._io.pos()
+        self._raw_records = []
         self.records = []
         for i in range(self.header1.num_records):
             if not 'arr' in self._debug['records']:
                 self._debug['records']['arr'] = []
             self._debug['records']['arr'].append({'start': self._io.pos()})
-            self.records.append(self._io.read_bytes(self.header1.len_record))
+            self._raw_records.append(self._io.read_bytes(self.header1.len_record))
+            _io__raw_records = KaitaiStream(BytesIO(self._raw_records[i]))
+            _t_records = Dbf.Record(_io__raw_records, self, self._root)
+            _t_records._read()
+            self.records.append(_t_records)
             self._debug['records']['arr'][i]['end'] = self._io.pos()
 
         self._debug['records']['end'] = self._io.pos()
 
     class Header2(KaitaiStruct):
         SEQ_FIELDS = ["header_dbase_3", "header_dbase_7", "fields"]
         def __init__(self, _io, _parent=None, _root=None):
@@ -192,22 +207,24 @@
                 self._debug['header_dbase_7']['start'] = self._io.pos()
                 self.header_dbase_7 = Dbf.HeaderDbase7(self._io, self, self._root)
                 self.header_dbase_7._read()
                 self._debug['header_dbase_7']['end'] = self._io.pos()
 
             self._debug['fields']['start'] = self._io.pos()
             self.fields = []
-            for i in range(11):
+            i = 0
+            while not self._io.is_eof():
                 if not 'arr' in self._debug['fields']:
                     self._debug['fields']['arr'] = []
                 self._debug['fields']['arr'].append({'start': self._io.pos()})
                 _t_fields = Dbf.Field(self._io, self, self._root)
                 _t_fields._read()
                 self.fields.append(_t_fields)
-                self._debug['fields']['arr'][i]['end'] = self._io.pos()
+                self._debug['fields']['arr'][len(self.fields) - 1]['end'] = self._io.pos()
+                i += 1
 
             self._debug['fields']['end'] = self._io.pos()
 
 
     class Field(KaitaiStruct):
         SEQ_FIELDS = ["name", "datatype", "data_address", "length", "decimal_count", "reserved1", "work_area_id", "reserved2", "set_fields_flag", "reserved3"]
         def __init__(self, _io, _parent=None, _root=None):
@@ -351,8 +368,32 @@
             self.language_driver_name = self._io.read_bytes(32)
             self._debug['language_driver_name']['end'] = self._io.pos()
             self._debug['reserved4']['start'] = self._io.pos()
             self.reserved4 = self._io.read_bytes(4)
             self._debug['reserved4']['end'] = self._io.pos()
 
 
+    class Record(KaitaiStruct):
+        SEQ_FIELDS = ["deleted", "record_fields"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['deleted']['start'] = self._io.pos()
+            self.deleted = KaitaiStream.resolve_enum(Dbf.DeleteState, self._io.read_u1())
+            self._debug['deleted']['end'] = self._io.pos()
+            self._debug['record_fields']['start'] = self._io.pos()
+            self.record_fields = []
+            for i in range(len(self._root.header2.fields)):
+                if not 'arr' in self._debug['record_fields']:
+                    self._debug['record_fields']['arr'] = []
+                self._debug['record_fields']['arr'].append({'start': self._io.pos()})
+                self.record_fields.append(self._io.read_bytes(self._root.header2.fields[i].length))
+                self._debug['record_fields']['arr'][i]['end'] = self._io.pos()
+
+            self._debug['record_fields']['end'] = self._io.pos()
+
+
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_0.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_0.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_1.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_1.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_2.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_2.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dcmp_variable_length_integer.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dcmp_variable_length_integer.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dex.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dex.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     machine.
     
     This format is loosely similar to Java .class file format and
     generally holds the similar set of data: i.e. classes, methods,
     fields, annotations, etc.
     
     .. seealso::
-       Source - https://source.android.com/devices/tech/dalvik/dex-format
+       Source - https://source.android.com/docs/core/runtime/dex-format
     """
 
     class ClassAccessFlags(Enum):
         public = 1
         private = 2
         protected = 4
         static = 8
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dicom.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dicom.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     
     DICOM defines two transfer syntaxes: implicit and explicit. This
     top-level parser attempts to autodetect and handle both of them. If
     any problems arise, one can use `file_explicit` and `file_implicit`
     subtypes to force parsing in particular transfer syntax.
     
     .. seealso::
-       Source - http://dicom.nema.org/medical/dicom/current/output/html/part10.html#chapter_7
+       Source - https://dicom.nema.org/medical/dicom/current/output/html/part10.html#chapter_7
     """
 
     class Tags(Enum):
         file_meta_information_group_length = 131072
         file_meta_information_version = 131073
         media_storage_sop_class_uid = 131074
         media_storage_sop_instance_uid = 131075
@@ -4118,15 +4118,15 @@
             if not self.magic == b"\x44\x49\x43\x4D":
                 raise kaitaistruct.ValidationNotEqualError(b"\x44\x49\x43\x4D", self.magic, self._io, u"/types/t_file_header/seq/1")
 
 
     class TDataElementExplicit(KaitaiStruct):
         """
         .. seealso::
-           Source - http://dicom.nema.org/medical/dicom/current/output/html/part05.html#sect_7.1.2
+           Source - https://dicom.nema.org/medical/dicom/current/output/html/part05.html#sect_7.1.2
         """
         SEQ_FIELDS = ["tag_group", "tag_elem", "vr", "reserved", "value_len", "value", "items", "elements_implicit"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -4227,15 +4227,15 @@
             self._m_tag = KaitaiStream.resolve_enum(Dicom.Tags, ((self.tag_group << 16) | self.tag_elem))
             return getattr(self, '_m_tag', None)
 
 
     class TDataElementImplicit(KaitaiStruct):
         """
         .. seealso::
-           Source - http://dicom.nema.org/medical/dicom/current/output/html/part05.html#sect_7.1.2
+           Source - https://dicom.nema.org/medical/dicom/current/output/html/part05.html#sect_7.1.2
         """
         SEQ_FIELDS = ["tag_group", "tag_elem", "vr", "reserved", "value_len", "value", "items", "elements"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dime_message.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dime_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,19 +143,19 @@
     SOAP messages, using standard transport protocols like HTTP.
     
     Sample file: `curl -LO
     https://github.com/kaitai-io/kaitai_struct_formats/files/5894723/scanner_withoptions.dump.gz
     && gunzip scanner_withoptions.dump.gz`
     
     .. seealso::
-       Source - https://tools.ietf.org/html/draft-nielsen-dime-02
+       Source - https://datatracker.ietf.org/doc/html/draft-nielsen-dime-02
     
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/archive/msdn-magazine/2002/december/sending-files-attachments-and-soap-messages-via-dime
+       Source - https://learn.microsoft.com/en-us/archive/msdn-magazine/2002/december/sending-files-attachments-and-soap-messages-via-dime
     
     
     .. seealso::
        Source - http://imrannazar.com/Parsing-the-DIME-Message-Format
     """
 
     class TypeFormats(Enum):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dns_packet.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dns_packet.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/doom_wad.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/doom_wad.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         """Used for TEXTURE1 and TEXTURE2 lumps, which designate how to
         combine wall patches to make wall textures. This essentially
         provides a very simple form of image compression, allowing
         certain elements ("patches") to be reused / recombined on
         different textures for more variety in the game.
         
         .. seealso::
-           Source - http://doom.wikia.com/wiki/TEXTURE1
+           Source - https://doom.fandom.com/wiki/TEXTURE1_and_TEXTURE2
         """
         SEQ_FIELDS = ["num_textures", "textures"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -357,15 +357,15 @@
             self.sidedef_left_idx = self._io.read_u2le()
             self._debug['sidedef_left_idx']['end'] = self._io.pos()
 
 
     class Pnames(KaitaiStruct):
         """
         .. seealso::
-           Source - http://doom.wikia.com/wiki/PNAMES
+           Source - https://doom.fandom.com/wiki/PNAMES
         """
         SEQ_FIELDS = ["num_patches", "names"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dos_datetime.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dos_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,23 +161,23 @@
       - [zip](/zip/)
       - [rar](/rar/)
       - [vfat](/vfat/) (FAT12)
       - [lzh](/lzh/)
       - [cab](http://justsolve.archiveteam.org/wiki/Cabinet)
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/sysinfo/ms-dos-date-and-time
+       Source - https://learn.microsoft.com/en-us/windows/win32/sysinfo/ms-dos-date-and-time
     
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-dosdatetimetofiletime
+       Source - https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-dosdatetimetofiletime
     
     
     .. seealso::
-       DosDateTimeToFileTime - https://github.com/reactos/reactos/blob/c6b6444/dll/win32/kernel32/client/time.c#L82-L87
+       DosDateTimeToFileTime - https://github.com/reactos/reactos/blob/c6b64448ce4/dll/win32/kernel32/client/time.c#L82-L87
     
     
     .. seealso::
        page 25/34 - https://download.microsoft.com/download/0/8/4/084c452b-b772-4fe5-89bb-a0cbf082286a/fatgen103.doc
     """
     SEQ_FIELDS = ["time", "date"]
     def __init__(self, _io, _parent=None, _root=None):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dos_mz.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dos_mz.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ds_store.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ds_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,22 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class DsStore(KaitaiStruct):
     """Apple macOS '.DS_Store' file format.
     
     .. seealso::
        Source - https://en.wikipedia.org/wiki/.DS_Store
-       https://metacpan.org/pod/distribution/Mac-Finder-DSStore/DSStoreFormat.pod
-       https://0day.work/parsing-the-ds_store-file-format
+    
+    
+    .. seealso::
+       Source - https://metacpan.org/dist/Mac-Finder-DSStore/view/DSStoreFormat.pod
+    
+    
+    .. seealso::
+       Source - https://0day.work/parsing-the-ds_store-file-format/
     """
     SEQ_FIELDS = ["alignment_header", "buddy_allocator_header"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
@@ -163,15 +169,15 @@
                 return getattr(self, '_m_offset', None)
 
             @property
             def size(self):
                 if hasattr(self, '_m_size'):
                     return self._m_size
 
-                self._m_size = ((1 << self.address_raw) & self._root.block_address_mask)
+                self._m_size = (1 << (self.address_raw & self._root.block_address_mask))
                 return getattr(self, '_m_size', None)
 
 
         class DirectoryEntry(KaitaiStruct):
             SEQ_FIELDS = ["len_name", "name", "block_id"]
             def __init__(self, _io, _parent=None, _root=None):
                 self._io = _io
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dtb.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dtb.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/dune_2_pak.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/dune_2_pak.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Dune2Pak(KaitaiStruct):
     """
     .. seealso::
-       Source - http://www.shikadi.net/moddingwiki/PAK_Format_(Westwood)
+       Source - https://moddingwiki.shikadi.net/wiki/PAK_Format_(Westwood)
     """
     SEQ_FIELDS = ["dir"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/edid.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/edid.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/efivar_signature_list.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/efivar_signature_list.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/elf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/elf.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     
     
     .. seealso::
        Source - https://refspecs.linuxfoundation.org/elf/gabi4+/contents.html
     
     
     .. seealso::
-       Source - https://docs.oracle.com/cd/E37838_01/html/E36783/glcfv.html
+       Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/elf-application-binary-interface.html
     """
 
     class SymbolVisibility(Enum):
         default = 0
         internal = 1
         hidden = 2
         protected = 3
@@ -1001,15 +1001,15 @@
                 self._debug['_m_flags_obj']['end'] = self._io.pos()
                 return getattr(self, '_m_flags_obj', None)
 
 
         class DynamicSectionEntry(KaitaiStruct):
             """
             .. seealso::
-               Source - https://docs.oracle.com/cd/E37838_01/html/E36783/chapter6-42444.html
+               Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/dynamic-section.html
             
             
             .. seealso::
                Source - https://refspecs.linuxfoundation.org/elf/gabi4+/ch5.dynamic.html#dynamic_section
             """
             SEQ_FIELDS = ["tag", "value_or_ptr"]
             def __init__(self, _io, _parent=None, _root=None, _is_le=None):
@@ -1398,15 +1398,15 @@
                 self._debug['_m_flags_obj']['end'] = self._io.pos()
                 return getattr(self, '_m_flags_obj', None)
 
 
         class RelocationSection(KaitaiStruct):
             """
             .. seealso::
-               Source - https://docs.oracle.com/cd/E37838_01/html/E36783/chapter6-54839.html
+               Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/relocation-sections.html
             
             
             .. seealso::
                Source - https://refspecs.linuxfoundation.org/elf/gabi4+/ch4.reloc.html
             """
             SEQ_FIELDS = ["entries"]
             def __init__(self, has_addend, _io, _parent=None, _root=None, _is_le=None):
@@ -1641,15 +1641,15 @@
                     self._debug['addend']['end'] = self._io.pos()
 
 
 
         class DynsymSectionEntry(KaitaiStruct):
             """
             .. seealso::
-               Source - https://docs.oracle.com/cd/E37838_01/html/E36783/man-sts.html
+               Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/symbol-table-section.html
             
             
             .. seealso::
                Source - https://refspecs.linuxfoundation.org/elf/gabi4+/ch4.symtab.html
             """
             SEQ_FIELDS = ["ofs_name", "value_b32", "size_b32", "bind", "type", "other", "sh_idx", "value_b64", "size_b64"]
             def __init__(self, _io, _parent=None, _root=None, _is_le=None):
@@ -1818,15 +1818,15 @@
                 self._m_sh_idx_special = KaitaiStream.resolve_enum(Elf.SectionHeaderIdxSpecial, self.sh_idx)
                 return getattr(self, '_m_sh_idx_special', None)
 
 
         class NoteSectionEntry(KaitaiStruct):
             """
             .. seealso::
-               Source - https://docs.oracle.com/cd/E37838_01/html/E36783/chapter6-18048.html
+               Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/note-section.html
             
             
             .. seealso::
                Source - https://refspecs.linuxfoundation.org/elf/gabi4+/ch5.pheader.html#note_section
             """
             SEQ_FIELDS = ["len_name", "len_descriptor", "type", "name", "name_padding", "descriptor", "descriptor_padding"]
             def __init__(self, _io, _parent=None, _root=None, _is_le=None):
@@ -2491,15 +2491,15 @@
         
         
         .. seealso::
            Source - https://github.com/golang/go/blob/48dfddbab3/src/debug/elf/elf.go#L1079-L1095
         
         
         .. seealso::
-           Source - https://docs.oracle.com/cd/E37838_01/html/E36783/chapter6-42444.html#OSLLGchapter7-tbl-5
+           Source - https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/linkers-libraries/dynamic-section.html#GUID-4336A69A-D905-4FCE-A398-80375A9E6464__CHAPTER7-TBL-5
         """
         SEQ_FIELDS = []
         def __init__(self, value, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self.value = value
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ethernet_frame.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ethernet_frame.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/exif.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/exif.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ext2.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ext2.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/fallout2_dat.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/fallout2_dat.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/fallout_dat.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/fallout_dat.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/fasttracker_xm_module.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/fasttracker_xm_module.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ftl_dat.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ftl_dat.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/genmidi_op2.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/genmidi_op2.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,19 @@
     * Raptor: Call of the Shadows
     
     .. seealso::
        Source - http://www.fit.vutbr.cz/~arnost/muslib/op2_form.zip
     
     
     .. seealso::
-       Source - http://doom.wikia.com/wiki/GENMIDI
+       Source - https://doom.fandom.com/wiki/GENMIDI
     
     
     .. seealso::
-       Source - http://www.shikadi.net/moddingwiki/OP2_Bank_Format
+       Source - https://moddingwiki.shikadi.net/wiki/OP2_Bank_Format
     """
     SEQ_FIELDS = ["magic", "instruments", "instrument_names"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gettext_mo.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gettext_mo.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gif.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gif.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gimp_brush.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gimp_brush.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     
     You can also use GIMP to create new brushes in this format. Custom brushes can be loaded
     into GIMP for use in the paint tools by copying them into one of the Brush Folders -
     select **Edit** > **Preferences** in the menu bar, expand the **Folders** section
     and choose **Brushes** to see the recognized Brush Folders or to add new ones.
     
     .. seealso::
-       Source - https://gitlab.gnome.org/GNOME/gimp/-/raw/4416313/devel-docs/gbr.txt
+       Source - https://github.com/GNOME/gimp/blob/441631322b/devel-docs/gbr.txt
     """
 
     class ColorDepth(Enum):
         grayscale = 1
         rgba = 4
     SEQ_FIELDS = ["len_header", "header"]
     def __init__(self, _io, _parent=None, _root=None):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/glibc_utmp.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/glibc_utmp.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gltf_binary.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gltf_binary.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/google_protobuf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/google_protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
       type specified in `.proto` file.
     * There's no direct information on which fields are optional /
       required, which fields may be repeated or constitute a map, what
       restrictions are placed on fields usage in a single message, what
       are the fields' default values, etc, etc.
     
     .. seealso::
-       Source - https://developers.google.com/protocol-buffers/docs/encoding
+       Source - https://protobuf.dev/programming-guides/encoding/
     """
     SEQ_FIELDS = ["pairs"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gpt_partition_table.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gpt_partition_table.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gran_turismo_vol.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gran_turismo_vol.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/grub2_font.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/grub2_font.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/gzip.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/gzip.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     CRCs, etc, and a file compressed by a chosen compression algorithm.
     
     As of 2019, there is actually only one working solution for
     compression algorithms, so it's typically raw DEFLATE stream
     (without zlib header) in all gzipped files.
     
     .. seealso::
-       Source - https://tools.ietf.org/html/rfc1952
+       Source - https://www.rfc-editor.org/rfc/rfc1952
     """
 
     class CompressionMethods(Enum):
         deflate = 8
 
     class Oses(Enum):
         fat = 0
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/hashcat_restore.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/hashcat_restore.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/hccap.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/hccap.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Hccap(KaitaiStruct):
     """Native format of Hashcat password "recovery" utility.
     
-    A sample of file for testing can be downloaded from https://web.archive.org/web/20150220013635if_/http://hashcat.net:80/misc/example_hashes/hashcat.hccap
+    A sample of file for testing can be downloaded from
+    <https://web.archive.org/web/20150220013635if_/http://hashcat.net:80/misc/example_hashes/hashcat.hccap>
     
     .. seealso::
        Source - https://hashcat.net/wiki/doku.php?id=hccap
     """
     SEQ_FIELDS = ["records"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/hccapx.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/hccapx.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/heaps_pak.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/heaps_pak.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/heroes_of_might_and_magic_agg.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/heroes_of_might_and_magic_agg.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/heroes_of_might_and_magic_bmp.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/heroes_of_might_and_magic_bmp.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/icmp_packet.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/icmp_packet.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ico.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ico.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 class Ico(KaitaiStruct):
     """Microsoft Windows uses specific file format to store applications
     icons - ICO. This is a container that contains one or more image
     files (effectively, DIB parts of BMP files or full PNG files are
     contained inside).
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/previous-versions/ms997538(v=msdn.10)
+       Source - https://learn.microsoft.com/en-us/previous-versions/ms997538(v=msdn.10)
     """
     SEQ_FIELDS = ["magic", "num_images", "images"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/id3v1_1.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/id3v1_1.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/id3v2_3.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/id3v2_3.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/id3v2_4.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/id3v2_4.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ines.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ines.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Ines(KaitaiStruct):
     """
     .. seealso::
-       Source - https://wiki.nesdev.com/w/index.php/INES
+       Source - https://www.nesdev.org/wiki/INES
     """
     SEQ_FIELDS = ["header", "trainer", "prg_rom", "chr_rom", "playchoice10", "title"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
@@ -111,15 +111,15 @@
             self._debug['reserved']['end'] = self._io.pos()
             if not self.reserved == b"\x00\x00\x00\x00\x00":
                 raise kaitaistruct.ValidationNotEqualError(b"\x00\x00\x00\x00\x00", self.reserved, self._io, u"/types/header/seq/8")
 
         class F6(KaitaiStruct):
             """
             .. seealso::
-               Source - https://wiki.nesdev.com/w/index.php/INES#Flags_6
+               Source - https://www.nesdev.org/wiki/INES#Flags_6
             """
 
             class Mirroring(Enum):
                 horizontal = 0
                 vertical = 1
             SEQ_FIELDS = ["lower_mapper", "four_screen", "trainer", "has_battery_ram", "mirroring"]
             def __init__(self, _io, _parent=None, _root=None):
@@ -145,15 +145,15 @@
                 self.mirroring = KaitaiStream.resolve_enum(Ines.Header.F6.Mirroring, self._io.read_bits_int_be(1))
                 self._debug['mirroring']['end'] = self._io.pos()
 
 
         class F7(KaitaiStruct):
             """
             .. seealso::
-               Source - https://wiki.nesdev.com/w/index.php/INES#Flags_7
+               Source - https://www.nesdev.org/wiki/INES#Flags_7
             """
             SEQ_FIELDS = ["upper_mapper", "format", "playchoice10", "vs_unisystem"]
             def __init__(self, _io, _parent=None, _root=None):
                 self._io = _io
                 self._parent = _parent
                 self._root = _root if _root else self
                 self._debug = collections.defaultdict(dict)
@@ -172,15 +172,15 @@
                 self.vs_unisystem = self._io.read_bits_int_be(1) != 0
                 self._debug['vs_unisystem']['end'] = self._io.pos()
 
 
         class F9(KaitaiStruct):
             """
             .. seealso::
-               Source - https://wiki.nesdev.com/w/index.php/INES#Flags_9
+               Source - https://www.nesdev.org/wiki/INES#Flags_9
             """
 
             class TvSystem(Enum):
                 ntsc = 0
                 pal = 1
             SEQ_FIELDS = ["reserved", "tv_system"]
             def __init__(self, _io, _parent=None, _root=None):
@@ -197,15 +197,15 @@
                 self.tv_system = KaitaiStream.resolve_enum(Ines.Header.F9.TvSystem, self._io.read_bits_int_be(1))
                 self._debug['tv_system']['end'] = self._io.pos()
 
 
         class F10(KaitaiStruct):
             """
             .. seealso::
-               Source - https://wiki.nesdev.com/w/index.php/INES#Flags_10
+               Source - https://www.nesdev.org/wiki/INES#Flags_10
             """
 
             class TvSystem(Enum):
                 ntsc = 0
                 dual1 = 1
                 pal = 2
                 dual2 = 3
@@ -234,27 +234,27 @@
                 self._debug['tv_system']['end'] = self._io.pos()
 
 
         @property
         def mapper(self):
             """
             .. seealso::
-               Source - https://wiki.nesdev.com/w/index.php/Mapper
+               Source - https://www.nesdev.org/wiki/Mapper
             """
             if hasattr(self, '_m_mapper'):
                 return self._m_mapper
 
             self._m_mapper = (self.f6.lower_mapper | (self.f7.upper_mapper << 4))
             return getattr(self, '_m_mapper', None)
 
 
     class Playchoice10(KaitaiStruct):
         """
         .. seealso::
-           Source - http://wiki.nesdev.com/w/index.php/PC10_ROM-Images
+           Source - https://www.nesdev.org/wiki/PC10_ROM-Images
         """
         SEQ_FIELDS = ["inst_rom", "prom"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ipv4_packet.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ipv4_packet.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ipv6_packet.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ipv6_packet.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/iso9660.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/iso9660.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
     def _read(self):
         pass
 
     class VolDescPrimary(KaitaiStruct):
         """
         .. seealso::
-           Source - http://wiki.osdev.org/ISO_9660#The_Primary_Volume_Descriptor
+           Source - https://wiki.osdev.org/ISO_9660#The_Primary_Volume_Descriptor
         """
         SEQ_FIELDS = ["unused1", "system_id", "volume_id", "unused2", "vol_space_size", "unused3", "vol_set_size", "vol_seq_num", "logical_block_size", "path_table_size", "lba_path_table_le", "lba_opt_path_table_le", "lba_path_table_be", "lba_opt_path_table_be", "root_dir", "vol_set_id", "publisher_id", "data_preparer_id", "application_id", "copyright_file_id", "abstract_file_id", "bibliographic_file_id", "vol_create_datetime", "vol_mod_datetime", "vol_expire_datetime", "vol_effective_datetime", "file_structure_version", "unused4", "application_area"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -487,15 +487,15 @@
             self.be = self._io.read_u2be()
             self._debug['be']['end'] = self._io.pos()
 
 
     class PathTableLe(KaitaiStruct):
         """
         .. seealso::
-           Source - http://wiki.osdev.org/ISO_9660#The_Path_Table
+           Source - https://wiki.osdev.org/ISO_9660#The_Path_Table
         """
         SEQ_FIELDS = ["entries"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -516,15 +516,15 @@
 
             self._debug['entries']['end'] = self._io.pos()
 
 
     class DecDatetime(KaitaiStruct):
         """
         .. seealso::
-           Source - http://wiki.osdev.org/ISO_9660#Date.2Ftime_format
+           Source - https://wiki.osdev.org/ISO_9660#Date.2Ftime_format
         """
         SEQ_FIELDS = ["year", "month", "day", "hour", "minute", "sec", "sec_hundreds", "timezone"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/java_class.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/java_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,31 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class JavaClass(KaitaiStruct):
     """
     .. seealso::
-       Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.1
+       Source - https://docs.oracle.com/javase/specs/jvms/se19/html/jvms-4.html
+    
+    
+    .. seealso::
+       Source - https://docs.oracle.com/javase/specs/jls/se6/jls3.pdf
+    
+    
+    .. seealso::
+       Source - https://github.com/openjdk/jdk/blob/jdk-21%2B14/src/jdk.hotspot.agent/share/classes/sun/jvm/hotspot/runtime/ClassConstants.java
+    
+    
+    .. seealso::
+       Source - https://github.com/openjdk/jdk/blob/jdk-21%2B14/src/java.base/share/native/include/classfile_constants.h.template
+    
+    
+    .. seealso::
+       Source - https://github.com/openjdk/jdk/blob/jdk-21%2B14/src/hotspot/share/classfile/classFileParser.cpp
     """
     SEQ_FIELDS = ["magic", "version_minor", "version_major", "constant_pool_count", "constant_pool", "access_flags", "this_class", "super_class", "interfaces_count", "interfaces", "fields_count", "fields", "methods_count", "methods", "attributes_count", "attributes"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
@@ -240,14 +256,46 @@
             _t_attributes = JavaClass.AttributeInfo(self._io, self, self._root)
             _t_attributes._read()
             self.attributes.append(_t_attributes)
             self._debug['attributes']['arr'][i]['end'] = self._io.pos()
 
         self._debug['attributes']['end'] = self._io.pos()
 
+    class VersionGuard(KaitaiStruct):
+        """`class` file format version 45.3 (appeared in the very first publicly
+        known release of Java SE AND JDK 1.0.2, released 23th January 1996) is so
+        ancient that it's taken for granted. Earlier formats seem to be
+        undocumented. Changes of `version_minor` don't change `class` format.
+        Earlier `version_major`s likely belong to Oak programming language, the
+        proprietary predecessor of Java.
+        
+        .. seealso::
+           James Gosling, Bill Joy and Guy Steele. The Java Language Specification. English. Ed. by Lisa Friendly. Addison-Wesley, Aug. 1996, p. 825. ISBN: 0-201-63451-1.
+        
+        
+        .. seealso::
+           Frank Yellin and Tim Lindholm. The Java Virtual Machine Specification. English. Ed. by Lisa Friendly. Addison-Wesley, Sept. 1996, p. 475. ISBN: 0-201-63452-X.
+        """
+        SEQ_FIELDS = ["_unnamed0"]
+        def __init__(self, major, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self.major = major
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = self._io.read_bytes(0)
+            self._debug['_unnamed0']['end'] = self._io.pos()
+            _ = self._unnamed0
+            if not self._root.version_major >= self.major:
+                raise kaitaistruct.ValidationExprError(self._unnamed0, self._io, u"/types/version_guard/seq/0")
+
+
     class FloatCpInfo(KaitaiStruct):
         """
         .. seealso::
            Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.4.5
         """
         SEQ_FIELDS = ["value"]
         def __init__(self, _io, _parent=None, _root=None):
@@ -641,14 +689,39 @@
 
         def _read(self):
             self._debug['value']['start'] = self._io.pos()
             self.value = self._io.read_f8be()
             self._debug['value']['end'] = self._io.pos()
 
 
+    class DynamicCpInfo(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://docs.oracle.com/javase/specs/jvms/se19/html/jvms-4.html#jvms-4.4.10
+        """
+        SEQ_FIELDS = ["_unnamed0", "bootstrap_method_attr_index", "name_and_type_index"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = JavaClass.VersionGuard(55, self._io, self, self._root)
+            self._unnamed0._read()
+            self._debug['_unnamed0']['end'] = self._io.pos()
+            self._debug['bootstrap_method_attr_index']['start'] = self._io.pos()
+            self.bootstrap_method_attr_index = self._io.read_u2be()
+            self._debug['bootstrap_method_attr_index']['end'] = self._io.pos()
+            self._debug['name_and_type_index']['start'] = self._io.pos()
+            self.name_and_type_index = self._io.read_u2be()
+            self._debug['name_and_type_index']['end'] = self._io.pos()
+
+
     class LongCpInfo(KaitaiStruct):
         """
         .. seealso::
            Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.4.5
         """
         SEQ_FIELDS = ["value"]
         def __init__(self, _io, _parent=None, _root=None):
@@ -664,22 +737,26 @@
 
 
     class InvokeDynamicCpInfo(KaitaiStruct):
         """
         .. seealso::
            Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.4.10
         """
-        SEQ_FIELDS = ["bootstrap_method_attr_index", "name_and_type_index"]
+        SEQ_FIELDS = ["_unnamed0", "bootstrap_method_attr_index", "name_and_type_index"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = JavaClass.VersionGuard(51, self._io, self, self._root)
+            self._unnamed0._read()
+            self._debug['_unnamed0']['end'] = self._io.pos()
             self._debug['bootstrap_method_attr_index']['start'] = self._io.pos()
             self.bootstrap_method_attr_index = self._io.read_u2be()
             self._debug['bootstrap_method_attr_index']['end'] = self._io.pos()
             self._debug['name_and_type_index']['start'] = self._io.pos()
             self.name_and_type_index = self._io.read_u2be()
             self._debug['name_and_type_index']['end'] = self._io.pos()
 
@@ -696,30 +773,81 @@
             put_field = 3
             put_static = 4
             invoke_virtual = 5
             invoke_static = 6
             invoke_special = 7
             new_invoke_special = 8
             invoke_interface = 9
-        SEQ_FIELDS = ["reference_kind", "reference_index"]
+        SEQ_FIELDS = ["_unnamed0", "reference_kind", "reference_index"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = JavaClass.VersionGuard(51, self._io, self, self._root)
+            self._unnamed0._read()
+            self._debug['_unnamed0']['end'] = self._io.pos()
             self._debug['reference_kind']['start'] = self._io.pos()
             self.reference_kind = KaitaiStream.resolve_enum(JavaClass.MethodHandleCpInfo.ReferenceKindEnum, self._io.read_u1())
             self._debug['reference_kind']['end'] = self._io.pos()
             self._debug['reference_index']['start'] = self._io.pos()
             self.reference_index = self._io.read_u2be()
             self._debug['reference_index']['end'] = self._io.pos()
 
 
+    class ModulePackageCpInfo(KaitaiStruct):
+        """Project Jigsaw modules introduced in Java 9
+        
+        .. seealso::
+           Source - https://docs.oracle.com/javase/specs/jvms/se19/html/jvms-3.html#jvms-3.16
+        
+        
+        .. seealso::
+           Source - https://docs.oracle.com/javase/specs/jvms/se19/html/jvms-4.html#jvms-4.4.11
+        
+        
+        .. seealso::
+           Source - https://docs.oracle.com/javase/specs/jvms/se19/html/jvms-4.html#jvms-4.4.12
+        """
+        SEQ_FIELDS = ["_unnamed0", "name_index"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = JavaClass.VersionGuard(53, self._io, self, self._root)
+            self._unnamed0._read()
+            self._debug['_unnamed0']['end'] = self._io.pos()
+            self._debug['name_index']['start'] = self._io.pos()
+            self.name_index = self._io.read_u2be()
+            self._debug['name_index']['end'] = self._io.pos()
+
+        @property
+        def name_as_info(self):
+            if hasattr(self, '_m_name_as_info'):
+                return self._m_name_as_info
+
+            self._m_name_as_info = self._root.constant_pool[(self.name_index - 1)].cp_info
+            return getattr(self, '_m_name_as_info', None)
+
+        @property
+        def name_as_str(self):
+            if hasattr(self, '_m_name_as_str'):
+                return self._m_name_as_str
+
+            self._m_name_as_str = self.name_as_info.value
+            return getattr(self, '_m_name_as_str', None)
+
+
     class NameAndTypeCpInfo(KaitaiStruct):
         """
         .. seealso::
            Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.4.6
         """
         SEQ_FIELDS = ["name_index", "descriptor_index"]
         def __init__(self, _io, _parent=None, _root=None):
@@ -809,22 +937,26 @@
 
 
     class MethodTypeCpInfo(KaitaiStruct):
         """
         .. seealso::
            Source - https://docs.oracle.com/javase/specs/jvms/se8/html/jvms-4.html#jvms-4.4.9
         """
-        SEQ_FIELDS = ["descriptor_index"]
+        SEQ_FIELDS = ["_unnamed0", "descriptor_index"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
+            self._debug['_unnamed0']['start'] = self._io.pos()
+            self._unnamed0 = JavaClass.VersionGuard(51, self._io, self, self._root)
+            self._unnamed0._read()
+            self._debug['_unnamed0']['end'] = self._io.pos()
             self._debug['descriptor_index']['start'] = self._io.pos()
             self.descriptor_index = self._io.read_u2be()
             self._debug['descriptor_index']['end'] = self._io.pos()
 
 
     class InterfaceMethodRefCpInfo(KaitaiStruct):
         """
@@ -913,15 +1045,18 @@
             string = 8
             field_ref = 9
             method_ref = 10
             interface_method_ref = 11
             name_and_type = 12
             method_handle = 15
             method_type = 16
+            dynamic = 17
             invoke_dynamic = 18
+            module = 19
+            package = 20
         SEQ_FIELDS = ["tag", "cp_info"]
         def __init__(self, is_prev_two_entries, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self.is_prev_two_entries = is_prev_two_entries
             self._debug = collections.defaultdict(dict)
@@ -937,14 +1072,17 @@
                 _on = self.tag
                 if _on == JavaClass.ConstantPoolEntry.TagEnum.interface_method_ref:
                     self.cp_info = JavaClass.InterfaceMethodRefCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.class_type:
                     self.cp_info = JavaClass.ClassCpInfo(self._io, self, self._root)
                     self.cp_info._read()
+                elif _on == JavaClass.ConstantPoolEntry.TagEnum.dynamic:
+                    self.cp_info = JavaClass.DynamicCpInfo(self._io, self, self._root)
+                    self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.utf8:
                     self.cp_info = JavaClass.Utf8CpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.method_type:
                     self.cp_info = JavaClass.MethodTypeCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.integer:
@@ -952,14 +1090,17 @@
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.string:
                     self.cp_info = JavaClass.StringCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.float:
                     self.cp_info = JavaClass.FloatCpInfo(self._io, self, self._root)
                     self.cp_info._read()
+                elif _on == JavaClass.ConstantPoolEntry.TagEnum.module:
+                    self.cp_info = JavaClass.ModulePackageCpInfo(self._io, self, self._root)
+                    self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.long:
                     self.cp_info = JavaClass.LongCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.method_ref:
                     self.cp_info = JavaClass.MethodRefCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.double:
@@ -970,14 +1111,17 @@
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.field_ref:
                     self.cp_info = JavaClass.FieldRefCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.method_handle:
                     self.cp_info = JavaClass.MethodHandleCpInfo(self._io, self, self._root)
                     self.cp_info._read()
+                elif _on == JavaClass.ConstantPoolEntry.TagEnum.package:
+                    self.cp_info = JavaClass.ModulePackageCpInfo(self._io, self, self._root)
+                    self.cp_info._read()
                 elif _on == JavaClass.ConstantPoolEntry.TagEnum.name_and_type:
                     self.cp_info = JavaClass.NameAndTypeCpInfo(self._io, self, self._root)
                     self.cp_info._read()
                 self._debug['cp_info']['end'] = self._io.pos()
 
 
         @property
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/jpeg.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/jpeg.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/luks.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/luks.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Luks(KaitaiStruct):
     """Linux Unified Key Setup (LUKS) is a format specification for storing disk
     encryption parameters and up to 8 user keys (which can unlock the master key).
     
     .. seealso::
-       Source - https://gitlab.com/cryptsetup/cryptsetup/wikis/LUKS-standard/on-disk-format.pdf
+       Source - https://gitlab.com/cryptsetup/cryptsetup/-/wikis/LUKS-standard/on-disk-format.pdf
     """
     SEQ_FIELDS = ["partition_header"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/lzh.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/lzh.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mac_os_resource_snd.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mac_os_resource_snd.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mach_o.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mach_o.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,44 @@
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 import asn1_der
 class MachO(KaitaiStruct):
+    """
+    .. seealso::
+       Source - https://www.stonedcoder.org/~kd/lib/MachORuntime.pdf
+    
+    
+    .. seealso::
+       Source - https://opensource.apple.com/source/python_modules/python_modules-43/Modules/macholib-1.5.1/macholib-1.5.1.tar.gz
+    
+    
+    .. seealso::
+       Source - https://github.com/comex/cs/blob/07a88f9/macho_cs.py
+    
+    
+    .. seealso::
+       Source - https://opensource.apple.com/source/Security/Security-55471/libsecurity_codesigning/requirements.grammar.auto.html
+    
+    
+    .. seealso::
+       Source - https://github.com/apple/darwin-xnu/blob/xnu-2782.40.9/bsd/sys/codesign.h
+    
+    
+    .. seealso::
+       Source - https://opensource.apple.com/source/dyld/dyld-852/src/ImageLoaderMachO.cpp.auto.html
+    
+    
+    .. seealso::
+       Source - https://opensource.apple.com/source/dyld/dyld-852/src/ImageLoaderMachOCompressed.cpp.auto.html
+    """
 
     class MagicType(Enum):
-        fat_le = 3199925962
-        fat_be = 3405691582
         macho_le_x86 = 3472551422
         macho_le_x64 = 3489328638
         macho_be_x86 = 4277009102
         macho_be_x64 = 4277009103
 
     class CpuType(Enum):
         vax = 1
@@ -443,15 +469,15 @@
                 self._debug['length']['start'] = self._io.pos()
                 self.length = self._io.read_u4be()
                 self._debug['length']['end'] = self._io.pos()
                 self._debug['value']['start'] = self._io.pos()
                 self.value = self._io.read_bytes(self.length)
                 self._debug['value']['end'] = self._io.pos()
                 self._debug['padding']['start'] = self._io.pos()
-                self.padding = self._io.read_bytes((4 - (self.length & 3)))
+                self.padding = self._io.read_bytes((-(self.length) % 4))
                 self._debug['padding']['end'] = self._io.pos()
 
 
         class SuperBlob(KaitaiStruct):
             SEQ_FIELDS = ["count", "blobs"]
             def __init__(self, _io, _parent=None, _root=None):
                 self._io = _io
@@ -2067,61 +2093,14 @@
             self._debug['export_off']['start'] = self._io.pos()
             self.export_off = self._io.read_u4le()
             self._debug['export_off']['end'] = self._io.pos()
             self._debug['export_size']['start'] = self._io.pos()
             self.export_size = self._io.read_u4le()
             self._debug['export_size']['end'] = self._io.pos()
 
-        class BindItem(KaitaiStruct):
-            SEQ_FIELDS = ["opcode_and_immediate", "uleb", "skip", "symbol"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['opcode_and_immediate']['start'] = self._io.pos()
-                self.opcode_and_immediate = self._io.read_u1()
-                self._debug['opcode_and_immediate']['end'] = self._io.pos()
-                if  ((self.opcode == MachO.DyldInfoCommand.BindOpcode.set_dylib_ordinal_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.set_append_sleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.set_segment_and_offset_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.add_address_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_add_address_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_uleb_times_skipping_uleb)) :
-                    self._debug['uleb']['start'] = self._io.pos()
-                    self.uleb = MachO.Uleb128(self._io, self, self._root)
-                    self.uleb._read()
-                    self._debug['uleb']['end'] = self._io.pos()
-
-                if self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_uleb_times_skipping_uleb:
-                    self._debug['skip']['start'] = self._io.pos()
-                    self.skip = MachO.Uleb128(self._io, self, self._root)
-                    self.skip._read()
-                    self._debug['skip']['end'] = self._io.pos()
-
-                if self.opcode == MachO.DyldInfoCommand.BindOpcode.set_symbol_trailing_flags_immediate:
-                    self._debug['symbol']['start'] = self._io.pos()
-                    self.symbol = (self._io.read_bytes_term(0, False, True, True)).decode(u"ascii")
-                    self._debug['symbol']['end'] = self._io.pos()
-
-
-            @property
-            def opcode(self):
-                if hasattr(self, '_m_opcode'):
-                    return self._m_opcode
-
-                self._m_opcode = KaitaiStream.resolve_enum(MachO.DyldInfoCommand.BindOpcode, (self.opcode_and_immediate & 240))
-                return getattr(self, '_m_opcode', None)
-
-            @property
-            def immediate(self):
-                if hasattr(self, '_m_immediate'):
-                    return self._m_immediate
-
-                self._m_immediate = (self.opcode_and_immediate & 15)
-                return getattr(self, '_m_immediate', None)
-
-
         class RebaseData(KaitaiStruct):
 
             class Opcode(Enum):
                 done = 0
                 set_type_immediate = 16
                 set_segment_and_offset_uleb = 32
                 add_address_uleb = 48
@@ -2194,14 +2173,86 @@
                         return self._m_immediate
 
                     self._m_immediate = (self.opcode_and_immediate & 15)
                     return getattr(self, '_m_immediate', None)
 
 
 
+        class BindItem(KaitaiStruct):
+            SEQ_FIELDS = ["opcode_and_immediate", "uleb", "skip", "symbol"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['opcode_and_immediate']['start'] = self._io.pos()
+                self.opcode_and_immediate = self._io.read_u1()
+                self._debug['opcode_and_immediate']['end'] = self._io.pos()
+                if  ((self.opcode == MachO.DyldInfoCommand.BindOpcode.set_dylib_ordinal_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.set_append_sleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.set_segment_and_offset_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.add_address_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_add_address_uleb) or (self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_uleb_times_skipping_uleb)) :
+                    self._debug['uleb']['start'] = self._io.pos()
+                    self.uleb = MachO.Uleb128(self._io, self, self._root)
+                    self.uleb._read()
+                    self._debug['uleb']['end'] = self._io.pos()
+
+                if self.opcode == MachO.DyldInfoCommand.BindOpcode.do_bind_uleb_times_skipping_uleb:
+                    self._debug['skip']['start'] = self._io.pos()
+                    self.skip = MachO.Uleb128(self._io, self, self._root)
+                    self.skip._read()
+                    self._debug['skip']['end'] = self._io.pos()
+
+                if self.opcode == MachO.DyldInfoCommand.BindOpcode.set_symbol_trailing_flags_immediate:
+                    self._debug['symbol']['start'] = self._io.pos()
+                    self.symbol = (self._io.read_bytes_term(0, False, True, True)).decode(u"ascii")
+                    self._debug['symbol']['end'] = self._io.pos()
+
+
+            @property
+            def opcode(self):
+                if hasattr(self, '_m_opcode'):
+                    return self._m_opcode
+
+                self._m_opcode = KaitaiStream.resolve_enum(MachO.DyldInfoCommand.BindOpcode, (self.opcode_and_immediate & 240))
+                return getattr(self, '_m_opcode', None)
+
+            @property
+            def immediate(self):
+                if hasattr(self, '_m_immediate'):
+                    return self._m_immediate
+
+                self._m_immediate = (self.opcode_and_immediate & 15)
+                return getattr(self, '_m_immediate', None)
+
+
+        class BindData(KaitaiStruct):
+            SEQ_FIELDS = ["items"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['items']['start'] = self._io.pos()
+                self.items = []
+                i = 0
+                while not self._io.is_eof():
+                    if not 'arr' in self._debug['items']:
+                        self._debug['items']['arr'] = []
+                    self._debug['items']['arr'].append({'start': self._io.pos()})
+                    _t_items = MachO.DyldInfoCommand.BindItem(self._io, self, self._root)
+                    _t_items._read()
+                    self.items.append(_t_items)
+                    self._debug['items']['arr'][len(self.items) - 1]['end'] = self._io.pos()
+                    i += 1
+
+                self._debug['items']['end'] = self._io.pos()
+
+
         class ExportNode(KaitaiStruct):
             SEQ_FIELDS = ["terminal_size", "children_count", "children", "terminal"]
             def __init__(self, _io, _parent=None, _root=None):
                 self._io = _io
                 self._parent = _parent
                 self._root = _root if _root else self
                 self._debug = collections.defaultdict(dict)
@@ -2259,133 +2310,108 @@
                     self._m_value._read()
                     self._debug['_m_value']['end'] = self._io.pos()
                     self._io.seek(_pos)
                     return getattr(self, '_m_value', None)
 
 
 
-        class BindData(KaitaiStruct):
-            SEQ_FIELDS = ["items"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
+        @property
+        def bind(self):
+            if hasattr(self, '_m_bind'):
+                return self._m_bind
 
-            def _read(self):
-                self._debug['items']['start'] = self._io.pos()
-                self.items = []
-                i = 0
-                while True:
-                    if not 'arr' in self._debug['items']:
-                        self._debug['items']['arr'] = []
-                    self._debug['items']['arr'].append({'start': self._io.pos()})
-                    _t_items = MachO.DyldInfoCommand.BindItem(self._io, self, self._root)
-                    _t_items._read()
-                    _ = _t_items
-                    self.items.append(_)
-                    self._debug['items']['arr'][len(self.items) - 1]['end'] = self._io.pos()
-                    if _.opcode == MachO.DyldInfoCommand.BindOpcode.done:
-                        break
-                    i += 1
-                self._debug['items']['end'] = self._io.pos()
+            if self.bind_size != 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.bind_off)
+                self._debug['_m_bind']['start'] = io.pos()
+                self._raw__m_bind = io.read_bytes(self.bind_size)
+                _io__raw__m_bind = KaitaiStream(BytesIO(self._raw__m_bind))
+                self._m_bind = MachO.DyldInfoCommand.BindData(_io__raw__m_bind, self, self._root)
+                self._m_bind._read()
+                self._debug['_m_bind']['end'] = io.pos()
+                io.seek(_pos)
 
+            return getattr(self, '_m_bind', None)
 
-        class LazyBindData(KaitaiStruct):
-            SEQ_FIELDS = ["items"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
+        @property
+        def exports(self):
+            if hasattr(self, '_m_exports'):
+                return self._m_exports
 
-            def _read(self):
-                self._debug['items']['start'] = self._io.pos()
-                self.items = []
-                i = 0
-                while not self._io.is_eof():
-                    if not 'arr' in self._debug['items']:
-                        self._debug['items']['arr'] = []
-                    self._debug['items']['arr'].append({'start': self._io.pos()})
-                    _t_items = MachO.DyldInfoCommand.BindItem(self._io, self, self._root)
-                    _t_items._read()
-                    self.items.append(_t_items)
-                    self._debug['items']['arr'][len(self.items) - 1]['end'] = self._io.pos()
-                    i += 1
+            if self.export_size != 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.export_off)
+                self._debug['_m_exports']['start'] = io.pos()
+                self._raw__m_exports = io.read_bytes(self.export_size)
+                _io__raw__m_exports = KaitaiStream(BytesIO(self._raw__m_exports))
+                self._m_exports = MachO.DyldInfoCommand.ExportNode(_io__raw__m_exports, self, self._root)
+                self._m_exports._read()
+                self._debug['_m_exports']['end'] = io.pos()
+                io.seek(_pos)
 
-                self._debug['items']['end'] = self._io.pos()
+            return getattr(self, '_m_exports', None)
 
+        @property
+        def weak_bind(self):
+            if hasattr(self, '_m_weak_bind'):
+                return self._m_weak_bind
+
+            if self.weak_bind_size != 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.weak_bind_off)
+                self._debug['_m_weak_bind']['start'] = io.pos()
+                self._raw__m_weak_bind = io.read_bytes(self.weak_bind_size)
+                _io__raw__m_weak_bind = KaitaiStream(BytesIO(self._raw__m_weak_bind))
+                self._m_weak_bind = MachO.DyldInfoCommand.BindData(_io__raw__m_weak_bind, self, self._root)
+                self._m_weak_bind._read()
+                self._debug['_m_weak_bind']['end'] = io.pos()
+                io.seek(_pos)
+
+            return getattr(self, '_m_weak_bind', None)
 
         @property
         def rebase(self):
             if hasattr(self, '_m_rebase'):
                 return self._m_rebase
 
-            io = self._root._io
-            _pos = io.pos()
-            io.seek(self.rebase_off)
-            self._debug['_m_rebase']['start'] = io.pos()
-            self._raw__m_rebase = io.read_bytes(self.rebase_size)
-            _io__raw__m_rebase = KaitaiStream(BytesIO(self._raw__m_rebase))
-            self._m_rebase = MachO.DyldInfoCommand.RebaseData(_io__raw__m_rebase, self, self._root)
-            self._m_rebase._read()
-            self._debug['_m_rebase']['end'] = io.pos()
-            io.seek(_pos)
-            return getattr(self, '_m_rebase', None)
-
-        @property
-        def bind(self):
-            if hasattr(self, '_m_bind'):
-                return self._m_bind
+            if self.rebase_size != 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.rebase_off)
+                self._debug['_m_rebase']['start'] = io.pos()
+                self._raw__m_rebase = io.read_bytes(self.rebase_size)
+                _io__raw__m_rebase = KaitaiStream(BytesIO(self._raw__m_rebase))
+                self._m_rebase = MachO.DyldInfoCommand.RebaseData(_io__raw__m_rebase, self, self._root)
+                self._m_rebase._read()
+                self._debug['_m_rebase']['end'] = io.pos()
+                io.seek(_pos)
 
-            io = self._root._io
-            _pos = io.pos()
-            io.seek(self.bind_off)
-            self._debug['_m_bind']['start'] = io.pos()
-            self._raw__m_bind = io.read_bytes(self.bind_size)
-            _io__raw__m_bind = KaitaiStream(BytesIO(self._raw__m_bind))
-            self._m_bind = MachO.DyldInfoCommand.BindData(_io__raw__m_bind, self, self._root)
-            self._m_bind._read()
-            self._debug['_m_bind']['end'] = io.pos()
-            io.seek(_pos)
-            return getattr(self, '_m_bind', None)
+            return getattr(self, '_m_rebase', None)
 
         @property
         def lazy_bind(self):
             if hasattr(self, '_m_lazy_bind'):
                 return self._m_lazy_bind
 
-            io = self._root._io
-            _pos = io.pos()
-            io.seek(self.lazy_bind_off)
-            self._debug['_m_lazy_bind']['start'] = io.pos()
-            self._raw__m_lazy_bind = io.read_bytes(self.lazy_bind_size)
-            _io__raw__m_lazy_bind = KaitaiStream(BytesIO(self._raw__m_lazy_bind))
-            self._m_lazy_bind = MachO.DyldInfoCommand.LazyBindData(_io__raw__m_lazy_bind, self, self._root)
-            self._m_lazy_bind._read()
-            self._debug['_m_lazy_bind']['end'] = io.pos()
-            io.seek(_pos)
-            return getattr(self, '_m_lazy_bind', None)
-
-        @property
-        def exports(self):
-            if hasattr(self, '_m_exports'):
-                return self._m_exports
+            if self.lazy_bind_size != 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.lazy_bind_off)
+                self._debug['_m_lazy_bind']['start'] = io.pos()
+                self._raw__m_lazy_bind = io.read_bytes(self.lazy_bind_size)
+                _io__raw__m_lazy_bind = KaitaiStream(BytesIO(self._raw__m_lazy_bind))
+                self._m_lazy_bind = MachO.DyldInfoCommand.BindData(_io__raw__m_lazy_bind, self, self._root)
+                self._m_lazy_bind._read()
+                self._debug['_m_lazy_bind']['end'] = io.pos()
+                io.seek(_pos)
 
-            io = self._root._io
-            _pos = io.pos()
-            io.seek(self.export_off)
-            self._debug['_m_exports']['start'] = io.pos()
-            self._raw__m_exports = io.read_bytes(self.export_size)
-            _io__raw__m_exports = KaitaiStream(BytesIO(self._raw__m_exports))
-            self._m_exports = MachO.DyldInfoCommand.ExportNode(_io__raw__m_exports, self, self._root)
-            self._m_exports._read()
-            self._debug['_m_exports']['end'] = io.pos()
-            io.seek(_pos)
-            return getattr(self, '_m_exports', None)
+            return getattr(self, '_m_lazy_bind', None)
 
 
     class DylinkerCommand(KaitaiStruct):
         SEQ_FIELDS = ["name"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/magicavoxel_vox.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/magicavoxel_vox.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mbr_partition_table.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mbr_partition_table.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mcap.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mcap.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_cfb.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_cfb.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_network_monitor_v2.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_network_monitor_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     contain some additional info - enhanced network info, calculated
     statistics, etc.
     
     There are at least 2 different versions of the format: v1 and
     v2. Netmon v3 seems to use the same file format as v1.
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/netmon2/capturefile-header-values
+       Source - https://learn.microsoft.com/en-us/windows/win32/netmon2/capturefile-header-values
     """
 
     class Linktype(Enum):
         null_linktype = 0
         ethernet = 1
         ax25 = 3
         ieee802_5 = 6
@@ -379,15 +379,15 @@
 
     class Frame(KaitaiStruct):
         """A container for actually captured network data. Allow to
         timestamp individual frames and designates how much data from
         the original packet was actually written into the file.
         
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/netmon2/frame
+           Source - https://learn.microsoft.com/en-us/windows/win32/netmon2/frame
         """
         SEQ_FIELDS = ["ts_delta", "orig_len", "inc_len", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/microsoft_pe.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/microsoft_pe.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class MicrosoftPe(KaitaiStruct):
     """
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/debug/pe-format
+       Source - https://learn.microsoft.com/en-us/windows/win32/debug/pe-format
     """
 
     class PeFormat(Enum):
         rom_image = 263
         pe32 = 267
         pe32_plus = 523
     SEQ_FIELDS = ["mz"]
@@ -157,15 +157,15 @@
         self.mz = MicrosoftPe.MzPlaceholder(self._io, self, self._root)
         self.mz._read()
         self._debug['mz']['end'] = self._io.pos()
 
     class CertificateEntry(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/desktop/debug/pe-format#the-attribute-certificate-table-image-only
+           Source - https://learn.microsoft.com/en-us/windows/win32/debug/pe-format#the-attribute-certificate-table-image-only
         """
 
         class CertificateRevision(Enum):
             revision_1_0 = 256
             revision_2_0 = 512
 
         class CertificateTypeEnum(Enum):
@@ -705,14 +705,16 @@
             mips16 = 614
             mipsfpu = 870
             mipsfpu16 = 1126
             ebc = 3772
             riscv32 = 20530
             riscv64 = 20580
             riscv128 = 20776
+            loongarch32 = 25138
+            loongarch64 = 25188
             amd64 = 34404
             m32r = 36929
             arm64 = 43620
         SEQ_FIELDS = ["machine", "number_of_sections", "time_date_stamp", "pointer_to_symbol_table", "number_of_symbols", "size_of_optional_header", "characteristics"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mifare_classic.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mifare_classic.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class MifareClassic(KaitaiStruct):
-    """You can get a dump for testing by the link: https://github.com/zhovner/mfdread/raw/master/dump.mfd
+    """You can get a dump for testing from this link:
+    <https://github.com/zhovner/mfdread/raw/master/dump.mfd>
     
     .. seealso::
        Source - https://github.com/nfc-tools/libnfc
        https://www.nxp.com/docs/en/data-sheet/MF1S70YYX_V1.pdf
     """
     SEQ_FIELDS = ["sectors"]
     def __init__(self, _io, _parent=None, _root=None):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/minecraft_nbt.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/minecraft_nbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,22 +134,22 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class MinecraftNbt(KaitaiStruct):
     """A structured binary format native to Minecraft for saving game data and transferring
     it over the network (in multiplayer), such as player data
-    ([`<player>.dat`](https://minecraft.gamepedia.com/Player.dat_format); contains
+    ([`<player>.dat`](https://minecraft.fandom.com/wiki/Player.dat_format); contains
     e.g. player's inventory and location), saved worlds
     ([`level.dat`](
-      https://minecraft.gamepedia.com/Java_Edition_level_format#level.dat_format
-    ) and [Chunk format](https://minecraft.gamepedia.com/Chunk_format#NBT_structure)),
+      https://minecraft.fandom.com/wiki/Java_Edition_level_format#level.dat_format
+    ) and [Chunk format](https://minecraft.fandom.com/wiki/Chunk_format#NBT_structure)),
     list of saved multiplayer servers
-    ([`servers.dat`](https://minecraft.gamepedia.com/Servers.dat_format)) and so on -
-    see <https://minecraft.gamepedia.com/NBT_format#Uses>.
+    ([`servers.dat`](https://minecraft.fandom.com/wiki/Servers.dat_format)) and so on -
+    see <https://minecraft.fandom.com/wiki/NBT_format#Uses>.
     
     The entire file should be _gzip_-compressed (in accordance with the original
     specification [NBT.txt](
       https://web.archive.org/web/20110723210920/https://www.minecraft.net/docs/NBT.txt
     ) by Notch), but can also be compressed with _zlib_ or uncompressed.
     
     This spec can only handle uncompressed NBT data, so be sure to first detect
@@ -210,15 +210,15 @@
     
     
     .. seealso::
        Source - https://web.archive.org/web/20110723210920/https://www.minecraft.net/docs/NBT.txt
     
     
     .. seealso::
-       Source - https://minecraft.gamepedia.com/NBT_format
+       Source - https://minecraft.fandom.com/wiki/NBT_format
     """
 
     class Tag(Enum):
         end = 0
         byte = 1
         short = 2
         int = 3
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/monomakh_sapr_chg.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/monomakh_sapr_chg.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class MonomakhSaprChg(KaitaiStruct):
     """CHG is a container format file used by
-    [MONOMAKH-SAPR](https://www.liraland.com/mono/index.php), a software
+    [MONOMAKH-SAPR](https://www.liraland.com/mono/), a software
     package for analysis & design of reinforced concrete multi-storey
     buildings with arbitrary configuration in plan.
     
     CHG is a simple container, which bundles several project files
     together.
     
     Written and tested by Vladimir Shulzhitskiy, 2017
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/mozilla_mar.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/mozilla_mar.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/msgpack.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/nitf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/nitf.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     
     According to the [foreword of the specification](https://web.archive.org/web/20181105050336/https://www.gwg.nga.mil/ntb/baseline/docs/2500c/2500C.pdf):
     > The National Imagery Transmission Format Standard (NITFS) is the suite of standards for formatting digital
     > imagery and imagery-related products and exchanging them among members of the Intelligence Community (IC) as
     > defined by the Executive Order 12333, and other United States Government departments and agencies."
     
     This implementation is set to version format (`file_version`) of 02.10 and `standard_type` of `BF01`.
-    It was implemented by [River Loop Security](https://riverloopsecurity.com).
+    It was implemented by [River Loop Security](https://www.riverloopsecurity.com/).
     
     .. seealso::
        Source - https://web.archive.org/web/20181105050336/https://www.gwg.nga.mil/ntb/baseline/docs/2500c/2500C.pdf
     """
     SEQ_FIELDS = ["header", "image_segments", "graphics_segments", "text_segments", "data_extension_segments", "reserved_extension_segments"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/nt_mdt_pal.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/nt_mdt_pal.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ogg.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ogg.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/openpgp_message.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/openpgp_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class OpenpgpMessage(KaitaiStruct):
     """The OpenPGP Message Format is a format to store encryption and signature keys for emails.
     
     .. seealso::
-       Source - https://tools.ietf.org/html/rfc4880
+       Source - https://www.rfc-editor.org/rfc/rfc4880
     """
 
     class PublicKeyAlgorithms(Enum):
         rsa_encrypt_or_sign_hac = 1
         rsa_encrypt_only_hac = 2
         rsa_sign_only_hac = 3
         elgamal_encrypt_only_elgamal_hac = 16
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/packet_ppi.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/packet_ppi.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,16 @@
 import ethernet_frame
 class PacketPpi(KaitaiStruct):
     """PPI is a standard for link layer packet encapsulation, proposed as
     generic extensible container to store both captured in-band data and
     out-of-band data. Originally it was developed to provide 802.11n
     radio information, but can be used for other purposes as well.
     
-    Sample capture: https://wiki.wireshark.org/SampleCaptures?action=AttachFile&do=get&target=Http.cap
+    Sample capture:
+    <https://wiki.wireshark.org/uploads/27707187aeb30df68e70c8fb9d614981/http.cap>
     
     .. seealso::
        PPI header format spec, section 3 - https://web.archive.org/web/20090206112419/https://www.cacetech.com/documents/PPI_Header_format_1.0.1.pdf
     """
 
     class PfhType(Enum):
         radio_802_11_common = 2
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/pcap.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/rar.py`

 * *Files 11% similar despite different names*

```diff
@@ -131,262 +131,260 @@
 from enum import Enum
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-import ethernet_frame
-import packet_ppi
-class Pcap(KaitaiStruct):
-    """PCAP (named after libpcap / winpcap) is a popular format for saving
-    network traffic grabbed by network sniffers. It is typically
-    produced by tools like [tcpdump](https://www.tcpdump.org/) or
-    [Wireshark](https://www.wireshark.org/).
+import dos_datetime
+class Rar(KaitaiStruct):
+    """RAR is a archive format used by popular proprietary RAR archiver,
+    created by Eugene Roshal. There are two major versions of format
+    (v1.5-4.0 and RAR v5+).
+    
+    File format essentially consists of a linear sequence of
+    blocks. Each block has fixed header and custom body (that depends on
+    block type), so it's possible to skip block even if one doesn't know
+    how to process a certain block type.
     
     .. seealso::
-       Source - http://wiki.wireshark.org/Development/LibpcapFileFormat
+       Source - http://acritum.com/winrar/rar-format
     """
 
-    class Linktype(Enum):
-        null_linktype = 0
-        ethernet = 1
-        ax25 = 3
-        ieee802_5 = 6
-        arcnet_bsd = 7
-        slip = 8
-        ppp = 9
-        fddi = 10
-        ppp_hdlc = 50
-        ppp_ether = 51
-        atm_rfc1483 = 100
-        raw = 101
-        c_hdlc = 104
-        ieee802_11 = 105
-        frelay = 107
-        loop = 108
-        linux_sll = 113
-        ltalk = 114
-        pflog = 117
-        ieee802_11_prism = 119
-        ip_over_fc = 122
-        sunatm = 123
-        ieee802_11_radiotap = 127
-        arcnet_linux = 129
-        apple_ip_over_ieee1394 = 138
-        mtp2_with_phdr = 139
-        mtp2 = 140
-        mtp3 = 141
-        sccp = 142
-        docsis = 143
-        linux_irda = 144
-        user0 = 147
-        user1 = 148
-        user2 = 149
-        user3 = 150
-        user4 = 151
-        user5 = 152
-        user6 = 153
-        user7 = 154
-        user8 = 155
-        user9 = 156
-        user10 = 157
-        user11 = 158
-        user12 = 159
-        user13 = 160
-        user14 = 161
-        user15 = 162
-        ieee802_11_avs = 163
-        bacnet_ms_tp = 165
-        ppp_pppd = 166
-        gprs_llc = 169
-        gpf_t = 170
-        gpf_f = 171
-        linux_lapd = 177
-        mfr = 182
-        bluetooth_hci_h4 = 187
-        usb_linux = 189
-        ppi = 192
-        ieee802_15_4_withfcs = 195
-        sita = 196
-        erf = 197
-        bluetooth_hci_h4_with_phdr = 201
-        ax25_kiss = 202
-        lapd = 203
-        ppp_with_dir = 204
-        c_hdlc_with_dir = 205
-        frelay_with_dir = 206
-        lapb_with_dir = 207
-        ipmb_linux = 209
-        flexray = 210
-        lin = 212
-        ieee802_15_4_nonask_phy = 215
-        usb_linux_mmapped = 220
-        fc_2 = 224
-        fc_2_with_frame_delims = 225
-        ipnet = 226
-        can_socketcan = 227
-        ipv4 = 228
-        ipv6 = 229
-        ieee802_15_4_nofcs = 230
-        dbus = 231
-        dvb_ci = 235
-        mux27010 = 236
-        stanag_5066_d_pdu = 237
-        nflog = 239
-        netanalyzer = 240
-        netanalyzer_transparent = 241
-        ipoib = 242
-        mpeg_2_ts = 243
-        ng40 = 244
-        nfc_llcp = 245
-        infiniband = 247
-        sctp = 248
-        usbpcap = 249
-        rtac_serial = 250
-        bluetooth_le_ll = 251
-        netlink = 253
-        bluetooth_linux_monitor = 254
-        bluetooth_bredr_bb = 255
-        bluetooth_le_ll_with_phdr = 256
-        profibus_dl = 257
-        pktap = 258
-        epon = 259
-        ipmi_hpm_2 = 260
-        zwave_r1_r2 = 261
-        zwave_r3 = 262
-        wattstopper_dlm = 263
-        iso_14443 = 264
-        rds = 265
-        usb_darwin = 266
-        sdlc = 268
-        loratap = 270
-        vsock = 271
-        nordic_ble = 272
-        docsis31_xra31 = 273
-        ethernet_mpacket = 274
-        displayport_aux = 275
-        linux_sll2 = 276
-        openvizsla = 278
-        ebhscr = 279
-        vpp_dispatch = 280
-        dsa_tag_brcm = 281
-        dsa_tag_brcm_prepend = 282
-        ieee802_15_4_tap = 283
-        dsa_tag_dsa = 284
-        dsa_tag_edsa = 285
-        elee = 286
-        zwave_serial = 287
-        usb_2_0 = 288
-        atsc_alp = 289
-        etw = 290
-        zboss_ncp = 292
-    SEQ_FIELDS = ["hdr", "packets"]
+    class BlockTypes(Enum):
+        marker = 114
+        archive_header = 115
+        file_header = 116
+        old_style_comment_header = 117
+        old_style_authenticity_info_76 = 118
+        old_style_subblock = 119
+        old_style_recovery_record = 120
+        old_style_authenticity_info_79 = 121
+        subblock = 122
+        terminator = 123
+
+    class Oses(Enum):
+        ms_dos = 0
+        os_2 = 1
+        windows = 2
+        unix = 3
+        mac_os = 4
+        beos = 5
+
+    class Methods(Enum):
+        store = 48
+        fastest = 49
+        fast = 50
+        normal = 51
+        good = 52
+        best = 53
+    SEQ_FIELDS = ["magic", "blocks"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
-        self._debug['hdr']['start'] = self._io.pos()
-        self.hdr = Pcap.Header(self._io, self, self._root)
-        self.hdr._read()
-        self._debug['hdr']['end'] = self._io.pos()
-        self._debug['packets']['start'] = self._io.pos()
-        self.packets = []
+        self._debug['magic']['start'] = self._io.pos()
+        self.magic = Rar.MagicSignature(self._io, self, self._root)
+        self.magic._read()
+        self._debug['magic']['end'] = self._io.pos()
+        self._debug['blocks']['start'] = self._io.pos()
+        self.blocks = []
         i = 0
         while not self._io.is_eof():
-            if not 'arr' in self._debug['packets']:
-                self._debug['packets']['arr'] = []
-            self._debug['packets']['arr'].append({'start': self._io.pos()})
-            _t_packets = Pcap.Packet(self._io, self, self._root)
-            _t_packets._read()
-            self.packets.append(_t_packets)
-            self._debug['packets']['arr'][len(self.packets) - 1]['end'] = self._io.pos()
+            if not 'arr' in self._debug['blocks']:
+                self._debug['blocks']['arr'] = []
+            self._debug['blocks']['arr'].append({'start': self._io.pos()})
+            _on = self.magic.version
+            if _on == 0:
+                if not 'arr' in self._debug['blocks']:
+                    self._debug['blocks']['arr'] = []
+                self._debug['blocks']['arr'].append({'start': self._io.pos()})
+                _t_blocks = Rar.Block(self._io, self, self._root)
+                _t_blocks._read()
+                self.blocks.append(_t_blocks)
+                self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
+            elif _on == 1:
+                if not 'arr' in self._debug['blocks']:
+                    self._debug['blocks']['arr'] = []
+                self._debug['blocks']['arr'].append({'start': self._io.pos()})
+                _t_blocks = Rar.BlockV5(self._io, self, self._root)
+                _t_blocks._read()
+                self.blocks.append(_t_blocks)
+                self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
+            self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
             i += 1
 
-        self._debug['packets']['end'] = self._io.pos()
+        self._debug['blocks']['end'] = self._io.pos()
 
-    class Header(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://wiki.wireshark.org/Development/LibpcapFileFormat#Global_Header
+    class MagicSignature(KaitaiStruct):
+        """RAR uses either 7-byte magic for RAR versions 1.5 to 4.0, and
+        8-byte magic (and pretty different block format) for v5+. This
+        type would parse and validate both versions of signature. Note
+        that actually this signature is a valid RAR "block": in theory,
+        one can omit signature reading at all, and read this normally,
+        as a block, if exact RAR version is known (and thus it's
+        possible to choose correct block format).
         """
-        SEQ_FIELDS = ["magic_number", "version_major", "version_minor", "thiszone", "sigfigs", "snaplen", "network"]
+        SEQ_FIELDS = ["magic1", "version", "magic3"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['magic_number']['start'] = self._io.pos()
-            self.magic_number = self._io.read_bytes(4)
-            self._debug['magic_number']['end'] = self._io.pos()
-            if not self.magic_number == b"\xD4\xC3\xB2\xA1":
-                raise kaitaistruct.ValidationNotEqualError(b"\xD4\xC3\xB2\xA1", self.magic_number, self._io, u"/types/header/seq/0")
-            self._debug['version_major']['start'] = self._io.pos()
-            self.version_major = self._io.read_u2le()
-            self._debug['version_major']['end'] = self._io.pos()
-            if not self.version_major == 2:
-                raise kaitaistruct.ValidationNotEqualError(2, self.version_major, self._io, u"/types/header/seq/1")
-            self._debug['version_minor']['start'] = self._io.pos()
-            self.version_minor = self._io.read_u2le()
-            self._debug['version_minor']['end'] = self._io.pos()
-            self._debug['thiszone']['start'] = self._io.pos()
-            self.thiszone = self._io.read_s4le()
-            self._debug['thiszone']['end'] = self._io.pos()
-            self._debug['sigfigs']['start'] = self._io.pos()
-            self.sigfigs = self._io.read_u4le()
-            self._debug['sigfigs']['end'] = self._io.pos()
-            self._debug['snaplen']['start'] = self._io.pos()
-            self.snaplen = self._io.read_u4le()
-            self._debug['snaplen']['end'] = self._io.pos()
-            self._debug['network']['start'] = self._io.pos()
-            self.network = KaitaiStream.resolve_enum(Pcap.Linktype, self._io.read_u4le())
-            self._debug['network']['end'] = self._io.pos()
+            self._debug['magic1']['start'] = self._io.pos()
+            self.magic1 = self._io.read_bytes(6)
+            self._debug['magic1']['end'] = self._io.pos()
+            if not self.magic1 == b"\x52\x61\x72\x21\x1A\x07":
+                raise kaitaistruct.ValidationNotEqualError(b"\x52\x61\x72\x21\x1A\x07", self.magic1, self._io, u"/types/magic_signature/seq/0")
+            self._debug['version']['start'] = self._io.pos()
+            self.version = self._io.read_u1()
+            self._debug['version']['end'] = self._io.pos()
+            if self.version == 1:
+                self._debug['magic3']['start'] = self._io.pos()
+                self.magic3 = self._io.read_bytes(1)
+                self._debug['magic3']['end'] = self._io.pos()
+                if not self.magic3 == b"\x00":
+                    raise kaitaistruct.ValidationNotEqualError(b"\x00", self.magic3, self._io, u"/types/magic_signature/seq/2")
 
 
-    class Packet(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://wiki.wireshark.org/Development/LibpcapFileFormat#Record_.28Packet.29_Header
+
+    class Block(KaitaiStruct):
+        """Basic block that RAR files consist of. There are several block
+        types (see `block_type`), which have different `body` and
+        `add_body`.
         """
-        SEQ_FIELDS = ["ts_sec", "ts_usec", "incl_len", "orig_len", "body"]
+        SEQ_FIELDS = ["crc16", "block_type", "flags", "block_size", "add_size", "body", "add_body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['ts_sec']['start'] = self._io.pos()
-            self.ts_sec = self._io.read_u4le()
-            self._debug['ts_sec']['end'] = self._io.pos()
-            self._debug['ts_usec']['start'] = self._io.pos()
-            self.ts_usec = self._io.read_u4le()
-            self._debug['ts_usec']['end'] = self._io.pos()
-            self._debug['incl_len']['start'] = self._io.pos()
-            self.incl_len = self._io.read_u4le()
-            self._debug['incl_len']['end'] = self._io.pos()
-            self._debug['orig_len']['start'] = self._io.pos()
-            self.orig_len = self._io.read_u4le()
-            self._debug['orig_len']['end'] = self._io.pos()
+            self._debug['crc16']['start'] = self._io.pos()
+            self.crc16 = self._io.read_u2le()
+            self._debug['crc16']['end'] = self._io.pos()
+            self._debug['block_type']['start'] = self._io.pos()
+            self.block_type = KaitaiStream.resolve_enum(Rar.BlockTypes, self._io.read_u1())
+            self._debug['block_type']['end'] = self._io.pos()
+            self._debug['flags']['start'] = self._io.pos()
+            self.flags = self._io.read_u2le()
+            self._debug['flags']['end'] = self._io.pos()
+            self._debug['block_size']['start'] = self._io.pos()
+            self.block_size = self._io.read_u2le()
+            self._debug['block_size']['end'] = self._io.pos()
+            if self.has_add:
+                self._debug['add_size']['start'] = self._io.pos()
+                self.add_size = self._io.read_u4le()
+                self._debug['add_size']['end'] = self._io.pos()
+
             self._debug['body']['start'] = self._io.pos()
-            _on = self._root.hdr.network
-            if _on == Pcap.Linktype.ppi:
-                self._raw_body = self._io.read_bytes(self.incl_len)
+            _on = self.block_type
+            if _on == Rar.BlockTypes.file_header:
+                self._raw_body = self._io.read_bytes(self.body_size)
                 _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = packet_ppi.PacketPpi(_io__raw_body)
-                self.body._read()
-            elif _on == Pcap.Linktype.ethernet:
-                self._raw_body = self._io.read_bytes(self.incl_len)
-                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = ethernet_frame.EthernetFrame(_io__raw_body)
+                self.body = Rar.BlockFileHeader(_io__raw_body, self, self._root)
                 self.body._read()
             else:
-                self.body = self._io.read_bytes(self.incl_len)
+                self.body = self._io.read_bytes(self.body_size)
             self._debug['body']['end'] = self._io.pos()
+            if self.has_add:
+                self._debug['add_body']['start'] = self._io.pos()
+                self.add_body = self._io.read_bytes(self.add_size)
+                self._debug['add_body']['end'] = self._io.pos()
+
+
+        @property
+        def has_add(self):
+            """True if block has additional content attached to it."""
+            if hasattr(self, '_m_has_add'):
+                return self._m_has_add
+
+            self._m_has_add = (self.flags & 32768) != 0
+            return getattr(self, '_m_has_add', None)
+
+        @property
+        def header_size(self):
+            if hasattr(self, '_m_header_size'):
+                return self._m_header_size
+
+            self._m_header_size = (11 if self.has_add else 7)
+            return getattr(self, '_m_header_size', None)
+
+        @property
+        def body_size(self):
+            if hasattr(self, '_m_body_size'):
+                return self._m_body_size
+
+            self._m_body_size = (self.block_size - self.header_size)
+            return getattr(self, '_m_body_size', None)
+
+
+    class BlockFileHeader(KaitaiStruct):
+        SEQ_FIELDS = ["low_unp_size", "host_os", "file_crc32", "file_time", "rar_version", "method", "name_size", "attr", "high_pack_size", "file_name", "salt"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['low_unp_size']['start'] = self._io.pos()
+            self.low_unp_size = self._io.read_u4le()
+            self._debug['low_unp_size']['end'] = self._io.pos()
+            self._debug['host_os']['start'] = self._io.pos()
+            self.host_os = KaitaiStream.resolve_enum(Rar.Oses, self._io.read_u1())
+            self._debug['host_os']['end'] = self._io.pos()
+            self._debug['file_crc32']['start'] = self._io.pos()
+            self.file_crc32 = self._io.read_u4le()
+            self._debug['file_crc32']['end'] = self._io.pos()
+            self._debug['file_time']['start'] = self._io.pos()
+            self._raw_file_time = self._io.read_bytes(4)
+            _io__raw_file_time = KaitaiStream(BytesIO(self._raw_file_time))
+            self.file_time = dos_datetime.DosDatetime(_io__raw_file_time)
+            self.file_time._read()
+            self._debug['file_time']['end'] = self._io.pos()
+            self._debug['rar_version']['start'] = self._io.pos()
+            self.rar_version = self._io.read_u1()
+            self._debug['rar_version']['end'] = self._io.pos()
+            self._debug['method']['start'] = self._io.pos()
+            self.method = KaitaiStream.resolve_enum(Rar.Methods, self._io.read_u1())
+            self._debug['method']['end'] = self._io.pos()
+            self._debug['name_size']['start'] = self._io.pos()
+            self.name_size = self._io.read_u2le()
+            self._debug['name_size']['end'] = self._io.pos()
+            self._debug['attr']['start'] = self._io.pos()
+            self.attr = self._io.read_u4le()
+            self._debug['attr']['end'] = self._io.pos()
+            if (self._parent.flags & 256) != 0:
+                self._debug['high_pack_size']['start'] = self._io.pos()
+                self.high_pack_size = self._io.read_u4le()
+                self._debug['high_pack_size']['end'] = self._io.pos()
+
+            self._debug['file_name']['start'] = self._io.pos()
+            self.file_name = self._io.read_bytes(self.name_size)
+            self._debug['file_name']['end'] = self._io.pos()
+            if (self._parent.flags & 1024) != 0:
+                self._debug['salt']['start'] = self._io.pos()
+                self.salt = self._io.read_u8le()
+                self._debug['salt']['end'] = self._io.pos()
+
+
+
+    class BlockV5(KaitaiStruct):
+        SEQ_FIELDS = []
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            pass
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/pcf_font.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/pcf_font.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/pcx.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/pcx.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/pcx_dcx.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/pcx_dcx.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/phar_without_stub.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/phar_without_stub.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/php_serialized_value.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/php_serialized_value.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/png.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/png.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
             self.value = self._io.read_u2be()
             self._debug['value']['end'] = self._io.pos()
 
 
     class ChrmChunk(KaitaiStruct):
         """
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11cHRM
+           Source - https://www.w3.org/TR/png/#11cHRM
         """
         SEQ_FIELDS = ["white_point", "red", "green", "blue"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -415,15 +415,15 @@
             self.blue._read()
             self._debug['blue']['end'] = self._io.pos()
 
 
     class IhdrChunk(KaitaiStruct):
         """
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11IHDR
+           Source - https://www.w3.org/TR/png/#11IHDR
         """
         SEQ_FIELDS = ["width", "height", "bit_depth", "color_type", "compression_method", "filter_method", "interlace_method"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -451,15 +451,15 @@
             self.interlace_method = self._io.read_u1()
             self._debug['interlace_method']['end'] = self._io.pos()
 
 
     class PlteChunk(KaitaiStruct):
         """
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11PLTE
+           Source - https://www.w3.org/TR/png/#11PLTE
         """
         SEQ_FIELDS = ["entries"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -480,15 +480,15 @@
 
             self._debug['entries']['end'] = self._io.pos()
 
 
     class SrgbChunk(KaitaiStruct):
         """
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11sRGB
+           Source - https://www.w3.org/TR/png/#11sRGB
         """
 
         class Intent(Enum):
             perceptual = 0
             relative_colorimetric = 1
             saturation = 2
             absolute_colorimetric = 3
@@ -507,15 +507,15 @@
 
     class CompressedTextChunk(KaitaiStruct):
         """Compressed text chunk effectively allows to store key-value
         string pairs in PNG container, compressing "value" part (which
         can be quite lengthy) with zlib compression.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11zTXt
+           Source - https://www.w3.org/TR/png/#11zTXt
         """
         SEQ_FIELDS = ["keyword", "compression_method", "text_datastream"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -574,15 +574,15 @@
             self.blue = self._io.read_u2be()
             self._debug['blue']['end'] = self._io.pos()
 
 
     class GamaChunk(KaitaiStruct):
         """
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11gAMA
+           Source - https://www.w3.org/TR/png/#11gAMA
         """
         SEQ_FIELDS = ["gamma_int"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -602,15 +602,15 @@
 
 
     class BkgdChunk(KaitaiStruct):
         """Background chunk stores default background color to display this
         image against. Contents depend on `color_type` of the image.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11bKGD
+           Source - https://www.w3.org/TR/png/#11bKGD
         """
         SEQ_FIELDS = ["bkgd"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -637,15 +637,15 @@
 
 
     class PhysChunk(KaitaiStruct):
         """"Physical size" chunk stores data that allows to translate
         logical pixels into physical units (meters, etc) and vice-versa.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11pHYs
+           Source - https://www.w3.org/TR/png/#11pHYs
         """
         SEQ_FIELDS = ["pixels_per_unit_x", "pixels_per_unit_y", "unit"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -728,15 +728,15 @@
     class InternationalTextChunk(KaitaiStruct):
         """International text chunk effectively allows to store key-value string pairs in
         PNG container. Both "key" (keyword) and "value" (text) parts are
         given in pre-defined subset of iso8859-1 without control
         characters.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11iTXt
+           Source - https://www.w3.org/TR/png/#11iTXt
         """
         SEQ_FIELDS = ["keyword", "compression_flag", "compression_method", "language_tag", "translated_keyword", "text"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -765,15 +765,15 @@
     class TextChunk(KaitaiStruct):
         """Text chunk effectively allows to store key-value string pairs in
         PNG container. Both "key" (keyword) and "value" (text) parts are
         given in pre-defined subset of iso8859-1 without control
         characters.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11tEXt
+           Source - https://www.w3.org/TR/png/#11tEXt
         """
         SEQ_FIELDS = ["keyword", "text"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -809,15 +809,15 @@
 
 
     class TimeChunk(KaitaiStruct):
         """Time chunk stores time stamp of last modification of this image,
         up to 1 second precision in UTC timezone.
         
         .. seealso::
-           Source - https://www.w3.org/TR/PNG/#11tIME
+           Source - https://www.w3.org/TR/png/#11tIME
         """
         SEQ_FIELDS = ["year", "month", "day", "hour", "minute", "second"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/protocol_body.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/protocol_body.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/psx_tim.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/psx_tim.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 class PsxTim(KaitaiStruct):
     """
     .. seealso::
        Source - http://fileformats.archiveteam.org/wiki/TIM_(PlayStation_graphics)
     
     
     .. seealso::
-       Source - http://mrclick.zophar.net/TilEd/download/timgfx.txt
+       Source - https://mrclick.zophar.net/TilEd/download/timgfx.txt
     
     
     .. seealso::
        Source - https://www.romhacking.net/documents/31/
     """
 
     class BppType(Enum):
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/python_pickle.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/python_pickle.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,21 +150,21 @@
     can cause arbitrary code execution.
     
     Pickle format has evolved with Python, later protocols add opcodes & types.
     Later Python releases can pickle to or unpickle from any earlier protocol.
     
     * Protocol 0: ASCII clean, no explicit version, fields are '\n' terminated.
     * Protocol 1: Binary, no explicit version, first length prefixed types.
-    * Protocol 2: Python 2.3+. Explicit versioning, more length prefixed types.
-      https://www.python.org/dev/peps/pep-0307/
+    * Protocol 2 ([PEP 307](https://peps.python.org/pep-0307/)): Python 2.3+.
+      Explicit versioning, more length prefixed types.
     * Protocol 3: Python 3.0+. Dedicated opcodes for `bytes` objects.
-    * Protocol 4: Python 3.4+. Opcodes for 64 bit strings, framing, `set`.
-      https://www.python.org/dev/peps/pep-3154/
-    * Protocol 5: Python 3.8+: Opcodes for `bytearray` and out of band data
-      https://www.python.org/dev/peps/pep-0574/
+    * Protocol 4 ([PEP 3154](https://peps.python.org/pep-3154/)): Python 3.4+.
+      Opcodes for 64 bit strings, framing, `set`.
+    * Protocol 5 ([PEP 574](https://peps.python.org/pep-0574/)): Python 3.8+:
+    Opcodes for `bytearray` and out of band data
     
     .. seealso::
        Source - https://github.com/python/cpython/blob/v3.8.1/Lib/pickletools.py
     """
 
     class Opcode(Enum):
         mark = 40
@@ -472,15 +472,15 @@
         Instead, opcodes and types with a known encoding are used.
         When unpickling
         
         - `pickle.Unpickler` objects default to ASCII, which can be overriden
         - `pickletools.dis` uses latin1, and cannot be overriden
         
         .. seealso::
-           Source - https://github.com/python/cpython/blob/bb8071a4/Lib/pickle.py#L486-L495
+           Source - https://github.com/python/cpython/blob/bb8071a4cae/Lib/pickle.py#L486-L495
         """
         SEQ_FIELDS = ["len", "val"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -593,15 +593,15 @@
         
         Although the len field is signed, any length < 0 will raise an exception
         during unpickling.
         
         See the documentation for `string1` for further detail about encodings.
         
         .. seealso::
-           Source - https://github.com/python/cpython/blob/bb8071a4/Lib/pickle.py#L486-L495
+           Source - https://github.com/python/cpython/blob/bb8071a4cae/Lib/pickle.py#L486-L495
         """
         SEQ_FIELDS = ["len", "val"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/python_pyc_27.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/python_pyc_27.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/quake_mdl.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_evt_log.py`

 * *Files 15% similar despite different names*

```diff
@@ -125,382 +125,305 @@
 
 
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
 import collections
+from enum import Enum
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-class QuakeMdl(KaitaiStruct):
-    SEQ_FIELDS = ["header", "skins", "texture_coordinates", "triangles", "frames"]
+class WindowsEvtLog(KaitaiStruct):
+    """EVT files are Windows Event Log files written by older Windows
+    operating systems (2000, XP, 2003). They are used as binary log
+    files by several major Windows subsystems and
+    applications. Typically, several of them can be found in
+    `%WINDIR%\system32\config` directory:
+    
+    * Application = `AppEvent.evt`
+    * System = `SysEvent.evt`
+    * Security = `SecEvent.evt`
+    
+    Alternatively, one can export any system event log as distinct .evt
+    file using relevant option in Event Viewer application.
+    
+    A Windows application can submit an entry into these logs using
+    [ReportEventA](https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-reporteventa)
+    function of Windows API.
+    
+    Internally, EVT files consist of a fixed-size header and event
+    records. There are several usage scenarios (non-wrapping vs wrapping
+    log files) which result in slightly different organization of
+    records.
+    
+    .. seealso::
+       Source - https://learn.microsoft.com/en-us/windows/win32/eventlog/event-log-file-format
+    """
+    SEQ_FIELDS = ["header", "records"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
         self._debug['header']['start'] = self._io.pos()
-        self.header = QuakeMdl.MdlHeader(self._io, self, self._root)
+        self.header = WindowsEvtLog.Header(self._io, self, self._root)
         self.header._read()
         self._debug['header']['end'] = self._io.pos()
-        self._debug['skins']['start'] = self._io.pos()
-        self.skins = []
-        for i in range(self.header.num_skins):
-            if not 'arr' in self._debug['skins']:
-                self._debug['skins']['arr'] = []
-            self._debug['skins']['arr'].append({'start': self._io.pos()})
-            _t_skins = QuakeMdl.MdlSkin(self._io, self, self._root)
-            _t_skins._read()
-            self.skins.append(_t_skins)
-            self._debug['skins']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['skins']['end'] = self._io.pos()
-        self._debug['texture_coordinates']['start'] = self._io.pos()
-        self.texture_coordinates = []
-        for i in range(self.header.num_verts):
-            if not 'arr' in self._debug['texture_coordinates']:
-                self._debug['texture_coordinates']['arr'] = []
-            self._debug['texture_coordinates']['arr'].append({'start': self._io.pos()})
-            _t_texture_coordinates = QuakeMdl.MdlTexcoord(self._io, self, self._root)
-            _t_texture_coordinates._read()
-            self.texture_coordinates.append(_t_texture_coordinates)
-            self._debug['texture_coordinates']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['texture_coordinates']['end'] = self._io.pos()
-        self._debug['triangles']['start'] = self._io.pos()
-        self.triangles = []
-        for i in range(self.header.num_tris):
-            if not 'arr' in self._debug['triangles']:
-                self._debug['triangles']['arr'] = []
-            self._debug['triangles']['arr'].append({'start': self._io.pos()})
-            _t_triangles = QuakeMdl.MdlTriangle(self._io, self, self._root)
-            _t_triangles._read()
-            self.triangles.append(_t_triangles)
-            self._debug['triangles']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['triangles']['end'] = self._io.pos()
-        self._debug['frames']['start'] = self._io.pos()
-        self.frames = []
-        for i in range(self.header.num_frames):
-            if not 'arr' in self._debug['frames']:
-                self._debug['frames']['arr'] = []
-            self._debug['frames']['arr'].append({'start': self._io.pos()})
-            _t_frames = QuakeMdl.MdlFrame(self._io, self, self._root)
-            _t_frames._read()
-            self.frames.append(_t_frames)
-            self._debug['frames']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['frames']['end'] = self._io.pos()
-
-    class MdlVertex(KaitaiStruct):
-        SEQ_FIELDS = ["values", "normal_index"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['values']['start'] = self._io.pos()
-            self.values = []
-            for i in range(3):
-                if not 'arr' in self._debug['values']:
-                    self._debug['values']['arr'] = []
-                self._debug['values']['arr'].append({'start': self._io.pos()})
-                self.values.append(self._io.read_u1())
-                self._debug['values']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['values']['end'] = self._io.pos()
-            self._debug['normal_index']['start'] = self._io.pos()
-            self.normal_index = self._io.read_u1()
-            self._debug['normal_index']['end'] = self._io.pos()
-
-
-    class MdlTexcoord(KaitaiStruct):
-        SEQ_FIELDS = ["on_seam", "s", "t"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['on_seam']['start'] = self._io.pos()
-            self.on_seam = self._io.read_s4le()
-            self._debug['on_seam']['end'] = self._io.pos()
-            self._debug['s']['start'] = self._io.pos()
-            self.s = self._io.read_s4le()
-            self._debug['s']['end'] = self._io.pos()
-            self._debug['t']['start'] = self._io.pos()
-            self.t = self._io.read_s4le()
-            self._debug['t']['end'] = self._io.pos()
-
-
-    class MdlHeader(KaitaiStruct):
-        SEQ_FIELDS = ["ident", "version_must_be_6", "scale", "origin", "radius", "eye_position", "num_skins", "skin_width", "skin_height", "num_verts", "num_tris", "num_frames", "synctype", "flags", "size"]
+        self._debug['records']['start'] = self._io.pos()
+        self.records = []
+        i = 0
+        while not self._io.is_eof():
+            if not 'arr' in self._debug['records']:
+                self._debug['records']['arr'] = []
+            self._debug['records']['arr'].append({'start': self._io.pos()})
+            _t_records = WindowsEvtLog.Record(self._io, self, self._root)
+            _t_records._read()
+            self.records.append(_t_records)
+            self._debug['records']['arr'][len(self.records) - 1]['end'] = self._io.pos()
+            i += 1
+
+        self._debug['records']['end'] = self._io.pos()
+
+    class Header(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/previous-versions/windows/desktop/legacy/bb309024(v=vs.85)
+        """
+        SEQ_FIELDS = ["len_header", "magic", "version_major", "version_minor", "ofs_start", "ofs_end", "cur_rec_idx", "oldest_rec_idx", "len_file_max", "flags", "retention", "len_header_2"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['ident']['start'] = self._io.pos()
-            self.ident = self._io.read_bytes(4)
-            self._debug['ident']['end'] = self._io.pos()
-            if not self.ident == b"\x49\x44\x50\x4F":
-                raise kaitaistruct.ValidationNotEqualError(b"\x49\x44\x50\x4F", self.ident, self._io, u"/types/mdl_header/seq/0")
-            self._debug['version_must_be_6']['start'] = self._io.pos()
-            self.version_must_be_6 = self._io.read_bytes(4)
-            self._debug['version_must_be_6']['end'] = self._io.pos()
-            if not self.version_must_be_6 == b"\x06\x00\x00\x00":
-                raise kaitaistruct.ValidationNotEqualError(b"\x06\x00\x00\x00", self.version_must_be_6, self._io, u"/types/mdl_header/seq/1")
-            self._debug['scale']['start'] = self._io.pos()
-            self.scale = QuakeMdl.Vec3(self._io, self, self._root)
-            self.scale._read()
-            self._debug['scale']['end'] = self._io.pos()
-            self._debug['origin']['start'] = self._io.pos()
-            self.origin = QuakeMdl.Vec3(self._io, self, self._root)
-            self.origin._read()
-            self._debug['origin']['end'] = self._io.pos()
-            self._debug['radius']['start'] = self._io.pos()
-            self.radius = self._io.read_f4le()
-            self._debug['radius']['end'] = self._io.pos()
-            self._debug['eye_position']['start'] = self._io.pos()
-            self.eye_position = QuakeMdl.Vec3(self._io, self, self._root)
-            self.eye_position._read()
-            self._debug['eye_position']['end'] = self._io.pos()
-            self._debug['num_skins']['start'] = self._io.pos()
-            self.num_skins = self._io.read_s4le()
-            self._debug['num_skins']['end'] = self._io.pos()
-            self._debug['skin_width']['start'] = self._io.pos()
-            self.skin_width = self._io.read_s4le()
-            self._debug['skin_width']['end'] = self._io.pos()
-            self._debug['skin_height']['start'] = self._io.pos()
-            self.skin_height = self._io.read_s4le()
-            self._debug['skin_height']['end'] = self._io.pos()
-            self._debug['num_verts']['start'] = self._io.pos()
-            self.num_verts = self._io.read_s4le()
-            self._debug['num_verts']['end'] = self._io.pos()
-            self._debug['num_tris']['start'] = self._io.pos()
-            self.num_tris = self._io.read_s4le()
-            self._debug['num_tris']['end'] = self._io.pos()
-            self._debug['num_frames']['start'] = self._io.pos()
-            self.num_frames = self._io.read_s4le()
-            self._debug['num_frames']['end'] = self._io.pos()
-            self._debug['synctype']['start'] = self._io.pos()
-            self.synctype = self._io.read_s4le()
-            self._debug['synctype']['end'] = self._io.pos()
+            self._debug['len_header']['start'] = self._io.pos()
+            self.len_header = self._io.read_u4le()
+            self._debug['len_header']['end'] = self._io.pos()
+            self._debug['magic']['start'] = self._io.pos()
+            self.magic = self._io.read_bytes(4)
+            self._debug['magic']['end'] = self._io.pos()
+            if not self.magic == b"\x4C\x66\x4C\x65":
+                raise kaitaistruct.ValidationNotEqualError(b"\x4C\x66\x4C\x65", self.magic, self._io, u"/types/header/seq/1")
+            self._debug['version_major']['start'] = self._io.pos()
+            self.version_major = self._io.read_u4le()
+            self._debug['version_major']['end'] = self._io.pos()
+            self._debug['version_minor']['start'] = self._io.pos()
+            self.version_minor = self._io.read_u4le()
+            self._debug['version_minor']['end'] = self._io.pos()
+            self._debug['ofs_start']['start'] = self._io.pos()
+            self.ofs_start = self._io.read_u4le()
+            self._debug['ofs_start']['end'] = self._io.pos()
+            self._debug['ofs_end']['start'] = self._io.pos()
+            self.ofs_end = self._io.read_u4le()
+            self._debug['ofs_end']['end'] = self._io.pos()
+            self._debug['cur_rec_idx']['start'] = self._io.pos()
+            self.cur_rec_idx = self._io.read_u4le()
+            self._debug['cur_rec_idx']['end'] = self._io.pos()
+            self._debug['oldest_rec_idx']['start'] = self._io.pos()
+            self.oldest_rec_idx = self._io.read_u4le()
+            self._debug['oldest_rec_idx']['end'] = self._io.pos()
+            self._debug['len_file_max']['start'] = self._io.pos()
+            self.len_file_max = self._io.read_u4le()
+            self._debug['len_file_max']['end'] = self._io.pos()
             self._debug['flags']['start'] = self._io.pos()
-            self.flags = self._io.read_s4le()
+            self.flags = WindowsEvtLog.Header.Flags(self._io, self, self._root)
+            self.flags._read()
             self._debug['flags']['end'] = self._io.pos()
-            self._debug['size']['start'] = self._io.pos()
-            self.size = self._io.read_f4le()
-            self._debug['size']['end'] = self._io.pos()
-
-        @property
-        def version(self):
-            if hasattr(self, '_m_version'):
-                return self._m_version
-
-            self._m_version = 6
-            return getattr(self, '_m_version', None)
-
-        @property
-        def skin_size(self):
-            if hasattr(self, '_m_skin_size'):
-                return self._m_skin_size
+            self._debug['retention']['start'] = self._io.pos()
+            self.retention = self._io.read_u4le()
+            self._debug['retention']['end'] = self._io.pos()
+            self._debug['len_header_2']['start'] = self._io.pos()
+            self.len_header_2 = self._io.read_u4le()
+            self._debug['len_header_2']['end'] = self._io.pos()
+
+        class Flags(KaitaiStruct):
+            SEQ_FIELDS = ["reserved", "archive", "log_full", "wrap", "dirty"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['reserved']['start'] = self._io.pos()
+                self.reserved = self._io.read_bits_int_be(28)
+                self._debug['reserved']['end'] = self._io.pos()
+                self._debug['archive']['start'] = self._io.pos()
+                self.archive = self._io.read_bits_int_be(1) != 0
+                self._debug['archive']['end'] = self._io.pos()
+                self._debug['log_full']['start'] = self._io.pos()
+                self.log_full = self._io.read_bits_int_be(1) != 0
+                self._debug['log_full']['end'] = self._io.pos()
+                self._debug['wrap']['start'] = self._io.pos()
+                self.wrap = self._io.read_bits_int_be(1) != 0
+                self._debug['wrap']['end'] = self._io.pos()
+                self._debug['dirty']['start'] = self._io.pos()
+                self.dirty = self._io.read_bits_int_be(1) != 0
+                self._debug['dirty']['end'] = self._io.pos()
 
-            self._m_skin_size = (self.skin_width * self.skin_height)
-            return getattr(self, '_m_skin_size', None)
 
 
-    class MdlSkin(KaitaiStruct):
-        SEQ_FIELDS = ["group", "single_texture_data", "num_frames", "frame_times", "group_texture_data"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['group']['start'] = self._io.pos()
-            self.group = self._io.read_s4le()
-            self._debug['group']['end'] = self._io.pos()
-            if self.group == 0:
-                self._debug['single_texture_data']['start'] = self._io.pos()
-                self.single_texture_data = self._io.read_bytes(self._root.header.skin_size)
-                self._debug['single_texture_data']['end'] = self._io.pos()
-
-            if self.group != 0:
-                self._debug['num_frames']['start'] = self._io.pos()
-                self.num_frames = self._io.read_u4le()
-                self._debug['num_frames']['end'] = self._io.pos()
-
-            if self.group != 0:
-                self._debug['frame_times']['start'] = self._io.pos()
-                self.frame_times = []
-                for i in range(self.num_frames):
-                    if not 'arr' in self._debug['frame_times']:
-                        self._debug['frame_times']['arr'] = []
-                    self._debug['frame_times']['arr'].append({'start': self._io.pos()})
-                    self.frame_times.append(self._io.read_f4le())
-                    self._debug['frame_times']['arr'][i]['end'] = self._io.pos()
-
-                self._debug['frame_times']['end'] = self._io.pos()
-
-            if self.group != 0:
-                self._debug['group_texture_data']['start'] = self._io.pos()
-                self.group_texture_data = []
-                for i in range(self.num_frames):
-                    if not 'arr' in self._debug['group_texture_data']:
-                        self._debug['group_texture_data']['arr'] = []
-                    self._debug['group_texture_data']['arr'].append({'start': self._io.pos()})
-                    self.group_texture_data.append(self._io.read_bytes(self._root.header.skin_size))
-                    self._debug['group_texture_data']['arr'][i]['end'] = self._io.pos()
-
-                self._debug['group_texture_data']['end'] = self._io.pos()
-
-
-
-    class MdlFrame(KaitaiStruct):
-        SEQ_FIELDS = ["type", "min", "max", "time", "frames"]
+    class Record(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/winnt/ns-winnt-eventlogrecord
+        """
+        SEQ_FIELDS = ["len_record", "type", "body", "len_record2"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
+            self._debug['len_record']['start'] = self._io.pos()
+            self.len_record = self._io.read_u4le()
+            self._debug['len_record']['end'] = self._io.pos()
             self._debug['type']['start'] = self._io.pos()
-            self.type = self._io.read_s4le()
+            self.type = self._io.read_u4le()
             self._debug['type']['end'] = self._io.pos()
-            if self.type != 0:
-                self._debug['min']['start'] = self._io.pos()
-                self.min = QuakeMdl.MdlVertex(self._io, self, self._root)
-                self.min._read()
-                self._debug['min']['end'] = self._io.pos()
-
-            if self.type != 0:
-                self._debug['max']['start'] = self._io.pos()
-                self.max = QuakeMdl.MdlVertex(self._io, self, self._root)
-                self.max._read()
-                self._debug['max']['end'] = self._io.pos()
-
-            if self.type != 0:
-                self._debug['time']['start'] = self._io.pos()
-                self.time = []
-                for i in range(self.type):
-                    if not 'arr' in self._debug['time']:
-                        self._debug['time']['arr'] = []
-                    self._debug['time']['arr'].append({'start': self._io.pos()})
-                    self.time.append(self._io.read_f4le())
-                    self._debug['time']['arr'][i]['end'] = self._io.pos()
-
-                self._debug['time']['end'] = self._io.pos()
-
-            self._debug['frames']['start'] = self._io.pos()
-            self.frames = []
-            for i in range(self.num_simple_frames):
-                if not 'arr' in self._debug['frames']:
-                    self._debug['frames']['arr'] = []
-                self._debug['frames']['arr'].append({'start': self._io.pos()})
-                _t_frames = QuakeMdl.MdlSimpleFrame(self._io, self, self._root)
-                _t_frames._read()
-                self.frames.append(_t_frames)
-                self._debug['frames']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['frames']['end'] = self._io.pos()
-
-        @property
-        def num_simple_frames(self):
-            if hasattr(self, '_m_num_simple_frames'):
-                return self._m_num_simple_frames
-
-            self._m_num_simple_frames = (1 if self.type == 0 else self.type)
-            return getattr(self, '_m_num_simple_frames', None)
-
-
-    class MdlSimpleFrame(KaitaiStruct):
-        SEQ_FIELDS = ["bbox_min", "bbox_max", "name", "vertices"]
+            self._debug['body']['start'] = self._io.pos()
+            _on = self.type
+            if _on == 1699505740:
+                self._raw_body = self._io.read_bytes((self.len_record - 12))
+                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                self.body = WindowsEvtLog.RecordBody(_io__raw_body, self, self._root)
+                self.body._read()
+            elif _on == 286331153:
+                self._raw_body = self._io.read_bytes((self.len_record - 12))
+                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                self.body = WindowsEvtLog.CursorRecordBody(_io__raw_body, self, self._root)
+                self.body._read()
+            else:
+                self.body = self._io.read_bytes((self.len_record - 12))
+            self._debug['body']['end'] = self._io.pos()
+            self._debug['len_record2']['start'] = self._io.pos()
+            self.len_record2 = self._io.read_u4le()
+            self._debug['len_record2']['end'] = self._io.pos()
+
+
+    class RecordBody(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/winnt/ns-winnt-eventlogrecord
+        """
+
+        class EventTypes(Enum):
+            error = 1
+            audit_failure = 2
+            audit_success = 3
+            info = 4
+            warning = 5
+        SEQ_FIELDS = ["idx", "time_generated", "time_written", "event_id", "event_type", "num_strings", "event_category", "reserved", "ofs_strings", "len_user_sid", "ofs_user_sid", "len_data", "ofs_data"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['bbox_min']['start'] = self._io.pos()
-            self.bbox_min = QuakeMdl.MdlVertex(self._io, self, self._root)
-            self.bbox_min._read()
-            self._debug['bbox_min']['end'] = self._io.pos()
-            self._debug['bbox_max']['start'] = self._io.pos()
-            self.bbox_max = QuakeMdl.MdlVertex(self._io, self, self._root)
-            self.bbox_max._read()
-            self._debug['bbox_max']['end'] = self._io.pos()
-            self._debug['name']['start'] = self._io.pos()
-            self.name = (KaitaiStream.bytes_terminate(KaitaiStream.bytes_strip_right(self._io.read_bytes(16), 0), 0, False)).decode(u"ASCII")
-            self._debug['name']['end'] = self._io.pos()
-            self._debug['vertices']['start'] = self._io.pos()
-            self.vertices = []
-            for i in range(self._root.header.num_verts):
-                if not 'arr' in self._debug['vertices']:
-                    self._debug['vertices']['arr'] = []
-                self._debug['vertices']['arr'].append({'start': self._io.pos()})
-                _t_vertices = QuakeMdl.MdlVertex(self._io, self, self._root)
-                _t_vertices._read()
-                self.vertices.append(_t_vertices)
-                self._debug['vertices']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['vertices']['end'] = self._io.pos()
-
-
-    class MdlTriangle(KaitaiStruct):
-        SEQ_FIELDS = ["faces_front", "vertices"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['faces_front']['start'] = self._io.pos()
-            self.faces_front = self._io.read_s4le()
-            self._debug['faces_front']['end'] = self._io.pos()
-            self._debug['vertices']['start'] = self._io.pos()
-            self.vertices = []
-            for i in range(3):
-                if not 'arr' in self._debug['vertices']:
-                    self._debug['vertices']['arr'] = []
-                self._debug['vertices']['arr'].append({'start': self._io.pos()})
-                self.vertices.append(self._io.read_s4le())
-                self._debug['vertices']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['vertices']['end'] = self._io.pos()
+            self._debug['idx']['start'] = self._io.pos()
+            self.idx = self._io.read_u4le()
+            self._debug['idx']['end'] = self._io.pos()
+            self._debug['time_generated']['start'] = self._io.pos()
+            self.time_generated = self._io.read_u4le()
+            self._debug['time_generated']['end'] = self._io.pos()
+            self._debug['time_written']['start'] = self._io.pos()
+            self.time_written = self._io.read_u4le()
+            self._debug['time_written']['end'] = self._io.pos()
+            self._debug['event_id']['start'] = self._io.pos()
+            self.event_id = self._io.read_u4le()
+            self._debug['event_id']['end'] = self._io.pos()
+            self._debug['event_type']['start'] = self._io.pos()
+            self.event_type = KaitaiStream.resolve_enum(WindowsEvtLog.RecordBody.EventTypes, self._io.read_u2le())
+            self._debug['event_type']['end'] = self._io.pos()
+            self._debug['num_strings']['start'] = self._io.pos()
+            self.num_strings = self._io.read_u2le()
+            self._debug['num_strings']['end'] = self._io.pos()
+            self._debug['event_category']['start'] = self._io.pos()
+            self.event_category = self._io.read_u2le()
+            self._debug['event_category']['end'] = self._io.pos()
+            self._debug['reserved']['start'] = self._io.pos()
+            self.reserved = self._io.read_bytes(6)
+            self._debug['reserved']['end'] = self._io.pos()
+            self._debug['ofs_strings']['start'] = self._io.pos()
+            self.ofs_strings = self._io.read_u4le()
+            self._debug['ofs_strings']['end'] = self._io.pos()
+            self._debug['len_user_sid']['start'] = self._io.pos()
+            self.len_user_sid = self._io.read_u4le()
+            self._debug['len_user_sid']['end'] = self._io.pos()
+            self._debug['ofs_user_sid']['start'] = self._io.pos()
+            self.ofs_user_sid = self._io.read_u4le()
+            self._debug['ofs_user_sid']['end'] = self._io.pos()
+            self._debug['len_data']['start'] = self._io.pos()
+            self.len_data = self._io.read_u4le()
+            self._debug['len_data']['end'] = self._io.pos()
+            self._debug['ofs_data']['start'] = self._io.pos()
+            self.ofs_data = self._io.read_u4le()
+            self._debug['ofs_data']['end'] = self._io.pos()
 
+        @property
+        def user_sid(self):
+            if hasattr(self, '_m_user_sid'):
+                return self._m_user_sid
+
+            _pos = self._io.pos()
+            self._io.seek((self.ofs_user_sid - 8))
+            self._debug['_m_user_sid']['start'] = self._io.pos()
+            self._m_user_sid = self._io.read_bytes(self.len_user_sid)
+            self._debug['_m_user_sid']['end'] = self._io.pos()
+            self._io.seek(_pos)
+            return getattr(self, '_m_user_sid', None)
 
-    class Vec3(KaitaiStruct):
-        SEQ_FIELDS = ["x", "y", "z"]
+        @property
+        def data(self):
+            if hasattr(self, '_m_data'):
+                return self._m_data
+
+            _pos = self._io.pos()
+            self._io.seek((self.ofs_data - 8))
+            self._debug['_m_data']['start'] = self._io.pos()
+            self._m_data = self._io.read_bytes(self.len_data)
+            self._debug['_m_data']['end'] = self._io.pos()
+            self._io.seek(_pos)
+            return getattr(self, '_m_data', None)
+
+
+    class CursorRecordBody(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://forensics.wiki/windows_event_log_(evt)/#cursor-record
+        """
+        SEQ_FIELDS = ["magic", "ofs_first_record", "ofs_next_record", "idx_next_record", "idx_first_record"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['x']['start'] = self._io.pos()
-            self.x = self._io.read_f4le()
-            self._debug['x']['end'] = self._io.pos()
-            self._debug['y']['start'] = self._io.pos()
-            self.y = self._io.read_f4le()
-            self._debug['y']['end'] = self._io.pos()
-            self._debug['z']['start'] = self._io.pos()
-            self.z = self._io.read_f4le()
-            self._debug['z']['end'] = self._io.pos()
+            self._debug['magic']['start'] = self._io.pos()
+            self.magic = self._io.read_bytes(12)
+            self._debug['magic']['end'] = self._io.pos()
+            if not self.magic == b"\x22\x22\x22\x22\x33\x33\x33\x33\x44\x44\x44\x44":
+                raise kaitaistruct.ValidationNotEqualError(b"\x22\x22\x22\x22\x33\x33\x33\x33\x44\x44\x44\x44", self.magic, self._io, u"/types/cursor_record_body/seq/0")
+            self._debug['ofs_first_record']['start'] = self._io.pos()
+            self.ofs_first_record = self._io.read_u4le()
+            self._debug['ofs_first_record']['end'] = self._io.pos()
+            self._debug['ofs_next_record']['start'] = self._io.pos()
+            self.ofs_next_record = self._io.read_u4le()
+            self._debug['ofs_next_record']['end'] = self._io.pos()
+            self._debug['idx_next_record']['start'] = self._io.pos()
+            self.idx_next_record = self._io.read_u4le()
+            self._debug['idx_next_record']['end'] = self._io.pos()
+            self._debug['idx_first_record']['start'] = self._io.pos()
+            self.idx_first_record = self._io.read_u4le()
+            self._debug['idx_first_record']['end'] = self._io.pos()
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/quake_pak.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/quake_pak.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/quicktime_mov.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/quicktime_mov.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class QuicktimeMov(KaitaiStruct):
     """
     .. seealso::
-       Source - https://developer.apple.com/library/content/documentation/QuickTime/QTFF/QTFFChap1/qtff1.html#//apple_ref/doc/uid/TP40000939-CH203-BBCGDDDF
+       Source - https://developer.apple.com/library/archive/documentation/QuickTime/QTFF/QTFFChap1/qtff1.html#//apple_ref/doc/uid/TP40000939-CH203-BBCGDDDF
     """
 
     class AtomType(Enum):
         xtra = 1484026465
         dinf = 1684631142
         dref = 1685218662
         edts = 1701082227
@@ -277,14 +277,15 @@
         csh1 = 1668507697
         cud1 = 1668637745
         cud2 = 1668637746
         cud8 = 1668637752
         cud9 = 1668637753
         cuvd = 1668642404
         cvid = 1668704612
+        cvvc = 1668707939
         cwvt = 1668773492
         da0a = 1684090977
         da0b = 1684090978
         da1a = 1684091233
         da1b = 1684091234
         da2a = 1684091489
         da2b = 1684091490
@@ -319,14 +320,19 @@
         hevs = 1751479923
         hevx = 1751479928
         hvce = 1752589157
         hvci = 1752589161
         hvcx = 1752589176
         hvti = 1752593513
         ifaa = 1768317281
+        ifah = 1768317288
+        ifai = 1768317289
+        ifas = 1768317299
+        ifau = 1768317301
+        ifav = 1768317302
         ifhd = 1768319076
         ifhh = 1768319080
         ifhr = 1768319090
         ifhs = 1768319091
         ifhu = 1768319093
         ifhx = 1768319096
         ifrm = 1768321645
@@ -401,23 +407,30 @@
         relo = 1919249519
         risx = 1919513464
         sdv = 1935963680
         senv = 1936027254
         sims = 1936289139
         sisx = 1936290680
         siti = 1936290921
+        sitv = 1936290934
         slh1 = 1936484401
         slh2 = 1936484402
         slh3 = 1936484403
         ssss = 1936946035
         ttml = 1953787244
         ttwv = 1953789814
         uhvi = 1969780329
         unif = 1970170214
         uvvu = 1970697845
+        v3mp = 1983081840
+        v3mt = 1983081844
+        v3nt = 1983082100
+        v3st = 1983083380
+        vvci = 1987470185
+        vvoi = 1987473257
         vwpt = 1987539060
         yt4 = 2037658656
     SEQ_FIELDS = ["atoms"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
@@ -428,15 +441,15 @@
         self.atoms = QuicktimeMov.AtomList(self._io, self, self._root)
         self.atoms._read()
         self._debug['atoms']['end'] = self._io.pos()
 
     class MvhdBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://developer.apple.com/library/content/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html#//apple_ref/doc/uid/TP40000939-CH204-BBCGFGJG
+           Source - https://developer.apple.com/library/archive/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html#//apple_ref/doc/uid/TP40000939-CH204-BBCGFGJG
         """
         SEQ_FIELDS = ["version", "flags", "creation_time", "modification_time", "time_scale", "duration", "preferred_rate", "preferred_volume", "reserved1", "matrix", "preview_time", "preview_duration", "poster_time", "selection_time", "selection_duration", "current_time", "next_track_id"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -496,15 +509,15 @@
             self.next_track_id = self._io.read_u4be()
             self._debug['next_track_id']['end'] = self._io.pos()
 
 
     class FtypBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://developer.apple.com/library/content/documentation/QuickTime/QTFF/QTFFChap1/qtff1.html#//apple_ref/doc/uid/TP40000939-CH203-CJBCBIFF
+           Source - https://developer.apple.com/library/archive/documentation/QuickTime/QTFF/QTFFChap1/qtff1.html#//apple_ref/doc/uid/TP40000939-CH203-CJBCBIFF
         """
         SEQ_FIELDS = ["major_brand", "minor_version", "compatible_brands"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -655,15 +668,15 @@
             self._m_len = ((self._io.size() - 8) if self.len32 == 0 else ((self.len64 - 16) if self.len32 == 1 else (self.len32 - 8)))
             return getattr(self, '_m_len', None)
 
 
     class TkhdBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://developer.apple.com/library/content/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html#//apple_ref/doc/uid/TP40000939-CH204-25550
+           Source - https://developer.apple.com/library/archive/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html#//apple_ref/doc/uid/TP40000939-CH204-25550
         """
         SEQ_FIELDS = ["version", "flags", "creation_time", "modification_time", "track_id", "reserved1", "duration", "reserved2", "layer", "alternative_group", "volume", "reserved3", "matrix", "width", "height"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/rar.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/uefi_te.py`

 * *Files 11% similar despite different names*

```diff
@@ -124,267 +124,238 @@
 # https://github.com/kaitai-io/kaitai_struct_formats
 
 
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
-from enum import Enum
 import collections
+from enum import Enum
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-import dos_datetime
-class Rar(KaitaiStruct):
-    """RAR is a archive format used by popular proprietary RAR archiver,
-    created by Eugene Roshal. There are two major versions of format
-    (v1.5-4.0 and RAR v5+).
+class UefiTe(KaitaiStruct):
+    """This type of executables could be found inside the UEFI firmware. The UEFI
+    firmware is stored in SPI flash memory, which is a chip soldered on a
+    system's motherboard. UEFI firmware is very modular: it usually contains
+    dozens, if not hundreds, of executables. To store all these separates files,
+    the firmware is laid out in volumes using the Firmware File System (FFS), a
+    file system specifically designed to store firmware images. The volumes
+    contain files that are identified by GUIDs and each of these files contain
+    one or more sections holding the data. One of these sections contains the
+    actual executable image. Most of the executable images follow the PE format.
+    However, some of them follow the TE format.
+    
+    The Terse Executable (TE) image format was created as a mechanism to reduce
+    the overhead of the PE/COFF headers in PE32/PE32+ images, resulting in a
+    corresponding reduction of image sizes for executables running in the PI
+    (Platform Initialization) Architecture environment. Reducing image size
+    provides an opportunity for use of a smaller system flash part.
     
-    File format essentially consists of a linear sequence of
-    blocks. Each block has fixed header and custom body (that depends on
-    block type), so it's possible to skip block even if one doesn't know
-    how to process a certain block type.
+    So the TE format is basically a stripped version of PE.
     
     .. seealso::
-       Source - http://acritum.com/winrar/rar-format
+       Source - https://uefi.org/sites/default/files/resources/PI_Spec_1_6.pdf
     """
-
-    class BlockTypes(Enum):
-        marker = 114
-        archive_header = 115
-        file_header = 116
-        old_style_comment_header = 117
-        old_style_authenticity_info_76 = 118
-        old_style_subblock = 119
-        old_style_recovery_record = 120
-        old_style_authenticity_info_79 = 121
-        subblock = 122
-        terminator = 123
-
-    class Oses(Enum):
-        ms_dos = 0
-        os_2 = 1
-        windows = 2
-        unix = 3
-        mac_os = 4
-        beos = 5
-
-    class Methods(Enum):
-        store = 48
-        fastest = 49
-        fast = 50
-        normal = 51
-        good = 52
-        best = 53
-    SEQ_FIELDS = ["magic", "blocks"]
+    SEQ_FIELDS = ["te_hdr", "sections"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
-        self._debug['magic']['start'] = self._io.pos()
-        self.magic = Rar.MagicSignature(self._io, self, self._root)
-        self.magic._read()
-        self._debug['magic']['end'] = self._io.pos()
-        self._debug['blocks']['start'] = self._io.pos()
-        self.blocks = []
-        i = 0
-        while not self._io.is_eof():
-            if not 'arr' in self._debug['blocks']:
-                self._debug['blocks']['arr'] = []
-            self._debug['blocks']['arr'].append({'start': self._io.pos()})
-            _on = self.magic.version
-            if _on == 0:
-                if not 'arr' in self._debug['blocks']:
-                    self._debug['blocks']['arr'] = []
-                self._debug['blocks']['arr'].append({'start': self._io.pos()})
-                _t_blocks = Rar.Block(self._io, self, self._root)
-                _t_blocks._read()
-                self.blocks.append(_t_blocks)
-                self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
-            elif _on == 1:
-                if not 'arr' in self._debug['blocks']:
-                    self._debug['blocks']['arr'] = []
-                self._debug['blocks']['arr'].append({'start': self._io.pos()})
-                _t_blocks = Rar.BlockV5(self._io, self, self._root)
-                _t_blocks._read()
-                self.blocks.append(_t_blocks)
-                self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
-            self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
-            i += 1
-
-        self._debug['blocks']['end'] = self._io.pos()
-
-    class MagicSignature(KaitaiStruct):
-        """RAR uses either 7-byte magic for RAR versions 1.5 to 4.0, and
-        8-byte magic (and pretty different block format) for v5+. This
-        type would parse and validate both versions of signature. Note
-        that actually this signature is a valid RAR "block": in theory,
-        one can omit signature reading at all, and read this normally,
-        as a block, if exact RAR version is known (and thus it's
-        possible to choose correct block format).
-        """
-        SEQ_FIELDS = ["magic1", "version", "magic3"]
+        self._debug['te_hdr']['start'] = self._io.pos()
+        self._raw_te_hdr = self._io.read_bytes(40)
+        _io__raw_te_hdr = KaitaiStream(BytesIO(self._raw_te_hdr))
+        self.te_hdr = UefiTe.TeHeader(_io__raw_te_hdr, self, self._root)
+        self.te_hdr._read()
+        self._debug['te_hdr']['end'] = self._io.pos()
+        self._debug['sections']['start'] = self._io.pos()
+        self.sections = []
+        for i in range(self.te_hdr.num_sections):
+            if not 'arr' in self._debug['sections']:
+                self._debug['sections']['arr'] = []
+            self._debug['sections']['arr'].append({'start': self._io.pos()})
+            _t_sections = UefiTe.Section(self._io, self, self._root)
+            _t_sections._read()
+            self.sections.append(_t_sections)
+            self._debug['sections']['arr'][i]['end'] = self._io.pos()
+
+        self._debug['sections']['end'] = self._io.pos()
+
+    class TeHeader(KaitaiStruct):
+
+        class MachineType(Enum):
+            unknown = 0
+            i386 = 332
+            r4000 = 358
+            wcemipsv2 = 361
+            alpha = 388
+            sh3 = 418
+            sh3dsp = 419
+            sh4 = 422
+            sh5 = 424
+            arm = 448
+            thumb = 450
+            armnt = 452
+            am33 = 467
+            powerpc = 496
+            powerpcfp = 497
+            ia64 = 512
+            mips16 = 614
+            mipsfpu = 870
+            mipsfpu16 = 1126
+            ebc = 3772
+            riscv32 = 20530
+            riscv64 = 20580
+            riscv128 = 20776
+            amd64 = 34404
+            m32r = 36929
+            arm64 = 43620
+
+        class SubsystemEnum(Enum):
+            unknown = 0
+            native = 1
+            windows_gui = 2
+            windows_cui = 3
+            posix_cui = 7
+            windows_ce_gui = 9
+            efi_application = 10
+            efi_boot_service_driver = 11
+            efi_runtime_driver = 12
+            efi_rom = 13
+            xbox = 14
+            windows_boot_application = 16
+        SEQ_FIELDS = ["magic", "machine", "num_sections", "subsystem", "stripped_size", "entry_point_addr", "base_of_code", "image_base", "data_dirs"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['magic1']['start'] = self._io.pos()
-            self.magic1 = self._io.read_bytes(6)
-            self._debug['magic1']['end'] = self._io.pos()
-            if not self.magic1 == b"\x52\x61\x72\x21\x1A\x07":
-                raise kaitaistruct.ValidationNotEqualError(b"\x52\x61\x72\x21\x1A\x07", self.magic1, self._io, u"/types/magic_signature/seq/0")
-            self._debug['version']['start'] = self._io.pos()
-            self.version = self._io.read_u1()
-            self._debug['version']['end'] = self._io.pos()
-            if self.version == 1:
-                self._debug['magic3']['start'] = self._io.pos()
-                self.magic3 = self._io.read_bytes(1)
-                self._debug['magic3']['end'] = self._io.pos()
-                if not self.magic3 == b"\x00":
-                    raise kaitaistruct.ValidationNotEqualError(b"\x00", self.magic3, self._io, u"/types/magic_signature/seq/2")
-
+            self._debug['magic']['start'] = self._io.pos()
+            self.magic = self._io.read_bytes(2)
+            self._debug['magic']['end'] = self._io.pos()
+            if not self.magic == b"\x56\x5A":
+                raise kaitaistruct.ValidationNotEqualError(b"\x56\x5A", self.magic, self._io, u"/types/te_header/seq/0")
+            self._debug['machine']['start'] = self._io.pos()
+            self.machine = KaitaiStream.resolve_enum(UefiTe.TeHeader.MachineType, self._io.read_u2le())
+            self._debug['machine']['end'] = self._io.pos()
+            self._debug['num_sections']['start'] = self._io.pos()
+            self.num_sections = self._io.read_u1()
+            self._debug['num_sections']['end'] = self._io.pos()
+            self._debug['subsystem']['start'] = self._io.pos()
+            self.subsystem = KaitaiStream.resolve_enum(UefiTe.TeHeader.SubsystemEnum, self._io.read_u1())
+            self._debug['subsystem']['end'] = self._io.pos()
+            self._debug['stripped_size']['start'] = self._io.pos()
+            self.stripped_size = self._io.read_u2le()
+            self._debug['stripped_size']['end'] = self._io.pos()
+            self._debug['entry_point_addr']['start'] = self._io.pos()
+            self.entry_point_addr = self._io.read_u4le()
+            self._debug['entry_point_addr']['end'] = self._io.pos()
+            self._debug['base_of_code']['start'] = self._io.pos()
+            self.base_of_code = self._io.read_u4le()
+            self._debug['base_of_code']['end'] = self._io.pos()
+            self._debug['image_base']['start'] = self._io.pos()
+            self.image_base = self._io.read_u8le()
+            self._debug['image_base']['end'] = self._io.pos()
+            self._debug['data_dirs']['start'] = self._io.pos()
+            self.data_dirs = UefiTe.HeaderDataDirs(self._io, self, self._root)
+            self.data_dirs._read()
+            self._debug['data_dirs']['end'] = self._io.pos()
 
 
-    class Block(KaitaiStruct):
-        """Basic block that RAR files consist of. There are several block
-        types (see `block_type`), which have different `body` and
-        `add_body`.
-        """
-        SEQ_FIELDS = ["crc16", "block_type", "flags", "block_size", "add_size", "body", "add_body"]
+    class HeaderDataDirs(KaitaiStruct):
+        SEQ_FIELDS = ["base_relocation_table", "debug"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['crc16']['start'] = self._io.pos()
-            self.crc16 = self._io.read_u2le()
-            self._debug['crc16']['end'] = self._io.pos()
-            self._debug['block_type']['start'] = self._io.pos()
-            self.block_type = KaitaiStream.resolve_enum(Rar.BlockTypes, self._io.read_u1())
-            self._debug['block_type']['end'] = self._io.pos()
-            self._debug['flags']['start'] = self._io.pos()
-            self.flags = self._io.read_u2le()
-            self._debug['flags']['end'] = self._io.pos()
-            self._debug['block_size']['start'] = self._io.pos()
-            self.block_size = self._io.read_u2le()
-            self._debug['block_size']['end'] = self._io.pos()
-            if self.has_add:
-                self._debug['add_size']['start'] = self._io.pos()
-                self.add_size = self._io.read_u4le()
-                self._debug['add_size']['end'] = self._io.pos()
-
-            self._debug['body']['start'] = self._io.pos()
-            _on = self.block_type
-            if _on == Rar.BlockTypes.file_header:
-                self._raw_body = self._io.read_bytes(self.body_size)
-                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = Rar.BlockFileHeader(_io__raw_body, self, self._root)
-                self.body._read()
-            else:
-                self.body = self._io.read_bytes(self.body_size)
-            self._debug['body']['end'] = self._io.pos()
-            if self.has_add:
-                self._debug['add_body']['start'] = self._io.pos()
-                self.add_body = self._io.read_bytes(self.add_size)
-                self._debug['add_body']['end'] = self._io.pos()
-
-
-        @property
-        def has_add(self):
-            """True if block has additional content attached to it."""
-            if hasattr(self, '_m_has_add'):
-                return self._m_has_add
-
-            self._m_has_add = (self.flags & 32768) != 0
-            return getattr(self, '_m_has_add', None)
+            self._debug['base_relocation_table']['start'] = self._io.pos()
+            self.base_relocation_table = UefiTe.DataDir(self._io, self, self._root)
+            self.base_relocation_table._read()
+            self._debug['base_relocation_table']['end'] = self._io.pos()
+            self._debug['debug']['start'] = self._io.pos()
+            self.debug = UefiTe.DataDir(self._io, self, self._root)
+            self.debug._read()
+            self._debug['debug']['end'] = self._io.pos()
 
-        @property
-        def header_size(self):
-            if hasattr(self, '_m_header_size'):
-                return self._m_header_size
-
-            self._m_header_size = (11 if self.has_add else 7)
-            return getattr(self, '_m_header_size', None)
-
-        @property
-        def body_size(self):
-            if hasattr(self, '_m_body_size'):
-                return self._m_body_size
-
-            self._m_body_size = (self.block_size - self.header_size)
-            return getattr(self, '_m_body_size', None)
 
-
-    class BlockFileHeader(KaitaiStruct):
-        SEQ_FIELDS = ["low_unp_size", "host_os", "file_crc32", "file_time", "rar_version", "method", "name_size", "attr", "high_pack_size", "file_name", "salt"]
+    class DataDir(KaitaiStruct):
+        SEQ_FIELDS = ["virtual_address", "size"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['low_unp_size']['start'] = self._io.pos()
-            self.low_unp_size = self._io.read_u4le()
-            self._debug['low_unp_size']['end'] = self._io.pos()
-            self._debug['host_os']['start'] = self._io.pos()
-            self.host_os = KaitaiStream.resolve_enum(Rar.Oses, self._io.read_u1())
-            self._debug['host_os']['end'] = self._io.pos()
-            self._debug['file_crc32']['start'] = self._io.pos()
-            self.file_crc32 = self._io.read_u4le()
-            self._debug['file_crc32']['end'] = self._io.pos()
-            self._debug['file_time']['start'] = self._io.pos()
-            self._raw_file_time = self._io.read_bytes(4)
-            _io__raw_file_time = KaitaiStream(BytesIO(self._raw_file_time))
-            self.file_time = dos_datetime.DosDatetime(_io__raw_file_time)
-            self.file_time._read()
-            self._debug['file_time']['end'] = self._io.pos()
-            self._debug['rar_version']['start'] = self._io.pos()
-            self.rar_version = self._io.read_u1()
-            self._debug['rar_version']['end'] = self._io.pos()
-            self._debug['method']['start'] = self._io.pos()
-            self.method = KaitaiStream.resolve_enum(Rar.Methods, self._io.read_u1())
-            self._debug['method']['end'] = self._io.pos()
-            self._debug['name_size']['start'] = self._io.pos()
-            self.name_size = self._io.read_u2le()
-            self._debug['name_size']['end'] = self._io.pos()
-            self._debug['attr']['start'] = self._io.pos()
-            self.attr = self._io.read_u4le()
-            self._debug['attr']['end'] = self._io.pos()
-            if (self._parent.flags & 256) != 0:
-                self._debug['high_pack_size']['start'] = self._io.pos()
-                self.high_pack_size = self._io.read_u4le()
-                self._debug['high_pack_size']['end'] = self._io.pos()
-
-            self._debug['file_name']['start'] = self._io.pos()
-            self.file_name = self._io.read_bytes(self.name_size)
-            self._debug['file_name']['end'] = self._io.pos()
-            if (self._parent.flags & 1024) != 0:
-                self._debug['salt']['start'] = self._io.pos()
-                self.salt = self._io.read_u8le()
-                self._debug['salt']['end'] = self._io.pos()
-
+            self._debug['virtual_address']['start'] = self._io.pos()
+            self.virtual_address = self._io.read_u4le()
+            self._debug['virtual_address']['end'] = self._io.pos()
+            self._debug['size']['start'] = self._io.pos()
+            self.size = self._io.read_u4le()
+            self._debug['size']['end'] = self._io.pos()
 
 
-    class BlockV5(KaitaiStruct):
-        SEQ_FIELDS = []
+    class Section(KaitaiStruct):
+        SEQ_FIELDS = ["name", "virtual_size", "virtual_address", "size_of_raw_data", "pointer_to_raw_data", "pointer_to_relocations", "pointer_to_linenumbers", "num_relocations", "num_linenumbers", "characteristics"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            pass
+            self._debug['name']['start'] = self._io.pos()
+            self.name = (KaitaiStream.bytes_strip_right(self._io.read_bytes(8), 0)).decode(u"UTF-8")
+            self._debug['name']['end'] = self._io.pos()
+            self._debug['virtual_size']['start'] = self._io.pos()
+            self.virtual_size = self._io.read_u4le()
+            self._debug['virtual_size']['end'] = self._io.pos()
+            self._debug['virtual_address']['start'] = self._io.pos()
+            self.virtual_address = self._io.read_u4le()
+            self._debug['virtual_address']['end'] = self._io.pos()
+            self._debug['size_of_raw_data']['start'] = self._io.pos()
+            self.size_of_raw_data = self._io.read_u4le()
+            self._debug['size_of_raw_data']['end'] = self._io.pos()
+            self._debug['pointer_to_raw_data']['start'] = self._io.pos()
+            self.pointer_to_raw_data = self._io.read_u4le()
+            self._debug['pointer_to_raw_data']['end'] = self._io.pos()
+            self._debug['pointer_to_relocations']['start'] = self._io.pos()
+            self.pointer_to_relocations = self._io.read_u4le()
+            self._debug['pointer_to_relocations']['end'] = self._io.pos()
+            self._debug['pointer_to_linenumbers']['start'] = self._io.pos()
+            self.pointer_to_linenumbers = self._io.read_u4le()
+            self._debug['pointer_to_linenumbers']['end'] = self._io.pos()
+            self._debug['num_relocations']['start'] = self._io.pos()
+            self.num_relocations = self._io.read_u2le()
+            self._debug['num_relocations']['end'] = self._io.pos()
+            self._debug['num_linenumbers']['start'] = self._io.pos()
+            self.num_linenumbers = self._io.read_u2le()
+            self._debug['num_linenumbers']['end'] = self._io.pos()
+            self._debug['characteristics']['start'] = self._io.pos()
+            self.characteristics = self._io.read_u4le()
+            self._debug['characteristics']['end'] = self._io.pos()
+
+        @property
+        def body(self):
+            if hasattr(self, '_m_body'):
+                return self._m_body
+
+            _pos = self._io.pos()
+            self._io.seek(((self.pointer_to_raw_data - self._root.te_hdr.stripped_size) + self._root.te_hdr._io.size()))
+            self._debug['_m_body']['start'] = self._io.pos()
+            self._m_body = self._io.read_bytes(self.size_of_raw_data)
+            self._debug['_m_body']['end'] = self._io.pos()
+            self._io.seek(_pos)
+            return getattr(self, '_m_body', None)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/regf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/regf.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
       * `%USERPROFILE%\Local Settings\Application Data\Microsoft\Windows\Usrclass.dat` (localized, Windows 2000, Server 2003 and Windows XP)
       * `%USERPROFILE%\AppData\Local\Microsoft\Windows\Usrclass.dat` (non-localized, Windows Vista and later)
     
     Note that one typically can't access files directly on a mounted
     filesystem with a running Windows OS.
     
     .. seealso::
-       Source - https://github.com/libyal/libregf/blob/master/documentation/Windows%20NT%20Registry%20File%20(REGF)%20format.asciidoc
+       Source - https://github.com/libyal/libregf/blob/main/documentation/Windows%20NT%20Registry%20File%20(REGF)%20format.asciidoc
     """
     SEQ_FIELDS = ["header", "hive_bins"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/resource_fork.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/resource_fork.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     such as custom file icons.
     
     .. seealso::
        Inside Macintosh, More Macintosh Toolbox, Resource Manager, Resource Manager Reference, Resource File Format - https://developer.apple.com/library/archive/documentation/mac/pdf/MoreMacintoshToolbox.pdf#page=151
     
     
     .. seealso::
-       Inside Macintosh, Volume I, The Resource Manager, Format of a Resource File - http://www.pagetable.com/?p=50
+       Inside Macintosh, Volume I, The Resource Manager, Format of a Resource File - https://www.pagetable.com/?p=50
     
     
     .. seealso::
        Source - https://github.com/kreativekorp/ksfl/wiki/Macintosh-Resource-File-Format
     
     
     .. seealso::
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/riff.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/riff.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/rpm.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/rpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,19 +139,19 @@
     """This parser is for the RPM version 3 file format which is the current version
     of the file format used by RPM 2.1 and later (including RPM version 4.x, which
     is the current version of the RPM tool). There are historical versions of the
     RPM file format, as well as a currently abandoned fork (rpm5). These formats
     are not covered by this specification.
     
     .. seealso::
-       Source - https://github.com/rpm-software-management/rpm/blob/911448f2/doc/manual/format.md
+       Source - https://github.com/rpm-software-management/rpm/blob/afad3167/docs/manual/format.md
     
     
     .. seealso::
-       Source - https://github.com/rpm-software-management/rpm/blob/911448f2/doc/manual/tags.md
+       Source - https://github.com/rpm-software-management/rpm/blob/afad3167/docs/manual/tags.md
     
     
     .. seealso::
        Source - https://refspecs.linuxbase.org/LSB_5.0.0/LSB-Core-generic/LSB-Core-generic/pkgformat.html
     
     
     .. seealso::
@@ -487,14 +487,25 @@
         payload_digest = 5092
         payload_digest_algo = 5093
         auto_installed_unimplemented = 5094
         identity_unimplemented = 5095
         modularity_label = 5096
         payload_digest_alt = 5097
         arch_suffix = 5098
+        spec = 5099
+        translation_url = 5100
+        upstream_releases = 5101
+        source_license_internal = 5102
+        pre_untrans = 5103
+        post_untrans = 5104
+        pre_untrans_prog = 5105
+        post_untrans_prog = 5106
+        pre_untrans_flags = 5107
+        post_untrans_flags = 5108
+        sys_users = 5109
 
     class RpmTypes(Enum):
         binary = 0
         source = 1
 
     class Architectures(Enum):
         x86 = 1
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/rtcp_payload.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/rtcp_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class RtcpPayload(KaitaiStruct):
     """RTCP is the Real-Time Control Protocol.
     
     .. seealso::
-       Source - https://tools.ietf.org/html/rfc3550
+       Source - https://www.rfc-editor.org/rfc/rfc3550
     """
 
     class PayloadType(Enum):
         fir = 192
         nack = 193
         ij = 195
         sr = 200
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/rtp_packet.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/rtp_packet.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/rtpdump.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/rtpdump.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ruby_marshal.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ruby_marshal.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     
     Feature-wise, it is comparable to other language-specific
     implementations, such as:
     
     * Java's
       [Serializable](https://docs.oracle.com/javase/8/docs/api/java/io/Serializable.html)
     * .NET
-      [BinaryFormatter](https://docs.microsoft.com/en-us/dotnet/api/system.runtime.serialization.formatters.binary.binaryformatter)
+      [BinaryFormatter](https://learn.microsoft.com/en-us/dotnet/api/system.runtime.serialization.formatters.binary.binaryformatter?view=net-7.0)
     * Python's
       [marshal](https://docs.python.org/3/library/marshal.html),
       [pickle](https://docs.python.org/3/library/pickle.html) and
       [shelve](https://docs.python.org/3/library/shelve.html)
     
     From internal perspective, serialized stream consists of a simple
     magic header and a record.
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/s3m.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/s3m.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/saints_row_2_vpp_pc.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/saints_row_2_vpp_pc.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/shapefile_index.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/shapefile_index.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/shapefile_main.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/shapefile_main.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/some_ip.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/some_ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 import some_ip_sd
 class SomeIp(KaitaiStruct):
     """SOME/IP (Scalable service-Oriented MiddlewarE over IP) is an automotive/embedded
     communication protocol which supports remoteprocedure calls, event notifications
     and the underlying serialization/wire format.
     
     .. seealso::
-       Source - https://www.autosar.org/fileadmin/user_upload/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPProtocol.pdf
+       Source - https://www.autosar.org/fileadmin/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPProtocol.pdf
     """
     SEQ_FIELDS = ["header", "payload"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_container.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_container.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     availability of functional entities called services in the in-vehicle
     communication as well as controlling the send behavior of event messages.
     This allows sending only event messages to receivers requiring them (Publish/Subscribe).
     The solution described here is also known as SOME/IP-SD
     (Scalable service-Oriented MiddlewarE over IP - Service Discovery).
     
     .. seealso::
-       Source - https://www.autosar.org/fileadmin/user_upload/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
+       Source - https://www.autosar.org/fileadmin/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
     """
     SEQ_FIELDS = ["flags", "reserved", "len_entries", "entries", "len_options", "options"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd_entries.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd_entries.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class SomeIpSdEntries(KaitaiStruct):
     """The entries are used to synchronize the state of services instances and the
     Publish/-Subscribe handling.
     
     .. seealso::
-       section 4.1.2.3  Entry Format - https://www.autosar.org/fileadmin/user_upload/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
+       section 4.1.2.3  Entry Format - https://www.autosar.org/fileadmin/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
        -
     """
     SEQ_FIELDS = ["entries"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/some_ip_sd_options.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/some_ip_sd_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 class SomeIpSdOptions(KaitaiStruct):
     """FormatOptions are used to transport additional information to the entries.
     This includes forinstance the information how a service instance is
     reachable (IP-Address, TransportProtocol, Port Number).
     
     .. seealso::
-       section 4.1.2.4 Options Format - https://www.autosar.org/fileadmin/user_upload/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
+       section 4.1.2.4 Options Format - https://www.autosar.org/fileadmin/standards/foundation/19-11/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf
        -
     """
     SEQ_FIELDS = ["entries"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/specpr.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/specpr.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/sqlite3.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ssh_public_key.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ssh_public_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     and follows the same internal format.
     
     This format spec deals with this internal binary format (called "blob" in
     openssh sources) only. Buffer is expected to be raw binary and not base64-d.
     Implementation closely follows code in OpenSSH.
     
     .. seealso::
-       Source - https://github.com/openssh/openssh-portable/blob/master/sshkey.c#L1970
+       Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshkey.c#L1970
     """
     SEQ_FIELDS = ["key_name", "body"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
@@ -175,15 +175,15 @@
             self.body = SshPublicKey.KeyDsa(self._io, self, self._root)
             self.body._read()
         self._debug['body']['end'] = self._io.pos()
 
     class KeyRsa(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshkey.c#L2011-L2028
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshkey.c#L2011-L2028
         """
         SEQ_FIELDS = ["rsa_e", "rsa_n"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -207,15 +207,15 @@
             self._m_key_length = self.rsa_n.length_in_bits
             return getattr(self, '_m_key_length', None)
 
 
     class KeyEd25519(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshkey.c#L2111-L2124
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshkey.c#L2111-L2124
         """
         SEQ_FIELDS = ["len_pk", "pk"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -228,15 +228,15 @@
             self.pk = self._io.read_bytes(self.len_pk)
             self._debug['pk']['end'] = self._io.pos()
 
 
     class KeyEcdsa(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshkey.c#L2060-L2103
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshkey.c#L2060-L2103
         """
         SEQ_FIELDS = ["curve_name", "ec"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -254,15 +254,15 @@
 
     class Cstring(KaitaiStruct):
         """A integer-prefixed string designed to be read using `sshbuf_get_cstring`
         and written by `sshbuf_put_cstring` routines in ssh sources. Name is an
         obscure misnomer, as typically "C string" means a null-terminated string.
         
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshbuf-getput-basic.c#L181
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshbuf-getput-basic.c#L181
         """
         SEQ_FIELDS = ["len", "value"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -275,15 +275,15 @@
             self.value = (self._io.read_bytes(self.len)).decode(u"ASCII")
             self._debug['value']['end'] = self._io.pos()
 
 
     class KeyDsa(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshkey.c#L2036-L2051
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshkey.c#L2036-L2051
         """
         SEQ_FIELDS = ["dsa_p", "dsa_q", "dsa_g", "dsa_pub_key"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -311,16 +311,16 @@
         """Elliptic curve dump format used by ssh. In OpenSSH code, the following
         routines are used to read/write it:
         
         * sshbuf_get_ec
         * get_ec
         
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshbuf-getput-crypto.c#L90
-           https://github.com/openssh/openssh-portable/blob/master/sshbuf-getput-crypto.c#L76
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshbuf-getput-crypto.c#L90
+           https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshbuf-getput-crypto.c#L76
         """
         SEQ_FIELDS = ["len", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -340,16 +340,16 @@
         
         * sshbuf_get_bignum2
         * sshbuf_get_bignum2_bytes_direct
         * sshbuf_put_bignum2
         * sshbuf_get_bignum2_bytes_direct
         
         .. seealso::
-           Source - https://github.com/openssh/openssh-portable/blob/master/sshbuf-getput-crypto.c#L35
-           https://github.com/openssh/openssh-portable/blob/master/sshbuf-getput-basic.c#L431
+           Source - https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshbuf-getput-crypto.c#L35
+           https://github.com/openssh/openssh-portable/blob/b4d4eda6/sshbuf-getput-basic.c#L431
         """
         SEQ_FIELDS = ["len", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/standard_midi_file.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/standard_midi_file.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/stl.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/stl.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/sudoers_ts.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/sudoers_ts.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class SudoersTs(KaitaiStruct):
     """This spec can be used to parse sudo time stamp files located in directories
     such as /run/sudo/ts/$USER or /var/lib/sudo/ts/$USER.
     
     .. seealso::
-       Source - https://www.sudo.ws/man/1.8.27/sudoers_timestamp.man.html
+       Source - https://www.sudo.ws/docs/man/1.8.27/sudoers_timestamp.man/
     """
 
     class TsType(Enum):
         global = 1
         tty = 2
         ppid = 3
         lockexcl = 4
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/swf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/swf.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     (i.e. JavaScript engines and graphical approaches, such as WebGL)
     emerged.
     
     There are a lot of versions of SWF (~36), format is somewhat
     documented by Adobe.
     
     .. seealso::
-       Source - https://www.adobe.com/content/dam/acom/en/devnet/pdf/swf-file-format-spec.pdf
+       Source - https://open-flash.github.io/mirrors/swf-spec-19.pdf
     """
 
     class Compressions(Enum):
         zlib = 67
         none = 70
         lzma = 90
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/systemd_journal.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/systemd_journal.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/tcp_segment.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/tcp_segment.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/tga.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/tga.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/tls_client_hello.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/tls_client_hello.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/tr_dos_image.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/tr_dos_image.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/tsm.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/tsm.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/ttf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/ttf.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Ttf(KaitaiStruct):
     """A TrueType font file contains data, in table format, that comprises
     an outline font.
     
     .. seealso::
-       Source - https://www.microsoft.com/typography/tt/ttf_spec/ttch02.doc
+       Source - https://web.archive.org/web/20160410081432/https://www.microsoft.com/typography/tt/ttf_spec/ttch02.doc
     """
     SEQ_FIELDS = ["offset_table", "directory_table"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/udp_datagram.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/udp_datagram.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/uefi_te.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/zx_spectrum_tap.py`

 * *Files 20% similar despite different names*

```diff
@@ -124,238 +124,186 @@
 # https://github.com/kaitai-io/kaitai_struct_formats
 
 
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
-import collections
 from enum import Enum
+import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-class UefiTe(KaitaiStruct):
-    """This type of executables could be found inside the UEFI firmware. The UEFI
-    firmware is stored in SPI flash memory, which is a chip soldered on a
-    system's motherboard. UEFI firmware is very modular: it usually contains
-    dozens, if not hundreds, of executables. To store all these separates files,
-    the firmware is laid out in volumes using the Firmware File System (FFS), a
-    file system specifically designed to store firmware images. The volumes
-    contain files that are identified by GUIDs and each of these files contain
-    one or more sections holding the data. One of these sections contains the
-    actual executable image. Most of the executable images follow the PE format.
-    However, some of them follow the TE format.
-    
-    The Terse Executable (TE) image format was created as a mechanism to reduce
-    the overhead of the PE/COFF headers in PE32/PE32+ images, resulting in a
-    corresponding reduction of image sizes for executables running in the PI
-    (Platform Initialization) Architecture environment. Reducing image size
-    provides an opportunity for use of a smaller system flash part.
-    
-    So the TE format is basically a stripped version of PE.
+class ZxSpectrumTap(KaitaiStruct):
+    """TAP files are used by emulators of ZX Spectrum computer (released in
+    1982 by Sinclair Research). TAP file stores blocks of data as if
+    they are written to magnetic tape, which was used as primary media
+    for ZX Spectrum. Contents of this file can be viewed as a very
+    simple linear filesystem, storing named files with some basic
+    metainformation prepended as a header.
     
     .. seealso::
-       Source - https://uefi.org/sites/default/files/resources/PI_Spec_1_6.pdf
+       Source - https://sinclair.wiki.zxnet.co.uk/wiki/TAP_format
     """
-    SEQ_FIELDS = ["te_hdr", "sections"]
+
+    class FlagEnum(Enum):
+        header = 0
+        data = 255
+
+    class HeaderTypeEnum(Enum):
+        program = 0
+        num_array = 1
+        char_array = 2
+        bytes = 3
+    SEQ_FIELDS = ["blocks"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
-        self._debug['te_hdr']['start'] = self._io.pos()
-        self._raw_te_hdr = self._io.read_bytes(40)
-        _io__raw_te_hdr = KaitaiStream(BytesIO(self._raw_te_hdr))
-        self.te_hdr = UefiTe.TeHeader(_io__raw_te_hdr, self, self._root)
-        self.te_hdr._read()
-        self._debug['te_hdr']['end'] = self._io.pos()
-        self._debug['sections']['start'] = self._io.pos()
-        self.sections = []
-        for i in range(self.te_hdr.num_sections):
-            if not 'arr' in self._debug['sections']:
-                self._debug['sections']['arr'] = []
-            self._debug['sections']['arr'].append({'start': self._io.pos()})
-            _t_sections = UefiTe.Section(self._io, self, self._root)
-            _t_sections._read()
-            self.sections.append(_t_sections)
-            self._debug['sections']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['sections']['end'] = self._io.pos()
-
-    class TeHeader(KaitaiStruct):
-
-        class MachineType(Enum):
-            unknown = 0
-            i386 = 332
-            r4000 = 358
-            wcemipsv2 = 361
-            alpha = 388
-            sh3 = 418
-            sh3dsp = 419
-            sh4 = 422
-            sh5 = 424
-            arm = 448
-            thumb = 450
-            armnt = 452
-            am33 = 467
-            powerpc = 496
-            powerpcfp = 497
-            ia64 = 512
-            mips16 = 614
-            mipsfpu = 870
-            mipsfpu16 = 1126
-            ebc = 3772
-            riscv32 = 20530
-            riscv64 = 20580
-            riscv128 = 20776
-            amd64 = 34404
-            m32r = 36929
-            arm64 = 43620
-
-        class SubsystemEnum(Enum):
-            unknown = 0
-            native = 1
-            windows_gui = 2
-            windows_cui = 3
-            posix_cui = 7
-            windows_ce_gui = 9
-            efi_application = 10
-            efi_boot_service_driver = 11
-            efi_runtime_driver = 12
-            efi_rom = 13
-            xbox = 14
-            windows_boot_application = 16
-        SEQ_FIELDS = ["magic", "machine", "num_sections", "subsystem", "stripped_size", "entry_point_addr", "base_of_code", "image_base", "data_dirs"]
+        self._debug['blocks']['start'] = self._io.pos()
+        self.blocks = []
+        i = 0
+        while not self._io.is_eof():
+            if not 'arr' in self._debug['blocks']:
+                self._debug['blocks']['arr'] = []
+            self._debug['blocks']['arr'].append({'start': self._io.pos()})
+            _t_blocks = ZxSpectrumTap.Block(self._io, self, self._root)
+            _t_blocks._read()
+            self.blocks.append(_t_blocks)
+            self._debug['blocks']['arr'][len(self.blocks) - 1]['end'] = self._io.pos()
+            i += 1
+
+        self._debug['blocks']['end'] = self._io.pos()
+
+    class Block(KaitaiStruct):
+        SEQ_FIELDS = ["len_block", "flag", "header", "data", "headerless_data"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['len_block']['start'] = self._io.pos()
+            self.len_block = self._io.read_u2le()
+            self._debug['len_block']['end'] = self._io.pos()
+            self._debug['flag']['start'] = self._io.pos()
+            self.flag = KaitaiStream.resolve_enum(ZxSpectrumTap.FlagEnum, self._io.read_u1())
+            self._debug['flag']['end'] = self._io.pos()
+            if  ((self.len_block == 19) and (self.flag == ZxSpectrumTap.FlagEnum.header)) :
+                self._debug['header']['start'] = self._io.pos()
+                self.header = ZxSpectrumTap.Header(self._io, self, self._root)
+                self.header._read()
+                self._debug['header']['end'] = self._io.pos()
+
+            if self.len_block == 19:
+                self._debug['data']['start'] = self._io.pos()
+                self.data = self._io.read_bytes((self.header.len_data + 4))
+                self._debug['data']['end'] = self._io.pos()
+
+            if self.flag == ZxSpectrumTap.FlagEnum.data:
+                self._debug['headerless_data']['start'] = self._io.pos()
+                self.headerless_data = self._io.read_bytes((self.len_block - 1))
+                self._debug['headerless_data']['end'] = self._io.pos()
+
+
+
+    class ProgramParams(KaitaiStruct):
+        SEQ_FIELDS = ["autostart_line", "len_program"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['magic']['start'] = self._io.pos()
-            self.magic = self._io.read_bytes(2)
-            self._debug['magic']['end'] = self._io.pos()
-            if not self.magic == b"\x56\x5A":
-                raise kaitaistruct.ValidationNotEqualError(b"\x56\x5A", self.magic, self._io, u"/types/te_header/seq/0")
-            self._debug['machine']['start'] = self._io.pos()
-            self.machine = KaitaiStream.resolve_enum(UefiTe.TeHeader.MachineType, self._io.read_u2le())
-            self._debug['machine']['end'] = self._io.pos()
-            self._debug['num_sections']['start'] = self._io.pos()
-            self.num_sections = self._io.read_u1()
-            self._debug['num_sections']['end'] = self._io.pos()
-            self._debug['subsystem']['start'] = self._io.pos()
-            self.subsystem = KaitaiStream.resolve_enum(UefiTe.TeHeader.SubsystemEnum, self._io.read_u1())
-            self._debug['subsystem']['end'] = self._io.pos()
-            self._debug['stripped_size']['start'] = self._io.pos()
-            self.stripped_size = self._io.read_u2le()
-            self._debug['stripped_size']['end'] = self._io.pos()
-            self._debug['entry_point_addr']['start'] = self._io.pos()
-            self.entry_point_addr = self._io.read_u4le()
-            self._debug['entry_point_addr']['end'] = self._io.pos()
-            self._debug['base_of_code']['start'] = self._io.pos()
-            self.base_of_code = self._io.read_u4le()
-            self._debug['base_of_code']['end'] = self._io.pos()
-            self._debug['image_base']['start'] = self._io.pos()
-            self.image_base = self._io.read_u8le()
-            self._debug['image_base']['end'] = self._io.pos()
-            self._debug['data_dirs']['start'] = self._io.pos()
-            self.data_dirs = UefiTe.HeaderDataDirs(self._io, self, self._root)
-            self.data_dirs._read()
-            self._debug['data_dirs']['end'] = self._io.pos()
+            self._debug['autostart_line']['start'] = self._io.pos()
+            self.autostart_line = self._io.read_u2le()
+            self._debug['autostart_line']['end'] = self._io.pos()
+            self._debug['len_program']['start'] = self._io.pos()
+            self.len_program = self._io.read_u2le()
+            self._debug['len_program']['end'] = self._io.pos()
 
 
-    class HeaderDataDirs(KaitaiStruct):
-        SEQ_FIELDS = ["base_relocation_table", "debug"]
+    class BytesParams(KaitaiStruct):
+        SEQ_FIELDS = ["start_address", "reserved"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['base_relocation_table']['start'] = self._io.pos()
-            self.base_relocation_table = UefiTe.DataDir(self._io, self, self._root)
-            self.base_relocation_table._read()
-            self._debug['base_relocation_table']['end'] = self._io.pos()
-            self._debug['debug']['start'] = self._io.pos()
-            self.debug = UefiTe.DataDir(self._io, self, self._root)
-            self.debug._read()
-            self._debug['debug']['end'] = self._io.pos()
+            self._debug['start_address']['start'] = self._io.pos()
+            self.start_address = self._io.read_u2le()
+            self._debug['start_address']['end'] = self._io.pos()
+            self._debug['reserved']['start'] = self._io.pos()
+            self.reserved = self._io.read_bytes(2)
+            self._debug['reserved']['end'] = self._io.pos()
 
 
-    class DataDir(KaitaiStruct):
-        SEQ_FIELDS = ["virtual_address", "size"]
+    class Header(KaitaiStruct):
+        SEQ_FIELDS = ["header_type", "filename", "len_data", "params", "checksum"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['virtual_address']['start'] = self._io.pos()
-            self.virtual_address = self._io.read_u4le()
-            self._debug['virtual_address']['end'] = self._io.pos()
-            self._debug['size']['start'] = self._io.pos()
-            self.size = self._io.read_u4le()
-            self._debug['size']['end'] = self._io.pos()
+            self._debug['header_type']['start'] = self._io.pos()
+            self.header_type = KaitaiStream.resolve_enum(ZxSpectrumTap.HeaderTypeEnum, self._io.read_u1())
+            self._debug['header_type']['end'] = self._io.pos()
+            self._debug['filename']['start'] = self._io.pos()
+            self.filename = KaitaiStream.bytes_strip_right(self._io.read_bytes(10), 32)
+            self._debug['filename']['end'] = self._io.pos()
+            self._debug['len_data']['start'] = self._io.pos()
+            self.len_data = self._io.read_u2le()
+            self._debug['len_data']['end'] = self._io.pos()
+            self._debug['params']['start'] = self._io.pos()
+            _on = self.header_type
+            if _on == ZxSpectrumTap.HeaderTypeEnum.program:
+                self.params = ZxSpectrumTap.ProgramParams(self._io, self, self._root)
+                self.params._read()
+            elif _on == ZxSpectrumTap.HeaderTypeEnum.num_array:
+                self.params = ZxSpectrumTap.ArrayParams(self._io, self, self._root)
+                self.params._read()
+            elif _on == ZxSpectrumTap.HeaderTypeEnum.char_array:
+                self.params = ZxSpectrumTap.ArrayParams(self._io, self, self._root)
+                self.params._read()
+            elif _on == ZxSpectrumTap.HeaderTypeEnum.bytes:
+                self.params = ZxSpectrumTap.BytesParams(self._io, self, self._root)
+                self.params._read()
+            self._debug['params']['end'] = self._io.pos()
+            self._debug['checksum']['start'] = self._io.pos()
+            self.checksum = self._io.read_u1()
+            self._debug['checksum']['end'] = self._io.pos()
 
 
-    class Section(KaitaiStruct):
-        SEQ_FIELDS = ["name", "virtual_size", "virtual_address", "size_of_raw_data", "pointer_to_raw_data", "pointer_to_relocations", "pointer_to_linenumbers", "num_relocations", "num_linenumbers", "characteristics"]
+    class ArrayParams(KaitaiStruct):
+        SEQ_FIELDS = ["reserved", "var_name", "reserved1"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['name']['start'] = self._io.pos()
-            self.name = (KaitaiStream.bytes_strip_right(self._io.read_bytes(8), 0)).decode(u"UTF-8")
-            self._debug['name']['end'] = self._io.pos()
-            self._debug['virtual_size']['start'] = self._io.pos()
-            self.virtual_size = self._io.read_u4le()
-            self._debug['virtual_size']['end'] = self._io.pos()
-            self._debug['virtual_address']['start'] = self._io.pos()
-            self.virtual_address = self._io.read_u4le()
-            self._debug['virtual_address']['end'] = self._io.pos()
-            self._debug['size_of_raw_data']['start'] = self._io.pos()
-            self.size_of_raw_data = self._io.read_u4le()
-            self._debug['size_of_raw_data']['end'] = self._io.pos()
-            self._debug['pointer_to_raw_data']['start'] = self._io.pos()
-            self.pointer_to_raw_data = self._io.read_u4le()
-            self._debug['pointer_to_raw_data']['end'] = self._io.pos()
-            self._debug['pointer_to_relocations']['start'] = self._io.pos()
-            self.pointer_to_relocations = self._io.read_u4le()
-            self._debug['pointer_to_relocations']['end'] = self._io.pos()
-            self._debug['pointer_to_linenumbers']['start'] = self._io.pos()
-            self.pointer_to_linenumbers = self._io.read_u4le()
-            self._debug['pointer_to_linenumbers']['end'] = self._io.pos()
-            self._debug['num_relocations']['start'] = self._io.pos()
-            self.num_relocations = self._io.read_u2le()
-            self._debug['num_relocations']['end'] = self._io.pos()
-            self._debug['num_linenumbers']['start'] = self._io.pos()
-            self.num_linenumbers = self._io.read_u2le()
-            self._debug['num_linenumbers']['end'] = self._io.pos()
-            self._debug['characteristics']['start'] = self._io.pos()
-            self.characteristics = self._io.read_u4le()
-            self._debug['characteristics']['end'] = self._io.pos()
-
-        @property
-        def body(self):
-            if hasattr(self, '_m_body'):
-                return self._m_body
-
-            _pos = self._io.pos()
-            self._io.seek(((self.pointer_to_raw_data - self._root.te_hdr.stripped_size) + self._root.te_hdr._io.size()))
-            self._debug['_m_body']['start'] = self._io.pos()
-            self._m_body = self._io.read_bytes(self.size_of_raw_data)
-            self._debug['_m_body']['end'] = self._io.pos()
-            self._io.seek(_pos)
-            return getattr(self, '_m_body', None)
+            self._debug['reserved']['start'] = self._io.pos()
+            self.reserved = self._io.read_u1()
+            self._debug['reserved']['end'] = self._io.pos()
+            self._debug['var_name']['start'] = self._io.pos()
+            self.var_name = self._io.read_u1()
+            self._debug['var_name']['end'] = self._io.pos()
+            self._debug['reserved1']['start'] = self._io.pos()
+            self.reserved1 = self._io.read_bytes(2)
+            self._debug['reserved1']['end'] = self._io.pos()
+            if not self.reserved1 == b"\x00\x80":
+                raise kaitaistruct.ValidationNotEqualError(b"\x00\x80", self.reserved1, self._io, u"/types/array_params/seq/2")
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/uimage.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/uimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
 class Uimage(KaitaiStruct):
     """The new uImage format allows more flexibility in handling images of various
     types (kernel, ramdisk, etc.), it also enhances integrity protection of images
     with sha1 and md5 checksums.
     
     .. seealso::
-       Source - https://source.denx.de/u-boot/u-boot/-/raw/e4dba4b/include/image.h
+       Source - https://source.denx.de/u-boot/u-boot/-/raw/e4dba4ba6f/include/image.h
     """
 
     class UimageOs(Enum):
         invalid = 0
         openbsd = 1
         netbsd = 2
         freebsd = 3
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/utf8_string.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/utf8_string.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/vfat.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/vfat.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/vlq_base128_be.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/vlq_base128_be.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     This particular encoding is specified and used in:
     
     * Standard MIDI file format
     * ASN.1 BER encoding
     * RAR 5.0 file format
     
     More information on this encoding is available at
-    https://en.wikipedia.org/wiki/Variable-length_quantity
+    <https://en.wikipedia.org/wiki/Variable-length_quantity>
     
     This particular implementation supports serialized values to up 8 bytes long.
     """
     SEQ_FIELDS = ["groups"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/vlq_base128_le.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/vlq_base128_le.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,24 @@
     """A variable-length unsigned/signed integer using base128 encoding. 1-byte groups
     consist of 1-bit flag of continuation and 7-bit value chunk, and are ordered
     "least significant group first", i.e. in "little-endian" manner.
     
     This particular encoding is specified and used in:
     
     * DWARF debug file format, where it's dubbed "unsigned LEB128" or "ULEB128".
-      http://dwarfstd.org/doc/dwarf-2.0.0.pdf - page 139
+      <https://dwarfstd.org/doc/dwarf-2.0.0.pdf> - page 139
     * Google Protocol Buffers, where it's called "Base 128 Varints".
-      https://developers.google.com/protocol-buffers/docs/encoding?csw=1#varints
+      <https://protobuf.dev/programming-guides/encoding/#varints>
     * Apache Lucene, where it's called "VInt"
-      https://lucene.apache.org/core/3_5_0/fileformats.html#VInt
+      <https://lucene.apache.org/core/3_5_0/fileformats.html#VInt>
     * Apache Avro uses this as a basis for integer encoding, adding ZigZag on
       top of it for signed ints
-      https://avro.apache.org/docs/current/spec.html#binary_encode_primitive
+      <https://avro.apache.org/docs/current/spec.html#binary_encode_primitive>
     
-    More information on this encoding is available at https://en.wikipedia.org/wiki/LEB128
+    More information on this encoding is available at <https://en.wikipedia.org/wiki/LEB128>
     
     This particular implementation supports serialized values to up 8 bytes long.
     """
     SEQ_FIELDS = ["groups"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/vmware_vmdk.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/vmware_vmdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class VmwareVmdk(KaitaiStruct):
     """
     .. seealso::
-       Source - https://github.com/libyal/libvmdk/blob/master/documentation/VMWare%20Virtual%20Disk%20Format%20(VMDK).asciidoc#41-file-header
+       Source - https://github.com/libyal/libvmdk/blob/main/documentation/VMWare%20Virtual%20Disk%20Format%20(VMDK).asciidoc#41-file-header
     """
 
     class CompressionMethods(Enum):
         none = 0
         deflate = 1
     SEQ_FIELDS = ["magic", "version", "flags", "size_max", "size_grain", "start_descriptor", "size_descriptor", "num_grain_table_entries", "start_secondary_grain", "start_primary_grain", "size_metadata", "is_dirty", "stuff", "compression_method"]
     def __init__(self, _io, _parent=None, _root=None):
@@ -197,15 +197,15 @@
         self._debug['compression_method']['start'] = self._io.pos()
         self.compression_method = KaitaiStream.resolve_enum(VmwareVmdk.CompressionMethods, self._io.read_u2le())
         self._debug['compression_method']['end'] = self._io.pos()
 
     class HeaderFlags(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/libyal/libvmdk/blob/master/documentation/VMWare%20Virtual%20Disk%20Format%20(VMDK).asciidoc#411-flags
+           Source - https://github.com/libyal/libvmdk/blob/main/documentation/VMWare%20Virtual%20Disk%20Format%20(VMDK).asciidoc#411-flags
         """
         SEQ_FIELDS = ["reserved1", "zeroed_grain_table_entry", "use_secondary_grain_dir", "valid_new_line_detection_test", "reserved2", "reserved3", "has_metadata", "has_compressed_grain", "reserved4"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/vp8_ivf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/vp8_ivf.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,19 @@
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Vp8Ivf(KaitaiStruct):
-    """IVF is a simple container format for raw VP8 data, which is an open
-    and royalty-free video compression format, currently developed by
-    Google.
+    """IVF is a simple container format for raw VP8 data, which is an open and
+    royalty-free video compression format, currently developed by Google.
     
-    Test .ivf files are available at https://chromium.googlesource.com/webm/vp8-test-vectors
+    Test .ivf files are available at
+    <https://chromium.googlesource.com/webm/vp8-test-vectors>
     
     .. seealso::
        Source - https://wiki.multimedia.cx/index.php/IVF
     """
     SEQ_FIELDS = ["magic1", "version", "len_header", "codec", "width", "height", "framerate", "timescale", "num_frames", "unused", "image_data"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/warcraft_2_pud.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/warcraft_2_pud.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/wav.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/wav.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
 from enum import Enum
 import collections
 from riff import Riff
 
-
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class Wav(KaitaiStruct):
     """The WAVE file format is a subset of Microsoft's RIFF specification for the
     storage of multimedia files. A RIFF file starts out with a file header
     followed by a sequence of data chunks. A WAVE file is often just a RIFF
@@ -59,15 +58,15 @@
     (jbyrd@giganticsoftware.com), and it is likely to contain bugs.
     
     .. seealso::
        Source - http://soundfile.sapp.org/doc/WaveFormat/
     
     
     .. seealso::
-       Source - http://www-mmsp.ece.mcgill.ca/Documents/AudioFormats/WAVE/WAVE.html
+       Source - https://www.mmsp.ece.mcgill.ca/Documents/AudioFormats/WAVE/WAVE.html
     
     
     .. seealso::
        Source - https://web.archive.org/web/20101031101749/http://www.ebu.ch/fr/technical/publications/userguides/bwf_user_guide.php
     """
 
     class WFormatTagType(Enum):
@@ -792,15 +791,15 @@
             self.unused2 = self._io.read_bits_int_be(8)
             self._debug['unused2']['end'] = self._io.pos()
 
 
     class AfspChunkType(KaitaiStruct):
         """
         .. seealso::
-           Source - http://www-mmsp.ece.mcgill.ca/Documents/Downloads/AFsp/
+           Source - https://www.mmsp.ece.mcgill.ca/Documents/Downloads/AFsp/
         """
         SEQ_FIELDS = ["magic", "info_records"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/websocket.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/websocket.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_evt_log.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_lnk_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -124,306 +124,469 @@
 # https://github.com/kaitai-io/kaitai_struct_formats
 
 
 # This is a generated file! Please edit source .ksy file and use kaitai-struct-compiler to rebuild
 
 import kaitaistruct
 from kaitaistruct import KaitaiStruct, KaitaiStream, BytesIO
-import collections
 from enum import Enum
+import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-class WindowsEvtLog(KaitaiStruct):
-    """EVT files are Windows Event Log files written by older Windows
-    operating systems (2000, XP, 2003). They are used as binary log
-    files by several major Windows subsystems and
-    applications. Typically, several of them can be found in
-    `%WINDIR%\system32\config` directory:
-    
-    * Application = `AppEvent.evt`
-    * System = `SysEvent.evt`
-    * Security = `SecEvent.evt`
-    
-    Alternatively, one can export any system event log as distinct .evt
-    file using relevant option in Event Viewer application.
-    
-    A Windows application can submit an entry into these logs using
-    [ReportEventA](https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-reporteventa)
-    function of Windows API.
-    
-    Internally, EVT files consist of a fixed-size header and event
-    records. There are several usage scenarios (non-wrapping vs wrapping
-    log files) which result in slightly different organization of
-    records.
+import windows_shell_items
+class WindowsLnkFile(KaitaiStruct):
+    """Windows .lnk files (AKA "shell link" file) are most frequently used
+    in Windows shell to create "shortcuts" to another files, usually for
+    purposes of running a program from some other directory, sometimes
+    with certain preconfigured arguments and some other options.
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/eventlog/event-log-file-format
+       Source - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
     """
-    SEQ_FIELDS = ["header", "records"]
+
+    class WindowState(Enum):
+        normal = 1
+        maximized = 3
+        min_no_active = 7
+
+    class DriveTypes(Enum):
+        unknown = 0
+        no_root_dir = 1
+        removable = 2
+        fixed = 3
+        remote = 4
+        cdrom = 5
+        ramdisk = 6
+    SEQ_FIELDS = ["header", "target_id_list", "info", "name", "rel_path", "work_dir", "arguments", "icon_location"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
         self._debug['header']['start'] = self._io.pos()
-        self.header = WindowsEvtLog.Header(self._io, self, self._root)
+        self.header = WindowsLnkFile.FileHeader(self._io, self, self._root)
         self.header._read()
         self._debug['header']['end'] = self._io.pos()
-        self._debug['records']['start'] = self._io.pos()
-        self.records = []
-        i = 0
-        while not self._io.is_eof():
-            if not 'arr' in self._debug['records']:
-                self._debug['records']['arr'] = []
-            self._debug['records']['arr'].append({'start': self._io.pos()})
-            _t_records = WindowsEvtLog.Record(self._io, self, self._root)
-            _t_records._read()
-            self.records.append(_t_records)
-            self._debug['records']['arr'][len(self.records) - 1]['end'] = self._io.pos()
-            i += 1
+        if self.header.flags.has_link_target_id_list:
+            self._debug['target_id_list']['start'] = self._io.pos()
+            self.target_id_list = WindowsLnkFile.LinkTargetIdList(self._io, self, self._root)
+            self.target_id_list._read()
+            self._debug['target_id_list']['end'] = self._io.pos()
+
+        if self.header.flags.has_link_info:
+            self._debug['info']['start'] = self._io.pos()
+            self.info = WindowsLnkFile.LinkInfo(self._io, self, self._root)
+            self.info._read()
+            self._debug['info']['end'] = self._io.pos()
+
+        if self.header.flags.has_name:
+            self._debug['name']['start'] = self._io.pos()
+            self.name = WindowsLnkFile.StringData(self._io, self, self._root)
+            self.name._read()
+            self._debug['name']['end'] = self._io.pos()
+
+        if self.header.flags.has_rel_path:
+            self._debug['rel_path']['start'] = self._io.pos()
+            self.rel_path = WindowsLnkFile.StringData(self._io, self, self._root)
+            self.rel_path._read()
+            self._debug['rel_path']['end'] = self._io.pos()
+
+        if self.header.flags.has_work_dir:
+            self._debug['work_dir']['start'] = self._io.pos()
+            self.work_dir = WindowsLnkFile.StringData(self._io, self, self._root)
+            self.work_dir._read()
+            self._debug['work_dir']['end'] = self._io.pos()
+
+        if self.header.flags.has_arguments:
+            self._debug['arguments']['start'] = self._io.pos()
+            self.arguments = WindowsLnkFile.StringData(self._io, self, self._root)
+            self.arguments._read()
+            self._debug['arguments']['end'] = self._io.pos()
+
+        if self.header.flags.has_icon_location:
+            self._debug['icon_location']['start'] = self._io.pos()
+            self.icon_location = WindowsLnkFile.StringData(self._io, self, self._root)
+            self.icon_location._read()
+            self._debug['icon_location']['end'] = self._io.pos()
 
-        self._debug['records']['end'] = self._io.pos()
 
-    class Header(KaitaiStruct):
+    class LinkTargetIdList(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/previous-versions/windows/desktop/legacy/bb309024(v=vs.85)
+           Section 2.2 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
         """
-        SEQ_FIELDS = ["len_header", "magic", "version_major", "version_minor", "ofs_start", "ofs_end", "cur_rec_idx", "oldest_rec_idx", "len_file_max", "flags", "retention", "len_header_2"]
+        SEQ_FIELDS = ["len_id_list", "id_list"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_header']['start'] = self._io.pos()
-            self.len_header = self._io.read_u4le()
-            self._debug['len_header']['end'] = self._io.pos()
-            self._debug['magic']['start'] = self._io.pos()
-            self.magic = self._io.read_bytes(4)
-            self._debug['magic']['end'] = self._io.pos()
-            if not self.magic == b"\x4C\x66\x4C\x65":
-                raise kaitaistruct.ValidationNotEqualError(b"\x4C\x66\x4C\x65", self.magic, self._io, u"/types/header/seq/1")
-            self._debug['version_major']['start'] = self._io.pos()
-            self.version_major = self._io.read_u4le()
-            self._debug['version_major']['end'] = self._io.pos()
-            self._debug['version_minor']['start'] = self._io.pos()
-            self.version_minor = self._io.read_u4le()
-            self._debug['version_minor']['end'] = self._io.pos()
-            self._debug['ofs_start']['start'] = self._io.pos()
-            self.ofs_start = self._io.read_u4le()
-            self._debug['ofs_start']['end'] = self._io.pos()
-            self._debug['ofs_end']['start'] = self._io.pos()
-            self.ofs_end = self._io.read_u4le()
-            self._debug['ofs_end']['end'] = self._io.pos()
-            self._debug['cur_rec_idx']['start'] = self._io.pos()
-            self.cur_rec_idx = self._io.read_u4le()
-            self._debug['cur_rec_idx']['end'] = self._io.pos()
-            self._debug['oldest_rec_idx']['start'] = self._io.pos()
-            self.oldest_rec_idx = self._io.read_u4le()
-            self._debug['oldest_rec_idx']['end'] = self._io.pos()
-            self._debug['len_file_max']['start'] = self._io.pos()
-            self.len_file_max = self._io.read_u4le()
-            self._debug['len_file_max']['end'] = self._io.pos()
-            self._debug['flags']['start'] = self._io.pos()
-            self.flags = WindowsEvtLog.Header.Flags(self._io, self, self._root)
-            self.flags._read()
-            self._debug['flags']['end'] = self._io.pos()
-            self._debug['retention']['start'] = self._io.pos()
-            self.retention = self._io.read_u4le()
-            self._debug['retention']['end'] = self._io.pos()
-            self._debug['len_header_2']['start'] = self._io.pos()
-            self.len_header_2 = self._io.read_u4le()
-            self._debug['len_header_2']['end'] = self._io.pos()
+            self._debug['len_id_list']['start'] = self._io.pos()
+            self.len_id_list = self._io.read_u2le()
+            self._debug['len_id_list']['end'] = self._io.pos()
+            self._debug['id_list']['start'] = self._io.pos()
+            self._raw_id_list = self._io.read_bytes(self.len_id_list)
+            _io__raw_id_list = KaitaiStream(BytesIO(self._raw_id_list))
+            self.id_list = windows_shell_items.WindowsShellItems(_io__raw_id_list)
+            self.id_list._read()
+            self._debug['id_list']['end'] = self._io.pos()
 
-        class Flags(KaitaiStruct):
-            SEQ_FIELDS = ["reserved", "archive", "log_full", "wrap", "dirty"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
 
-            def _read(self):
-                self._debug['reserved']['start'] = self._io.pos()
-                self.reserved = self._io.read_bits_int_be(28)
-                self._debug['reserved']['end'] = self._io.pos()
-                self._debug['archive']['start'] = self._io.pos()
-                self.archive = self._io.read_bits_int_be(1) != 0
-                self._debug['archive']['end'] = self._io.pos()
-                self._debug['log_full']['start'] = self._io.pos()
-                self.log_full = self._io.read_bits_int_be(1) != 0
-                self._debug['log_full']['end'] = self._io.pos()
-                self._debug['wrap']['start'] = self._io.pos()
-                self.wrap = self._io.read_bits_int_be(1) != 0
-                self._debug['wrap']['end'] = self._io.pos()
-                self._debug['dirty']['start'] = self._io.pos()
-                self.dirty = self._io.read_bits_int_be(1) != 0
-                self._debug['dirty']['end'] = self._io.pos()
+    class StringData(KaitaiStruct):
+        SEQ_FIELDS = ["chars_str", "str"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
 
+        def _read(self):
+            self._debug['chars_str']['start'] = self._io.pos()
+            self.chars_str = self._io.read_u2le()
+            self._debug['chars_str']['end'] = self._io.pos()
+            self._debug['str']['start'] = self._io.pos()
+            self.str = (self._io.read_bytes((self.chars_str * 2))).decode(u"UTF-16LE")
+            self._debug['str']['end'] = self._io.pos()
 
 
-    class Record(KaitaiStruct):
+    class LinkInfo(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/winnt/ns-winnt-eventlogrecord
+           Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
         """
-        SEQ_FIELDS = ["len_record", "type", "body", "len_record2"]
+        SEQ_FIELDS = ["len_all", "all"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_record']['start'] = self._io.pos()
-            self.len_record = self._io.read_u4le()
-            self._debug['len_record']['end'] = self._io.pos()
-            self._debug['type']['start'] = self._io.pos()
-            self.type = self._io.read_u4le()
-            self._debug['type']['end'] = self._io.pos()
-            self._debug['body']['start'] = self._io.pos()
-            _on = self.type
-            if _on == 1699505740:
-                self._raw_body = self._io.read_bytes((self.len_record - 12))
-                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = WindowsEvtLog.RecordBody(_io__raw_body, self, self._root)
-                self.body._read()
-            elif _on == 286331153:
-                self._raw_body = self._io.read_bytes((self.len_record - 12))
+            self._debug['len_all']['start'] = self._io.pos()
+            self.len_all = self._io.read_u4le()
+            self._debug['len_all']['end'] = self._io.pos()
+            self._debug['all']['start'] = self._io.pos()
+            self._raw_all = self._io.read_bytes((self.len_all - 4))
+            _io__raw_all = KaitaiStream(BytesIO(self._raw_all))
+            self.all = WindowsLnkFile.LinkInfo.All(_io__raw_all, self, self._root)
+            self.all._read()
+            self._debug['all']['end'] = self._io.pos()
+
+        class VolumeIdBody(KaitaiStruct):
+            """
+            .. seealso::
+               Section 2.3.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+            """
+            SEQ_FIELDS = ["drive_type", "drive_serial_number", "ofs_volume_label", "ofs_volume_label_unicode"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['drive_type']['start'] = self._io.pos()
+                self.drive_type = KaitaiStream.resolve_enum(WindowsLnkFile.DriveTypes, self._io.read_u4le())
+                self._debug['drive_type']['end'] = self._io.pos()
+                self._debug['drive_serial_number']['start'] = self._io.pos()
+                self.drive_serial_number = self._io.read_u4le()
+                self._debug['drive_serial_number']['end'] = self._io.pos()
+                self._debug['ofs_volume_label']['start'] = self._io.pos()
+                self.ofs_volume_label = self._io.read_u4le()
+                self._debug['ofs_volume_label']['end'] = self._io.pos()
+                if self.is_unicode:
+                    self._debug['ofs_volume_label_unicode']['start'] = self._io.pos()
+                    self.ofs_volume_label_unicode = self._io.read_u4le()
+                    self._debug['ofs_volume_label_unicode']['end'] = self._io.pos()
+
+
+            @property
+            def is_unicode(self):
+                if hasattr(self, '_m_is_unicode'):
+                    return self._m_is_unicode
+
+                self._m_is_unicode = self.ofs_volume_label == 20
+                return getattr(self, '_m_is_unicode', None)
+
+            @property
+            def volume_label_ansi(self):
+                if hasattr(self, '_m_volume_label_ansi'):
+                    return self._m_volume_label_ansi
+
+                if not (self.is_unicode):
+                    _pos = self._io.pos()
+                    self._io.seek((self.ofs_volume_label - 4))
+                    self._debug['_m_volume_label_ansi']['start'] = self._io.pos()
+                    self._m_volume_label_ansi = (self._io.read_bytes_term(0, False, True, True)).decode(u"cp437")
+                    self._debug['_m_volume_label_ansi']['end'] = self._io.pos()
+                    self._io.seek(_pos)
+
+                return getattr(self, '_m_volume_label_ansi', None)
+
+
+        class All(KaitaiStruct):
+            """
+            .. seealso::
+               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+            """
+            SEQ_FIELDS = ["len_header", "header"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['len_header']['start'] = self._io.pos()
+                self.len_header = self._io.read_u4le()
+                self._debug['len_header']['end'] = self._io.pos()
+                self._debug['header']['start'] = self._io.pos()
+                self._raw_header = self._io.read_bytes((self.len_header - 8))
+                _io__raw_header = KaitaiStream(BytesIO(self._raw_header))
+                self.header = WindowsLnkFile.LinkInfo.Header(_io__raw_header, self, self._root)
+                self.header._read()
+                self._debug['header']['end'] = self._io.pos()
+
+            @property
+            def volume_id(self):
+                if hasattr(self, '_m_volume_id'):
+                    return self._m_volume_id
+
+                if self.header.flags.has_volume_id_and_local_base_path:
+                    _pos = self._io.pos()
+                    self._io.seek((self.header.ofs_volume_id - 4))
+                    self._debug['_m_volume_id']['start'] = self._io.pos()
+                    self._m_volume_id = WindowsLnkFile.LinkInfo.VolumeIdSpec(self._io, self, self._root)
+                    self._m_volume_id._read()
+                    self._debug['_m_volume_id']['end'] = self._io.pos()
+                    self._io.seek(_pos)
+
+                return getattr(self, '_m_volume_id', None)
+
+            @property
+            def local_base_path(self):
+                if hasattr(self, '_m_local_base_path'):
+                    return self._m_local_base_path
+
+                if self.header.flags.has_volume_id_and_local_base_path:
+                    _pos = self._io.pos()
+                    self._io.seek((self.header.ofs_local_base_path - 4))
+                    self._debug['_m_local_base_path']['start'] = self._io.pos()
+                    self._m_local_base_path = self._io.read_bytes_term(0, False, True, True)
+                    self._debug['_m_local_base_path']['end'] = self._io.pos()
+                    self._io.seek(_pos)
+
+                return getattr(self, '_m_local_base_path', None)
+
+
+        class VolumeIdSpec(KaitaiStruct):
+            """
+            .. seealso::
+               Section 2.3.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+            """
+            SEQ_FIELDS = ["len_all", "body"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['len_all']['start'] = self._io.pos()
+                self.len_all = self._io.read_u4le()
+                self._debug['len_all']['end'] = self._io.pos()
+                self._debug['body']['start'] = self._io.pos()
+                self._raw_body = self._io.read_bytes((self.len_all - 4))
                 _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = WindowsEvtLog.CursorRecordBody(_io__raw_body, self, self._root)
+                self.body = WindowsLnkFile.LinkInfo.VolumeIdBody(_io__raw_body, self, self._root)
                 self.body._read()
-            else:
-                self.body = self._io.read_bytes((self.len_record - 12))
-            self._debug['body']['end'] = self._io.pos()
-            self._debug['len_record2']['start'] = self._io.pos()
-            self.len_record2 = self._io.read_u4le()
-            self._debug['len_record2']['end'] = self._io.pos()
+                self._debug['body']['end'] = self._io.pos()
+
+
+        class LinkInfoFlags(KaitaiStruct):
+            """
+            .. seealso::
+               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+            """
+            SEQ_FIELDS = ["reserved1", "has_common_net_rel_link", "has_volume_id_and_local_base_path", "reserved2"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['reserved1']['start'] = self._io.pos()
+                self.reserved1 = self._io.read_bits_int_be(6)
+                self._debug['reserved1']['end'] = self._io.pos()
+                self._debug['has_common_net_rel_link']['start'] = self._io.pos()
+                self.has_common_net_rel_link = self._io.read_bits_int_be(1) != 0
+                self._debug['has_common_net_rel_link']['end'] = self._io.pos()
+                self._debug['has_volume_id_and_local_base_path']['start'] = self._io.pos()
+                self.has_volume_id_and_local_base_path = self._io.read_bits_int_be(1) != 0
+                self._debug['has_volume_id_and_local_base_path']['end'] = self._io.pos()
+                self._debug['reserved2']['start'] = self._io.pos()
+                self.reserved2 = self._io.read_bits_int_be(24)
+                self._debug['reserved2']['end'] = self._io.pos()
+
+
+        class Header(KaitaiStruct):
+            """
+            .. seealso::
+               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+            """
+            SEQ_FIELDS = ["flags", "ofs_volume_id", "ofs_local_base_path", "ofs_common_net_rel_link", "ofs_common_path_suffix", "ofs_local_base_path_unicode", "ofs_common_path_suffix_unicode"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['flags']['start'] = self._io.pos()
+                self.flags = WindowsLnkFile.LinkInfo.LinkInfoFlags(self._io, self, self._root)
+                self.flags._read()
+                self._debug['flags']['end'] = self._io.pos()
+                self._debug['ofs_volume_id']['start'] = self._io.pos()
+                self.ofs_volume_id = self._io.read_u4le()
+                self._debug['ofs_volume_id']['end'] = self._io.pos()
+                self._debug['ofs_local_base_path']['start'] = self._io.pos()
+                self.ofs_local_base_path = self._io.read_u4le()
+                self._debug['ofs_local_base_path']['end'] = self._io.pos()
+                self._debug['ofs_common_net_rel_link']['start'] = self._io.pos()
+                self.ofs_common_net_rel_link = self._io.read_u4le()
+                self._debug['ofs_common_net_rel_link']['end'] = self._io.pos()
+                self._debug['ofs_common_path_suffix']['start'] = self._io.pos()
+                self.ofs_common_path_suffix = self._io.read_u4le()
+                self._debug['ofs_common_path_suffix']['end'] = self._io.pos()
+                if not (self._io.is_eof()):
+                    self._debug['ofs_local_base_path_unicode']['start'] = self._io.pos()
+                    self.ofs_local_base_path_unicode = self._io.read_u4le()
+                    self._debug['ofs_local_base_path_unicode']['end'] = self._io.pos()
+
+                if not (self._io.is_eof()):
+                    self._debug['ofs_common_path_suffix_unicode']['start'] = self._io.pos()
+                    self.ofs_common_path_suffix_unicode = self._io.read_u4le()
+                    self._debug['ofs_common_path_suffix_unicode']['end'] = self._io.pos()
+
 
 
-    class RecordBody(KaitaiStruct):
+
+    class LinkFlags(KaitaiStruct):
         """
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/winnt/ns-winnt-eventlogrecord
+           Section 2.1.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
         """
-
-        class EventTypes(Enum):
-            error = 1
-            audit_failure = 2
-            audit_success = 3
-            info = 4
-            warning = 5
-        SEQ_FIELDS = ["idx", "time_generated", "time_written", "event_id", "event_type", "num_strings", "event_category", "reserved", "ofs_strings", "len_user_sid", "ofs_user_sid", "len_data", "ofs_data"]
+        SEQ_FIELDS = ["is_unicode", "has_icon_location", "has_arguments", "has_work_dir", "has_rel_path", "has_name", "has_link_info", "has_link_target_id_list", "_unnamed8", "reserved", "keep_local_id_list_for_unc_target", "_unnamed11"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['idx']['start'] = self._io.pos()
-            self.idx = self._io.read_u4le()
-            self._debug['idx']['end'] = self._io.pos()
-            self._debug['time_generated']['start'] = self._io.pos()
-            self.time_generated = self._io.read_u4le()
-            self._debug['time_generated']['end'] = self._io.pos()
-            self._debug['time_written']['start'] = self._io.pos()
-            self.time_written = self._io.read_u4le()
-            self._debug['time_written']['end'] = self._io.pos()
-            self._debug['event_id']['start'] = self._io.pos()
-            self.event_id = self._io.read_u4le()
-            self._debug['event_id']['end'] = self._io.pos()
-            self._debug['event_type']['start'] = self._io.pos()
-            self.event_type = KaitaiStream.resolve_enum(WindowsEvtLog.RecordBody.EventTypes, self._io.read_u2le())
-            self._debug['event_type']['end'] = self._io.pos()
-            self._debug['num_strings']['start'] = self._io.pos()
-            self.num_strings = self._io.read_u2le()
-            self._debug['num_strings']['end'] = self._io.pos()
-            self._debug['event_category']['start'] = self._io.pos()
-            self.event_category = self._io.read_u2le()
-            self._debug['event_category']['end'] = self._io.pos()
+            self._debug['is_unicode']['start'] = self._io.pos()
+            self.is_unicode = self._io.read_bits_int_be(1) != 0
+            self._debug['is_unicode']['end'] = self._io.pos()
+            self._debug['has_icon_location']['start'] = self._io.pos()
+            self.has_icon_location = self._io.read_bits_int_be(1) != 0
+            self._debug['has_icon_location']['end'] = self._io.pos()
+            self._debug['has_arguments']['start'] = self._io.pos()
+            self.has_arguments = self._io.read_bits_int_be(1) != 0
+            self._debug['has_arguments']['end'] = self._io.pos()
+            self._debug['has_work_dir']['start'] = self._io.pos()
+            self.has_work_dir = self._io.read_bits_int_be(1) != 0
+            self._debug['has_work_dir']['end'] = self._io.pos()
+            self._debug['has_rel_path']['start'] = self._io.pos()
+            self.has_rel_path = self._io.read_bits_int_be(1) != 0
+            self._debug['has_rel_path']['end'] = self._io.pos()
+            self._debug['has_name']['start'] = self._io.pos()
+            self.has_name = self._io.read_bits_int_be(1) != 0
+            self._debug['has_name']['end'] = self._io.pos()
+            self._debug['has_link_info']['start'] = self._io.pos()
+            self.has_link_info = self._io.read_bits_int_be(1) != 0
+            self._debug['has_link_info']['end'] = self._io.pos()
+            self._debug['has_link_target_id_list']['start'] = self._io.pos()
+            self.has_link_target_id_list = self._io.read_bits_int_be(1) != 0
+            self._debug['has_link_target_id_list']['end'] = self._io.pos()
+            self._debug['_unnamed8']['start'] = self._io.pos()
+            self._unnamed8 = self._io.read_bits_int_be(16)
+            self._debug['_unnamed8']['end'] = self._io.pos()
             self._debug['reserved']['start'] = self._io.pos()
-            self.reserved = self._io.read_bytes(6)
+            self.reserved = self._io.read_bits_int_be(5)
             self._debug['reserved']['end'] = self._io.pos()
-            self._debug['ofs_strings']['start'] = self._io.pos()
-            self.ofs_strings = self._io.read_u4le()
-            self._debug['ofs_strings']['end'] = self._io.pos()
-            self._debug['len_user_sid']['start'] = self._io.pos()
-            self.len_user_sid = self._io.read_u4le()
-            self._debug['len_user_sid']['end'] = self._io.pos()
-            self._debug['ofs_user_sid']['start'] = self._io.pos()
-            self.ofs_user_sid = self._io.read_u4le()
-            self._debug['ofs_user_sid']['end'] = self._io.pos()
-            self._debug['len_data']['start'] = self._io.pos()
-            self.len_data = self._io.read_u4le()
-            self._debug['len_data']['end'] = self._io.pos()
-            self._debug['ofs_data']['start'] = self._io.pos()
-            self.ofs_data = self._io.read_u4le()
-            self._debug['ofs_data']['end'] = self._io.pos()
-
-        @property
-        def user_sid(self):
-            if hasattr(self, '_m_user_sid'):
-                return self._m_user_sid
-
-            _pos = self._io.pos()
-            self._io.seek((self.ofs_user_sid - 8))
-            self._debug['_m_user_sid']['start'] = self._io.pos()
-            self._m_user_sid = self._io.read_bytes(self.len_user_sid)
-            self._debug['_m_user_sid']['end'] = self._io.pos()
-            self._io.seek(_pos)
-            return getattr(self, '_m_user_sid', None)
-
-        @property
-        def data(self):
-            if hasattr(self, '_m_data'):
-                return self._m_data
-
-            _pos = self._io.pos()
-            self._io.seek((self.ofs_data - 8))
-            self._debug['_m_data']['start'] = self._io.pos()
-            self._m_data = self._io.read_bytes(self.len_data)
-            self._debug['_m_data']['end'] = self._io.pos()
-            self._io.seek(_pos)
-            return getattr(self, '_m_data', None)
+            self._debug['keep_local_id_list_for_unc_target']['start'] = self._io.pos()
+            self.keep_local_id_list_for_unc_target = self._io.read_bits_int_be(1) != 0
+            self._debug['keep_local_id_list_for_unc_target']['end'] = self._io.pos()
+            self._debug['_unnamed11']['start'] = self._io.pos()
+            self._unnamed11 = self._io.read_bits_int_be(2)
+            self._debug['_unnamed11']['end'] = self._io.pos()
 
 
-    class CursorRecordBody(KaitaiStruct):
+    class FileHeader(KaitaiStruct):
         """
         .. seealso::
-           Source - http://www.forensicswiki.xyz/page/Windows_Event_Log_(EVT)#Cursor_Record
+           Section 2.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
         """
-        SEQ_FIELDS = ["magic", "ofs_first_record", "ofs_next_record", "idx_next_record", "idx_first_record"]
+        SEQ_FIELDS = ["len_header", "link_clsid", "flags", "file_attrs", "time_creation", "time_access", "time_write", "target_file_size", "icon_index", "show_command", "hotkey", "reserved"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['magic']['start'] = self._io.pos()
-            self.magic = self._io.read_bytes(12)
-            self._debug['magic']['end'] = self._io.pos()
-            if not self.magic == b"\x22\x22\x22\x22\x33\x33\x33\x33\x44\x44\x44\x44":
-                raise kaitaistruct.ValidationNotEqualError(b"\x22\x22\x22\x22\x33\x33\x33\x33\x44\x44\x44\x44", self.magic, self._io, u"/types/cursor_record_body/seq/0")
-            self._debug['ofs_first_record']['start'] = self._io.pos()
-            self.ofs_first_record = self._io.read_u4le()
-            self._debug['ofs_first_record']['end'] = self._io.pos()
-            self._debug['ofs_next_record']['start'] = self._io.pos()
-            self.ofs_next_record = self._io.read_u4le()
-            self._debug['ofs_next_record']['end'] = self._io.pos()
-            self._debug['idx_next_record']['start'] = self._io.pos()
-            self.idx_next_record = self._io.read_u4le()
-            self._debug['idx_next_record']['end'] = self._io.pos()
-            self._debug['idx_first_record']['start'] = self._io.pos()
-            self.idx_first_record = self._io.read_u4le()
-            self._debug['idx_first_record']['end'] = self._io.pos()
+            self._debug['len_header']['start'] = self._io.pos()
+            self.len_header = self._io.read_bytes(4)
+            self._debug['len_header']['end'] = self._io.pos()
+            if not self.len_header == b"\x4C\x00\x00\x00":
+                raise kaitaistruct.ValidationNotEqualError(b"\x4C\x00\x00\x00", self.len_header, self._io, u"/types/file_header/seq/0")
+            self._debug['link_clsid']['start'] = self._io.pos()
+            self.link_clsid = self._io.read_bytes(16)
+            self._debug['link_clsid']['end'] = self._io.pos()
+            if not self.link_clsid == b"\x01\x14\x02\x00\x00\x00\x00\x00\xC0\x00\x00\x00\x00\x00\x00\x46":
+                raise kaitaistruct.ValidationNotEqualError(b"\x01\x14\x02\x00\x00\x00\x00\x00\xC0\x00\x00\x00\x00\x00\x00\x46", self.link_clsid, self._io, u"/types/file_header/seq/1")
+            self._debug['flags']['start'] = self._io.pos()
+            self._raw_flags = self._io.read_bytes(4)
+            _io__raw_flags = KaitaiStream(BytesIO(self._raw_flags))
+            self.flags = WindowsLnkFile.LinkFlags(_io__raw_flags, self, self._root)
+            self.flags._read()
+            self._debug['flags']['end'] = self._io.pos()
+            self._debug['file_attrs']['start'] = self._io.pos()
+            self.file_attrs = self._io.read_u4le()
+            self._debug['file_attrs']['end'] = self._io.pos()
+            self._debug['time_creation']['start'] = self._io.pos()
+            self.time_creation = self._io.read_u8le()
+            self._debug['time_creation']['end'] = self._io.pos()
+            self._debug['time_access']['start'] = self._io.pos()
+            self.time_access = self._io.read_u8le()
+            self._debug['time_access']['end'] = self._io.pos()
+            self._debug['time_write']['start'] = self._io.pos()
+            self.time_write = self._io.read_u8le()
+            self._debug['time_write']['end'] = self._io.pos()
+            self._debug['target_file_size']['start'] = self._io.pos()
+            self.target_file_size = self._io.read_u4le()
+            self._debug['target_file_size']['end'] = self._io.pos()
+            self._debug['icon_index']['start'] = self._io.pos()
+            self.icon_index = self._io.read_s4le()
+            self._debug['icon_index']['end'] = self._io.pos()
+            self._debug['show_command']['start'] = self._io.pos()
+            self.show_command = KaitaiStream.resolve_enum(WindowsLnkFile.WindowState, self._io.read_u4le())
+            self._debug['show_command']['end'] = self._io.pos()
+            self._debug['hotkey']['start'] = self._io.pos()
+            self.hotkey = self._io.read_u2le()
+            self._debug['hotkey']['end'] = self._io.pos()
+            self._debug['reserved']['start'] = self._io.pos()
+            self.reserved = self._io.read_bytes(10)
+            self._debug['reserved']['end'] = self._io.pos()
+            if not self.reserved == b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00":
+                raise kaitaistruct.ValidationNotEqualError(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00", self.reserved, self._io, u"/types/file_header/seq/11")
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_lnk_file.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_minidump.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,462 +131,570 @@
 from enum import Enum
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-import windows_shell_items
-class WindowsLnkFile(KaitaiStruct):
-    """Windows .lnk files (AKA "shell link" file) are most frequently used
-    in Windows shell to create "shortcuts" to another files, usually for
-    purposes of running a program from some other directory, sometimes
-    with certain preconfigured arguments and some other options.
+class WindowsMinidump(KaitaiStruct):
+    """Windows MiniDump (MDMP) file provides a concise way to store process
+    core dumps, which is useful for debugging. Given its small size,
+    modularity, some cross-platform features and native support in some
+    debuggers, it is particularly useful for crash reporting, and is
+    used for that purpose in Windows and Google Chrome projects.
+    
+    The file itself is a container, which contains a number of typed
+    "streams", which contain some data according to its type attribute.
     
     .. seealso::
-       Source - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+       Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_header
     """
 
-    class WindowState(Enum):
-        normal = 1
-        maximized = 3
-        min_no_active = 7
-
-    class DriveTypes(Enum):
-        unknown = 0
-        no_root_dir = 1
-        removable = 2
-        fixed = 3
-        remote = 4
-        cdrom = 5
-        ramdisk = 6
-    SEQ_FIELDS = ["header", "target_id_list", "info", "name", "rel_path", "work_dir", "arguments", "icon_location"]
+    class StreamTypes(Enum):
+        unused = 0
+        reserved_0 = 1
+        reserved_1 = 2
+        thread_list = 3
+        module_list = 4
+        memory_list = 5
+        exception = 6
+        system_info = 7
+        thread_ex_list = 8
+        memory_64_list = 9
+        comment_a = 10
+        comment_w = 11
+        handle_data = 12
+        function_table = 13
+        unloaded_module_list = 14
+        misc_info = 15
+        memory_info_list = 16
+        thread_info_list = 17
+        handle_operation_list = 18
+        token = 19
+        java_script_data = 20
+        system_memory_info = 21
+        process_vm_counters = 22
+        ipt_trace = 23
+        thread_names = 24
+        ce_null = 32768
+        ce_system_info = 32769
+        ce_exception = 32770
+        ce_module_list = 32771
+        ce_process_list = 32772
+        ce_thread_list = 32773
+        ce_thread_context_list = 32774
+        ce_thread_call_stack_list = 32775
+        ce_memory_virtual_list = 32776
+        ce_memory_physical_list = 32777
+        ce_bucket_parameters = 32778
+        ce_process_module_map = 32779
+        ce_diagnosis_list = 32780
+        md_crashpad_info_stream = 1129316353
+        md_raw_breakpad_info = 1197932545
+        md_raw_assertion_info = 1197932546
+        md_linux_cpu_info = 1197932547
+        md_linux_proc_status = 1197932548
+        md_linux_lsb_release = 1197932549
+        md_linux_cmd_line = 1197932550
+        md_linux_environ = 1197932551
+        md_linux_auxv = 1197932552
+        md_linux_maps = 1197932553
+        md_linux_dso_debug = 1197932554
+    SEQ_FIELDS = ["magic1", "magic2", "version", "num_streams", "ofs_streams", "checksum", "timestamp", "flags"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
-        self._debug['header']['start'] = self._io.pos()
-        self.header = WindowsLnkFile.FileHeader(self._io, self, self._root)
-        self.header._read()
-        self._debug['header']['end'] = self._io.pos()
-        if self.header.flags.has_link_target_id_list:
-            self._debug['target_id_list']['start'] = self._io.pos()
-            self.target_id_list = WindowsLnkFile.LinkTargetIdList(self._io, self, self._root)
-            self.target_id_list._read()
-            self._debug['target_id_list']['end'] = self._io.pos()
+        self._debug['magic1']['start'] = self._io.pos()
+        self.magic1 = self._io.read_bytes(4)
+        self._debug['magic1']['end'] = self._io.pos()
+        if not self.magic1 == b"\x4D\x44\x4D\x50":
+            raise kaitaistruct.ValidationNotEqualError(b"\x4D\x44\x4D\x50", self.magic1, self._io, u"/seq/0")
+        self._debug['magic2']['start'] = self._io.pos()
+        self.magic2 = self._io.read_bytes(2)
+        self._debug['magic2']['end'] = self._io.pos()
+        if not self.magic2 == b"\x93\xA7":
+            raise kaitaistruct.ValidationNotEqualError(b"\x93\xA7", self.magic2, self._io, u"/seq/1")
+        self._debug['version']['start'] = self._io.pos()
+        self.version = self._io.read_u2le()
+        self._debug['version']['end'] = self._io.pos()
+        self._debug['num_streams']['start'] = self._io.pos()
+        self.num_streams = self._io.read_u4le()
+        self._debug['num_streams']['end'] = self._io.pos()
+        self._debug['ofs_streams']['start'] = self._io.pos()
+        self.ofs_streams = self._io.read_u4le()
+        self._debug['ofs_streams']['end'] = self._io.pos()
+        self._debug['checksum']['start'] = self._io.pos()
+        self.checksum = self._io.read_u4le()
+        self._debug['checksum']['end'] = self._io.pos()
+        self._debug['timestamp']['start'] = self._io.pos()
+        self.timestamp = self._io.read_u4le()
+        self._debug['timestamp']['end'] = self._io.pos()
+        self._debug['flags']['start'] = self._io.pos()
+        self.flags = self._io.read_u8le()
+        self._debug['flags']['end'] = self._io.pos()
+
+    class ThreadList(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_thread_list
+        """
+        SEQ_FIELDS = ["num_threads", "threads"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['num_threads']['start'] = self._io.pos()
+            self.num_threads = self._io.read_u4le()
+            self._debug['num_threads']['end'] = self._io.pos()
+            self._debug['threads']['start'] = self._io.pos()
+            self.threads = []
+            for i in range(self.num_threads):
+                if not 'arr' in self._debug['threads']:
+                    self._debug['threads']['arr'] = []
+                self._debug['threads']['arr'].append({'start': self._io.pos()})
+                _t_threads = WindowsMinidump.Thread(self._io, self, self._root)
+                _t_threads._read()
+                self.threads.append(_t_threads)
+                self._debug['threads']['arr'][i]['end'] = self._io.pos()
+
+            self._debug['threads']['end'] = self._io.pos()
+
+
+    class LocationDescriptor(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_location_descriptor
+        """
+        SEQ_FIELDS = ["len_data", "ofs_data"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['len_data']['start'] = self._io.pos()
+            self.len_data = self._io.read_u4le()
+            self._debug['len_data']['end'] = self._io.pos()
+            self._debug['ofs_data']['start'] = self._io.pos()
+            self.ofs_data = self._io.read_u4le()
+            self._debug['ofs_data']['end'] = self._io.pos()
+
+        @property
+        def data(self):
+            if hasattr(self, '_m_data'):
+                return self._m_data
+
+            io = self._root._io
+            _pos = io.pos()
+            io.seek(self.ofs_data)
+            self._debug['_m_data']['start'] = io.pos()
+            self._m_data = io.read_bytes(self.len_data)
+            self._debug['_m_data']['end'] = io.pos()
+            io.seek(_pos)
+            return getattr(self, '_m_data', None)
+
+
+    class MinidumpString(KaitaiStruct):
+        """Specific string serialization scheme used in MiniDump format is
+        actually a simple 32-bit length-prefixed UTF-16 string.
+        
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_string
+        """
+        SEQ_FIELDS = ["len_str", "str"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
 
-        if self.header.flags.has_link_info:
-            self._debug['info']['start'] = self._io.pos()
-            self.info = WindowsLnkFile.LinkInfo(self._io, self, self._root)
-            self.info._read()
-            self._debug['info']['end'] = self._io.pos()
+        def _read(self):
+            self._debug['len_str']['start'] = self._io.pos()
+            self.len_str = self._io.read_u4le()
+            self._debug['len_str']['end'] = self._io.pos()
+            self._debug['str']['start'] = self._io.pos()
+            self.str = (self._io.read_bytes(self.len_str)).decode(u"UTF-16LE")
+            self._debug['str']['end'] = self._io.pos()
 
-        if self.header.flags.has_name:
-            self._debug['name']['start'] = self._io.pos()
-            self.name = WindowsLnkFile.StringData(self._io, self, self._root)
-            self.name._read()
-            self._debug['name']['end'] = self._io.pos()
 
-        if self.header.flags.has_rel_path:
-            self._debug['rel_path']['start'] = self._io.pos()
-            self.rel_path = WindowsLnkFile.StringData(self._io, self, self._root)
-            self.rel_path._read()
-            self._debug['rel_path']['end'] = self._io.pos()
+    class SystemInfo(KaitaiStruct):
+        """"System info" stream provides basic information about the
+        hardware and operating system which produces this dump.
+        
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_system_info
+        """
 
-        if self.header.flags.has_work_dir:
-            self._debug['work_dir']['start'] = self._io.pos()
-            self.work_dir = WindowsLnkFile.StringData(self._io, self, self._root)
-            self.work_dir._read()
-            self._debug['work_dir']['end'] = self._io.pos()
+        class CpuArchs(Enum):
+            intel = 0
+            arm = 5
+            ia64 = 6
+            amd64 = 9
+            unknown = 65535
+        SEQ_FIELDS = ["cpu_arch", "cpu_level", "cpu_revision", "num_cpus", "os_type", "os_ver_major", "os_ver_minor", "os_build", "os_platform", "ofs_service_pack", "os_suite_mask", "reserved2"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
 
-        if self.header.flags.has_arguments:
-            self._debug['arguments']['start'] = self._io.pos()
-            self.arguments = WindowsLnkFile.StringData(self._io, self, self._root)
-            self.arguments._read()
-            self._debug['arguments']['end'] = self._io.pos()
+        def _read(self):
+            self._debug['cpu_arch']['start'] = self._io.pos()
+            self.cpu_arch = KaitaiStream.resolve_enum(WindowsMinidump.SystemInfo.CpuArchs, self._io.read_u2le())
+            self._debug['cpu_arch']['end'] = self._io.pos()
+            self._debug['cpu_level']['start'] = self._io.pos()
+            self.cpu_level = self._io.read_u2le()
+            self._debug['cpu_level']['end'] = self._io.pos()
+            self._debug['cpu_revision']['start'] = self._io.pos()
+            self.cpu_revision = self._io.read_u2le()
+            self._debug['cpu_revision']['end'] = self._io.pos()
+            self._debug['num_cpus']['start'] = self._io.pos()
+            self.num_cpus = self._io.read_u1()
+            self._debug['num_cpus']['end'] = self._io.pos()
+            self._debug['os_type']['start'] = self._io.pos()
+            self.os_type = self._io.read_u1()
+            self._debug['os_type']['end'] = self._io.pos()
+            self._debug['os_ver_major']['start'] = self._io.pos()
+            self.os_ver_major = self._io.read_u4le()
+            self._debug['os_ver_major']['end'] = self._io.pos()
+            self._debug['os_ver_minor']['start'] = self._io.pos()
+            self.os_ver_minor = self._io.read_u4le()
+            self._debug['os_ver_minor']['end'] = self._io.pos()
+            self._debug['os_build']['start'] = self._io.pos()
+            self.os_build = self._io.read_u4le()
+            self._debug['os_build']['end'] = self._io.pos()
+            self._debug['os_platform']['start'] = self._io.pos()
+            self.os_platform = self._io.read_u4le()
+            self._debug['os_platform']['end'] = self._io.pos()
+            self._debug['ofs_service_pack']['start'] = self._io.pos()
+            self.ofs_service_pack = self._io.read_u4le()
+            self._debug['ofs_service_pack']['end'] = self._io.pos()
+            self._debug['os_suite_mask']['start'] = self._io.pos()
+            self.os_suite_mask = self._io.read_u2le()
+            self._debug['os_suite_mask']['end'] = self._io.pos()
+            self._debug['reserved2']['start'] = self._io.pos()
+            self.reserved2 = self._io.read_u2le()
+            self._debug['reserved2']['end'] = self._io.pos()
+
+        @property
+        def service_pack(self):
+            if hasattr(self, '_m_service_pack'):
+                return self._m_service_pack
+
+            if self.ofs_service_pack > 0:
+                io = self._root._io
+                _pos = io.pos()
+                io.seek(self.ofs_service_pack)
+                self._debug['_m_service_pack']['start'] = io.pos()
+                self._m_service_pack = WindowsMinidump.MinidumpString(io, self, self._root)
+                self._m_service_pack._read()
+                self._debug['_m_service_pack']['end'] = io.pos()
+                io.seek(_pos)
 
-        if self.header.flags.has_icon_location:
-            self._debug['icon_location']['start'] = self._io.pos()
-            self.icon_location = WindowsLnkFile.StringData(self._io, self, self._root)
-            self.icon_location._read()
-            self._debug['icon_location']['end'] = self._io.pos()
+            return getattr(self, '_m_service_pack', None)
 
 
-    class LinkTargetIdList(KaitaiStruct):
+    class ExceptionRecord(KaitaiStruct):
         """
         .. seealso::
-           Section 2.2 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_exception
         """
-        SEQ_FIELDS = ["len_id_list", "id_list"]
+        SEQ_FIELDS = ["code", "flags", "inner_exception", "addr", "num_params", "reserved", "params"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_id_list']['start'] = self._io.pos()
-            self.len_id_list = self._io.read_u2le()
-            self._debug['len_id_list']['end'] = self._io.pos()
-            self._debug['id_list']['start'] = self._io.pos()
-            self._raw_id_list = self._io.read_bytes(self.len_id_list)
-            _io__raw_id_list = KaitaiStream(BytesIO(self._raw_id_list))
-            self.id_list = windows_shell_items.WindowsShellItems(_io__raw_id_list)
-            self.id_list._read()
-            self._debug['id_list']['end'] = self._io.pos()
+            self._debug['code']['start'] = self._io.pos()
+            self.code = self._io.read_u4le()
+            self._debug['code']['end'] = self._io.pos()
+            self._debug['flags']['start'] = self._io.pos()
+            self.flags = self._io.read_u4le()
+            self._debug['flags']['end'] = self._io.pos()
+            self._debug['inner_exception']['start'] = self._io.pos()
+            self.inner_exception = self._io.read_u8le()
+            self._debug['inner_exception']['end'] = self._io.pos()
+            self._debug['addr']['start'] = self._io.pos()
+            self.addr = self._io.read_u8le()
+            self._debug['addr']['end'] = self._io.pos()
+            self._debug['num_params']['start'] = self._io.pos()
+            self.num_params = self._io.read_u4le()
+            self._debug['num_params']['end'] = self._io.pos()
+            self._debug['reserved']['start'] = self._io.pos()
+            self.reserved = self._io.read_u4le()
+            self._debug['reserved']['end'] = self._io.pos()
+            self._debug['params']['start'] = self._io.pos()
+            self.params = []
+            for i in range(15):
+                if not 'arr' in self._debug['params']:
+                    self._debug['params']['arr'] = []
+                self._debug['params']['arr'].append({'start': self._io.pos()})
+                self.params.append(self._io.read_u8le())
+                self._debug['params']['arr'][i]['end'] = self._io.pos()
+
+            self._debug['params']['end'] = self._io.pos()
 
 
-    class StringData(KaitaiStruct):
-        SEQ_FIELDS = ["chars_str", "str"]
+    class MiscInfo(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_misc_info
+        """
+        SEQ_FIELDS = ["len_info", "flags1", "process_id", "process_create_time", "process_user_time", "process_kernel_time", "cpu_max_mhz", "cpu_cur_mhz", "cpu_limit_mhz", "cpu_max_idle_state", "cpu_cur_idle_state"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['chars_str']['start'] = self._io.pos()
-            self.chars_str = self._io.read_u2le()
-            self._debug['chars_str']['end'] = self._io.pos()
-            self._debug['str']['start'] = self._io.pos()
-            self.str = (self._io.read_bytes((self.chars_str * 2))).decode(u"UTF-16LE")
-            self._debug['str']['end'] = self._io.pos()
+            self._debug['len_info']['start'] = self._io.pos()
+            self.len_info = self._io.read_u4le()
+            self._debug['len_info']['end'] = self._io.pos()
+            self._debug['flags1']['start'] = self._io.pos()
+            self.flags1 = self._io.read_u4le()
+            self._debug['flags1']['end'] = self._io.pos()
+            self._debug['process_id']['start'] = self._io.pos()
+            self.process_id = self._io.read_u4le()
+            self._debug['process_id']['end'] = self._io.pos()
+            self._debug['process_create_time']['start'] = self._io.pos()
+            self.process_create_time = self._io.read_u4le()
+            self._debug['process_create_time']['end'] = self._io.pos()
+            self._debug['process_user_time']['start'] = self._io.pos()
+            self.process_user_time = self._io.read_u4le()
+            self._debug['process_user_time']['end'] = self._io.pos()
+            self._debug['process_kernel_time']['start'] = self._io.pos()
+            self.process_kernel_time = self._io.read_u4le()
+            self._debug['process_kernel_time']['end'] = self._io.pos()
+            self._debug['cpu_max_mhz']['start'] = self._io.pos()
+            self.cpu_max_mhz = self._io.read_u4le()
+            self._debug['cpu_max_mhz']['end'] = self._io.pos()
+            self._debug['cpu_cur_mhz']['start'] = self._io.pos()
+            self.cpu_cur_mhz = self._io.read_u4le()
+            self._debug['cpu_cur_mhz']['end'] = self._io.pos()
+            self._debug['cpu_limit_mhz']['start'] = self._io.pos()
+            self.cpu_limit_mhz = self._io.read_u4le()
+            self._debug['cpu_limit_mhz']['end'] = self._io.pos()
+            self._debug['cpu_max_idle_state']['start'] = self._io.pos()
+            self.cpu_max_idle_state = self._io.read_u4le()
+            self._debug['cpu_max_idle_state']['end'] = self._io.pos()
+            self._debug['cpu_cur_idle_state']['start'] = self._io.pos()
+            self.cpu_cur_idle_state = self._io.read_u4le()
+            self._debug['cpu_cur_idle_state']['end'] = self._io.pos()
 
 
-    class LinkInfo(KaitaiStruct):
+    class Dir(KaitaiStruct):
         """
         .. seealso::
-           Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_directory
         """
-        SEQ_FIELDS = ["len_all", "all"]
+        SEQ_FIELDS = ["stream_type", "len_data", "ofs_data"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_all']['start'] = self._io.pos()
-            self.len_all = self._io.read_u4le()
-            self._debug['len_all']['end'] = self._io.pos()
-            self._debug['all']['start'] = self._io.pos()
-            self._raw_all = self._io.read_bytes((self.len_all - 4))
-            _io__raw_all = KaitaiStream(BytesIO(self._raw_all))
-            self.all = WindowsLnkFile.LinkInfo.All(_io__raw_all, self, self._root)
-            self.all._read()
-            self._debug['all']['end'] = self._io.pos()
-
-        class VolumeIdBody(KaitaiStruct):
-            """
-            .. seealso::
-               Section 2.3.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-            """
-            SEQ_FIELDS = ["drive_type", "drive_serial_number", "ofs_volume_label", "ofs_volume_label_unicode"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['drive_type']['start'] = self._io.pos()
-                self.drive_type = KaitaiStream.resolve_enum(WindowsLnkFile.DriveTypes, self._io.read_u4le())
-                self._debug['drive_type']['end'] = self._io.pos()
-                self._debug['drive_serial_number']['start'] = self._io.pos()
-                self.drive_serial_number = self._io.read_u4le()
-                self._debug['drive_serial_number']['end'] = self._io.pos()
-                self._debug['ofs_volume_label']['start'] = self._io.pos()
-                self.ofs_volume_label = self._io.read_u4le()
-                self._debug['ofs_volume_label']['end'] = self._io.pos()
-                if self.is_unicode:
-                    self._debug['ofs_volume_label_unicode']['start'] = self._io.pos()
-                    self.ofs_volume_label_unicode = self._io.read_u4le()
-                    self._debug['ofs_volume_label_unicode']['end'] = self._io.pos()
-
-
-            @property
-            def is_unicode(self):
-                if hasattr(self, '_m_is_unicode'):
-                    return self._m_is_unicode
-
-                self._m_is_unicode = self.ofs_volume_label == 20
-                return getattr(self, '_m_is_unicode', None)
-
-            @property
-            def volume_label_ansi(self):
-                if hasattr(self, '_m_volume_label_ansi'):
-                    return self._m_volume_label_ansi
-
-                if not (self.is_unicode):
-                    _pos = self._io.pos()
-                    self._io.seek((self.ofs_volume_label - 4))
-                    self._debug['_m_volume_label_ansi']['start'] = self._io.pos()
-                    self._m_volume_label_ansi = (self._io.read_bytes_term(0, False, True, True)).decode(u"cp437")
-                    self._debug['_m_volume_label_ansi']['end'] = self._io.pos()
-                    self._io.seek(_pos)
-
-                return getattr(self, '_m_volume_label_ansi', None)
-
-
-        class All(KaitaiStruct):
-            """
-            .. seealso::
-               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-            """
-            SEQ_FIELDS = ["len_header", "header"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['len_header']['start'] = self._io.pos()
-                self.len_header = self._io.read_u4le()
-                self._debug['len_header']['end'] = self._io.pos()
-                self._debug['header']['start'] = self._io.pos()
-                self._raw_header = self._io.read_bytes((self.len_header - 8))
-                _io__raw_header = KaitaiStream(BytesIO(self._raw_header))
-                self.header = WindowsLnkFile.LinkInfo.Header(_io__raw_header, self, self._root)
-                self.header._read()
-                self._debug['header']['end'] = self._io.pos()
-
-            @property
-            def volume_id(self):
-                if hasattr(self, '_m_volume_id'):
-                    return self._m_volume_id
-
-                if self.header.flags.has_volume_id_and_local_base_path:
-                    _pos = self._io.pos()
-                    self._io.seek((self.header.ofs_volume_id - 4))
-                    self._debug['_m_volume_id']['start'] = self._io.pos()
-                    self._m_volume_id = WindowsLnkFile.LinkInfo.VolumeIdSpec(self._io, self, self._root)
-                    self._m_volume_id._read()
-                    self._debug['_m_volume_id']['end'] = self._io.pos()
-                    self._io.seek(_pos)
-
-                return getattr(self, '_m_volume_id', None)
-
-            @property
-            def local_base_path(self):
-                if hasattr(self, '_m_local_base_path'):
-                    return self._m_local_base_path
-
-                if self.header.flags.has_volume_id_and_local_base_path:
-                    _pos = self._io.pos()
-                    self._io.seek((self.header.ofs_local_base_path - 4))
-                    self._debug['_m_local_base_path']['start'] = self._io.pos()
-                    self._m_local_base_path = self._io.read_bytes_term(0, False, True, True)
-                    self._debug['_m_local_base_path']['end'] = self._io.pos()
-                    self._io.seek(_pos)
-
-                return getattr(self, '_m_local_base_path', None)
-
-
-        class VolumeIdSpec(KaitaiStruct):
-            """
-            .. seealso::
-               Section 2.3.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-            """
-            SEQ_FIELDS = ["len_all", "body"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['len_all']['start'] = self._io.pos()
-                self.len_all = self._io.read_u4le()
-                self._debug['len_all']['end'] = self._io.pos()
-                self._debug['body']['start'] = self._io.pos()
-                self._raw_body = self._io.read_bytes((self.len_all - 4))
-                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
-                self.body = WindowsLnkFile.LinkInfo.VolumeIdBody(_io__raw_body, self, self._root)
-                self.body._read()
-                self._debug['body']['end'] = self._io.pos()
-
-
-        class LinkInfoFlags(KaitaiStruct):
-            """
-            .. seealso::
-               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-            """
-            SEQ_FIELDS = ["reserved1", "has_common_net_rel_link", "has_volume_id_and_local_base_path", "reserved2"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['reserved1']['start'] = self._io.pos()
-                self.reserved1 = self._io.read_bits_int_be(6)
-                self._debug['reserved1']['end'] = self._io.pos()
-                self._debug['has_common_net_rel_link']['start'] = self._io.pos()
-                self.has_common_net_rel_link = self._io.read_bits_int_be(1) != 0
-                self._debug['has_common_net_rel_link']['end'] = self._io.pos()
-                self._debug['has_volume_id_and_local_base_path']['start'] = self._io.pos()
-                self.has_volume_id_and_local_base_path = self._io.read_bits_int_be(1) != 0
-                self._debug['has_volume_id_and_local_base_path']['end'] = self._io.pos()
-                self._debug['reserved2']['start'] = self._io.pos()
-                self.reserved2 = self._io.read_bits_int_be(24)
-                self._debug['reserved2']['end'] = self._io.pos()
-
-
-        class Header(KaitaiStruct):
-            """
-            .. seealso::
-               Section 2.3 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-            """
-            SEQ_FIELDS = ["flags", "ofs_volume_id", "ofs_local_base_path", "ofs_common_net_rel_link", "ofs_common_path_suffix", "ofs_local_base_path_unicode", "ofs_common_path_suffix_unicode"]
-            def __init__(self, _io, _parent=None, _root=None):
-                self._io = _io
-                self._parent = _parent
-                self._root = _root if _root else self
-                self._debug = collections.defaultdict(dict)
-
-            def _read(self):
-                self._debug['flags']['start'] = self._io.pos()
-                self.flags = WindowsLnkFile.LinkInfo.LinkInfoFlags(self._io, self, self._root)
-                self.flags._read()
-                self._debug['flags']['end'] = self._io.pos()
-                self._debug['ofs_volume_id']['start'] = self._io.pos()
-                self.ofs_volume_id = self._io.read_u4le()
-                self._debug['ofs_volume_id']['end'] = self._io.pos()
-                self._debug['ofs_local_base_path']['start'] = self._io.pos()
-                self.ofs_local_base_path = self._io.read_u4le()
-                self._debug['ofs_local_base_path']['end'] = self._io.pos()
-                self._debug['ofs_common_net_rel_link']['start'] = self._io.pos()
-                self.ofs_common_net_rel_link = self._io.read_u4le()
-                self._debug['ofs_common_net_rel_link']['end'] = self._io.pos()
-                self._debug['ofs_common_path_suffix']['start'] = self._io.pos()
-                self.ofs_common_path_suffix = self._io.read_u4le()
-                self._debug['ofs_common_path_suffix']['end'] = self._io.pos()
-                if not (self._io.is_eof()):
-                    self._debug['ofs_local_base_path_unicode']['start'] = self._io.pos()
-                    self.ofs_local_base_path_unicode = self._io.read_u4le()
-                    self._debug['ofs_local_base_path_unicode']['end'] = self._io.pos()
-
-                if not (self._io.is_eof()):
-                    self._debug['ofs_common_path_suffix_unicode']['start'] = self._io.pos()
-                    self.ofs_common_path_suffix_unicode = self._io.read_u4le()
-                    self._debug['ofs_common_path_suffix_unicode']['end'] = self._io.pos()
-
-
-
-
-    class LinkFlags(KaitaiStruct):
-        """
-        .. seealso::
-           Section 2.1.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
-        """
-        SEQ_FIELDS = ["is_unicode", "has_icon_location", "has_arguments", "has_work_dir", "has_rel_path", "has_name", "has_link_info", "has_link_target_id_list", "_unnamed8", "reserved", "keep_local_id_list_for_unc_target", "_unnamed11"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['is_unicode']['start'] = self._io.pos()
-            self.is_unicode = self._io.read_bits_int_be(1) != 0
-            self._debug['is_unicode']['end'] = self._io.pos()
-            self._debug['has_icon_location']['start'] = self._io.pos()
-            self.has_icon_location = self._io.read_bits_int_be(1) != 0
-            self._debug['has_icon_location']['end'] = self._io.pos()
-            self._debug['has_arguments']['start'] = self._io.pos()
-            self.has_arguments = self._io.read_bits_int_be(1) != 0
-            self._debug['has_arguments']['end'] = self._io.pos()
-            self._debug['has_work_dir']['start'] = self._io.pos()
-            self.has_work_dir = self._io.read_bits_int_be(1) != 0
-            self._debug['has_work_dir']['end'] = self._io.pos()
-            self._debug['has_rel_path']['start'] = self._io.pos()
-            self.has_rel_path = self._io.read_bits_int_be(1) != 0
-            self._debug['has_rel_path']['end'] = self._io.pos()
-            self._debug['has_name']['start'] = self._io.pos()
-            self.has_name = self._io.read_bits_int_be(1) != 0
-            self._debug['has_name']['end'] = self._io.pos()
-            self._debug['has_link_info']['start'] = self._io.pos()
-            self.has_link_info = self._io.read_bits_int_be(1) != 0
-            self._debug['has_link_info']['end'] = self._io.pos()
-            self._debug['has_link_target_id_list']['start'] = self._io.pos()
-            self.has_link_target_id_list = self._io.read_bits_int_be(1) != 0
-            self._debug['has_link_target_id_list']['end'] = self._io.pos()
-            self._debug['_unnamed8']['start'] = self._io.pos()
-            self._unnamed8 = self._io.read_bits_int_be(16)
-            self._debug['_unnamed8']['end'] = self._io.pos()
-            self._debug['reserved']['start'] = self._io.pos()
-            self.reserved = self._io.read_bits_int_be(5)
-            self._debug['reserved']['end'] = self._io.pos()
-            self._debug['keep_local_id_list_for_unc_target']['start'] = self._io.pos()
-            self.keep_local_id_list_for_unc_target = self._io.read_bits_int_be(1) != 0
-            self._debug['keep_local_id_list_for_unc_target']['end'] = self._io.pos()
-            self._debug['_unnamed11']['start'] = self._io.pos()
-            self._unnamed11 = self._io.read_bits_int_be(2)
-            self._debug['_unnamed11']['end'] = self._io.pos()
+            self._debug['stream_type']['start'] = self._io.pos()
+            self.stream_type = KaitaiStream.resolve_enum(WindowsMinidump.StreamTypes, self._io.read_u4le())
+            self._debug['stream_type']['end'] = self._io.pos()
+            self._debug['len_data']['start'] = self._io.pos()
+            self.len_data = self._io.read_u4le()
+            self._debug['len_data']['end'] = self._io.pos()
+            self._debug['ofs_data']['start'] = self._io.pos()
+            self.ofs_data = self._io.read_u4le()
+            self._debug['ofs_data']['end'] = self._io.pos()
+
+        @property
+        def data(self):
+            if hasattr(self, '_m_data'):
+                return self._m_data
+
+            _pos = self._io.pos()
+            self._io.seek(self.ofs_data)
+            self._debug['_m_data']['start'] = self._io.pos()
+            _on = self.stream_type
+            if _on == WindowsMinidump.StreamTypes.memory_list:
+                self._raw__m_data = self._io.read_bytes(self.len_data)
+                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
+                self._m_data = WindowsMinidump.MemoryList(_io__raw__m_data, self, self._root)
+                self._m_data._read()
+            elif _on == WindowsMinidump.StreamTypes.misc_info:
+                self._raw__m_data = self._io.read_bytes(self.len_data)
+                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
+                self._m_data = WindowsMinidump.MiscInfo(_io__raw__m_data, self, self._root)
+                self._m_data._read()
+            elif _on == WindowsMinidump.StreamTypes.thread_list:
+                self._raw__m_data = self._io.read_bytes(self.len_data)
+                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
+                self._m_data = WindowsMinidump.ThreadList(_io__raw__m_data, self, self._root)
+                self._m_data._read()
+            elif _on == WindowsMinidump.StreamTypes.exception:
+                self._raw__m_data = self._io.read_bytes(self.len_data)
+                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
+                self._m_data = WindowsMinidump.ExceptionStream(_io__raw__m_data, self, self._root)
+                self._m_data._read()
+            elif _on == WindowsMinidump.StreamTypes.system_info:
+                self._raw__m_data = self._io.read_bytes(self.len_data)
+                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
+                self._m_data = WindowsMinidump.SystemInfo(_io__raw__m_data, self, self._root)
+                self._m_data._read()
+            else:
+                self._m_data = self._io.read_bytes(self.len_data)
+            self._debug['_m_data']['end'] = self._io.pos()
+            self._io.seek(_pos)
+            return getattr(self, '_m_data', None)
 
 
-    class FileHeader(KaitaiStruct):
+    class Thread(KaitaiStruct):
         """
         .. seealso::
-           Section 2.1 - https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-SHLLINK/[MS-SHLLINK].pdf
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_thread
         """
-        SEQ_FIELDS = ["len_header", "link_clsid", "flags", "file_attrs", "time_creation", "time_access", "time_write", "target_file_size", "icon_index", "show_command", "hotkey", "reserved"]
+        SEQ_FIELDS = ["thread_id", "suspend_count", "priority_class", "priority", "teb", "stack", "thread_context"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_header']['start'] = self._io.pos()
-            self.len_header = self._io.read_bytes(4)
-            self._debug['len_header']['end'] = self._io.pos()
-            if not self.len_header == b"\x4C\x00\x00\x00":
-                raise kaitaistruct.ValidationNotEqualError(b"\x4C\x00\x00\x00", self.len_header, self._io, u"/types/file_header/seq/0")
-            self._debug['link_clsid']['start'] = self._io.pos()
-            self.link_clsid = self._io.read_bytes(16)
-            self._debug['link_clsid']['end'] = self._io.pos()
-            if not self.link_clsid == b"\x01\x14\x02\x00\x00\x00\x00\x00\xC0\x00\x00\x00\x00\x00\x00\x46":
-                raise kaitaistruct.ValidationNotEqualError(b"\x01\x14\x02\x00\x00\x00\x00\x00\xC0\x00\x00\x00\x00\x00\x00\x46", self.link_clsid, self._io, u"/types/file_header/seq/1")
-            self._debug['flags']['start'] = self._io.pos()
-            self._raw_flags = self._io.read_bytes(4)
-            _io__raw_flags = KaitaiStream(BytesIO(self._raw_flags))
-            self.flags = WindowsLnkFile.LinkFlags(_io__raw_flags, self, self._root)
-            self.flags._read()
-            self._debug['flags']['end'] = self._io.pos()
-            self._debug['file_attrs']['start'] = self._io.pos()
-            self.file_attrs = self._io.read_u4le()
-            self._debug['file_attrs']['end'] = self._io.pos()
-            self._debug['time_creation']['start'] = self._io.pos()
-            self.time_creation = self._io.read_u8le()
-            self._debug['time_creation']['end'] = self._io.pos()
-            self._debug['time_access']['start'] = self._io.pos()
-            self.time_access = self._io.read_u8le()
-            self._debug['time_access']['end'] = self._io.pos()
-            self._debug['time_write']['start'] = self._io.pos()
-            self.time_write = self._io.read_u8le()
-            self._debug['time_write']['end'] = self._io.pos()
-            self._debug['target_file_size']['start'] = self._io.pos()
-            self.target_file_size = self._io.read_u4le()
-            self._debug['target_file_size']['end'] = self._io.pos()
-            self._debug['icon_index']['start'] = self._io.pos()
-            self.icon_index = self._io.read_s4le()
-            self._debug['icon_index']['end'] = self._io.pos()
-            self._debug['show_command']['start'] = self._io.pos()
-            self.show_command = KaitaiStream.resolve_enum(WindowsLnkFile.WindowState, self._io.read_u4le())
-            self._debug['show_command']['end'] = self._io.pos()
-            self._debug['hotkey']['start'] = self._io.pos()
-            self.hotkey = self._io.read_u2le()
-            self._debug['hotkey']['end'] = self._io.pos()
+            self._debug['thread_id']['start'] = self._io.pos()
+            self.thread_id = self._io.read_u4le()
+            self._debug['thread_id']['end'] = self._io.pos()
+            self._debug['suspend_count']['start'] = self._io.pos()
+            self.suspend_count = self._io.read_u4le()
+            self._debug['suspend_count']['end'] = self._io.pos()
+            self._debug['priority_class']['start'] = self._io.pos()
+            self.priority_class = self._io.read_u4le()
+            self._debug['priority_class']['end'] = self._io.pos()
+            self._debug['priority']['start'] = self._io.pos()
+            self.priority = self._io.read_u4le()
+            self._debug['priority']['end'] = self._io.pos()
+            self._debug['teb']['start'] = self._io.pos()
+            self.teb = self._io.read_u8le()
+            self._debug['teb']['end'] = self._io.pos()
+            self._debug['stack']['start'] = self._io.pos()
+            self.stack = WindowsMinidump.MemoryDescriptor(self._io, self, self._root)
+            self.stack._read()
+            self._debug['stack']['end'] = self._io.pos()
+            self._debug['thread_context']['start'] = self._io.pos()
+            self.thread_context = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
+            self.thread_context._read()
+            self._debug['thread_context']['end'] = self._io.pos()
+
+
+    class MemoryList(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_memory64_list
+        """
+        SEQ_FIELDS = ["num_mem_ranges", "mem_ranges"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['num_mem_ranges']['start'] = self._io.pos()
+            self.num_mem_ranges = self._io.read_u4le()
+            self._debug['num_mem_ranges']['end'] = self._io.pos()
+            self._debug['mem_ranges']['start'] = self._io.pos()
+            self.mem_ranges = []
+            for i in range(self.num_mem_ranges):
+                if not 'arr' in self._debug['mem_ranges']:
+                    self._debug['mem_ranges']['arr'] = []
+                self._debug['mem_ranges']['arr'].append({'start': self._io.pos()})
+                _t_mem_ranges = WindowsMinidump.MemoryDescriptor(self._io, self, self._root)
+                _t_mem_ranges._read()
+                self.mem_ranges.append(_t_mem_ranges)
+                self._debug['mem_ranges']['arr'][i]['end'] = self._io.pos()
+
+            self._debug['mem_ranges']['end'] = self._io.pos()
+
+
+    class MemoryDescriptor(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_memory_descriptor
+        """
+        SEQ_FIELDS = ["addr_memory_range", "memory"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['addr_memory_range']['start'] = self._io.pos()
+            self.addr_memory_range = self._io.read_u8le()
+            self._debug['addr_memory_range']['end'] = self._io.pos()
+            self._debug['memory']['start'] = self._io.pos()
+            self.memory = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
+            self.memory._read()
+            self._debug['memory']['end'] = self._io.pos()
+
+
+    class ExceptionStream(KaitaiStruct):
+        """
+        .. seealso::
+           Source - https://learn.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_exception_stream
+        """
+        SEQ_FIELDS = ["thread_id", "reserved", "exception_rec", "thread_context"]
+        def __init__(self, _io, _parent=None, _root=None):
+            self._io = _io
+            self._parent = _parent
+            self._root = _root if _root else self
+            self._debug = collections.defaultdict(dict)
+
+        def _read(self):
+            self._debug['thread_id']['start'] = self._io.pos()
+            self.thread_id = self._io.read_u4le()
+            self._debug['thread_id']['end'] = self._io.pos()
             self._debug['reserved']['start'] = self._io.pos()
-            self.reserved = self._io.read_bytes(10)
+            self.reserved = self._io.read_u4le()
             self._debug['reserved']['end'] = self._io.pos()
-            if not self.reserved == b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00":
-                raise kaitaistruct.ValidationNotEqualError(b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00", self.reserved, self._io, u"/types/file_header/seq/11")
-
+            self._debug['exception_rec']['start'] = self._io.pos()
+            self.exception_rec = WindowsMinidump.ExceptionRecord(self._io, self, self._root)
+            self.exception_rec._read()
+            self._debug['exception_rec']['end'] = self._io.pos()
+            self._debug['thread_context']['start'] = self._io.pos()
+            self.thread_context = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
+            self.thread_context._read()
+            self._debug['thread_context']['end'] = self._io.pos()
+
+
+    @property
+    def streams(self):
+        if hasattr(self, '_m_streams'):
+            return self._m_streams
+
+        _pos = self._io.pos()
+        self._io.seek(self.ofs_streams)
+        self._debug['_m_streams']['start'] = self._io.pos()
+        self._m_streams = []
+        for i in range(self.num_streams):
+            if not 'arr' in self._debug['_m_streams']:
+                self._debug['_m_streams']['arr'] = []
+            self._debug['_m_streams']['arr'].append({'start': self._io.pos()})
+            _t__m_streams = WindowsMinidump.Dir(self._io, self, self._root)
+            _t__m_streams._read()
+            self._m_streams.append(_t__m_streams)
+            self._debug['_m_streams']['arr'][i]['end'] = self._io.pos()
+
+        self._debug['_m_streams']['end'] = self._io.pos()
+        self._io.seek(_pos)
+        return getattr(self, '_m_streams', None)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_minidump.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/zip.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,570 +131,680 @@
 from enum import Enum
 import collections
 
 
 if getattr(kaitaistruct, 'API_VERSION', (0, 9)) < (0, 9):
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
-class WindowsMinidump(KaitaiStruct):
-    """Windows MiniDump (MDMP) file provides a concise way to store process
-    core dumps, which is useful for debugging. Given its small size,
-    modularity, some cross-platform features and native support in some
-    debuggers, it is particularly useful for crash reporting, and is
-    used for that purpose in Windows and Google Chrome projects.
+import dos_datetime
+class Zip(KaitaiStruct):
+    """ZIP is a popular archive file format, introduced in 1989 by Phil Katz
+    and originally implemented in PKZIP utility by PKWARE.
     
-    The file itself is a container, which contains a number of typed
-    "streams", which contain some data according to its type attribute.
+    Thanks to solid support of it in most desktop environments and
+    operating systems, and algorithms / specs availability in public
+    domain, it quickly became tool of choice for implementing file
+    containers.
+    
+    For example, Java .jar files, OpenDocument, Office Open XML, EPUB files
+    are actually ZIP archives.
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_header
+       Source - https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
+    
+    
+    .. seealso::
+       Source - https://users.cs.jmu.edu/buchhofp/forensics/formats/pkzip.html
     """
 
-    class StreamTypes(Enum):
-        unused = 0
-        reserved_0 = 1
-        reserved_1 = 2
-        thread_list = 3
-        module_list = 4
-        memory_list = 5
-        exception = 6
-        system_info = 7
-        thread_ex_list = 8
-        memory_64_list = 9
-        comment_a = 10
-        comment_w = 11
-        handle_data = 12
-        function_table = 13
-        unloaded_module_list = 14
-        misc_info = 15
-        memory_info_list = 16
-        thread_info_list = 17
-        handle_operation_list = 18
-        token = 19
-        java_script_data = 20
-        system_memory_info = 21
-        process_vm_counters = 22
-        ipt_trace = 23
-        thread_names = 24
-        ce_null = 32768
-        ce_system_info = 32769
-        ce_exception = 32770
-        ce_module_list = 32771
-        ce_process_list = 32772
-        ce_thread_list = 32773
-        ce_thread_context_list = 32774
-        ce_thread_call_stack_list = 32775
-        ce_memory_virtual_list = 32776
-        ce_memory_physical_list = 32777
-        ce_bucket_parameters = 32778
-        ce_process_module_map = 32779
-        ce_diagnosis_list = 32780
-        md_crashpad_info_stream = 1129316353
-        md_raw_breakpad_info = 1197932545
-        md_raw_assertion_info = 1197932546
-        md_linux_cpu_info = 1197932547
-        md_linux_proc_status = 1197932548
-        md_linux_lsb_release = 1197932549
-        md_linux_cmd_line = 1197932550
-        md_linux_environ = 1197932551
-        md_linux_auxv = 1197932552
-        md_linux_maps = 1197932553
-        md_linux_dso_debug = 1197932554
-    SEQ_FIELDS = ["magic1", "magic2", "version", "num_streams", "ofs_streams", "checksum", "timestamp", "flags"]
+    class Compression(Enum):
+        none = 0
+        shrunk = 1
+        reduced_1 = 2
+        reduced_2 = 3
+        reduced_3 = 4
+        reduced_4 = 5
+        imploded = 6
+        deflated = 8
+        enhanced_deflated = 9
+        pkware_dcl_imploded = 10
+        bzip2 = 12
+        lzma = 14
+        ibm_terse = 18
+        ibm_lz77_z = 19
+        zstandard = 93
+        mp3 = 94
+        xz = 95
+        jpeg = 96
+        wavpack = 97
+        ppmd = 98
+        aex_encryption_marker = 99
+
+    class ExtraCodes(Enum):
+        zip64 = 1
+        av_info = 7
+        os2 = 9
+        ntfs = 10
+        openvms = 12
+        pkware_unix = 13
+        file_stream_and_fork_descriptors = 14
+        patch_descriptor = 15
+        pkcs7 = 20
+        x509_cert_id_and_signature_for_file = 21
+        x509_cert_id_for_central_dir = 22
+        strong_encryption_header = 23
+        record_management_controls = 24
+        pkcs7_enc_recip_cert_list = 25
+        ibm_s390_uncomp = 101
+        ibm_s390_comp = 102
+        poszip_4690 = 18064
+        extended_timestamp = 21589
+        beos = 25922
+        asi_unix = 30062
+        infozip_unix = 30805
+        infozip_unix_var_size = 30837
+        aex_encryption = 39169
+        apache_commons_compress = 41246
+        microsoft_open_packaging_growth_hint = 41504
+        sms_qdos = 64842
+    SEQ_FIELDS = ["sections"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
 
     def _read(self):
-        self._debug['magic1']['start'] = self._io.pos()
-        self.magic1 = self._io.read_bytes(4)
-        self._debug['magic1']['end'] = self._io.pos()
-        if not self.magic1 == b"\x4D\x44\x4D\x50":
-            raise kaitaistruct.ValidationNotEqualError(b"\x4D\x44\x4D\x50", self.magic1, self._io, u"/seq/0")
-        self._debug['magic2']['start'] = self._io.pos()
-        self.magic2 = self._io.read_bytes(2)
-        self._debug['magic2']['end'] = self._io.pos()
-        if not self.magic2 == b"\x93\xA7":
-            raise kaitaistruct.ValidationNotEqualError(b"\x93\xA7", self.magic2, self._io, u"/seq/1")
-        self._debug['version']['start'] = self._io.pos()
-        self.version = self._io.read_u2le()
-        self._debug['version']['end'] = self._io.pos()
-        self._debug['num_streams']['start'] = self._io.pos()
-        self.num_streams = self._io.read_u4le()
-        self._debug['num_streams']['end'] = self._io.pos()
-        self._debug['ofs_streams']['start'] = self._io.pos()
-        self.ofs_streams = self._io.read_u4le()
-        self._debug['ofs_streams']['end'] = self._io.pos()
-        self._debug['checksum']['start'] = self._io.pos()
-        self.checksum = self._io.read_u4le()
-        self._debug['checksum']['end'] = self._io.pos()
-        self._debug['timestamp']['start'] = self._io.pos()
-        self.timestamp = self._io.read_u4le()
-        self._debug['timestamp']['end'] = self._io.pos()
-        self._debug['flags']['start'] = self._io.pos()
-        self.flags = self._io.read_u8le()
-        self._debug['flags']['end'] = self._io.pos()
-
-    class ThreadList(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_thread_list
-        """
-        SEQ_FIELDS = ["num_threads", "threads"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['num_threads']['start'] = self._io.pos()
-            self.num_threads = self._io.read_u4le()
-            self._debug['num_threads']['end'] = self._io.pos()
-            self._debug['threads']['start'] = self._io.pos()
-            self.threads = []
-            for i in range(self.num_threads):
-                if not 'arr' in self._debug['threads']:
-                    self._debug['threads']['arr'] = []
-                self._debug['threads']['arr'].append({'start': self._io.pos()})
-                _t_threads = WindowsMinidump.Thread(self._io, self, self._root)
-                _t_threads._read()
-                self.threads.append(_t_threads)
-                self._debug['threads']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['threads']['end'] = self._io.pos()
-
-
-    class LocationDescriptor(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_location_descriptor
-        """
-        SEQ_FIELDS = ["len_data", "ofs_data"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
+        self._debug['sections']['start'] = self._io.pos()
+        self.sections = []
+        i = 0
+        while not self._io.is_eof():
+            if not 'arr' in self._debug['sections']:
+                self._debug['sections']['arr'] = []
+            self._debug['sections']['arr'].append({'start': self._io.pos()})
+            _t_sections = Zip.PkSection(self._io, self, self._root)
+            _t_sections._read()
+            self.sections.append(_t_sections)
+            self._debug['sections']['arr'][len(self.sections) - 1]['end'] = self._io.pos()
+            i += 1
 
-        def _read(self):
-            self._debug['len_data']['start'] = self._io.pos()
-            self.len_data = self._io.read_u4le()
-            self._debug['len_data']['end'] = self._io.pos()
-            self._debug['ofs_data']['start'] = self._io.pos()
-            self.ofs_data = self._io.read_u4le()
-            self._debug['ofs_data']['end'] = self._io.pos()
+        self._debug['sections']['end'] = self._io.pos()
 
-        @property
-        def data(self):
-            if hasattr(self, '_m_data'):
-                return self._m_data
-
-            io = self._root._io
-            _pos = io.pos()
-            io.seek(self.ofs_data)
-            self._debug['_m_data']['start'] = io.pos()
-            self._m_data = io.read_bytes(self.len_data)
-            self._debug['_m_data']['end'] = io.pos()
-            io.seek(_pos)
-            return getattr(self, '_m_data', None)
-
-
-    class MinidumpString(KaitaiStruct):
-        """Specific string serialization scheme used in MiniDump format is
-        actually a simple 32-bit length-prefixed UTF-16 string.
-        
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_string
-        """
-        SEQ_FIELDS = ["len_str", "str"]
+    class LocalFile(KaitaiStruct):
+        SEQ_FIELDS = ["header", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['len_str']['start'] = self._io.pos()
-            self.len_str = self._io.read_u4le()
-            self._debug['len_str']['end'] = self._io.pos()
-            self._debug['str']['start'] = self._io.pos()
-            self.str = (self._io.read_bytes(self.len_str)).decode(u"UTF-16LE")
-            self._debug['str']['end'] = self._io.pos()
+            self._debug['header']['start'] = self._io.pos()
+            self.header = Zip.LocalFileHeader(self._io, self, self._root)
+            self.header._read()
+            self._debug['header']['end'] = self._io.pos()
+            self._debug['body']['start'] = self._io.pos()
+            self.body = self._io.read_bytes(self.header.len_body_compressed)
+            self._debug['body']['end'] = self._io.pos()
 
 
-    class SystemInfo(KaitaiStruct):
-        """"System info" stream provides basic information about the
-        hardware and operating system which produces this dump.
-        
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_system_info
-        """
-
-        class CpuArchs(Enum):
-            intel = 0
-            arm = 5
-            ia64 = 6
-            amd64 = 9
-            unknown = 65535
-        SEQ_FIELDS = ["cpu_arch", "cpu_level", "cpu_revision", "num_cpus", "os_type", "os_ver_major", "os_ver_minor", "os_build", "os_platform", "ofs_service_pack", "os_suite_mask", "reserved2"]
+    class DataDescriptor(KaitaiStruct):
+        SEQ_FIELDS = ["crc32", "len_body_compressed", "len_body_uncompressed"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['cpu_arch']['start'] = self._io.pos()
-            self.cpu_arch = KaitaiStream.resolve_enum(WindowsMinidump.SystemInfo.CpuArchs, self._io.read_u2le())
-            self._debug['cpu_arch']['end'] = self._io.pos()
-            self._debug['cpu_level']['start'] = self._io.pos()
-            self.cpu_level = self._io.read_u2le()
-            self._debug['cpu_level']['end'] = self._io.pos()
-            self._debug['cpu_revision']['start'] = self._io.pos()
-            self.cpu_revision = self._io.read_u2le()
-            self._debug['cpu_revision']['end'] = self._io.pos()
-            self._debug['num_cpus']['start'] = self._io.pos()
-            self.num_cpus = self._io.read_u1()
-            self._debug['num_cpus']['end'] = self._io.pos()
-            self._debug['os_type']['start'] = self._io.pos()
-            self.os_type = self._io.read_u1()
-            self._debug['os_type']['end'] = self._io.pos()
-            self._debug['os_ver_major']['start'] = self._io.pos()
-            self.os_ver_major = self._io.read_u4le()
-            self._debug['os_ver_major']['end'] = self._io.pos()
-            self._debug['os_ver_minor']['start'] = self._io.pos()
-            self.os_ver_minor = self._io.read_u4le()
-            self._debug['os_ver_minor']['end'] = self._io.pos()
-            self._debug['os_build']['start'] = self._io.pos()
-            self.os_build = self._io.read_u4le()
-            self._debug['os_build']['end'] = self._io.pos()
-            self._debug['os_platform']['start'] = self._io.pos()
-            self.os_platform = self._io.read_u4le()
-            self._debug['os_platform']['end'] = self._io.pos()
-            self._debug['ofs_service_pack']['start'] = self._io.pos()
-            self.ofs_service_pack = self._io.read_u4le()
-            self._debug['ofs_service_pack']['end'] = self._io.pos()
-            self._debug['os_suite_mask']['start'] = self._io.pos()
-            self.os_suite_mask = self._io.read_u2le()
-            self._debug['os_suite_mask']['end'] = self._io.pos()
-            self._debug['reserved2']['start'] = self._io.pos()
-            self.reserved2 = self._io.read_u2le()
-            self._debug['reserved2']['end'] = self._io.pos()
-
-        @property
-        def service_pack(self):
-            if hasattr(self, '_m_service_pack'):
-                return self._m_service_pack
-
-            if self.ofs_service_pack > 0:
-                io = self._root._io
-                _pos = io.pos()
-                io.seek(self.ofs_service_pack)
-                self._debug['_m_service_pack']['start'] = io.pos()
-                self._m_service_pack = WindowsMinidump.MinidumpString(io, self, self._root)
-                self._m_service_pack._read()
-                self._debug['_m_service_pack']['end'] = io.pos()
-                io.seek(_pos)
+            self._debug['crc32']['start'] = self._io.pos()
+            self.crc32 = self._io.read_u4le()
+            self._debug['crc32']['end'] = self._io.pos()
+            self._debug['len_body_compressed']['start'] = self._io.pos()
+            self.len_body_compressed = self._io.read_u4le()
+            self._debug['len_body_compressed']['end'] = self._io.pos()
+            self._debug['len_body_uncompressed']['start'] = self._io.pos()
+            self.len_body_uncompressed = self._io.read_u4le()
+            self._debug['len_body_uncompressed']['end'] = self._io.pos()
 
-            return getattr(self, '_m_service_pack', None)
 
-
-    class ExceptionRecord(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_exception
-        """
-        SEQ_FIELDS = ["code", "flags", "inner_exception", "addr", "num_params", "reserved", "params"]
+    class ExtraField(KaitaiStruct):
+        SEQ_FIELDS = ["code", "len_body", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
             self._debug['code']['start'] = self._io.pos()
-            self.code = self._io.read_u4le()
+            self.code = KaitaiStream.resolve_enum(Zip.ExtraCodes, self._io.read_u2le())
             self._debug['code']['end'] = self._io.pos()
-            self._debug['flags']['start'] = self._io.pos()
-            self.flags = self._io.read_u4le()
-            self._debug['flags']['end'] = self._io.pos()
-            self._debug['inner_exception']['start'] = self._io.pos()
-            self.inner_exception = self._io.read_u8le()
-            self._debug['inner_exception']['end'] = self._io.pos()
-            self._debug['addr']['start'] = self._io.pos()
-            self.addr = self._io.read_u8le()
-            self._debug['addr']['end'] = self._io.pos()
-            self._debug['num_params']['start'] = self._io.pos()
-            self.num_params = self._io.read_u4le()
-            self._debug['num_params']['end'] = self._io.pos()
-            self._debug['reserved']['start'] = self._io.pos()
-            self.reserved = self._io.read_u4le()
-            self._debug['reserved']['end'] = self._io.pos()
-            self._debug['params']['start'] = self._io.pos()
-            self.params = []
-            for i in range(15):
-                if not 'arr' in self._debug['params']:
-                    self._debug['params']['arr'] = []
-                self._debug['params']['arr'].append({'start': self._io.pos()})
-                self.params.append(self._io.read_u8le())
-                self._debug['params']['arr'][i]['end'] = self._io.pos()
-
-            self._debug['params']['end'] = self._io.pos()
-
-
-    class MiscInfo(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_misc_info
-        """
-        SEQ_FIELDS = ["len_info", "flags1", "process_id", "process_create_time", "process_user_time", "process_kernel_time", "cpu_max_mhz", "cpu_cur_mhz", "cpu_limit_mhz", "cpu_max_idle_state", "cpu_cur_idle_state"]
-        def __init__(self, _io, _parent=None, _root=None):
-            self._io = _io
-            self._parent = _parent
-            self._root = _root if _root else self
-            self._debug = collections.defaultdict(dict)
-
-        def _read(self):
-            self._debug['len_info']['start'] = self._io.pos()
-            self.len_info = self._io.read_u4le()
-            self._debug['len_info']['end'] = self._io.pos()
-            self._debug['flags1']['start'] = self._io.pos()
-            self.flags1 = self._io.read_u4le()
-            self._debug['flags1']['end'] = self._io.pos()
-            self._debug['process_id']['start'] = self._io.pos()
-            self.process_id = self._io.read_u4le()
-            self._debug['process_id']['end'] = self._io.pos()
-            self._debug['process_create_time']['start'] = self._io.pos()
-            self.process_create_time = self._io.read_u4le()
-            self._debug['process_create_time']['end'] = self._io.pos()
-            self._debug['process_user_time']['start'] = self._io.pos()
-            self.process_user_time = self._io.read_u4le()
-            self._debug['process_user_time']['end'] = self._io.pos()
-            self._debug['process_kernel_time']['start'] = self._io.pos()
-            self.process_kernel_time = self._io.read_u4le()
-            self._debug['process_kernel_time']['end'] = self._io.pos()
-            self._debug['cpu_max_mhz']['start'] = self._io.pos()
-            self.cpu_max_mhz = self._io.read_u4le()
-            self._debug['cpu_max_mhz']['end'] = self._io.pos()
-            self._debug['cpu_cur_mhz']['start'] = self._io.pos()
-            self.cpu_cur_mhz = self._io.read_u4le()
-            self._debug['cpu_cur_mhz']['end'] = self._io.pos()
-            self._debug['cpu_limit_mhz']['start'] = self._io.pos()
-            self.cpu_limit_mhz = self._io.read_u4le()
-            self._debug['cpu_limit_mhz']['end'] = self._io.pos()
-            self._debug['cpu_max_idle_state']['start'] = self._io.pos()
-            self.cpu_max_idle_state = self._io.read_u4le()
-            self._debug['cpu_max_idle_state']['end'] = self._io.pos()
-            self._debug['cpu_cur_idle_state']['start'] = self._io.pos()
-            self.cpu_cur_idle_state = self._io.read_u4le()
-            self._debug['cpu_cur_idle_state']['end'] = self._io.pos()
-
+            self._debug['len_body']['start'] = self._io.pos()
+            self.len_body = self._io.read_u2le()
+            self._debug['len_body']['end'] = self._io.pos()
+            self._debug['body']['start'] = self._io.pos()
+            _on = self.code
+            if _on == Zip.ExtraCodes.ntfs:
+                self._raw_body = self._io.read_bytes(self.len_body)
+                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                self.body = Zip.ExtraField.Ntfs(_io__raw_body, self, self._root)
+                self.body._read()
+            elif _on == Zip.ExtraCodes.extended_timestamp:
+                self._raw_body = self._io.read_bytes(self.len_body)
+                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                self.body = Zip.ExtraField.ExtendedTimestamp(_io__raw_body, self, self._root)
+                self.body._read()
+            elif _on == Zip.ExtraCodes.infozip_unix_var_size:
+                self._raw_body = self._io.read_bytes(self.len_body)
+                _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                self.body = Zip.ExtraField.InfozipUnixVarSize(_io__raw_body, self, self._root)
+                self.body._read()
+            else:
+                self.body = self._io.read_bytes(self.len_body)
+            self._debug['body']['end'] = self._io.pos()
 
-    class Dir(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_directory
-        """
-        SEQ_FIELDS = ["stream_type", "len_data", "ofs_data"]
+        class Ntfs(KaitaiStruct):
+            """
+            .. seealso::
+               Source - https://github.com/LuaDist/zip/blob/b710806/proginfo/extrafld.txt#L191
+            """
+            SEQ_FIELDS = ["reserved", "attributes"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['reserved']['start'] = self._io.pos()
+                self.reserved = self._io.read_u4le()
+                self._debug['reserved']['end'] = self._io.pos()
+                self._debug['attributes']['start'] = self._io.pos()
+                self.attributes = []
+                i = 0
+                while not self._io.is_eof():
+                    if not 'arr' in self._debug['attributes']:
+                        self._debug['attributes']['arr'] = []
+                    self._debug['attributes']['arr'].append({'start': self._io.pos()})
+                    _t_attributes = Zip.ExtraField.Ntfs.Attribute(self._io, self, self._root)
+                    _t_attributes._read()
+                    self.attributes.append(_t_attributes)
+                    self._debug['attributes']['arr'][len(self.attributes) - 1]['end'] = self._io.pos()
+                    i += 1
+
+                self._debug['attributes']['end'] = self._io.pos()
+
+            class Attribute(KaitaiStruct):
+                SEQ_FIELDS = ["tag", "len_body", "body"]
+                def __init__(self, _io, _parent=None, _root=None):
+                    self._io = _io
+                    self._parent = _parent
+                    self._root = _root if _root else self
+                    self._debug = collections.defaultdict(dict)
+
+                def _read(self):
+                    self._debug['tag']['start'] = self._io.pos()
+                    self.tag = self._io.read_u2le()
+                    self._debug['tag']['end'] = self._io.pos()
+                    self._debug['len_body']['start'] = self._io.pos()
+                    self.len_body = self._io.read_u2le()
+                    self._debug['len_body']['end'] = self._io.pos()
+                    self._debug['body']['start'] = self._io.pos()
+                    _on = self.tag
+                    if _on == 1:
+                        self._raw_body = self._io.read_bytes(self.len_body)
+                        _io__raw_body = KaitaiStream(BytesIO(self._raw_body))
+                        self.body = Zip.ExtraField.Ntfs.Attribute1(_io__raw_body, self, self._root)
+                        self.body._read()
+                    else:
+                        self.body = self._io.read_bytes(self.len_body)
+                    self._debug['body']['end'] = self._io.pos()
+
+
+            class Attribute1(KaitaiStruct):
+                SEQ_FIELDS = ["last_mod_time", "last_access_time", "creation_time"]
+                def __init__(self, _io, _parent=None, _root=None):
+                    self._io = _io
+                    self._parent = _parent
+                    self._root = _root if _root else self
+                    self._debug = collections.defaultdict(dict)
+
+                def _read(self):
+                    self._debug['last_mod_time']['start'] = self._io.pos()
+                    self.last_mod_time = self._io.read_u8le()
+                    self._debug['last_mod_time']['end'] = self._io.pos()
+                    self._debug['last_access_time']['start'] = self._io.pos()
+                    self.last_access_time = self._io.read_u8le()
+                    self._debug['last_access_time']['end'] = self._io.pos()
+                    self._debug['creation_time']['start'] = self._io.pos()
+                    self.creation_time = self._io.read_u8le()
+                    self._debug['creation_time']['end'] = self._io.pos()
+
+
+
+        class ExtendedTimestamp(KaitaiStruct):
+            """
+            .. seealso::
+               Source - https://github.com/LuaDist/zip/blob/b710806/proginfo/extrafld.txt#L817
+            """
+            SEQ_FIELDS = ["flags", "mod_time", "access_time", "create_time"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['flags']['start'] = self._io.pos()
+                self._raw_flags = self._io.read_bytes(1)
+                _io__raw_flags = KaitaiStream(BytesIO(self._raw_flags))
+                self.flags = Zip.ExtraField.ExtendedTimestamp.InfoFlags(_io__raw_flags, self, self._root)
+                self.flags._read()
+                self._debug['flags']['end'] = self._io.pos()
+                if self.flags.has_mod_time:
+                    self._debug['mod_time']['start'] = self._io.pos()
+                    self.mod_time = self._io.read_u4le()
+                    self._debug['mod_time']['end'] = self._io.pos()
+
+                if self.flags.has_access_time:
+                    self._debug['access_time']['start'] = self._io.pos()
+                    self.access_time = self._io.read_u4le()
+                    self._debug['access_time']['end'] = self._io.pos()
+
+                if self.flags.has_create_time:
+                    self._debug['create_time']['start'] = self._io.pos()
+                    self.create_time = self._io.read_u4le()
+                    self._debug['create_time']['end'] = self._io.pos()
+
+
+            class InfoFlags(KaitaiStruct):
+                SEQ_FIELDS = ["has_mod_time", "has_access_time", "has_create_time", "reserved"]
+                def __init__(self, _io, _parent=None, _root=None):
+                    self._io = _io
+                    self._parent = _parent
+                    self._root = _root if _root else self
+                    self._debug = collections.defaultdict(dict)
+
+                def _read(self):
+                    self._debug['has_mod_time']['start'] = self._io.pos()
+                    self.has_mod_time = self._io.read_bits_int_le(1) != 0
+                    self._debug['has_mod_time']['end'] = self._io.pos()
+                    self._debug['has_access_time']['start'] = self._io.pos()
+                    self.has_access_time = self._io.read_bits_int_le(1) != 0
+                    self._debug['has_access_time']['end'] = self._io.pos()
+                    self._debug['has_create_time']['start'] = self._io.pos()
+                    self.has_create_time = self._io.read_bits_int_le(1) != 0
+                    self._debug['has_create_time']['end'] = self._io.pos()
+                    self._debug['reserved']['start'] = self._io.pos()
+                    self.reserved = self._io.read_bits_int_le(5)
+                    self._debug['reserved']['end'] = self._io.pos()
+
+
+
+        class InfozipUnixVarSize(KaitaiStruct):
+            """
+            .. seealso::
+               Source - https://github.com/LuaDist/zip/blob/b710806/proginfo/extrafld.txt#L1339
+            """
+            SEQ_FIELDS = ["version", "len_uid", "uid", "len_gid", "gid"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['version']['start'] = self._io.pos()
+                self.version = self._io.read_u1()
+                self._debug['version']['end'] = self._io.pos()
+                self._debug['len_uid']['start'] = self._io.pos()
+                self.len_uid = self._io.read_u1()
+                self._debug['len_uid']['end'] = self._io.pos()
+                self._debug['uid']['start'] = self._io.pos()
+                self.uid = self._io.read_bytes(self.len_uid)
+                self._debug['uid']['end'] = self._io.pos()
+                self._debug['len_gid']['start'] = self._io.pos()
+                self.len_gid = self._io.read_u1()
+                self._debug['len_gid']['end'] = self._io.pos()
+                self._debug['gid']['start'] = self._io.pos()
+                self.gid = self._io.read_bytes(self.len_gid)
+                self._debug['gid']['end'] = self._io.pos()
+
+
+
+    class CentralDirEntry(KaitaiStruct):
+        """
+        .. seealso::
+           - 4.3.12 - https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
+        """
+        SEQ_FIELDS = ["version_made_by", "version_needed_to_extract", "flags", "compression_method", "file_mod_time", "crc32", "len_body_compressed", "len_body_uncompressed", "len_file_name", "len_extra", "len_comment", "disk_number_start", "int_file_attr", "ext_file_attr", "ofs_local_header", "file_name", "extra", "comment"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['stream_type']['start'] = self._io.pos()
-            self.stream_type = KaitaiStream.resolve_enum(WindowsMinidump.StreamTypes, self._io.read_u4le())
-            self._debug['stream_type']['end'] = self._io.pos()
-            self._debug['len_data']['start'] = self._io.pos()
-            self.len_data = self._io.read_u4le()
-            self._debug['len_data']['end'] = self._io.pos()
-            self._debug['ofs_data']['start'] = self._io.pos()
-            self.ofs_data = self._io.read_u4le()
-            self._debug['ofs_data']['end'] = self._io.pos()
+            self._debug['version_made_by']['start'] = self._io.pos()
+            self.version_made_by = self._io.read_u2le()
+            self._debug['version_made_by']['end'] = self._io.pos()
+            self._debug['version_needed_to_extract']['start'] = self._io.pos()
+            self.version_needed_to_extract = self._io.read_u2le()
+            self._debug['version_needed_to_extract']['end'] = self._io.pos()
+            self._debug['flags']['start'] = self._io.pos()
+            self.flags = self._io.read_u2le()
+            self._debug['flags']['end'] = self._io.pos()
+            self._debug['compression_method']['start'] = self._io.pos()
+            self.compression_method = KaitaiStream.resolve_enum(Zip.Compression, self._io.read_u2le())
+            self._debug['compression_method']['end'] = self._io.pos()
+            self._debug['file_mod_time']['start'] = self._io.pos()
+            self._raw_file_mod_time = self._io.read_bytes(4)
+            _io__raw_file_mod_time = KaitaiStream(BytesIO(self._raw_file_mod_time))
+            self.file_mod_time = dos_datetime.DosDatetime(_io__raw_file_mod_time)
+            self.file_mod_time._read()
+            self._debug['file_mod_time']['end'] = self._io.pos()
+            self._debug['crc32']['start'] = self._io.pos()
+            self.crc32 = self._io.read_u4le()
+            self._debug['crc32']['end'] = self._io.pos()
+            self._debug['len_body_compressed']['start'] = self._io.pos()
+            self.len_body_compressed = self._io.read_u4le()
+            self._debug['len_body_compressed']['end'] = self._io.pos()
+            self._debug['len_body_uncompressed']['start'] = self._io.pos()
+            self.len_body_uncompressed = self._io.read_u4le()
+            self._debug['len_body_uncompressed']['end'] = self._io.pos()
+            self._debug['len_file_name']['start'] = self._io.pos()
+            self.len_file_name = self._io.read_u2le()
+            self._debug['len_file_name']['end'] = self._io.pos()
+            self._debug['len_extra']['start'] = self._io.pos()
+            self.len_extra = self._io.read_u2le()
+            self._debug['len_extra']['end'] = self._io.pos()
+            self._debug['len_comment']['start'] = self._io.pos()
+            self.len_comment = self._io.read_u2le()
+            self._debug['len_comment']['end'] = self._io.pos()
+            self._debug['disk_number_start']['start'] = self._io.pos()
+            self.disk_number_start = self._io.read_u2le()
+            self._debug['disk_number_start']['end'] = self._io.pos()
+            self._debug['int_file_attr']['start'] = self._io.pos()
+            self.int_file_attr = self._io.read_u2le()
+            self._debug['int_file_attr']['end'] = self._io.pos()
+            self._debug['ext_file_attr']['start'] = self._io.pos()
+            self.ext_file_attr = self._io.read_u4le()
+            self._debug['ext_file_attr']['end'] = self._io.pos()
+            self._debug['ofs_local_header']['start'] = self._io.pos()
+            self.ofs_local_header = self._io.read_s4le()
+            self._debug['ofs_local_header']['end'] = self._io.pos()
+            self._debug['file_name']['start'] = self._io.pos()
+            self.file_name = (self._io.read_bytes(self.len_file_name)).decode(u"UTF-8")
+            self._debug['file_name']['end'] = self._io.pos()
+            self._debug['extra']['start'] = self._io.pos()
+            self._raw_extra = self._io.read_bytes(self.len_extra)
+            _io__raw_extra = KaitaiStream(BytesIO(self._raw_extra))
+            self.extra = Zip.Extras(_io__raw_extra, self, self._root)
+            self.extra._read()
+            self._debug['extra']['end'] = self._io.pos()
+            self._debug['comment']['start'] = self._io.pos()
+            self.comment = (self._io.read_bytes(self.len_comment)).decode(u"UTF-8")
+            self._debug['comment']['end'] = self._io.pos()
 
         @property
-        def data(self):
-            if hasattr(self, '_m_data'):
-                return self._m_data
+        def local_header(self):
+            if hasattr(self, '_m_local_header'):
+                return self._m_local_header
 
             _pos = self._io.pos()
-            self._io.seek(self.ofs_data)
-            self._debug['_m_data']['start'] = self._io.pos()
-            _on = self.stream_type
-            if _on == WindowsMinidump.StreamTypes.memory_list:
-                self._raw__m_data = self._io.read_bytes(self.len_data)
-                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
-                self._m_data = WindowsMinidump.MemoryList(_io__raw__m_data, self, self._root)
-                self._m_data._read()
-            elif _on == WindowsMinidump.StreamTypes.misc_info:
-                self._raw__m_data = self._io.read_bytes(self.len_data)
-                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
-                self._m_data = WindowsMinidump.MiscInfo(_io__raw__m_data, self, self._root)
-                self._m_data._read()
-            elif _on == WindowsMinidump.StreamTypes.thread_list:
-                self._raw__m_data = self._io.read_bytes(self.len_data)
-                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
-                self._m_data = WindowsMinidump.ThreadList(_io__raw__m_data, self, self._root)
-                self._m_data._read()
-            elif _on == WindowsMinidump.StreamTypes.exception:
-                self._raw__m_data = self._io.read_bytes(self.len_data)
-                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
-                self._m_data = WindowsMinidump.ExceptionStream(_io__raw__m_data, self, self._root)
-                self._m_data._read()
-            elif _on == WindowsMinidump.StreamTypes.system_info:
-                self._raw__m_data = self._io.read_bytes(self.len_data)
-                _io__raw__m_data = KaitaiStream(BytesIO(self._raw__m_data))
-                self._m_data = WindowsMinidump.SystemInfo(_io__raw__m_data, self, self._root)
-                self._m_data._read()
-            else:
-                self._m_data = self._io.read_bytes(self.len_data)
-            self._debug['_m_data']['end'] = self._io.pos()
+            self._io.seek(self.ofs_local_header)
+            self._debug['_m_local_header']['start'] = self._io.pos()
+            self._m_local_header = Zip.PkSection(self._io, self, self._root)
+            self._m_local_header._read()
+            self._debug['_m_local_header']['end'] = self._io.pos()
             self._io.seek(_pos)
-            return getattr(self, '_m_data', None)
+            return getattr(self, '_m_local_header', None)
 
 
-    class Thread(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_thread
-        """
-        SEQ_FIELDS = ["thread_id", "suspend_count", "priority_class", "priority", "teb", "stack", "thread_context"]
+    class PkSection(KaitaiStruct):
+        SEQ_FIELDS = ["magic", "section_type", "body"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['thread_id']['start'] = self._io.pos()
-            self.thread_id = self._io.read_u4le()
-            self._debug['thread_id']['end'] = self._io.pos()
-            self._debug['suspend_count']['start'] = self._io.pos()
-            self.suspend_count = self._io.read_u4le()
-            self._debug['suspend_count']['end'] = self._io.pos()
-            self._debug['priority_class']['start'] = self._io.pos()
-            self.priority_class = self._io.read_u4le()
-            self._debug['priority_class']['end'] = self._io.pos()
-            self._debug['priority']['start'] = self._io.pos()
-            self.priority = self._io.read_u4le()
-            self._debug['priority']['end'] = self._io.pos()
-            self._debug['teb']['start'] = self._io.pos()
-            self.teb = self._io.read_u8le()
-            self._debug['teb']['end'] = self._io.pos()
-            self._debug['stack']['start'] = self._io.pos()
-            self.stack = WindowsMinidump.MemoryDescriptor(self._io, self, self._root)
-            self.stack._read()
-            self._debug['stack']['end'] = self._io.pos()
-            self._debug['thread_context']['start'] = self._io.pos()
-            self.thread_context = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
-            self.thread_context._read()
-            self._debug['thread_context']['end'] = self._io.pos()
+            self._debug['magic']['start'] = self._io.pos()
+            self.magic = self._io.read_bytes(2)
+            self._debug['magic']['end'] = self._io.pos()
+            if not self.magic == b"\x50\x4B":
+                raise kaitaistruct.ValidationNotEqualError(b"\x50\x4B", self.magic, self._io, u"/types/pk_section/seq/0")
+            self._debug['section_type']['start'] = self._io.pos()
+            self.section_type = self._io.read_u2le()
+            self._debug['section_type']['end'] = self._io.pos()
+            self._debug['body']['start'] = self._io.pos()
+            _on = self.section_type
+            if _on == 513:
+                self.body = Zip.CentralDirEntry(self._io, self, self._root)
+                self.body._read()
+            elif _on == 1027:
+                self.body = Zip.LocalFile(self._io, self, self._root)
+                self.body._read()
+            elif _on == 1541:
+                self.body = Zip.EndOfCentralDir(self._io, self, self._root)
+                self.body._read()
+            elif _on == 2055:
+                self.body = Zip.DataDescriptor(self._io, self, self._root)
+                self.body._read()
+            self._debug['body']['end'] = self._io.pos()
 
 
-    class MemoryList(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_memory64_list
-        """
-        SEQ_FIELDS = ["num_mem_ranges", "mem_ranges"]
+    class Extras(KaitaiStruct):
+        SEQ_FIELDS = ["entries"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['num_mem_ranges']['start'] = self._io.pos()
-            self.num_mem_ranges = self._io.read_u4le()
-            self._debug['num_mem_ranges']['end'] = self._io.pos()
-            self._debug['mem_ranges']['start'] = self._io.pos()
-            self.mem_ranges = []
-            for i in range(self.num_mem_ranges):
-                if not 'arr' in self._debug['mem_ranges']:
-                    self._debug['mem_ranges']['arr'] = []
-                self._debug['mem_ranges']['arr'].append({'start': self._io.pos()})
-                _t_mem_ranges = WindowsMinidump.MemoryDescriptor(self._io, self, self._root)
-                _t_mem_ranges._read()
-                self.mem_ranges.append(_t_mem_ranges)
-                self._debug['mem_ranges']['arr'][i]['end'] = self._io.pos()
+            self._debug['entries']['start'] = self._io.pos()
+            self.entries = []
+            i = 0
+            while not self._io.is_eof():
+                if not 'arr' in self._debug['entries']:
+                    self._debug['entries']['arr'] = []
+                self._debug['entries']['arr'].append({'start': self._io.pos()})
+                _t_entries = Zip.ExtraField(self._io, self, self._root)
+                _t_entries._read()
+                self.entries.append(_t_entries)
+                self._debug['entries']['arr'][len(self.entries) - 1]['end'] = self._io.pos()
+                i += 1
 
-            self._debug['mem_ranges']['end'] = self._io.pos()
+            self._debug['entries']['end'] = self._io.pos()
 
 
-    class MemoryDescriptor(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_memory_descriptor
-        """
-        SEQ_FIELDS = ["addr_memory_range", "memory"]
+    class LocalFileHeader(KaitaiStruct):
+        SEQ_FIELDS = ["version", "flags", "compression_method", "file_mod_time", "crc32", "len_body_compressed", "len_body_uncompressed", "len_file_name", "len_extra", "file_name", "extra"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['addr_memory_range']['start'] = self._io.pos()
-            self.addr_memory_range = self._io.read_u8le()
-            self._debug['addr_memory_range']['end'] = self._io.pos()
-            self._debug['memory']['start'] = self._io.pos()
-            self.memory = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
-            self.memory._read()
-            self._debug['memory']['end'] = self._io.pos()
-
-
-    class ExceptionStream(KaitaiStruct):
-        """
-        .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/api/minidumpapiset/ns-minidumpapiset-minidump_exception_stream
-        """
-        SEQ_FIELDS = ["thread_id", "reserved", "exception_rec", "thread_context"]
+            self._debug['version']['start'] = self._io.pos()
+            self.version = self._io.read_u2le()
+            self._debug['version']['end'] = self._io.pos()
+            self._debug['flags']['start'] = self._io.pos()
+            self._raw_flags = self._io.read_bytes(2)
+            _io__raw_flags = KaitaiStream(BytesIO(self._raw_flags))
+            self.flags = Zip.LocalFileHeader.GpFlags(_io__raw_flags, self, self._root)
+            self.flags._read()
+            self._debug['flags']['end'] = self._io.pos()
+            self._debug['compression_method']['start'] = self._io.pos()
+            self.compression_method = KaitaiStream.resolve_enum(Zip.Compression, self._io.read_u2le())
+            self._debug['compression_method']['end'] = self._io.pos()
+            self._debug['file_mod_time']['start'] = self._io.pos()
+            self._raw_file_mod_time = self._io.read_bytes(4)
+            _io__raw_file_mod_time = KaitaiStream(BytesIO(self._raw_file_mod_time))
+            self.file_mod_time = dos_datetime.DosDatetime(_io__raw_file_mod_time)
+            self.file_mod_time._read()
+            self._debug['file_mod_time']['end'] = self._io.pos()
+            self._debug['crc32']['start'] = self._io.pos()
+            self.crc32 = self._io.read_u4le()
+            self._debug['crc32']['end'] = self._io.pos()
+            self._debug['len_body_compressed']['start'] = self._io.pos()
+            self.len_body_compressed = self._io.read_u4le()
+            self._debug['len_body_compressed']['end'] = self._io.pos()
+            self._debug['len_body_uncompressed']['start'] = self._io.pos()
+            self.len_body_uncompressed = self._io.read_u4le()
+            self._debug['len_body_uncompressed']['end'] = self._io.pos()
+            self._debug['len_file_name']['start'] = self._io.pos()
+            self.len_file_name = self._io.read_u2le()
+            self._debug['len_file_name']['end'] = self._io.pos()
+            self._debug['len_extra']['start'] = self._io.pos()
+            self.len_extra = self._io.read_u2le()
+            self._debug['len_extra']['end'] = self._io.pos()
+            self._debug['file_name']['start'] = self._io.pos()
+            self.file_name = (self._io.read_bytes(self.len_file_name)).decode(u"UTF-8")
+            self._debug['file_name']['end'] = self._io.pos()
+            self._debug['extra']['start'] = self._io.pos()
+            self._raw_extra = self._io.read_bytes(self.len_extra)
+            _io__raw_extra = KaitaiStream(BytesIO(self._raw_extra))
+            self.extra = Zip.Extras(_io__raw_extra, self, self._root)
+            self.extra._read()
+            self._debug['extra']['end'] = self._io.pos()
+
+        class GpFlags(KaitaiStruct):
+            """
+            .. seealso::
+               - 4.4.4 - https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
+            
+            
+            .. seealso::
+               Local file headers - https://users.cs.jmu.edu/buchhofp/forensics/formats/pkzip.html
+            """
+
+            class DeflateMode(Enum):
+                normal = 0
+                maximum = 1
+                fast = 2
+                super_fast = 3
+            SEQ_FIELDS = ["file_encrypted", "comp_options_raw", "has_data_descriptor", "reserved_1", "comp_patched_data", "strong_encrypt", "reserved_2", "lang_encoding", "reserved_3", "mask_header_values", "reserved_4"]
+            def __init__(self, _io, _parent=None, _root=None):
+                self._io = _io
+                self._parent = _parent
+                self._root = _root if _root else self
+                self._debug = collections.defaultdict(dict)
+
+            def _read(self):
+                self._debug['file_encrypted']['start'] = self._io.pos()
+                self.file_encrypted = self._io.read_bits_int_le(1) != 0
+                self._debug['file_encrypted']['end'] = self._io.pos()
+                self._debug['comp_options_raw']['start'] = self._io.pos()
+                self.comp_options_raw = self._io.read_bits_int_le(2)
+                self._debug['comp_options_raw']['end'] = self._io.pos()
+                self._debug['has_data_descriptor']['start'] = self._io.pos()
+                self.has_data_descriptor = self._io.read_bits_int_le(1) != 0
+                self._debug['has_data_descriptor']['end'] = self._io.pos()
+                self._debug['reserved_1']['start'] = self._io.pos()
+                self.reserved_1 = self._io.read_bits_int_le(1) != 0
+                self._debug['reserved_1']['end'] = self._io.pos()
+                self._debug['comp_patched_data']['start'] = self._io.pos()
+                self.comp_patched_data = self._io.read_bits_int_le(1) != 0
+                self._debug['comp_patched_data']['end'] = self._io.pos()
+                self._debug['strong_encrypt']['start'] = self._io.pos()
+                self.strong_encrypt = self._io.read_bits_int_le(1) != 0
+                self._debug['strong_encrypt']['end'] = self._io.pos()
+                self._debug['reserved_2']['start'] = self._io.pos()
+                self.reserved_2 = self._io.read_bits_int_le(4)
+                self._debug['reserved_2']['end'] = self._io.pos()
+                self._debug['lang_encoding']['start'] = self._io.pos()
+                self.lang_encoding = self._io.read_bits_int_le(1) != 0
+                self._debug['lang_encoding']['end'] = self._io.pos()
+                self._debug['reserved_3']['start'] = self._io.pos()
+                self.reserved_3 = self._io.read_bits_int_le(1) != 0
+                self._debug['reserved_3']['end'] = self._io.pos()
+                self._debug['mask_header_values']['start'] = self._io.pos()
+                self.mask_header_values = self._io.read_bits_int_le(1) != 0
+                self._debug['mask_header_values']['end'] = self._io.pos()
+                self._debug['reserved_4']['start'] = self._io.pos()
+                self.reserved_4 = self._io.read_bits_int_le(2)
+                self._debug['reserved_4']['end'] = self._io.pos()
+
+            @property
+            def deflated_mode(self):
+                if hasattr(self, '_m_deflated_mode'):
+                    return self._m_deflated_mode
+
+                if  ((self._parent.compression_method == Zip.Compression.deflated) or (self._parent.compression_method == Zip.Compression.enhanced_deflated)) :
+                    self._m_deflated_mode = KaitaiStream.resolve_enum(Zip.LocalFileHeader.GpFlags.DeflateMode, self.comp_options_raw)
+
+                return getattr(self, '_m_deflated_mode', None)
+
+            @property
+            def imploded_dict_byte_size(self):
+                """8KiB or 4KiB in bytes."""
+                if hasattr(self, '_m_imploded_dict_byte_size'):
+                    return self._m_imploded_dict_byte_size
+
+                if self._parent.compression_method == Zip.Compression.imploded:
+                    self._m_imploded_dict_byte_size = ((8 if (self.comp_options_raw & 1) != 0 else 4) * 1024)
+
+                return getattr(self, '_m_imploded_dict_byte_size', None)
+
+            @property
+            def imploded_num_sf_trees(self):
+                if hasattr(self, '_m_imploded_num_sf_trees'):
+                    return self._m_imploded_num_sf_trees
+
+                if self._parent.compression_method == Zip.Compression.imploded:
+                    self._m_imploded_num_sf_trees = (3 if (self.comp_options_raw & 2) != 0 else 2)
+
+                return getattr(self, '_m_imploded_num_sf_trees', None)
+
+            @property
+            def lzma_has_eos_marker(self):
+                if hasattr(self, '_m_lzma_has_eos_marker'):
+                    return self._m_lzma_has_eos_marker
+
+                if self._parent.compression_method == Zip.Compression.lzma:
+                    self._m_lzma_has_eos_marker = (self.comp_options_raw & 1) != 0
+
+                return getattr(self, '_m_lzma_has_eos_marker', None)
+
+
+
+    class EndOfCentralDir(KaitaiStruct):
+        SEQ_FIELDS = ["disk_of_end_of_central_dir", "disk_of_central_dir", "num_central_dir_entries_on_disk", "num_central_dir_entries_total", "len_central_dir", "ofs_central_dir", "len_comment", "comment"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
 
         def _read(self):
-            self._debug['thread_id']['start'] = self._io.pos()
-            self.thread_id = self._io.read_u4le()
-            self._debug['thread_id']['end'] = self._io.pos()
-            self._debug['reserved']['start'] = self._io.pos()
-            self.reserved = self._io.read_u4le()
-            self._debug['reserved']['end'] = self._io.pos()
-            self._debug['exception_rec']['start'] = self._io.pos()
-            self.exception_rec = WindowsMinidump.ExceptionRecord(self._io, self, self._root)
-            self.exception_rec._read()
-            self._debug['exception_rec']['end'] = self._io.pos()
-            self._debug['thread_context']['start'] = self._io.pos()
-            self.thread_context = WindowsMinidump.LocationDescriptor(self._io, self, self._root)
-            self.thread_context._read()
-            self._debug['thread_context']['end'] = self._io.pos()
-
-
-    @property
-    def streams(self):
-        if hasattr(self, '_m_streams'):
-            return self._m_streams
-
-        _pos = self._io.pos()
-        self._io.seek(self.ofs_streams)
-        self._debug['_m_streams']['start'] = self._io.pos()
-        self._m_streams = []
-        for i in range(self.num_streams):
-            if not 'arr' in self._debug['_m_streams']:
-                self._debug['_m_streams']['arr'] = []
-            self._debug['_m_streams']['arr'].append({'start': self._io.pos()})
-            _t__m_streams = WindowsMinidump.Dir(self._io, self, self._root)
-            _t__m_streams._read()
-            self._m_streams.append(_t__m_streams)
-            self._debug['_m_streams']['arr'][i]['end'] = self._io.pos()
-
-        self._debug['_m_streams']['end'] = self._io.pos()
-        self._io.seek(_pos)
-        return getattr(self, '_m_streams', None)
+            self._debug['disk_of_end_of_central_dir']['start'] = self._io.pos()
+            self.disk_of_end_of_central_dir = self._io.read_u2le()
+            self._debug['disk_of_end_of_central_dir']['end'] = self._io.pos()
+            self._debug['disk_of_central_dir']['start'] = self._io.pos()
+            self.disk_of_central_dir = self._io.read_u2le()
+            self._debug['disk_of_central_dir']['end'] = self._io.pos()
+            self._debug['num_central_dir_entries_on_disk']['start'] = self._io.pos()
+            self.num_central_dir_entries_on_disk = self._io.read_u2le()
+            self._debug['num_central_dir_entries_on_disk']['end'] = self._io.pos()
+            self._debug['num_central_dir_entries_total']['start'] = self._io.pos()
+            self.num_central_dir_entries_total = self._io.read_u2le()
+            self._debug['num_central_dir_entries_total']['end'] = self._io.pos()
+            self._debug['len_central_dir']['start'] = self._io.pos()
+            self.len_central_dir = self._io.read_u4le()
+            self._debug['len_central_dir']['end'] = self._io.pos()
+            self._debug['ofs_central_dir']['start'] = self._io.pos()
+            self.ofs_central_dir = self._io.read_u4le()
+            self._debug['ofs_central_dir']['end'] = self._io.pos()
+            self._debug['len_comment']['start'] = self._io.pos()
+            self.len_comment = self._io.read_u2le()
+            self._debug['len_comment']['end'] = self._io.pos()
+            self._debug['comment']['start'] = self._io.pos()
+            self.comment = (self._io.read_bytes(self.len_comment)).decode(u"UTF-8")
+            self._debug['comment']['end'] = self._io.pos()
+
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_resource_file.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_resource_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
     class Resource(KaitaiStruct):
         """Each resource has a `type` and a `name`, which can be used to
         identify it, and a `value`. Both `type` and `name` can be a
         number or a string.
         
         .. seealso::
-           Source - https://docs.microsoft.com/en-us/windows/win32/menurc/resourceheader
+           Source - https://learn.microsoft.com/en-us/windows/win32/menurc/resourceheader
         """
 
         class PredefTypes(Enum):
             cursor = 1
             bitmap = 2
             icon = 3
             menu = 4
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_shell_items.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_shell_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     * Windows Shell link files (.lnk) Windows registry
     * Windows registry "ShellBags" keys
     
     The format is mostly undocumented, and is known to vary between
     various Windows versions.
     
     .. seealso::
-       Source - https://github.com/libyal/libfwsi/blob/master/documentation/Windows%20Shell%20Item%20format.asciidoc
+       Source - https://github.com/libyal/libfwsi/blob/main/documentation/Windows%20Shell%20Item%20format.asciidoc
     """
     SEQ_FIELDS = ["items"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
@@ -229,15 +229,15 @@
                 self._debug['data']['end'] = self._io.pos()
 
 
 
     class RootFolderBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/libyal/libfwsi/blob/master/documentation/Windows%20Shell%20Item%20format.asciidoc#32-root-folder-shell-item
+           Source - https://github.com/libyal/libfwsi/blob/main/documentation/Windows%20Shell%20Item%20format.asciidoc#32-root-folder-shell-item
         """
         SEQ_FIELDS = ["sort_index", "shell_folder_id"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -250,15 +250,15 @@
             self.shell_folder_id = self._io.read_bytes(16)
             self._debug['shell_folder_id']['end'] = self._io.pos()
 
 
     class VolumeBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/libyal/libfwsi/blob/master/documentation/Windows%20Shell%20Item%20format.asciidoc#33-volume-shell-item
+           Source - https://github.com/libyal/libfwsi/blob/main/documentation/Windows%20Shell%20Item%20format.asciidoc#33-volume-shell-item
         """
         SEQ_FIELDS = ["flags"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
@@ -268,15 +268,15 @@
             self.flags = self._io.read_u1()
             self._debug['flags']['end'] = self._io.pos()
 
 
     class FileEntryBody(KaitaiStruct):
         """
         .. seealso::
-           Source - https://github.com/libyal/libfwsi/blob/master/documentation/Windows%20Shell%20Item%20format.asciidoc#34-file-entry-shell-item
+           Source - https://github.com/libyal/libfwsi/blob/main/documentation/Windows%20Shell%20Item%20format.asciidoc#34-file-entry-shell-item
         """
         SEQ_FIELDS = ["_unnamed0", "file_size", "last_mod_time", "file_attrs"]
         def __init__(self, _io, _parent=None, _root=None):
             self._io = _io
             self._parent = _parent
             self._root = _root if _root else self
             self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/windows_systemtime.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/windows_systemtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     raise Exception("Incompatible Kaitai Struct Python API: 0.9 or later is required, but you have %s" % (kaitaistruct.__version__))
 
 class WindowsSystemtime(KaitaiStruct):
     """Microsoft Windows SYSTEMTIME structure, stores individual components
     of date and time as individual fields, up to millisecond precision.
     
     .. seealso::
-       Source - https://docs.microsoft.com/en-us/windows/win32/api/minwinbase/ns-minwinbase-systemtime
+       Source - https://learn.microsoft.com/en-us/windows/win32/api/minwinbase/ns-minwinbase-systemtime
     """
     SEQ_FIELDS = ["year", "month", "dow", "day", "hour", "min", "sec", "msec"]
     def __init__(self, _io, _parent=None, _root=None):
         self._io = _io
         self._parent = _parent
         self._root = _root if _root else self
         self._debug = collections.defaultdict(dict)
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/wmf.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/wmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     
     Inside, it provides a serialized list of Windows GDI (Graphics
     Device Interface) function calls, which, if played back, result in
     an image being drawn on a given surface (display, off-screen buffer,
     printer, etc).
     
     .. seealso::
-       Source - http://www.digitalpreservation.gov/formats/digformatspecs/WindowsMetafileFormat(wmf)Specification.pdf
+       Source - https://www.loc.gov/preservation/digital/formats/digformatspecs/WindowsMetafileFormat(wmf)Specification.pdf
     """
 
     class Func(Enum):
         eof = 0
         savedc = 30
         realizepalette = 53
         setpalentries = 55
```

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/xar.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/xar.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/xwd.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/xwd.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/formats/zisofs.py` & `pytai-hex-0.2.7/pytai/kaitai/formats/zisofs.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/kaitai/kaitaistruct.py` & `pytai-hex-0.2.7/pytai/kaitai/kaitaistruct.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/model.py` & `pytai-hex-0.2.7/pytai/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -292,14 +292,15 @@
             except PytaiUnparsedAccessException:
                 yield None
 
 class Model(object):
 
     def __init__(self):
         self.parsers = {}
+        self.highlight_context = {ht: set() for ht in HighlightType if HighlightType.is_custom(ht)}
 
     def get_parser(self, **kwargs) -> Parser:
         """Return a parser to parse the required files.
 
         Keyword Args:
             kaitai_format:
                 Path to a compiled Kaitai Structure definition 
@@ -404,14 +405,128 @@
                     raise PyTaiException("Unable to parse file!")
 
         except PyTaiException as e:
             comm_queue.put(e)
         except Exception as e:
             comm_queue.put(PyTaiException(f"Error while parsing file:\n'{str(e)}'"))
 
+    def get_byte_range(self, mmap: mmap.mmap, start_offset: int, end_offset: int, byte_representation: ByteRepresentation):
+        """Retrieve a byte range according to a given representation
+
+        This function returns the byte array in the given range formatted according to the given
+        representation.
+        
+        Args:
+            mmap:
+                Memory map of the file to extract the byte array from.
+            start_offset:
+                Start offset of the given range.
+            end_offset:
+                End offset of the given range.
+            byte_representation:
+                The byte representation to return.
+        """
+        if byte_representation == ByteRepresentation.HEX_STREAM:
+            return mmap[start_offset:end_offset].hex()
+        elif byte_representation == ByteRepresentation.HEX:
+            return mmap[start_offset:end_offset].hex(" ")
+        elif byte_representation == ByteRepresentation.RAW_BYTES:
+            return mmap[start_offset:end_offset]
+
+    @staticmethod    
+    def _s1_contains_s2(s1: Tuple[int, int], s2: Tuple[int, int]):
+        """Returns whether the range in s1 is contained withing the range in s2"""
+        return s1[0] <= s2[0] and s1[1] >= s2[1]
+        
+    def process_highlight(self, start_offset: int, end_offset: int, mark: bool, highlight_type: HighlightType) -> bool:       
+        """Handle a highlight/un-highlight request.
+
+        If the request is to highlight a range:
+            Iterate all existing highlighted ranges. 
+            If the requested range is already within a previously-highlighted range: Nothing to do.
+            If the requested range contains a previously-highlighted range: Remove the old one in 
+            favor of the new one.
+            If the requested range does not overlap an existing range: Just add the new one.
+        If the request is to remove a range:
+            Just remove it, since we make sure during addition that there's no overlap between
+            added ranges.
+
+        Args:
+            start_offset:
+                The start offset for the requested range.
+
+            end_offset:
+                The end offset for the requested range.
+
+            mark:
+                True if the request is to highlight the range, False to un-highlight
+
+            highlight_type:
+                The highlight type
+
+        Returns:
+            False if no action was needed, True otherwise.
+        
+        """
+        this_segment = (start_offset, end_offset)
+        if mark:
+            new_set = set()
+            for segment in self.highlight_context[highlight_type]:
+                if self._s1_contains_s2(segment, this_segment):
+                    return False
+                elif not self._s1_contains_s2(this_segment, segment):
+                    new_set.add(segment)
+            new_set.add(this_segment)
+            self.highlight_context[highlight_type] = new_set
+            return True
+        else:
+            res = this_segment in self.highlight_context[highlight_type]
+            if res:
+                self.highlight_context[highlight_type].remove(this_segment)
+            return res
+
+    def get_highlighted_colors(self, start_offset: int, end_offset: int) -> Dict[HighlightType, HighlightDetails]:
+        """Return the highlighted colors for the given range.
+
+        Args:
+            start_offset:
+                The start offset for the requested range.
+
+            end_offset:
+                The end offset for the requested range
+
+        Returns:
+            A mapping between highlight types and the following information:
+                - Whether the given highlighter is active for the range
+                - If it is active, whether the range was explicitly highlighted itself,
+                  or whether it is highlighted as a result of being included in a larger
+                  highlighted range.
+
+        """
+        res = {}
+        this_segment = (start_offset, end_offset)
+        for ht in HighlightType:
+            if not HighlightType.is_custom(ht):
+                continue
+            
+            is_active = False
+            is_exact_match = False
+
+            for segment in self.highlight_context[ht]:
+                if segment == this_segment:
+                    is_active = True
+                    is_exact_match = True
+                    break
+                elif self._s1_contains_s2(segment, this_segment):
+                    is_active = True
+                    break
+            
+            res[ht] = HighlightDetails(is_active = is_active, is_exact_match = is_exact_match)
+        return res
+    
         
 class SearchContext(object):
     """Context for searching within a given binary.
     
     Supports a single search term and allows searching forward and backwards for it.
     The context remembers the previous occurrance of the term and the next search request
     continues from the previous one.
```

### Comparing `pytai-hex-0.2.6/pytai/tests/kaitai_to_xml.py` & `pytai-hex-0.2.7/pytai/tests/kaitai_to_xml.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/tests/xml_utils.py` & `pytai-hex-0.2.7/pytai/tests/xml_utils.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/utils.py` & `pytai-hex-0.2.7/pytai/utils.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/view/assets/pytai.ico` & `pytai-hex-0.2.7/pytai/view/assets/pytai.ico`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/view/bars.py` & `pytai-hex-0.2.7/pytai/view/bars.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/view/events.py` & `pytai-hex-0.2.7/pytai/view/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,8 +57,20 @@
     # Find next result for search
     FIND_NEXT          = enum.auto()
 
     # Find previous result for search
     FIND_PREV          = enum.auto()
 
     # Get x-ref
-    GET_XREF           = enum.auto()
+    GET_XREF           = enum.auto()
+
+    # Copy the selection to the clipboard
+    COPY_SELECTION     = enum.auto()
+
+    # Return the selection as a raw byte array
+    GET_SELECTION      = enum.auto()
+
+    # Highlight the selection with a custom color
+    HIGHLIGHT_SELECTION      = enum.auto()
+
+    # Get the active/inactive highlighters for the given selection
+    GET_HIGHLIGHTED_COLORS   = enum.auto()
```

### Comparing `pytai-hex-0.2.6/pytai/view/hex_area.py` & `pytai-hex-0.2.7/pytai/view/hex_area.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,22 +38,29 @@
 from io import StringIO
 
 import queue
 
 from .events import *
 from .menus import *
 
+from ..common import *
 from ..utils import *
 
 TAG_JUSTIFY_RIGHT = 'justify_right'
 TAG_HIGHLIGHT = 'highlight'
 TAG_SELECTION = 'selection'
 TAG_GOTO = 'goto'
-
-TAGS = [TAG_JUSTIFY_RIGHT, TAG_HIGHLIGHT, TAG_SELECTION, TAG_GOTO]
+TAG_HIGHLIGHT_CUSTOM1 = 'highlight_c1'
+TAG_HIGHLIGHT_CUSTOM2 = 'highlight_c2'
+TAG_HIGHLIGHT_CUSTOM3 = 'highlight_c3'
+
+TAGS = [
+    TAG_JUSTIFY_RIGHT, TAG_HIGHLIGHT, TAG_SELECTION, TAG_GOTO, 
+    TAG_HIGHLIGHT_CUSTOM1, TAG_HIGHLIGHT_CUSTOM2, TAG_HIGHLIGHT_CUSTOM3
+]
 
 class HexAreaView():
     """Implements the view for the hex area."""
 
     # Bytes to show per row in hex view
     BYTES_PER_ROW = 16
     REPR_CHARS_PER_BYTE_HEX = 3 # Two chars for hex representation + one space
@@ -84,21 +91,27 @@
         self.textbox_address.pack(side=tk.LEFT, fill=tk.Y, expand=False)
 
         self.textbox_address.tag_configure(TAG_JUSTIFY_RIGHT, justify = tk.RIGHT)
 
         self.textbox_hex = tk.Text(self.main_frame, width = 47, padx = 10, wrap = tk.NONE, bd = 0)
         self.textbox_hex.pack(side=tk.LEFT, fill=tk.Y, expand=False)
 
-        self.textbox_hex.tag_config(TAG_HIGHLIGHT, background='gold3')
+        self.textbox_hex.tag_config(TAG_HIGHLIGHT_CUSTOM1, background='khaki1')
+        self.textbox_hex.tag_config(TAG_HIGHLIGHT_CUSTOM2, background='DarkSeaGreen1')
+        self.textbox_hex.tag_config(TAG_HIGHLIGHT_CUSTOM3, background='thistle1')
+        self.textbox_hex.tag_config(TAG_HIGHLIGHT, background='gold3') # Must be last of highlight tags
         self.textbox_hex.tag_config(TAG_GOTO, background='lightcyan')
 
         self.textbox_ascii = tk.Text(self.main_frame, width = 17, padx = 10, wrap = tk.NONE, bd = 0)
         self.textbox_ascii.pack(side=tk.LEFT, fill=tk.Y, expand=False)
 
-        self.textbox_ascii.tag_config(TAG_HIGHLIGHT, background='gold3')
+        self.textbox_ascii.tag_config(TAG_HIGHLIGHT_CUSTOM1, background='khaki1')
+        self.textbox_ascii.tag_config(TAG_HIGHLIGHT_CUSTOM2, background='DarkSeaGreen1')
+        self.textbox_ascii.tag_config(TAG_HIGHLIGHT_CUSTOM3, background='thistle1')
+        self.textbox_ascii.tag_config(TAG_HIGHLIGHT, background='gold3') # Must be last of highlight tags
         self.textbox_ascii.tag_config(TAG_SELECTION, background='lightgray')
 
 
         self.textboxes = [self.textbox_address, self.textbox_hex, self.textbox_ascii]
 
         self.scrollbar = tk.Scrollbar(self.main_frame)
         self.scrollbar.pack(side=tk.RIGHT, fill=tk.Y, expand = False)
@@ -303,35 +316,62 @@
         
         Returns:
             Offset in tkinter line.column notation.
         """
         line = (offset // cls.BYTES_PER_ROW) + 1 # Line is 1-based
         column = ((offset % cls.BYTES_PER_ROW) * chars_per_byte)
         return f"{line}.{column + adjust_column}"
+    
+    @staticmethod
+    def _highlight_to_tag(highlight_type: HighlightType):
+        """Mapping of highlighter to tag."""
+        tag = {
+            HighlightType.DEFAULT: TAG_HIGHLIGHT,
+            HighlightType.CUSTOM1: TAG_HIGHLIGHT_CUSTOM1,    
+            HighlightType.CUSTOM2: TAG_HIGHLIGHT_CUSTOM2,
+            HighlightType.CUSTOM3: TAG_HIGHLIGHT_CUSTOM3    
+        }.get(highlight_type)
+
+        return tag
+
+    def unmark_range(self, start_offset: int, end_offset: int, highlight_type: HighlightType = HighlightType.DEFAULT) -> None:
+        """Unmarks the given range for the given highlighter."""
+        tag = self._highlight_to_tag(highlight_type)
+
+        self.textbox_hex.tag_remove(tag, 
+            self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_HEX, start_offset) if start_offset is not None else "1.0", 
+            self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_HEX, end_offset, -1) if end_offset is not None else tk.END)
+        self.textbox_ascii.tag_remove(tag, 
+            self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_ASCII, start_offset) if start_offset is not None else "1.0", 
+            self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_ASCII, end_offset) if end_offset is not None else tk.END)
+
 
-    def mark_range(self, start_offset: int, end_offset: int) -> None:
+    def mark_range(self, start_offset: int, end_offset: int, mark: bool, highlight_type: HighlightType = HighlightType.DEFAULT) -> None:
         """Highlight a range between the given offsets, and optionally jump to it.
         
         Args:
             start_offset:
                 Offset to highlight from (absolute index of byte in file)
             end_offset:
                 Offset to highlight to (absolute index of byte in file)
+            highlight_type:
+                Type of highlight to use. Use HighlightType.DEFAULT for selection, 
+                or HighlightType.CUSTOMx for user triggered custom highlights
         """
-        self.textbox_hex.tag_remove(TAG_HIGHLIGHT, "1.0", tk.END)
-        self.textbox_ascii.tag_remove(TAG_HIGHLIGHT, "1.0", tk.END)
+
+        tag = self._highlight_to_tag(highlight_type)
 
         if start_offset is not None and end_offset is not None:
             # Mark in hex view:
-            self.textbox_hex.tag_add(TAG_HIGHLIGHT, 
+            self.textbox_hex.tag_add(tag, 
                                      self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_HEX, start_offset), 
                                      self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_HEX, end_offset, -1)) # Remove trailing space
 
             # Mark in ASCII view:
-            self.textbox_ascii.tag_add(TAG_HIGHLIGHT, 
+            self.textbox_ascii.tag_add(tag, 
                                        self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_ASCII, start_offset), 
                                        self._offset_to_line_column(self.REPR_CHARS_PER_BYTE_ASCII, end_offset))
 
     def make_visible(self, offset: Optional[int], length: int = 1, highlight: bool = False) -> None:
         """Jump to a given offset in the HEX viewer, and optionally highlight it.
         
         Args:
```

### Comparing `pytai-hex-0.2.6/pytai/view/main.py` & `pytai-hex-0.2.7/pytai/view/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,38 +198,43 @@
         
         Args:
             msg:
                 Error message to display.
         """
         messagebox.showerror("Error", msg)
 
-    def mark_range(self, start_offset: int, end_offset: int) -> None:
+    def mark_range(self, start_offset: int, end_offset: int, mark: bool, highlight_type: HighlightType = HighlightType.DEFAULT) -> None:
         """Highlight a range between the given offsets.
         
         Args:
             start_offset:
                 Offset to highlight from (absolute index of byte in file)
             end_offset:
                 Offset to highlight to (absolute index of byte in file)
+            mark:
+                True to highlight a range, False to remove the highlight
+            highlight_type:
+                Type of highlight to use. Use HighlightType.DEFAULT for selection, 
+                or HighlightType.CUSTOMx for user triggered custom highlights
         """
-        if start_offset is not None and end_offset is not None:
+        if mark and start_offset is not None and end_offset is not None:
             length = end_offset - start_offset
             
             status = []
             if length > 0:
                 # end offset is exclusive, but we want to show inclusive range
                 status.append(f"Range: {hex(start_offset)}-{hex(end_offset - 1)}")
 
             status.append(f"Length: {length} ({hex(length)}) bytes")
 
             self.set_status(" | ".join(status))
+            self.hex_view.mark_range(start_offset, end_offset, mark, highlight_type)
         else:
             self.set_status("")
-        self.hex_view.mark_range(start_offset, end_offset)
-
+            self.hex_view.unmark_range(start_offset, end_offset, highlight_type)
 
     def show_loading(self) -> None:
         """Show the loading window."""
         
         # tkinter has better performance when the widgets aren't visible
         self.pw.pack_forget()
```

### Comparing `pytai-hex-0.2.6/pytai/view/menus.py` & `pytai-hex-0.2.7/pytai/view/menus.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,18 +21,19 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 """
 from typing import Dict, Callable
-from tkinter import messagebox
+from functools import partial
 
 import tkinter as tk
 import enum
+from ..common import *
 
 
 class BaseHexAreaMenu():
     """Base class for a menu in the Hex area."""
     def __init__(self, parent):
         self.parent = parent
 
@@ -98,31 +99,40 @@
         self.commands_require_file = {}
 
         def add_command(menu, requires_file: bool, **kwargs) -> None:
             self.commands_require_file[(menu, kwargs['label'])] = requires_file
             menu.add_command(**kwargs)
 
         filemenu = tk.Menu(self, tearoff=0)
-        add_command(filemenu, False, label = "Open...", command = lambda: self.callbacks[self.Events.OPEN](None), accelerator = "Ctrl+O")
-        add_command(filemenu, False, label = "Exit", command = parent.quit)
+        add_command(filemenu, False, label = "Open...", 
+                    command = lambda: self.callbacks[self.Events.OPEN](None), accelerator = "Ctrl+O")
+        add_command(filemenu, False, label = "Exit", 
+                    command = parent.quit)
         self.add_cascade(label = "File", menu = filemenu)
 
         searchmenu = tk.Menu(self, tearoff = 0)
-        add_command(searchmenu, True, label = "Find...", command = lambda: self.callbacks[self.Events.SEARCH](None), accelerator = "Ctrl+F")
-        add_command(searchmenu, True, label = "Find Next", command = lambda: self.callbacks[self.Events.FIND_NEXT](None), accelerator = "F3")
-        add_command(searchmenu, True, label = "Find Previous", command = lambda: self.callbacks[self.Events.FIND_PREV](None), accelerator = "Shift+F3")
+        add_command(searchmenu, True, label = "Find...", 
+                    command = lambda: self.callbacks[self.Events.SEARCH](None), accelerator = "Ctrl+F")
+        add_command(searchmenu, True, label = "Find Next", 
+                    command = lambda: self.callbacks[self.Events.FIND_NEXT](None), accelerator = "F3")
+        add_command(searchmenu, True, label = "Find Previous", 
+                    command = lambda: self.callbacks[self.Events.FIND_PREV](None), accelerator = "Shift+F3")
         searchmenu.add_separator()
-        add_command(searchmenu, True, label = "Go to...", command = lambda: self.callbacks[self.Events.GOTO](None), accelerator = "Ctrl+G")
+        add_command(searchmenu, True, label = "Go to...", 
+                    command = lambda: self.callbacks[self.Events.GOTO](None), accelerator = "Ctrl+G")
         self.add_cascade(label = "Search", menu = searchmenu)
         
         viewmenu = tk.Menu(self, tearoff = 0)
-        add_command(viewmenu, True, label = "Refresh", command = lambda: self.callbacks[self.Events.REFRESH](None), accelerator = "F5")
+        add_command(viewmenu, True, label = "Refresh", 
+                    command = lambda: self.callbacks[self.Events.REFRESH](None), accelerator = "F5")
         viewmenu.add_separator()
-        add_command(viewmenu, True, label = "Expand Tree", command = lambda: self.callbacks[self.Events.EXPAND_TREE]())
-        add_command(viewmenu, True, label = "Collapse Tree", command = lambda: self.callbacks[self.Events.COLLAPSE_TREE]())
+        add_command(viewmenu, True, label = "Expand Tree", 
+                    command = lambda: self.callbacks[self.Events.EXPAND_TREE]())
+        add_command(viewmenu, True, label = "Collapse Tree", 
+                    command = lambda: self.callbacks[self.Events.COLLAPSE_TREE]())
         self.add_cascade(label = "View", menu = viewmenu)
 
         helpmenu = tk.Menu(self, tearoff = 0)
         add_command(helpmenu, False, label = "About...", command = self.show_about)
         self.add_cascade(label = "Help", menu = helpmenu)
 
         self.toggle_loaded_file_commands(enable = False)
@@ -162,13 +172,122 @@
 
         self.menu = tk.Menu(self.parent, tearoff = 0)
 
         if callbacks.keys() != set(self.Events):
             raise KeyError(f"Callbacks must contain all events in {set(self.Events)} ")
         self.callbacks = callbacks
 
-        self.menu.add_command(label = "Show X-Ref", command = lambda: self.callbacks[self.Events.GET_XREF](self._current_event))
+        self.menu.add_command(label = "Show X-Ref", 
+                              command = lambda: self.callbacks[self.Events.GET_XREF](self._current_event))
 
     def show(self, event) -> None:
         """Show the menu."""
         self._current_event = event
-        super().show(event)
+        super().show(event)
+
+class TreeItemMenu():
+    """Menu displayed after right-clicking an item in the tree area."""
+
+    class Events(enum.Enum):
+        """Events that can be triggered by the menu."""
+        
+        # User wants to copy the selection to the clipboard
+        COPY = enum.auto()
+        
+        # User wants to export the selection to a binary
+        SAVE_AS = enum.auto()
+
+        # User wants to highlight a selection with a custom color
+        HIGHLIGHT = enum.auto()
+
+    def __init__(self, parent, callbacks: Dict[Events, Callable[..., None]]):
+        """Instantiate the class.
+        
+        Args:
+            parent: 
+                Parent tk class.
+                
+            callbacks:
+                Dictionary of callbacks to call when an event from Events occurs
+                
+        """
+        self.parent = parent
+        self.menu = tk.Menu(self.parent, tearoff = 0)
+
+        if callbacks.keys() != set(self.Events):
+            raise KeyError(f"Callbacks must contain all events in {set(self.Events)} ")
+        self.callbacks = callbacks
+
+        copy_menu = tk.Menu(self.parent, tearoff=0)
+        copy_menu.add_command(label = "Copy as Hex Array",  command = self._copy_hex)
+        copy_menu.add_command(label = "Copy as Hex Stream", command = self._copy_hex_stream)
+        copy_menu.add_command(label = "Copy as Raw Bytes",  command = self._copy_raw_bytes)
+
+        self.highlight_menu = tk.Menu(self.parent, tearoff=0)
+        self.highlight_colors = {}
+        for ht in HighlightType:
+            if (not HighlightType.is_custom(ht)):
+                continue
+
+            self.highlight_colors[ht] = {
+                "label": f"Color {len(self.highlight_colors) + 1}", 
+                "variable": tk.BooleanVar(), 
+                "command": partial(self._highlight, highlight_type = ht)
+            }
+            self.highlight_menu.add_checkbutton(self.highlight_colors[ht])
+
+ 
+        self.menu.add_cascade(label='Highlight', menu = self.highlight_menu)
+        self.menu.add_cascade(label = "Copy", menu = copy_menu)
+        self.menu.add_separator()
+        self.menu.add_command(label ="Save as...", command = self._save_as)
+        
+
+    def show(self, event, highlighted_colors: Dict[HighlightType, HighlightDetails]) -> None:
+        """Show the menu.
+        
+        Args:
+            highlighted_colors:
+                A mapping between the different highlighters available and their details:
+                    - Whether the given highlighter is active for this item
+                    - If it's active, whether it was added explicitly for this item
+        """
+        self._current_event = event
+        for ht, details in highlighted_colors.items():
+            self.highlight_colors[ht]["variable"].set(details.is_active)
+
+            # If the highlighter was added for the parent, don't allow removing
+            # if from this item, only from the parent.
+            is_disabled = details.is_active and not details.is_exact_match
+
+            self.highlight_menu.entryconfig(self.highlight_colors[ht]["label"], 
+                                            state = tk.DISABLED if is_disabled else tk.NORMAL)
+
+        try:
+            self.menu.tk_popup(event.x_root, event.y_root)
+        finally:
+            self.menu.grab_release()
+
+    def hide(self):
+        """Hide the menu"""
+        self.menu.unpost()
+
+    def _copy_hex(self):
+        """Copy the selection as a Hex Array"""
+        self.callbacks[self.Events.COPY](self._current_event, ByteRepresentation.HEX)
+
+    def _copy_hex_stream(self):
+        """Copy the selection as a Hex Stream"""
+        self.callbacks[self.Events.COPY](self._current_event, ByteRepresentation.HEX_STREAM)
+
+    def _copy_raw_bytes(self):
+        """Copy the selection as raw bytes"""
+        self.callbacks[self.Events.COPY](self._current_event, ByteRepresentation.RAW_BYTES)
+
+    def _save_as(self):
+        """Export the selection to a binary"""
+        self.callbacks[self.Events.SAVE_AS](self._current_event)
+
+    def _highlight(self, highlight_type: HighlightType):
+        """Highlight a selection with a custom color"""
+        self.callbacks[self.Events.HIGHLIGHT](self._current_event, highlight_type, 
+                                              bool(self.highlight_colors[highlight_type]["variable"].get()))
```

### Comparing `pytai-hex-0.2.6/pytai/view/tree_area.py` & `pytai-hex-0.2.7/pytai/view/tree_area.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import tkinter as tk
 from tkinter import ttk
 
 from typing import Dict, Callable, Tuple
 
 from .bars import *
 from .events import *
+from .menus import TreeItemMenu
 
 from ..common import *
 
 TAG_OFFSET_PREFIX = "_offset_"
 TAG_OFFSET_SEPARATOR = "-"
 TAG_METAVAR = "metavar"
 
@@ -99,14 +100,22 @@
                 range_tag = tag.replace(TAG_OFFSET_PREFIX, "")
                 break
         
         if range_tag == None:
             return (None, None)
 
         return tuple(map(int, range_tag.split(TAG_OFFSET_SEPARATOR)))
+    
+    def is_metavar(self) -> bool:
+        """Returns True if and only if this is a metavar"""
+        return TAG_METAVAR in self._item["tags"]
+    
+    def is_root(self) -> bool:
+        """Returns True for the root and False for other nodes"""
+        return self._tree.parent(self._id) == ""
 
 
 class TreeAreaView():
     """Implements the view for the key area."""
 
     def __init__(self, root, parent, address_bar: AddressBar, callbacks: Dict[Events, Callable[..., None]]):
         """Instantiate the class.
@@ -135,21 +144,29 @@
 
         for i, column in enumerate(columns):
             self.tree.heading(f"#{i}", text = column, anchor = tk.W)
             self.tree.column(f"#{i}", minwidth = 100, stretch = tk.NO, anchor = tk.W)
 
         self.tree.pack(side = tk.LEFT, fill = tk.BOTH, expand=True)
         self.tree.bind('<<TreeviewSelect>>', self._item_selected)
+        self.tree.bind('<Button-3>', self._on_right_click)
+        self.tree.bind('<Button-1>', lambda event: self.right_click_menu.hide())
         self.tree.tag_configure(TAG_METAVAR, foreground = 'gray')
 
         self.vsb = ttk.Scrollbar(self.wrapper, orient = tk.VERTICAL, command = self.tree.yview)
         self.vsb.pack(side = tk.RIGHT, fill = tk.Y)
 
         self.tree.configure(yscrollcommand = self.vsb.set)
 
+        self.right_click_menu = TreeItemMenu(self.parent, {
+            TreeItemMenu.Events.COPY: self._copy,
+            TreeItemMenu.Events.SAVE_AS: self._save_as,
+            TreeItemMenu.Events.HIGHLIGHT: self._highlight
+        })
+
         self.fix_tkinter_color_tags()
 
 
     def reset(self) -> None:
         """Reset the key area to its initial state."""
         self.tree.delete(*self.tree.get_children())
         self.address_bar.set_address('')
@@ -167,14 +184,48 @@
     def _item_selected(self, event) -> None:
         """Handle an event where the user selects a key."""
         selected_item = self.selected_item
 
         self.callbacks[Events.STRUCTURE_SELECTED](selected_item.path, *selected_item.range)
         self.address_bar.set_address(selected_item.path)
         
+    def _on_right_click(self, event) -> None:
+        """Handle a right click on a tree item."""
+        item = self.tree.identify('item', event.x, event.y)
+        show_menu = False
+        if item:
+            # Right click was on an actual item (not free space)
+            tree_item = TreeItem(self.tree, item)
+            if not tree_item.is_metavar() and not tree_item.is_root():
+                show_menu = True
+
+        if show_menu:
+            self.mark_tree_element(item)
+            selected_item = self.selected_item
+            highlighted_colors = self.callbacks[Events.GET_HIGHLIGHTED_COLORS](selected_item.path, *selected_item.range)
+            self.right_click_menu.show(event, highlighted_colors)
+        else:
+            self.right_click_menu.hide()
+
+    def _copy(self, event, byte_representation: ByteRepresentation) -> None:
+        """Copy the selection to the clipboard."""
+        selected_item = self.selected_item
+        self.callbacks[Events.COPY_SELECTION](selected_item.path, *selected_item.range, byte_representation)
+
+    def _save_as(self, event) -> None:
+        """Save the selection to a binary file."""
+        with tk.filedialog.asksaveasfile(mode = 'wb', defaultextension = '.bin', title = 'Export bytes...') as newf:
+            selected_item = self.selected_item
+            newf.write(self.callbacks[Events.GET_SELECTION](selected_item.path, *selected_item.range))
+
+    def _highlight(self, event, highlight_type: HighlightType, mark: bool) -> None:
+        """Highlight the selection with a custom color."""
+        selected_item = self.selected_item
+        self.callbacks[Events.HIGHLIGHT_SELECTION](selected_item.path, *selected_item.range, highlight_type, mark)
+
     def add_item(self, parent_handle: str, name: str, extra_info: str, start_offset: int, end_offset: int, is_metavar: bool) -> str:
         """Add an item to the structure tree.
         
         Args:
             parent_handle:
                 Handle to the parent of the current item, based on a previous
                 return value of add_item() (or '' for the root)
```

### Comparing `pytai-hex-0.2.6/pytai/view/widgets.py` & `pytai-hex-0.2.7/pytai/view/widgets.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/pytai/view/windows.py` & `pytai-hex-0.2.7/pytai/view/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,40 +398,52 @@
 
         self.window = tk.Toplevel(self.parent, bg = background)
         self.window.title(f"About {APP_NAME}") 
         self.window.resizable(0, 0)
         self.window.transient(self.parent)
         self.window.grab_set()
 
+        row = 0
 
         frame = tk.Frame(self.window, background = background)
 
         title = tk.Label(frame, text = APP_NAME, font=("Arial", 18, 'bold'), background = background)
-        title.grid(row = 0, column = 0, pady = (0, 7))
+        title.grid(row = row, column = 0, pady = (0, 7))
 
+        version_str = get_version()
+        if version_str:
+            row += 1
+            version = tk.Label(frame, text = f"Version: {version_str}", font=("Arial", 8), background = background) 
+            version.grid(row = row, column = 0, pady = (0, 7))
+
+        row += 1
         line1 = tk.Label(frame, text = "A Kaitai Struct Visualizer and Hex Viewer GUI in Python", background = background)
-        line1.grid(row = 1, column = 0, sticky = tk.W)
+        line1.grid(row = row, column = 0, sticky = tk.W)
 
+        row += 1
         link1 = tk.Label(frame, text="https://github.com/Dvd848/pytai", fg="blue", cursor="hand2", background = background)
         link1.bind("<Button-1>", open_link)
-        link1.grid(row = 2, column = 0, sticky = tk.W, pady = (0, 15))
+        link1.grid(row = row, column = 0, sticky = tk.W, pady = (0, 15))
 
+        row += 1
         line2 = tk.Label(frame, text = "Based on structure parsers provided by the Kaitai project", background = background)
-        line2.grid(row = 3, column = 0, sticky = tk.W)
+        line2.grid(row = row, column = 0, sticky = tk.W)
 
+        row += 1
         link2 = tk.Label(frame, text="https://kaitai.io/", fg="blue", cursor="hand2", background = background)
         link2.bind("<Button-1>", open_link)
-        link2.grid(row = 4, column = 0, sticky = tk.W)
+        link2.grid(row = row, column = 0, sticky = tk.W)
 
+        row += 1
         button_close = tk.Button(frame, text = "Close", command = self.close, width = 7)
-        button_close.grid(row = 5, column = 0, columnspan = 2)
+        button_close.grid(row = row, column = 0, columnspan = 2)
 
         frame.pack(padx = 15, pady = 15)
         
         self.window.bind('<Escape>', self.close)
         self.center_window(self.parent)
         self.window.focus_force()
 
 
     def close(self, event = None) -> None:
         """Close the window."""
-        self.window.destroy()
+        self.window.destroy()
```

### Comparing `pytai-hex-0.2.6/pytai_hex.egg-info/PKG-INFO` & `pytai-hex-0.2.7/pytai_hex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytai-hex
-Version: 0.2.6
+Version: 0.2.7
 Summary: Kaitai Struct: Visualizer and Hex Viewer GUI in Python
 Author: Dvd848
 License: MIT
 Project-URL: Homepage, https://github.com/Dvd848/pytai
 Keywords: pytai,python,kaitai,gui
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pytai-hex-0.2.6/pytai_hex.egg-info/SOURCES.txt` & `pytai-hex-0.2.7/pytai_hex.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 pytai/kaitai/formats/iso9660.py
 pytai/kaitai/formats/java_class.py
 pytai/kaitai/formats/jpeg.py
 pytai/kaitai/formats/luks.py
 pytai/kaitai/formats/lzh.py
 pytai/kaitai/formats/mac_os_resource_snd.py
 pytai/kaitai/formats/mach_o.py
+pytai/kaitai/formats/mach_o_fat.py
 pytai/kaitai/formats/magicavoxel_vox.py
 pytai/kaitai/formats/mbr_partition_table.py
 pytai/kaitai/formats/mcap.py
 pytai/kaitai/formats/microsoft_cfb.py
 pytai/kaitai/formats/microsoft_network_monitor_v2.py
 pytai/kaitai/formats/microsoft_pe.py
 pytai/kaitai/formats/mifare_classic.py
@@ -138,14 +139,15 @@
 pytai/kaitai/formats/python_pyc_27.py
 pytai/kaitai/formats/quake_mdl.py
 pytai/kaitai/formats/quake_pak.py
 pytai/kaitai/formats/quicktime_mov.py
 pytai/kaitai/formats/rar.py
 pytai/kaitai/formats/regf.py
 pytai/kaitai/formats/resource_fork.py
+pytai/kaitai/formats/respack.py
 pytai/kaitai/formats/riff.py
 pytai/kaitai/formats/rpm.py
 pytai/kaitai/formats/rtcp_payload.py
 pytai/kaitai/formats/rtp_packet.py
 pytai/kaitai/formats/rtpdump.py
 pytai/kaitai/formats/ruby_marshal.py
 pytai/kaitai/formats/s3m.py
```

### Comparing `pytai-hex-0.2.6/tests/resources/bmp.xml` & `pytai-hex-0.2.7/tests/resources/bmp.xml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/elf.elf` & `pytai-hex-0.2.7/tests/resources/elf.elf`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/elf.xml` & `pytai-hex-0.2.7/tests/resources/elf.xml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/png.xml` & `pytai-hex-0.2.7/tests/resources/png.xml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/wav.wav` & `pytai-hex-0.2.7/tests/resources/wav.wav`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/wav.xml` & `pytai-hex-0.2.7/tests/resources/wav.xml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/resources/zip.xml` & `pytai-hex-0.2.7/tests/resources/zip.xml`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/tests/test_application.py` & `pytai-hex-0.2.7/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/utils/Dockerfile` & `pytai-hex-0.2.7/utils/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     
 RUN curl -LO https://github.com/kaitai-io/kaitai_struct_compiler/releases/download/0.10/kaitai-struct-compiler_0.10_all.deb \
     && apt-get install ./kaitai-struct-compiler_0.10_all.deb
     
 WORKDIR /home/pytai/shared/utils
 
 ### Build: docker build -t pytai .
-### Run  : docker run -it --mount type=bind,source="$PWD/../",target=/home/pytai/shared/ pytai python3 compile_kaitai_formats.py
+### Run  : docker run -it --rm --mount type=bind,source="$PWD/../",target=/home/pytai/shared/ pytai python3 compile_kaitai_formats.py
```

### Comparing `pytai-hex-0.2.6/utils/compile_kaitai_formats.py` & `pytai-hex-0.2.7/utils/compile_kaitai_formats.py`

 * *Files identical despite different names*

### Comparing `pytai-hex-0.2.6/utils/packer.py` & `pytai-hex-0.2.7/utils/packer.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,29 +20,45 @@
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 """
 import zipapp
 import argparse
 from pathlib import Path
+import os
 
-def filter(path: Path) -> bool:
+def filter_func(path: Path) -> bool:
     for part in path.parts:
         if part.startswith(".") or part in ["__pycache__", "tmp", "tests", "docs"]:
             return False
 
     for pattern in ["*.pyc", "*.ini", "*.pyz"]:
         if path.match(pattern):
             return False
 
     return True
 
 
-def main(source, target) -> None:
-    zipapp.create_archive(source, target, filter = filter)
-    print(f"File created: {target}")
+def main(source, target, version) -> None:
+    version_file_path = str(Path(source) / "pytai" / "version.py")
+    with open(version_file_path, "w") as version_file:
+        version_file.write(f"__version__ = '{version}'")
+        
+    zipapp.create_archive(source, target, filter = filter_func)
+    os.remove(version_file_path) 
+    print(f"File created: {target}, version: {version}")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='Pack pytai to a *.pyz file.')
     args = parser.parse_args()
 
-    main("..", "pytai.pyz")
+    try:
+        import setuptools_scm
+        
+        source = ".."
+        version = setuptools_scm.get_version(root=source, relative_to=__file__)
+        
+        main(source, "pytai.pyz", version)
+    except Exception as e:
+        print(f"Error: {e}")
+    
+    input("Press Enter to continue...")
```

