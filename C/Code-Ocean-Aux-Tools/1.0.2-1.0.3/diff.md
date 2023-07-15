# Comparing `tmp/code_ocean_aux_tools-1.0.2.tar.gz` & `tmp/code_ocean_aux_tools-1.0.3.tar.gz`

## Comparing `code_ocean_aux_tools-1.0.2.tar` & `code_ocean_aux_tools-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/setup.py
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/index.html
--rwxr-xr-x   0        0        0   145343 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/search.js
--rwxr-xr-x   0        0        0    35405 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools.html
--rwxr-xr-x   0        0        0    64876 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fasta.html
--rwxr-xr-x   0        0        0   137471 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fastq.html
--rwxr-xr-x   0        0        0    95633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_utils.html
--rwxr-xr-x   0        0        0    38262 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_cpu_count.html
--rwxr-xr-x   0        0        0    46146 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_dir_contents.html
--rwxr-xr-x   0        0        0    45020 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fasta_file.html
--rwxr-xr-x   0        0        0    43404 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fastq_pair.html
--rwxr-xr-x   0        0        0    44350 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fwd_fastqs.html
--rwxr-xr-x   0        0        0    43368 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_groups.html
--rwxr-xr-x   0        0        0    77308 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_logger.html
--rwxr-xr-x   0        0        0    38284 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_pipeline_confirm.html
--rwxr-xr-x   0        0        0    43353 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_direction.html
--rwxr-xr-x   0        0        0    45190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_pattern.html
--rwxr-xr-x   0        0        0    45128 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_prefix.html
--rwxr-xr-x   0        0        0    45408 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_rev_file.html
--rwxr-xr-x   0        0        0    43629 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/set_log_msg.html
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/__init__.py
--rwxr-xr-x   0        0        0     2028 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_fasta.py
--rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_fastq.py
--rwxr-xr-x   0        0        0     4363 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_utils.py
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_cpu_count.py
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_dir_contents.py
--rwxr-xr-x   0        0        0      707 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fasta_file.py
--rwxr-xr-x   0        0        0      529 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fastq_pair.py
--rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      517 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_groups.py
--rwxr-xr-x   0        0        0     3826 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_logger.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_pipeline_confirm.py
--rwxr-xr-x   0        0        0      548 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_direction.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_pattern.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_prefix.py
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_rev_file.py
--rwxr-xr-x   0        0        0      570 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/set_log_msg.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/__init__.py
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/conftest.py
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_cpu_count.py
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_dir_contents.py
--rwxr-xr-x   0        0        0     1781 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_fasta_file.py
--rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_groups.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_pipeline_confirm.py
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_direction.py
--rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_pattern.py
--rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_prefix.py
--rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_rev_file.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/__init__.py
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/dirs_of_files.py
--rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/fastq_file.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/sample_sheets.py
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/.gitignore
--rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/LICENSE
--rwxr-xr-x   0        0        0     3985 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/README.md
--rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/setup.py
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/index.html
+-rwxr-xr-x   0        0        0   145343 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/search.js
+-rwxr-xr-x   0        0        0    35405 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools.html
+-rwxr-xr-x   0        0        0    64876 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_fasta.html
+-rwxr-xr-x   0        0        0   137471 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_fastq.html
+-rwxr-xr-x   0        0        0    95633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_utils.html
+-rwxr-xr-x   0        0        0    38262 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_cpu_count.html
+-rwxr-xr-x   0        0        0    46146 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_dir_contents.html
+-rwxr-xr-x   0        0        0    45020 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fasta_file.html
+-rwxr-xr-x   0        0        0    43404 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fastq_pair.html
+-rwxr-xr-x   0        0        0    44350 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fwd_fastqs.html
+-rwxr-xr-x   0        0        0    43368 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_groups.html
+-rwxr-xr-x   0        0        0    77308 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_logger.html
+-rwxr-xr-x   0        0        0    38284 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_pipeline_confirm.html
+-rwxr-xr-x   0        0        0    43353 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_direction.html
+-rwxr-xr-x   0        0        0    45190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_pattern.html
+-rwxr-xr-x   0        0        0    45128 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_prefix.html
+-rwxr-xr-x   0        0        0    45408 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_rev_file.html
+-rwxr-xr-x   0        0        0    43629 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/docs/src/co_tools/set_log_msg.html
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/__init__.py
+-rwxr-xr-x   0        0        0     2009 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/co_fasta.py
+-rwxr-xr-x   0        0        0     7521 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/co_fastq.py
+-rwxr-xr-x   0        0        0     4488 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/co_utils.py
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_cpu_count.py
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_dir_contents.py
+-rwxr-xr-x   0        0        0      707 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_fasta_file.py
+-rwxr-xr-x   0        0        0      529 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_fastq_pair.py
+-rwxr-xr-x   0        0        0      833 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_fastqs.py
+-rwxr-xr-x   0        0        0      517 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_groups.py
+-rwxr-xr-x   0        0        0     3826 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_logger.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0      548 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_read_direction.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_read_pattern.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_read_prefix.py
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/get_rev_file.py
+-rwxr-xr-x   0        0        0      570 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/src/co_tools/set_log_msg.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/__init__.py
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/conftest.py
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_cpu_count.py
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_dir_contents.py
+-rwxr-xr-x   0        0        0     1766 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_fasta_file.py
+-rwxr-xr-x   0        0        0     1179 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_fastqs.py
+-rwxr-xr-x   0        0        0      530 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_groups.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_read_direction.py
+-rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_read_pattern.py
+-rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_read_prefix.py
+-rwxr-xr-x   0        0        0     2171 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/test_get_rev_file.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/fixtures/__init__.py
+-rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/fixtures/dirs_of_files.py
+-rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/fixtures/fastq_file.py
+-rwxr-xr-x   0        0        0      768 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/tests/fixtures/sample_sheets.py
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/LICENSE
+-rwxr-xr-x   0        0        0     3977 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/README.md
+-rwxr-xr-x   0        0        0     1380 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.3/PKG-INFO
```

### Comparing `code_ocean_aux_tools-1.0.2/docs/search.js` & `code_ocean_aux_tools-1.0.3/docs/search.js`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fasta.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_fasta.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fastq.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_fastq.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_utils.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/co_utils.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_cpu_count.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_cpu_count.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_dir_contents.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_dir_contents.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fasta_file.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fasta_file.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fastq_pair.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fastq_pair.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fwd_fastqs.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_fwd_fastqs.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_groups.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_groups.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_logger.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_logger.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_pipeline_confirm.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_pipeline_confirm.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_direction.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_direction.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_pattern.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_pattern.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_prefix.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_read_prefix.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_rev_file.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/get_rev_file.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/docs/src/co_tools/set_log_msg.html` & `code_ocean_aux_tools-1.0.3/docs/src/co_tools/set_log_msg.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/co_fasta.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/co_fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import re
 from glob import glob
-from pathlib import Path
-from pathlib import PurePath
+from pathlib import Path, PurePath
 
 if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
```

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/co_fastq.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/co_fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,34 +63,37 @@
         log.info(f"returning {fwd},{rev}")
         return f"{fwd},{rev}"
     else:
         log.warning(f"Could not find complementary pair of fastq files in {dir_path}")
         return 0
 
 
