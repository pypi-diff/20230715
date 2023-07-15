# Comparing `tmp/nanoCEM-0.0.2.1.tar.gz` & `tmp/nanoCEM-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.1.tar", last modified: Fri Jul 14 09:47:58 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.2.tar", last modified: Sat Jul 15 03:22:23 2023, max compression
```

## Comparing `nanoCEM-0.0.2.1.tar` & `nanoCEM-0.0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9994 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9411 2023-07-14 09:46:47.000000 nanoCEM-0.0.2.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9703 2023-07-14 09:46:47.000000 nanoCEM-0.0.2.1/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.1/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.1/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8110 2023-07-13 02:50:55.000000 nanoCEM-0.0.2.1/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.1/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.1/nanoCEM/extract_sub_fastq_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.1/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.1/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11481 2023-07-11 12:11:54.000000 nanoCEM-0.0.2.1/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.1/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9994 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      467 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1201 2023-07-14 09:47:48.000000 nanoCEM-0.0.2.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10150 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9567 2023-07-14 09:50:15.000000 nanoCEM-0.0.2.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9760 2023-07-15 03:18:59.000000 nanoCEM-0.0.2.2/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.2/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.2/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8163 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.2/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.2/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.2/nanoCEM/extract_sub_fastq_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.2/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.2/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.2/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.2/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10150 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      467 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1201 2023-07-15 03:21:32.000000 nanoCEM-0.0.2.2/setup.py
```

### Comparing `nanoCEM-0.0.2.1/LICENSE` & `nanoCEM-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/PKG-INFO` & `nanoCEM-0.0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -141,14 +141,16 @@
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+# Remember to sample fastq if you sampled your fast5
+extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -186,14 +188,15 @@
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
+
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
```

### Comparing `nanoCEM-0.0.2.1/README.md` & `nanoCEM-0.0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,16 @@
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+# Remember to sample fastq if you sampled your fast5
+extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -172,14 +174,15 @@
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
+
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
```

### Comparing `nanoCEM-0.0.2.1/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.2/nanoCEM/CE_magnifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
+    df.to_csv(results_path + '/feature.csv', index=None)
     # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter=False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
```

### Comparing `nanoCEM-0.0.2.1/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.2/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.2.2/nanoCEM/current_events_magnifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,16 @@
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
-    # if args.function == 'f5c':
+    df.to_csv(results_path+'/feature.csv',index=None)
+   # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
     percentile_filter=False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
         percentile_filter=True
```

### Comparing `nanoCEM-0.0.2.1/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.2.2/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM/extract_sub_fastq_from_bam.py` & `nanoCEM-0.0.2.2/nanoCEM/extract_sub_fastq_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM/normalization.py` & `nanoCEM-0.0.2.2/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM/plot.py` & `nanoCEM-0.0.2.2/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.2/nanoCEM/read_f5c_resquiggle.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
         if position < start_position or position > end_position:
             continue
         # unit
         aligned_pair = np.array(read.aligned_pairs)
         aligned_pair = pd.DataFrame(aligned_pair)
         if strand == '-':
             aligned_pair[0] = aligned_pair[0].iloc[::-1]
-        aligned_pair.dropna(inplace=True,ignore_index=True)
+        aligned_pair = aligned_pair.dropna()
+        aligned_pair.reset_index(drop=True, inplace=True)
         aligned_pair = aligned_pair[(aligned_pair[1] >= position - length) & (aligned_pair[1] <= position + length)]
 
         temp={}
         temp['pairs']=aligned_pair
         temp['query_length'] = read.query_length
         result_dict[read.qname] = temp
     return result_dict
```

### Comparing `nanoCEM-0.0.2.1/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.2/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.1/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.2/nanoCEM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -141,14 +141,16 @@
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
 extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+# Remember to sample fastq if you sampled your fast5
+extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -186,14 +188,15 @@
 slow5tools merge blow5_dir -o file.blow5
 slow5tools index file.blow5
 ```
 2. Run f5c resquiggle
 
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
+
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
```

### Comparing `nanoCEM-0.0.2.1/setup.py` & `nanoCEM-0.0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.1",
+    version="0.0.2.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
@@ -19,15 +19,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7,<3.10',
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.23.0',
-        'pandas>=1.1.5',
+        'pandas>=1.2.0',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
         "pyslow5>=1.0.0",
         "vbz_h5py_plugin>=1.0.1",
         "biopython>=1.80"
     ],
```

