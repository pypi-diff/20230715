# Comparing `tmp/MisER-0.0.1.tar.gz` & `tmp/MisER-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MisER-0.0.1.tar", last modified: Sun Jan  8 15:05:56 2023, max compression
+gzip compressed data, was "MisER-0.0.2.tar", last modified: Sat Jul 15 14:58:54 2023, max compression
```

## Comparing `MisER-0.0.1.tar` & `MisER-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 15:05:56.450295 MisER-0.0.1/
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     1065 2023-01-08 14:32:54.000000 MisER-0.0.1/LICENSE
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 15:05:56.450295 MisER-0.0.1/MisER/
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 14:32:54.000000 MisER-0.0.1/MisER/__init__.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)    12220 2023-01-08 14:32:54.000000 MisER-0.0.1/MisER/block_class.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     7902 2023-01-08 14:32:54.000000 MisER-0.0.1/MisER/find_small_exon.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)    34617 2023-01-08 14:32:54.000000 MisER-0.0.1/MisER/fix_small_exon_multiproc.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     4403 2023-01-08 14:51:55.000000 MisER-0.0.1/MisER/run_miser.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)       18 2023-01-08 14:52:20.000000 MisER-0.0.1/MisER/version.py
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 15:05:56.450295 MisER-0.0.1/MisER.egg-info/
--rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/PKG-INFO
--rw-rw-r--   0 zhen      (1000) zhen      (1000)      336 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/SOURCES.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)        1 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/dependency_links.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       47 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/entry_points.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       36 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/requires.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)        6 2023-01-08 15:05:56.000000 MisER-0.0.1/MisER.egg-info/top_level.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-01-08 15:05:56.450295 MisER-0.0.1/PKG-INFO
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     6460 2023-01-08 14:49:13.000000 MisER-0.0.1/README.md
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       38 2023-01-08 15:05:56.450295 MisER-0.0.1/setup.cfg
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)      974 2023-01-08 14:53:34.000000 MisER-0.0.1/setup.py
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     1065 2023-01-08 14:32:54.000000 MisER-0.0.2/LICENSE
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/MisER/
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/__init__.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)    12220 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/block_class.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     7902 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/find_small_exon.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)    35631 2023-07-15 14:41:38.000000 MisER-0.0.2/MisER/fix_small_exon_multiproc.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     4403 2023-01-08 14:51:55.000000 MisER-0.0.2/MisER/run_miser.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)       18 2023-07-15 14:54:02.000000 MisER-0.0.2/MisER/version.py
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/MisER.egg-info/
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/PKG-INFO
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)      336 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)        1 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       47 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/entry_points.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       42 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/requires.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)        6 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/top_level.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-15 14:58:54.892251 MisER-0.0.2/PKG-INFO
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     6460 2023-01-08 14:49:13.000000 MisER-0.0.2/README.md
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       38 2023-07-15 14:58:54.892251 MisER-0.0.2/setup.cfg
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)      980 2023-07-15 07:39:37.000000 MisER-0.0.2/setup.py
```

### Comparing `MisER-0.0.1/LICENSE` & `MisER-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MisER-0.0.1/MisER/block_class.py` & `MisER-0.0.2/MisER/block_class.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.1/MisER/find_small_exon.py` & `MisER-0.0.2/MisER/find_small_exon.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.1/MisER/fix_small_exon_multiproc.py` & `MisER-0.0.2/MisER/fix_small_exon_multiproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,27 +413,30 @@
     end_read_id = proc_region["end_read_id"]
     if not only_region:
         out_bam_path_proc = out_bam_path + ".tmp{0}".format(proc_id)
         realign_bam = pysam.AlignmentFile(
             out_bam_path_proc, "wb", template=ori_bam)
     filter_list = []
     read_i = 0  # 0 based
+    spliced_read_num = 0
     total_intron = 0
     misaligned_read_num = 0
     misaligned_intron_num = 0
     fix_read_num = 0
     fix_intron_num = 0
     for read in ori_bam.fetch(until_eof=True):
         if not(start_read_id <= read_i and read_i < end_read_id):
             read_i += 1
             continue
         if read.cigarstring is None or read.query_sequence is None:
             if not only_region:
                 realign_bam.write(read)
             read_i += 1
+            if read.cigarstring is not None and "N" in read.cigarstring:
+                spliced_read_num += 1
             continue
         read_miss_exon_flag = False
         read_fix_flag = False
         read_block = ReadBlock(read, read_i)
         realign_list = find_missed_exons(read_block, annot_bed, annot_exon, ignore_strand=ignore_strand,
                                          flank_len=flank_len, small_exon_size=small_exon_size)
         if realign_list is not False:
@@ -493,20 +496,22 @@
                 read.cigarstring = new_cigar_str
                 if set_tag:
                     if read.has_tag('fr'):
                         warnings.warn("Overwrite the existed fr tags on read:", read.qname)
                     read.set_tag('fr', fix_region_num, 'i')
             realign_bam.write(read)
         read_i += 1