-def get_fwd_fastqs(dir: str = "../data"):
-    """Returns all the forward reads files in ascending alphabetical order
+def get_fastqs(fwd: str = "", dir: str = "../data"):
+    """Returns all the reads files in ascending alphabetical order
 
     Args:
         dir (str, optional): The folder where all the reads file are.
         Defaults to "../data".
 
     Returns:
-        str: newline-separated string of forward reads files
+        str: newline-separated string of reads files
     """
+    if not dir:
+        dir = "../data"
     if fastq_files := glob(str(f"{dir}/**/*.fastq.gz"), recursive=True):
         log.debug(
             f"Found the following fastq files in the {dir} folder:\n{fastq_files}"
         )
-        pattern = get_read_pattern(fastq_files[0])
-        fwd_fastqs_list = glob(str(f"{dir}/**/*{pattern}"), recursive=True)
-        fwd_fastqs_list.sort()
-        fwd_fastqs = "\n".join(fwd_fastqs_list)
-        log.debug(f"Returning the following fwd fastq files\n{fwd_fastqs}")
-        return fwd_fastqs
+        if "true" in fwd.lower() or "fwd" in fwd.lower():
+            pattern = get_read_pattern(fastq_files[0])
+            fastq_files = glob(str(f"{dir}/**/*{pattern}"), recursive=True)
+        fastq_files.sort()
+        fastqs = "\n".join(fastq_files)
+        log.debug(f"Returning the following fastq files\n{fastqs}")
+        return fastqs
     else:
         log.error(f"There are no fastq.gz files in the {dir} directory")
         return 0
 
 
 def get_read_direction(filepath: str):
     """This function returns the direction of a single paired-end reads file
```

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/co_utils.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/co_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,45 +53,47 @@
     if dir_contents := glob(str(f"{dir}/**/*"), recursive=True):
         log.debug(f"Found the following files in {dir} {dir_contents}")
         return "\n".join(dir_contents)
     log.warning(f"There are no files or folders in the {dir} folder.")
     return 0
 
 
-def get_groups(filename: str = "../data/sample_sheet.csv"):
+def get_groups(filename: str = "../data/sample_sheet.csv", test: bool = False):
     """This function returns all the groups in a .csv
 
     Args:
         filename (None): Path to a sample sheet. Will default to
         ../data/sample_sheet.csv if no path supplied. If a filename is supplied,
         this function will attempt to find the path to the file in the
         ../data folder
 
     Returns:
         str: comma-separated string of groups in ascending alphabetical order.
     """
-    # if not filename:
-    #     sample_sheet = "../data/sample_sheet.csv"
-    if Path(filename).is_file():
+    if not filename:
+        log.error(f"Improper filename given for sample_sheet. filename={filename}")
+        return 1
+    elif Path(filename).is_file():
         log.debug(f"{filename} is a file.")
         sample_sheet = filename
     else:
         log.debug(f"type for {filename}: {type(filename)}")
         if files_found := glob(str(f"../data/{filename}"), recursive=True):
             if len(files_found) > 1:
                 log.warning(f"Found multiple sample_sheets. Will use {files_found[0]}")
             log.debug(f"Searching found the following sample sheet(s): {files_found}")
             sample_sheet = files_found[0]
         else:
             log.warning(f"No sample sheet found for '{filename}'")
-            return 0
+            sample_sheet = filename
     groups_set = set()
     try:
         with open(f"{sample_sheet}", "r") as infile:
             lines = infile.readlines()
+            log.debug(f"lines: {lines}")
             for line in lines:
                 line = line.strip()
                 line_group = line.split(",")[0]
                 groups_set.add(line_group)
             groups = sorted(list(groups_set))
             log.debug(f"Returning the following groups from sample sheet: {groups}")
             return ",".join(groups)
```

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_dir_contents.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_dir_contents.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_fasta_file.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_fasta_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_fastq_pair.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_fastq_pair.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_fwd_fastqs.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/set_log_msg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fastq import get_fwd_fastqs
+from .co_utils import print_log_msg
 
 if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
-    log.debug(f"args: {sys.argv}")
-    if len(argv) > 1:
-        log.info(f"Searching in {argv[1]} dir for files")
-        print(get_fwd_fastqs(argv[1]))
-        return 0
-    print(get_fwd_fastqs())
-    return 0
+    if len(argv) == 1:
+        sys.exit(log.error("You failed to provide a log message"))
+    elif len(argv) == 2:
+        return print_log_msg(argv[1])
+    return print_log_msg(argv[1], argv[2])
 
 
 if __name__ == "__main__":
     log.debug(f"args: {sys.argv}")
     sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_groups.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_groups.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_logger.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_logger.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_read_direction.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_read_direction.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_read_pattern.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_read_pattern.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_read_prefix.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_read_prefix.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/src/co_tools/get_rev_file.py` & `code_ocean_aux_tools-1.0.3/src/co_tools/get_rev_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_cpu_count.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_cpu_count.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_dir_contents.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_dir_contents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import subprocess
 from glob import glob
 
 import pytest
 
 from src.co_tools.co_utils import get_dir_contents