+        if read.cigarstring is not None and "N" in read.cigarstring:
+            spliced_read_num += 1
         total_intron += read_block.introns["intron_num"]
         if read_miss_exon_flag:
             misaligned_read_num += 1
         if read_fix_flag:
             fix_read_num += 1
-    stat_dict = {"read_count": read_i, "total_intron": total_intron,
+    stat_dict = {"read_count": read_i, "spliced_read_num": spliced_read_num, "total_intron": total_intron,
                  "misaligned_read_num": misaligned_read_num,
                  "misaligned_intron_num": misaligned_intron_num,
                  "fix_read_num": fix_read_num, "fix_intron_num": fix_intron_num}
     # The read_count in stat_dict is the count of the whole bam file, not the part in the process.
     res_dict = {"filter_list": filter_list, "stat_dict": stat_dict}
     ori_bam.close()
     if not only_region:
@@ -541,28 +546,31 @@
     end_read_id = proc_region["end_read_id"]
     if not only_region:
         out_bam_path_proc = out_bam_path + ".tmp{0}".format(proc_id)
         realign_bam = pysam.AlignmentFile(
             out_bam_path_proc, "wb", template=ori_bam)
     filter_list = []
     read_i = 0  # 0 based
+    spliced_read_num = 0
     total_intron = 0
     misaligned_read_num = 0
     misaligned_intron_num = 0
     fix_read_num = 0
     fix_intron_num = 0
     for read in ori_bam.fetch(until_eof=True):
         try:
             if not(start_read_id <= read_i and read_i < end_read_id):
                 read_i += 1
                 continue
             if read.cigarstring is None or read.query_sequence is None:
                 if not only_region:
                     realign_bam.write(read)
                 read_i += 1
+                if read.cigarstring is not None and "N" in read.cigarstring:
+                    spliced_read_num += 1
                 continue
             read_miss_exon_flag = False
             read_fix_flag = False
             read_block = ReadBlock(read, read_i)
             realign_list = find_missed_exons(
                 read_block, annot_bed, annot_exon, ignore_strand=ignore_strand,
                 flank_len=flank_len, small_exon_size=small_exon_size
@@ -624,24 +632,26 @@
                     read.cigarstring = new_cigar_str
                     if set_tag:
                         if read.has_tag('fr'):
                             warnings.warn("Overwrite the existed fr tags on read:", read.qname)
                         read.set_tag('fr', fix_region_num, 'i')
                 realign_bam.write(read)
             read_i += 1
+            if read.cigarstring is not None and "N" in read.cigarstring:
+                spliced_read_num += 1
             total_intron += read_block.introns["intron_num"]
             if read_miss_exon_flag:
                 misaligned_read_num += 1
             if read_fix_flag:
                 fix_read_num += 1
         except Exception as e:
             logging.exception(e)
             error_case += 1
             error_bam.write(read)
-    stat_dict = {"read_count": read_i, "total_intron": total_intron,
+    stat_dict = {"read_count": read_i, "spliced_read_num": spliced_read_num, "total_intron": total_intron,
                  "misaligned_read_num": misaligned_read_num,
                  "misaligned_intron_num": misaligned_intron_num,
                  "fix_read_num": fix_read_num, "fix_intron_num": fix_intron_num}
     # The read_count in stat_dict is the count of the whole bam file, not the part in the process.
     res_dict = {"filter_list": filter_list, "stat_dict": stat_dict}
     ori_bam.close()
     error_bam.close()
@@ -664,14 +674,15 @@
     annot_bed = annot_bed[annot_bed["exon_num"] != 1]  # Filter out singleten
     # In order to avoid repetitive computation, we extend the bed file in advance.
     annot_exon = extend_tx(annot_bed)
     read_count = int(pysam.view("-c", ori_bam_path).strip())
     filter_list = []
     if not only_region:
         out_bam_list = []
+    spliced_read_num = 0
     total_intron = 0
     misaligned_read_num = 0
     misaligned_intron_num = 0
     fix_read_num = 0
     fix_intron_num = 0
     proc_list = []  # contain the list of proc_region
     per_read_num = int(read_count / nprocess)
@@ -708,14 +719,15 @@
     pool.join()
     res_list = [res.get() for res in multi_res]
     # res_list = pool.map(find_fix_proc, proc_list)
     for res_dict in res_list:
         filter_list.extend(res_dict["filter_list"])
         if not only_region:
             out_bam_list.append(res_dict["out_bam_path_proc"])
+        spliced_read_num += res_dict["stat_dict"]["spliced_read_num"]
         total_intron += res_dict["stat_dict"]["total_intron"]
         misaligned_read_num += res_dict["stat_dict"]["misaligned_read_num"]
         misaligned_intron_num += res_dict["stat_dict"]["misaligned_intron_num"]
         fix_read_num += res_dict["stat_dict"]["fix_read_num"]
         fix_intron_num += res_dict["stat_dict"]["fix_intron_num"]
     if res_list[0]["stat_dict"]["read_count"] != read_count:
         print(
@@ -729,37 +741,30 @@
     # Merge all output bam file in processes.
     pysam.merge("-cp", "-h", ori_bam_path, out_bam_path, *out_bam_list)
     for out_bam in out_bam_list:
         os.remove(out_bam)  # Remove tmp file
     end_time = time.process_time()
     end_time2 = time.time()
     print("Input BAM information:")
-    print("\tTotal number of reads:", read_count)
-    print("\tTotal number of introns:", total_intron)
-    print("The result of finding misaligned exons:")
-    if read_count == 0:
-        print("\tThe number of misaligned reads:", misaligned_read_num)
-    else:
-        print("\tThe number of misaligned reads: {0}\tratio: {1:.2f}%".format(
-            misaligned_read_num, misaligned_read_num/read_count*100
-        ))
-    if total_intron == 0:
-        print("\tThe number of misaligned introns:", misaligned_intron_num)
-    else:
-        print("\tThe number of misaligned introns: {0}\tratio: {1:.2f}%".format(
-            misaligned_intron_num, misaligned_intron_num/total_intron*100
-        ))
-    print("The result of realignment:")
-    if misaligned_read_num == 0:
-        print("\tThe number of fixed reads:", fix_read_num)
-    else:
-        print("\tThe number of fixed reads: {0}\tratio to misaligned reads: {1:.2f}%".format(
-            fix_read_num, fix_read_num/misaligned_read_num*100
-        ))
-    if misaligned_intron_num == 0:
-        print("\tThe number of fixed introns:", fix_intron_num)
-    else:
-        print("\tThe numberr of fixed introns: {0}\tratio to misaligned introns: {1:.2f}%".format(
-            fix_intron_num, fix_intron_num/misaligned_intron_num*100
-        ))
+    print("\tTotal number of read alignment records (equal to \"samtools view -c bam\"):", read_count)
+    print("\tTotal number of spliced read alignment records (containing \"N\" in CIGAR strings):", spliced_read_num)
+    print("\tTotal number of intron regions on read alignment records:", total_intron)
+    print("The result of finding potential misaligned regions (PMRs):")
+    print("\tThe number of PMRs:", misaligned_intron_num)
+    if total_intron != 0:
+        print("\t\tPercentage to total number of intron regions: {0:.2f}%".format(misaligned_intron_num/total_intron*100))
+    print("\tThe number of read alignment records containing PMRs:", misaligned_read_num)
+    if read_count != 0:
+        print("\t\tPercentage to total number of read alignment records: {0:.2f}%".format(misaligned_read_num/read_count*100))
+    if spliced_read_num != 0:
+        print("\t\tPercentage to total number of spliced read alignment records: {0:.2f}%".format(misaligned_read_num/spliced_read_num*100))
+    print("The result of realignment (judged as misaligned cases):")
+    print("\tThe number of fixed PMRs:", fix_intron_num)
+    if total_intron != 0:
+        print("\t\tPercentage to total number of intron regions: {0:.2f}%".format(fix_intron_num/total_intron*100))
+    print("\tThe number of fixed read alignment records:", fix_read_num)
+    if read_count != 0:
+        print("\t\tPercentage to total number of read alignment records: {0:.2f}%".format(fix_read_num/read_count*100))
+    if spliced_read_num != 0:
+        print("\t\tPercentage to total number of spliced read alignment records: {0:.2f}%".format(fix_read_num/spliced_read_num*100))
     print("Main process time used: {:.2f}s".format(end_time - start_time))
     print("Time used: {:.2f}s".format(end_time2 - start_time2))
```

### Comparing `MisER-0.0.1/MisER/run_miser.py` & `MisER-0.0.2/MisER/run_miser.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.1/MisER.egg-info/PKG-INFO` & `MisER-0.0.2/MisER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MisER
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find and fix missed small exons.
 Home-page: https://github.com/zhenLiuXplr/MisER-project
 Author: Zhen Liu
 Author-email: liuzhen_sirius@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `MisER-0.0.1/PKG-INFO` & `MisER-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MisER
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find and fix missed small exons.
 Home-page: https://github.com/zhenLiuXplr/MisER-project
 Author: Zhen Liu
 Author-email: liuzhen_sirius@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `MisER-0.0.1/README.md` & `MisER-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MisER-0.0.1/setup.py` & `MisER-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	long_description = fh.read()
 
 exec(codecs.open("MisER/version.py").read())
 
 
 INSTALL_REQUIRES = [
     'numpy',
-    'pandas',
+    'pandas<2.0.0',
     'pysam',
     'parasail>=1.1.17'
 ]
 
 setuptools.setup(
     name='MisER',
     version=VERSION,
```