```

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_fasta_file.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_fasta_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from pathlib import Path
-from src.co_tools.co_fasta import find_extension, find_fasta_file
+
+from src.co_tools.co_fasta import find_extension
+
 
 # Tests for find_extension
 def test_generic_fasta():
     input_file = "/data/test.fa"
     assert str(find_extension(input_file)) == "/data/test.fa"
```

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_read_direction.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_read_direction.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_read_pattern.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_read_pattern.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_read_prefix.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_read_prefix.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/tests/test_get_rev_file.py` & `code_ocean_aux_tools-1.0.3/tests/test_get_rev_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,28 +30,24 @@
 
 
 def test_get_rev_file_R2_path():
     filepath = "/path/to/reads/gsm123_rep1_R2.fastq.gz"
     assert get_rev_file(filepath) == "/path/to/reads/gsm123_rep1_R2.fastq.gz"
 
 
-
 def test_get_rev_filename_R1_path():
     filepath = "/path/to/reads/gsm123_rep1_R1.fastq.gz"
     assert get_rev_file(filepath, name_only=True) == "gsm123_rep1_R2.fastq.gz"
 
 
 def test_get_rev_filename_R2_path():
     filepath = "/path/to/reads/gsm123_rep1_R2.fastq.gz"
     assert get_rev_file(filepath, name_only=True) == "gsm123_rep1_R2.fastq.gz"
 
 
-
-
-
 def test_get_rev_file_1():
     filepath = "gsm123_rep1_1.fastq.gz"
     assert get_rev_file(filepath) == "gsm123_rep1_2.fastq.gz"
 
 
 def test_get_rev_file_2():
     filepath = "gsm123_rep1_2.fastq.gz"
```

### Comparing `code_ocean_aux_tools-1.0.2/tests/fixtures/dirs_of_files.py` & `code_ocean_aux_tools-1.0.3/tests/fixtures/dirs_of_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import subprocess
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture()
 def fastq_dir(tmp_path):
@@ -32,8 +31,8 @@
         "gsm124_R2.fastq.gz",
     ]
     d = tmp_path / "fastqdir"
     d.mkdir()
     for fastq in fastq_files:
         Path(f"{d}/{fastq}").touch()
     assert Path(d).is_dir()
-    return d
+    return d
```

### Comparing `code_ocean_aux_tools-1.0.2/tests/fixtures/sample_sheets.py` & `code_ocean_aux_tools-1.0.3/tests/fixtures/sample_sheets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import pytest
+from six import PY2
 
 
 @pytest.fixture
 def mocker_samplesheet(mocker):
     # Read a mocked file
     mocked_sample_sheet = mocker.mock_open(
-        read_data="case1,SRR10388935_R1.fastq.gz,SRR10388935_R2.fastq.gz\ncase1,SRR10388936_R1.fastq.gz,"
-        + "SRR10388936_R2.fastq.gz\ncase2,SRR10388937_R1.fastq.gz,SRR10388937_R2.fastq.gz\ncase2,"
-        + "SRR10388938_R1.fastq.gz,SRR10388938_R2.fastq.gz\ncontrol1,SRR10388939_R1.fastq.gz,"
-        + "SRR10388939_R2.fastq.gz\ncontrol1,SRR10388940_R1.fastq.gz,SRR10388940_R2.fastq.gz\n"
-        + "control2,SRR10388941_R1.fastq.gz,SRR10388941_R2.fastq.gz"
+        read_data="case1,SRR10388935_R1.fastq.gz,SRR10388935_R2.fastq.gz"
+        + "\ncase1,SRR10388936_R1.fastq.gz,SRR10388936_R2.fastq.gz\ncase2,"
+        + "SRR10388937_R1.fastq.gz,SRR10388937_R2.fastq.gz\ncase2,"
+        + "SRR10388938_R1.fastq.gz,SRR10388938_R2.fastq.gz\ncontrol1,"
+        + "SRR10388939_R1.fastq.gz,SRR10388939_R2.fastq.gz\ncontrol1,"
+        + "SRR10388940_R1.fastq.gz,SRR10388940_R2.fastq.gz\ncontrol2,"
+        + "SRR10388941_R1.fastq.gz,SRR10388941_R2.fastq.gz"
     )
-    mocker.patch("builtins.open", mocked_sample_sheet)
+    builtin_open = "__builtin__.open" if PY2 else "builtins.open"
+    mocker.patch(builtin_open, mocked_sample_sheet)
```

### Comparing `code_ocean_aux_tools-1.0.2/LICENSE` & `code_ocean_aux_tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.2/README.md` & `code_ocean_aux_tools-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 The following commands will work at the terminal or in a bash script
 
     - get_cpu_count
     - get_dir_contents
     - get_fasta_file
     - get_fastq_pair
-    - get_fwd_fastqs
+    - get_fastqs
     - get_groups
     - get_pipeline_confirm
     - get_read_direction
     - get_read_pattern
     - get_read_prefix
     - get_rev_file
     - set_log_msg
@@ -62,15 +62,15 @@
     - get_dir_contents()
     - get_groups()
     - is_pipeline()
 
 **co_fastq**
 
     - get_fastq_pair()
-    - get_fwd_fastqs()
+    - get_fastqs()
     - get_read_direction()
     - get_read_pattern()
     - get_prefix()
     - get_rev_file()
 
 ---
```

### Comparing `code_ocean_aux_tools-1.0.2/pyproject.toml` & `code_ocean_aux_tools-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/co_tools"]
 
 [project]
 name = "Code_Ocean_Aux_Tools"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Frank Zappulla", email="frank@codeocean.com" },
 ]
 maintainers = [
     { name="Frank Zappulla", email="frank@codeocean.com" }
 ]
 description = "A suite of convenience tools for working with sequencing files and Code Ocean capsules."
@@ -24,15 +24,15 @@
 ]
 
 [project.scripts]
 get_cpu_count = "co_tools.get_cpu_count:main"
 get_dir_contents = "co_tools.get_dir_contents:main"
 get_fasta_file = "co_tools.get_fasta_file:main"
 get_fastq_pair = "co_tools.get_fastq_pair:main"
-get_fwd_fastqs = "co_tools.get_fwd_fastqs:main"
+get_fastqs = "co_tools.get_fastqs:main"
 get_groups = "co_tools.get_groups:main"
 get_pipeline_confirm = "co_tools.get_pipeline_confirm:main"
 get_read_direction = "co_tools.get_read_direction:main"
 get_read_pattern = "co_tools.get_read_pattern:main"
 get_read_prefix = "co_tools.get_read_prefix:main"
 get_rev_file = "co_tools.get_rev_file:main"
 set_log_msg = "co_tools.set_log_msg:main"
```

### Comparing `code_ocean_aux_tools-1.0.2/PKG-INFO` & `code_ocean_aux_tools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Code_Ocean_Aux_Tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: A suite of convenience tools for working with sequencing files and Code Ocean capsules.
 Project-URL: Homepage, https://github.com/codeocean/co_aux_tools
 Project-URL: Bug Tracker, https://github.com/codeocean/co_aux_tools/issues
 Author-email: Frank Zappulla <frank@codeocean.com>
 Maintainer-email: Frank Zappulla <frank@codeocean.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -47,15 +47,15 @@
 
 The following commands will work at the terminal or in a bash script
 
     - get_cpu_count
     - get_dir_contents
     - get_fasta_file
     - get_fastq_pair
-    - get_fwd_fastqs
+    - get_fastqs
     - get_groups
     - get_pipeline_confirm
     - get_read_direction
     - get_read_pattern
     - get_read_prefix
     - get_rev_file
     - set_log_msg
@@ -77,15 +77,15 @@
     - get_dir_contents()
     - get_groups()
     - is_pipeline()
 
 **co_fastq**
 
     - get_fastq_pair()
-    - get_fwd_fastqs()
+    - get_fastqs()
     - get_read_direction()
     - get_read_pattern()
     - get_prefix()
     - get_rev_file()
 
 ---
```

