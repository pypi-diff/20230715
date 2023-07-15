# Comparing `tmp/multi-freq-ldpy-0.2.4.tar.gz` & `tmp/multi-freq-ldpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-freq-ldpy-0.2.4.tar", last modified: Tue Jul 26 11:33:28 2022, max compression
+gzip compressed data, was "multi-freq-ldpy-0.2.5.tar", last modified: Sat Jul 15 08:59:23 2023, max compression
```

## Comparing `multi-freq-ldpy-0.2.4.tar` & `multi-freq-ldpy-0.2.5.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.469995 multi-freq-ldpy-0.2.4/
--rw-rw-rw-   0        0        0     1099 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     9545 2022-07-26 11:33:28.469995 multi-freq-ldpy-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     8974 2022-07-26 09:20:18.000000 multi-freq-ldpy-0.2.4/README.md
--rw-rw-rw-   0        0        0       86 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      652 2022-07-26 11:33:28.469995 multi-freq-ldpy-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      930 2022-07-26 11:31:33.000000 multi-freq-ldpy-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.376267 multi-freq-ldpy-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.391888 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/
--rw-rw-rw-   0        0        0        2 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.423132 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/
--rw-rw-rw-   0        0        0     4619 2022-04-28 21:05:05.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_ADP.py
--rw-rw-rw-   0        0        0     3793 2022-04-28 21:04:39.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_GRR.py
--rw-rw-rw-   0        0        0     4151 2022-07-26 09:57:20.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_OSUE.py
--rw-rw-rw-   0        0        0     4924 2022-07-26 09:57:14.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_OUE.py
--rw-rw-rw-   0        0        0     8822 2022-07-26 09:57:09.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_SOUE.py
--rw-rw-rw-   0        0        0     6222 2022-07-26 09:57:03.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_SUE.py
--rw-rw-rw-   0        0        0     1228 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/Variance_LONG_PURE.py
--rw-rw-rw-   0        0        0        0 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/__init__.py
--rw-rw-rw-   0        0        0     2812 2022-07-26 10:59:30.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/dBitFlipPM.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.438752 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/
--rw-rw-rw-   0        0        0    14827 2022-07-26 11:14:38.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/L_SMP_Solution.py
--rw-rw-rw-   0        0        0    14746 2022-07-26 11:27:38.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/L_SPL_Solution.py
--rw-rw-rw-   0        0        0        2 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.438752 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/
--rw-rw-rw-   0        0        0    13171 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/RSpFD_solution.py
--rw-rw-rw-   0        0        0    10161 2022-07-26 09:07:48.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/SMP_solution.py
--rw-rw-rw-   0        0        0     9773 2022-07-26 09:07:58.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/SPL_solution.py
--rw-rw-rw-   0        0        0     2097 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/Variance_RSpFD.py
--rw-rw-rw-   0        0        0        2 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.469995 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/
--rw-rw-rw-   0        0        0     3138 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/ADP.py
--rw-rw-rw-   0        0        0     2481 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/GRR.py
--rw-rw-rw-   0        0        0     3042 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/LH.py
--rw-rw-rw-   0        0        0     2839 2022-07-26 08:24:52.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/SS.py
--rw-rw-rw-   0        0        0     2782 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/UE.py
--rw-rw-rw-   0        0        0      612 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/Variance_PURE.py
--rw-rw-rw-   0        0        0        2 2022-04-21 12:00:57.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-26 11:33:28.407512 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/
--rw-rw-rw-   0        0        0     9545 2022-07-26 11:33:28.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1484 2022-07-26 11:33:28.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 11:33:28.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-07-26 11:33:28.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-07-26 11:33:28.000000 multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:23.311020 multi-freq-ldpy-0.2.5/
+-rw-rw-rw-   0        0        0     1097 2022-04-14 11:47:54.000000 multi-freq-ldpy-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    11369 2023-07-15 08:59:23.311020 multi-freq-ldpy-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10792 2023-07-12 09:58:49.000000 multi-freq-ldpy-0.2.5/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-15 10:43:02.000000 multi-freq-ldpy-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      652 2023-07-15 08:59:23.311020 multi-freq-ldpy-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-07-15 08:57:40.000000 multi-freq-ldpy-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:22.808570 multi-freq-ldpy-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:22.835955 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/
+-rw-rw-rw-   0        0        0        2 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:22.887279 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/estimators/
+-rw-rw-rw-   0        0        0     4892 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/estimators/Histogram_estimator.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/estimators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:23.059610 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/
+-rw-rw-rw-   0        0        0     8440 2023-04-05 11:04:04.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_ADP.py
+-rw-rw-rw-   0        0        0     7058 2023-04-05 08:53:32.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_GRR.py
+-rw-rw-rw-   0        0        0     8059 2023-04-05 09:58:38.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_LH.py
+-rw-rw-rw-   0        0        0     7233 2023-04-05 08:53:32.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_OSUE.py
+-rw-rw-rw-   0        0        0     8454 2023-04-05 08:53:32.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_OUE.py
+-rw-rw-rw-   0        0        0    14361 2023-04-05 08:53:32.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_SOUE.py
+-rw-rw-rw-   0        0        0    10309 2023-04-05 08:53:32.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_SUE.py
+-rw-rw-rw-   0        0        0     1228 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/Variance_LONG_PURE.py
+-rw-rw-rw-   0        0        0        0 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/__init__.py
+-rw-rw-rw-   0        0        0     3646 2023-07-12 07:31:18.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/dBitFlipPM.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:23.106610 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/
+-rw-rw-rw-   0        0        0    14880 2023-07-12 07:36:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/L_SMP_Solution.py
+-rw-rw-rw-   0        0        0    14797 2023-07-12 07:32:59.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/L_SPL_Solution.py
+-rw-rw-rw-   0        0        0        2 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:23.184614 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/
+-rw-rw-rw-   0        0        0    13183 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/RSpFD_solution.py
+-rw-rw-rw-   0        0        0    10229 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/SMP_solution.py
+-rw-rw-rw-   0        0        0     9837 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/SPL_solution.py
+-rw-rw-rw-   0        0        0     2097 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/Variance_RSpFD.py
+-rw-rw-rw-   0        0        0        2 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:23.311020 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/
+-rw-rw-rw-   0        0        0     5338 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/ADP.py
+-rw-rw-rw-   0        0        0     4306 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/GRR.py
+-rw-rw-rw-   0        0        0     5787 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/HE.py
+-rw-rw-rw-   0        0        0     5685 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/LH.py
+-rw-rw-rw-   0        0        0     5178 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/SS.py
+-rw-rw-rw-   0        0        0     5006 2023-07-12 08:08:48.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/UE.py
+-rw-rw-rw-   0        0        0      612 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/Variance_PURE.py
+-rw-rw-rw-   0        0        0        2 2023-03-04 21:32:30.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:59:22.871370 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/
+-rw-rw-rw-   0        0        0    11369 2023-07-15 08:59:22.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1676 2023-07-15 08:59:22.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 08:59:22.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-15 08:59:22.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-15 08:59:22.000000 multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/top_level.txt
```

### Comparing `multi-freq-ldpy-0.2.4/LICENSE` & `multi-freq-ldpy-0.2.5/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `multi-freq-ldpy-0.2.4/PKG-INFO` & `multi-freq-ldpy-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 2.1
-Name: multi-freq-ldpy
-Version: 0.2.4
-Summary: Multiple Frequency Estimation Under Local Differential Privacy in Python
-Home-page: https://github.com/hharcolezi/multi-freq-ldpy
-Author: Héber H. Arcolezi
-Author-email: hh.arcolezi@gmail.com
-License: MIT
-Keywords: local-differential-privacy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python
 
-Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
+Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (one-time, multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
 
 Here's an introductory [Video_Presentation](https://screencast-o-matic.com/watch/c3hhQYVYNDi), [Slide_Presentation](http://hharcolezi.github.io/files/2022_Multi_Freq_LDPy_Presentation.pdf), and [arXived Demonstration Paper](https://arxiv.org/abs/2205.02648) of our package.
 
 If our codes and work are useful to you, we would appreciate a reference to:
 
 ```
-@article{arcolezi2022multi,
-  title={Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python},
-  author={Arcolezi, H{\'e}ber H and Couchot, Jean-Fran{\c{c}}ois and Gambs, S{\'e}bastien and Palamidessi, Catuscia and Zolfaghari, Majid},
-  journal={arXiv preprint arXiv:2205.02648},
-  year={2022}
+@incollection{Arcolezi2022,
+  doi = {10.1007/978-3-031-17143-7_40},
+  url = {https://doi.org/10.1007/978-3-031-17143-7_40},
+  year = {2022},
+  publisher = {Springer Nature Switzerland},
+  pages = {770--775},
+  author = {H{\'{e}}ber H. Arcolezi and Jean-Fran{\c{c}}ois Couchot and S{\'{e}}bastien Gambs and Catuscia Palamidessi and Majid Zolfaghari},
+  title = {Multi-Freq-{LDPy}: Multiple Frequency Estimation Under Local Differential Privacy in~Python},
+  booktitle = {Computer Security {\textendash} {ESORICS} 2022}
+}
+```
+
+```
+@incollection{Arcolezi2023,
+  doi = {10.1007/978-3-031-37586-6_11},
+  url = {https://doi.org/10.1007/978-3-031-37586-6_11},
+  year = {2023},
+  publisher = {Springer Nature Switzerland},
+  pages = {165--183},
+  author = {H{\'{e}}ber H. Arcolezi and Selene Cerna and Catuscia Palamidessi},
+  title = {On the Utility Gain of Iterative Bayesian Update for Locally Differentially Private Mechanisms},
+  booktitle = {Data and Applications Security and Privacy {XXXVII}}
 }
 ```
 
+
+
 ## Installation
 
 Please use the package manager [pip](https://pypi.org/project/multi-freq-ldpy/) to install multi-freq-ldpy.
 
 ```bash
 pip install multi-freq-ldpy
 ```
@@ -60,14 +63,17 @@
 multi-freq-ldpy package
 |
 |- pure_frequency_oracles (Single Frequency Estimation)
 |  |- GRR (Generalized Randomized Response[1,2] a.k.a. k-RR or Direct Encoding)
 |  |- UE (Unary Encoding)
 |  |  |- SUE (Symmetric UE[3] a.k.a. Basic One-Time RAPPOR[11])
 |  |  |- OUE (Optimized UE[3])
+|  |- HE (Histogram Encoding)
+|  |  |- SHE (Summation with HE[3])
+|  |  |- THE (Thresholding with HE[3])
 |  |- LH (Local Hashing)
 |  |  |- BLH (Binary LH[3,4])
 |  |  |- OLH (Optimized LH[3])
 |  |- SS (Subset Selection[5,6])
 |  |- ADP (Adaptive, i.e., GRR or OUE)
 |
 |- mdim_freq_est (Multidimensional Frequency Estimation)
@@ -81,89 +87,102 @@
 |  |  |- RSpFD_SUE_rnd (fake data generated with SUE applied to a random bit-vector)
 |  |  |- RSpFD_OUE_zero (fake data generated with OUE applied to a zero-vector)
 |  |  |- RSpFD_OUE_rnd (fake data generated with OUE applied to a random bit-vector)
 |  |  |- RSpFD_ADP (RSpFD_GRR or RSpFD_OUE_z)
 |
 |- long_freq_est (Longitudinal Single Frequency Estimation)
 |  |- L_GRR (Longitudinal GRR[10])
+|  |- L_LH (Longitudinal LH[12])
+|  |  |- L_BLH (Binary LH[12])
+|  |  |- L_OLH (Optimized LH[12])
 |  |- L_OUE (Longitudinal OUE[10])
 |  |- L_OSUE (Longitudinal OUE-SUE[10])
 |  |- L_SUE (Longitudinal SUE[10], a.k.a. Basic RAPPOR[11])
 |  |- L_SOUE (Longitudinal SUE-OUE[10])
 |  |- L_ADP (Longitudinal ADP[10], i.e., L-GRR or L-OSUE)
-|  |- dBitFlipPM[12]
+|  |- dBitFlipPM[13]
 |
 |- long_mdim_freq_est (Longitudinal Multidimensional Frequency Estimation)
 |  |- Longitudinal SPL (L_SPL_Solution[10]): Splits the privacy budget and sanitizes using long_freq_est LDP protocols
 |  |  |- SPL_L_GRR, SPL_L_OUE, SPL_L_OSUE, SPL_L_SUE, SPL_L_SOUE, SPL_L_ADP, SPL_dBitFlipPM
 |  |- Longitudinal SMP (L_SMP_Solution[10]): Samples a single attribute and sanitizes using long_freq_est LDP protocols
 |  |  |- SMP_L_GRR, SMP_L_OUE, SMP_L_OSUE, SMP_L_SUE, SMP_L_SOUE, SMP_L_ADP, SMP_dBitFlipPM
+|
+| - estimators (Distribution Estimator Methods)
+|  |- MI (Matrix Inverse)
+|  |- IBU (Iterative Bayesian Estimator[14])
 ```
 
 ## Usage
 This is a function-based package that simulates the LDP data collection pipeline of users and the server. For each functionality, there is always a ```Client``` and an ```Aggregator``` function. For more details, please refer to the [tutorials](https://github.com/hharcolezi/multi-freq-ldpy/tree/main/tutorials) folder, which covers all 1--4 tasks with real-world open datasets ([Adult](https://archive.ics.uci.edu/ml/datasets/adult), [Nursery](https://archive.ics.uci.edu/ml/datasets/nursery), [MS-FIMU](https://github.com/hharcolezi/OpenMSFIMU)).
 
 ```python
 # Common libraries
 import numpy as np
 import matplotlib.pyplot as plt
 
 # Multi-Freq-LDPy functions for L-SUE protocol (a.k.a. Basic RAPPOR[11])
-from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator
+from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator_MI, L_SUE_Aggregator_IBU
 
 # Parameters for simulation
 epsilon_perm = 2 # longitudinal privacy guarantee, i.e., upper bound (infinity reports)
 epsilon_1 = 0.5 * epsilon_perm # single report privacy guarantee, i.e., lower bound
 n = int(1e6) # number of users
 k = 5 # attribute's domain size
 
 # Simulation dataset where every user has a number between [0-k) with n users
 data = np.random.randint(k, size=n)
 
 # Simulation of client-side
 l_sue_reports = [L_SUE_Client(input_data, k, epsilon_perm, epsilon_1) for input_data in data]
 
-# Simulation of server-side aggregation
-l_sue_est_freq = L_SUE_Aggregator(l_sue_reports, epsilon_perm, epsilon_1)
+# Simulation of server-side aggregation with Matrix Inversion (MI)
+l_sue_est_freq_MI = L_SUE_Aggregator_MI(l_sue_reports, epsilon_perm, epsilon_1)
+
+# Simulation of server-side aggregation with Iterative Bayesian Updates (IBU)[14]
+l_sue_est_freq_IBU = L_SUE_Aggregator_IBU(l_sue_reports, k, epsilon_perm, epsilon_1)
 
 # Real frequency 
 real_freq = np.unique(data, return_counts=True)[-1] / n
 
 # Visualizing results
-barwidth = 0.45
-x_axis = np.arange(k)
+x = np.arange(k)  # the label locations
+barwidth = 0.3 # the width of the bars
 
-plt.bar(x_axis - barwidth/2, real_freq, label='Real Freq', width=barwidth)
-plt.bar(x_axis + barwidth/2 , l_sue_est_freq, label='Est Freq: L-SUE', width=barwidth)
+plt.bar(x - barwidth, real_freq, label='Real Freq', width=barwidth)
+plt.bar(x , l_sue_est_freq_MI, label='MI Est Freq: L-SUE', width=barwidth)
+plt.bar(x + barwidth, l_sue_est_freq_IBU, label='IBU Est Freq: L-SUE', width=barwidth)
 plt.ylabel('Normalized Frequency')
 plt.xlabel('Domain values')
-plt.legend(loc='upper right', bbox_to_anchor=(1.015, 1.15))
+plt.legend(ncol=3, loc='upper right', bbox_to_anchor=(1., 1.1))
 plt.show();
 ```
 
 ## Contributing
 Multi-Freq-LDPy is a work in progress, and we expect to release new versions frequently, incorporating feedback and code contributions from the community. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Contact
-For any question, please contact [Heber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
+For any question, please contact [Héber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
 
 ## Acknowledgments
    * The Local Hashing (LH) functions were adapted from the [pure-LDP](https://github.com/Samuel-Maddock/pure-LDP) package, which covers a wider range of frequency oracles for single-frequency estimation.
-   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) repository. 
+   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) and [LOLOHA](https://github.com/hharcolezi/LOLOHA) repositories. 
 
 ## License
 [MIT](https://github.com/hharcolezi/multi-freq-ldpy/blob/main/LICENSE)
 
 
-## References
+## Main References
 - [1] Kairouz, Peter, Keith Bonawitz, and Daniel Ramage. "Discrete distribution estimation under local privacy." International Conference on Machine Learning. PMLR, 2016.
 - [2] Kairouz, Peter, Sewoong Oh, and Pramod Viswanath. "Extremal mechanisms for local differential privacy." Advances in neural information processing systems 27 (2014).
 - [3] Wang, Tianhao, et al. "Locally differentially private protocols for frequency estimation." 26th USENIX Security Symposium (USENIX Security 17). 2017.
 - [4] Bassily, Raef, and Adam Smith. "Local, private, efficient protocols for succinct histograms." Proceedings of the forty-seventh annual ACM symposium on Theory of computing. 2015.
 - [5] Ye, Min, and Alexander Barg. "Optimal schemes for discrete distribution estimation under locally differential privacy." IEEE Transactions on Information Theory 64.8 (2018): 5662-5676.
 - [6] Wang, Shaowei, et al. "Mutual information optimally local private discrete distribution estimation." arXiv preprint arXiv:1607.08025 (2016).
-- [7] NguyÃªn, ThÃ´ng T., et al. "Collecting and analyzing data from smart device users with local differential privacy." arXiv preprint arXiv:1606.05053 (2016).
+- [7] Nguyên, Thông T., et al. "Collecting and analyzing data from smart device users with local differential privacy." arXiv preprint arXiv:1606.05053 (2016).
 - [8] Wang, Ning, et al. "Collecting and analyzing multidimensional data with local differential privacy." 2019 IEEE 35th International Conference on Data Engineering (ICDE). IEEE, 2019.
-- [9] Arcolezi, HÃ©ber H., et al. "Random sampling plus fake data: Multidimensional frequency estimates with local differential privacy." Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021.
-- [10] Arcolezi, HÃ©ber H., et al. "Improving the utility of locally differentially private protocols for longitudinal and multidimensional frequency estimates." Digital Communications and Networks (2022).
-- [11] Erlingsson, Ãšlfar, Vasyl Pihur, and Aleksandra Korolova. "Rappor: Randomized aggregatable privacy-preserving ordinal response." Proceedings of the 2014 ACM SIGSAC conference on computer and communications security. 2014.
-- [12] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [9] Arcolezi, Héber H., et al. "Random sampling plus fake data: Multidimensional frequency estimates with local differential privacy." Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021.
+- [10] Arcolezi, Héber H., et al. "Improving the utility of locally differentially private protocols for longitudinal and multidimensional frequency estimates." Digital Communications and Networks (2022).
+- [11] Erlingsson, Úlfar, Vasyl Pihur, and Aleksandra Korolova. "Rappor: Randomized aggregatable privacy-preserving ordinal response." Proceedings of the 2014 ACM SIGSAC conference on computer and communications security. 2014.
+- [12] Arcolezi, Héber H., et al. "Frequency Estimation of Evolving Data Under Local Differential Privacy." arXiv preprint arXiv:2210.00262 (2022).
+- [13] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [14] Agrawal, Dakshi, and Charu C. Aggarwal. "On the design and quantification of privacy preserving data mining algorithms." Proceedings of the twentieth ACM SIGMOD-SIGACT-SIGART symposium on Principles of database systems. 2001.
```

### Comparing `multi-freq-ldpy-0.2.4/README.md` & `multi-freq-ldpy-0.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,59 @@
+Metadata-Version: 2.1
+Name: multi-freq-ldpy
+Version: 0.2.5
+Summary: Multiple Frequency Estimation Under Local Differential Privacy in Python
+Home-page: https://github.com/hharcolezi/multi-freq-ldpy
+Author: Héber H. Arcolezi
+Author-email: hh.arcolezi@gmail.com
+License: MIT
+Keywords: local-differential-privacy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python
 
-Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
+Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (one-time, multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
 
 Here's an introductory [Video_Presentation](https://screencast-o-matic.com/watch/c3hhQYVYNDi), [Slide_Presentation](http://hharcolezi.github.io/files/2022_Multi_Freq_LDPy_Presentation.pdf), and [arXived Demonstration Paper](https://arxiv.org/abs/2205.02648) of our package.
 
 If our codes and work are useful to you, we would appreciate a reference to:
 
 ```
-@article{arcolezi2022multi,
-  title={Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python},
-  author={Arcolezi, H{\'e}ber H and Couchot, Jean-Fran{\c{c}}ois and Gambs, S{\'e}bastien and Palamidessi, Catuscia and Zolfaghari, Majid},
-  journal={arXiv preprint arXiv:2205.02648},
-  year={2022}
+@incollection{Arcolezi2022,
+  doi = {10.1007/978-3-031-17143-7_40},
+  url = {https://doi.org/10.1007/978-3-031-17143-7_40},
+  year = {2022},
+  publisher = {Springer Nature Switzerland},
+  pages = {770--775},
+  author = {H{\'{e}}ber H. Arcolezi and Jean-Fran{\c{c}}ois Couchot and S{\'{e}}bastien Gambs and Catuscia Palamidessi and Majid Zolfaghari},
+  title = {Multi-Freq-{LDPy}: Multiple Frequency Estimation Under Local Differential Privacy in~Python},
+  booktitle = {Computer Security {\textendash} {ESORICS} 2022}
+}
+```
+
+```
+@incollection{Arcolezi2023,
+  doi = {10.1007/978-3-031-37586-6_11},
+  url = {https://doi.org/10.1007/978-3-031-37586-6_11},
+  year = {2023},
+  publisher = {Springer Nature Switzerland},
+  pages = {165--183},
+  author = {H{\'{e}}ber H. Arcolezi and Selene Cerna and Catuscia Palamidessi},
+  title = {On the Utility Gain of Iterative Bayesian Update for Locally Differentially Private Mechanisms},
+  booktitle = {Data and Applications Security and Privacy {XXXVII}}
 }
 ```
 
+
+
 ## Installation
 
 Please use the package manager [pip](https://pypi.org/project/multi-freq-ldpy/) to install multi-freq-ldpy.
 
 ```bash
 pip install multi-freq-ldpy
 ```
@@ -44,14 +79,17 @@
 multi-freq-ldpy package
 |
 |- pure_frequency_oracles (Single Frequency Estimation)
 |  |- GRR (Generalized Randomized Response[1,2] a.k.a. k-RR or Direct Encoding)
 |  |- UE (Unary Encoding)
 |  |  |- SUE (Symmetric UE[3] a.k.a. Basic One-Time RAPPOR[11])
 |  |  |- OUE (Optimized UE[3])
+|  |- HE (Histogram Encoding)
+|  |  |- SHE (Summation with HE[3])
+|  |  |- THE (Thresholding with HE[3])
 |  |- LH (Local Hashing)
 |  |  |- BLH (Binary LH[3,4])
 |  |  |- OLH (Optimized LH[3])
 |  |- SS (Subset Selection[5,6])
 |  |- ADP (Adaptive, i.e., GRR or OUE)
 |
 |- mdim_freq_est (Multidimensional Frequency Estimation)
@@ -65,89 +103,102 @@
 |  |  |- RSpFD_SUE_rnd (fake data generated with SUE applied to a random bit-vector)
 |  |  |- RSpFD_OUE_zero (fake data generated with OUE applied to a zero-vector)
 |  |  |- RSpFD_OUE_rnd (fake data generated with OUE applied to a random bit-vector)
 |  |  |- RSpFD_ADP (RSpFD_GRR or RSpFD_OUE_z)
 |
 |- long_freq_est (Longitudinal Single Frequency Estimation)
 |  |- L_GRR (Longitudinal GRR[10])
+|  |- L_LH (Longitudinal LH[12])
+|  |  |- L_BLH (Binary LH[12])
+|  |  |- L_OLH (Optimized LH[12])
 |  |- L_OUE (Longitudinal OUE[10])
 |  |- L_OSUE (Longitudinal OUE-SUE[10])
 |  |- L_SUE (Longitudinal SUE[10], a.k.a. Basic RAPPOR[11])
 |  |- L_SOUE (Longitudinal SUE-OUE[10])
 |  |- L_ADP (Longitudinal ADP[10], i.e., L-GRR or L-OSUE)
-|  |- dBitFlipPM[12]
+|  |- dBitFlipPM[13]
 |
 |- long_mdim_freq_est (Longitudinal Multidimensional Frequency Estimation)
 |  |- Longitudinal SPL (L_SPL_Solution[10]): Splits the privacy budget and sanitizes using long_freq_est LDP protocols
 |  |  |- SPL_L_GRR, SPL_L_OUE, SPL_L_OSUE, SPL_L_SUE, SPL_L_SOUE, SPL_L_ADP, SPL_dBitFlipPM
 |  |- Longitudinal SMP (L_SMP_Solution[10]): Samples a single attribute and sanitizes using long_freq_est LDP protocols
 |  |  |- SMP_L_GRR, SMP_L_OUE, SMP_L_OSUE, SMP_L_SUE, SMP_L_SOUE, SMP_L_ADP, SMP_dBitFlipPM
+|
+| - estimators (Distribution Estimator Methods)
+|  |- MI (Matrix Inverse)
+|  |- IBU (Iterative Bayesian Estimator[14])
 ```
 
 ## Usage
 This is a function-based package that simulates the LDP data collection pipeline of users and the server. For each functionality, there is always a ```Client``` and an ```Aggregator``` function. For more details, please refer to the [tutorials](https://github.com/hharcolezi/multi-freq-ldpy/tree/main/tutorials) folder, which covers all 1--4 tasks with real-world open datasets ([Adult](https://archive.ics.uci.edu/ml/datasets/adult), [Nursery](https://archive.ics.uci.edu/ml/datasets/nursery), [MS-FIMU](https://github.com/hharcolezi/OpenMSFIMU)).
 
 ```python
 # Common libraries
 import numpy as np
 import matplotlib.pyplot as plt
 
 # Multi-Freq-LDPy functions for L-SUE protocol (a.k.a. Basic RAPPOR[11])
-from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator
+from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator_MI, L_SUE_Aggregator_IBU
 
 # Parameters for simulation
 epsilon_perm = 2 # longitudinal privacy guarantee, i.e., upper bound (infinity reports)
 epsilon_1 = 0.5 * epsilon_perm # single report privacy guarantee, i.e., lower bound
 n = int(1e6) # number of users
 k = 5 # attribute's domain size
 
 # Simulation dataset where every user has a number between [0-k) with n users
 data = np.random.randint(k, size=n)
 
 # Simulation of client-side
 l_sue_reports = [L_SUE_Client(input_data, k, epsilon_perm, epsilon_1) for input_data in data]
 
-# Simulation of server-side aggregation
-l_sue_est_freq = L_SUE_Aggregator(l_sue_reports, epsilon_perm, epsilon_1)
+# Simulation of server-side aggregation with Matrix Inversion (MI)
+l_sue_est_freq_MI = L_SUE_Aggregator_MI(l_sue_reports, epsilon_perm, epsilon_1)
+
+# Simulation of server-side aggregation with Iterative Bayesian Updates (IBU)[14]
+l_sue_est_freq_IBU = L_SUE_Aggregator_IBU(l_sue_reports, k, epsilon_perm, epsilon_1)
 
 # Real frequency 
 real_freq = np.unique(data, return_counts=True)[-1] / n
 
 # Visualizing results
-barwidth = 0.45
-x_axis = np.arange(k)
+x = np.arange(k)  # the label locations
+barwidth = 0.3 # the width of the bars
 
-plt.bar(x_axis - barwidth/2, real_freq, label='Real Freq', width=barwidth)
-plt.bar(x_axis + barwidth/2 , l_sue_est_freq, label='Est Freq: L-SUE', width=barwidth)
+plt.bar(x - barwidth, real_freq, label='Real Freq', width=barwidth)
+plt.bar(x , l_sue_est_freq_MI, label='MI Est Freq: L-SUE', width=barwidth)
+plt.bar(x + barwidth, l_sue_est_freq_IBU, label='IBU Est Freq: L-SUE', width=barwidth)
 plt.ylabel('Normalized Frequency')
 plt.xlabel('Domain values')
-plt.legend(loc='upper right', bbox_to_anchor=(1.015, 1.15))
+plt.legend(ncol=3, loc='upper right', bbox_to_anchor=(1., 1.1))
 plt.show();
 ```
 
 ## Contributing
 Multi-Freq-LDPy is a work in progress, and we expect to release new versions frequently, incorporating feedback and code contributions from the community. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Contact
-For any question, please contact [Heber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
+For any question, please contact [HÃ©ber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
 
 ## Acknowledgments
    * The Local Hashing (LH) functions were adapted from the [pure-LDP](https://github.com/Samuel-Maddock/pure-LDP) package, which covers a wider range of frequency oracles for single-frequency estimation.
-   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) repository. 
+   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) and [LOLOHA](https://github.com/hharcolezi/LOLOHA) repositories. 
 
 ## License
 [MIT](https://github.com/hharcolezi/multi-freq-ldpy/blob/main/LICENSE)
 
 
-## References
+## Main References
 - [1] Kairouz, Peter, Keith Bonawitz, and Daniel Ramage. "Discrete distribution estimation under local privacy." International Conference on Machine Learning. PMLR, 2016.
 - [2] Kairouz, Peter, Sewoong Oh, and Pramod Viswanath. "Extremal mechanisms for local differential privacy." Advances in neural information processing systems 27 (2014).
 - [3] Wang, Tianhao, et al. "Locally differentially private protocols for frequency estimation." 26th USENIX Security Symposium (USENIX Security 17). 2017.
 - [4] Bassily, Raef, and Adam Smith. "Local, private, efficient protocols for succinct histograms." Proceedings of the forty-seventh annual ACM symposium on Theory of computing. 2015.
 - [5] Ye, Min, and Alexander Barg. "Optimal schemes for discrete distribution estimation under locally differential privacy." IEEE Transactions on Information Theory 64.8 (2018): 5662-5676.
 - [6] Wang, Shaowei, et al. "Mutual information optimally local private discrete distribution estimation." arXiv preprint arXiv:1607.08025 (2016).
-- [7] Nguyên, Thông T., et al. "Collecting and analyzing data from smart device users with local differential privacy." arXiv preprint arXiv:1606.05053 (2016).
+- [7] NguyÃªn, ThÃ´ng T., et al. "Collecting and analyzing data from smart device users with local differential privacy." arXiv preprint arXiv:1606.05053 (2016).
 - [8] Wang, Ning, et al. "Collecting and analyzing multidimensional data with local differential privacy." 2019 IEEE 35th International Conference on Data Engineering (ICDE). IEEE, 2019.
-- [9] Arcolezi, Héber H., et al. "Random sampling plus fake data: Multidimensional frequency estimates with local differential privacy." Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021.
-- [10] Arcolezi, Héber H., et al. "Improving the utility of locally differentially private protocols for longitudinal and multidimensional frequency estimates." Digital Communications and Networks (2022).
-- [11] Erlingsson, Úlfar, Vasyl Pihur, and Aleksandra Korolova. "Rappor: Randomized aggregatable privacy-preserving ordinal response." Proceedings of the 2014 ACM SIGSAC conference on computer and communications security. 2014.
-- [12] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [9] Arcolezi, HÃ©ber H., et al. "Random sampling plus fake data: Multidimensional frequency estimates with local differential privacy." Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021.
+- [10] Arcolezi, HÃ©ber H., et al. "Improving the utility of locally differentially private protocols for longitudinal and multidimensional frequency estimates." Digital Communications and Networks (2022).
+- [11] Erlingsson, Ãšlfar, Vasyl Pihur, and Aleksandra Korolova. "Rappor: Randomized aggregatable privacy-preserving ordinal response." Proceedings of the 2014 ACM SIGSAC conference on computer and communications security. 2014.
+- [12] Arcolezi, HÃ©ber H., et al. "Frequency Estimation of Evolving Data Under Local Differential Privacy." arXiv preprint arXiv:2210.00262 (2022).
+- [13] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [14] Agrawal, Dakshi, and Charu C. Aggarwal. "On the design and quantification of privacy preserving data mining algorithms." Proceedings of the twentieth ACM SIGMOD-SIGACT-SIGART symposium on Principles of database systems. 2001.
```

### Comparing `multi-freq-ldpy-0.2.4/setup.cfg` & `multi-freq-ldpy-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `multi-freq-ldpy-0.2.4/setup.py` & `multi-freq-ldpy-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 with open("README.md", "r") as fh:
     describe_package = fh.read()
 
 setup(
     name='multi-freq-ldpy',
-    version='0.2.4',
+    version='0.2.5',
     license='MIT',
     author="Héber H. Arcolezi",
     author_email='hh.arcolezi@gmail.com',
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     url='https://github.com/hharcolezi/multi-freq-ldpy',
     classifiers=[
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_SOUE.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_SOUE.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 from numba import jit
+from multi_freq_ldpy.estimators.Histogram_estimator import MI_long, IBU
 
 # [1] Arcolezi et al (2021) "Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates" (arXiv:2111.04636).
 # [2] Wang et al (2017) "Locally differentially private protocols for frequency estimation" (USENIX Security).
+# [3] Agrawal and Aggarwal (2001,) "On the design and quantification of privacy preserving data mining algorithms" (PODS).
+# [4] ElSalamouny and Palamidessi (2020) "Generalized iterative bayesian update and applications to mechanisms for privacy protection" (EuroS&P).
 
 # The analytical analysis of how to calculate parameters (p1, q2, p2, q2) is from: https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B4%5D/1_ALLOMFREE_Analysis.ipynb
 
 @jit(nopython=True)
 def L_SOUE_Client(input_data, k, eps_perm, eps_1):
 
     """
@@ -14,19 +17,24 @@
 
     :param input_data: user's true value;
     :param k: attribute's domain size;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: sanitized UE vector.
     """
-    
-    if eps_1 >= eps_perm:
-        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
-    
-    else:
+
+    # Validations
+    if input_data < 0 or input_data >= k:
+        raise ValueError('input_data (integer) should be in the range [0, k-1].')
+    if not isinstance(k, int) or k < 2:
+        raise ValueError('k needs an integer value >=2.')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
+
         # SUE parameters for round 1
         p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
         q1 = 1 - p1
 
         # OUE parameters for round 2
         p2 = 0.5
         q2 = (3.35410196624968 * (np.exp(eps_1) - 1) * (
@@ -87,71 +95,160 @@
             else:
                 rnd = np.random.random()
                 if rnd <= p2:
                     second_sanitization[ind] = 1
 
         return second_sanitization
 
-def L_SOUE_Aggregator(ue_reports, eps_perm, eps_1):
+    else:
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
+
+
+def L_SOUE_Aggregator_MI(reports, eps_perm, eps_1):
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) with post-processing to ensure non-negativity.
 
     :param reports: list of all L-SOUE sanitized UE-based vectors;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation.
     """
 
-    if len(ue_reports) == 0:
+    # Validations
+    if len(reports) == 0:
         raise ValueError('List of reports is empty.')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
+
+        # Number of reports
+        n = len(reports)
+
+        # SUE parameters for round 1
+        p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
+        q1 = 1 - p1
+
+        # OUE parameters for round 2
+        p2 = 0.5
+        q2 = (3.35410196624968 * (np.exp(eps_1) - 1) * (
+                np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * np.sqrt(
+            0.0111111111111111 * np.exp(eps_1) + 0.00555555555555556 * np.exp(2 * eps_1) + 0.0444444444444444 * np.exp(
+                0.5 * eps_perm) + 0.155555555555556 * np.exp(eps_perm) + 0.311111111111111 * np.exp(
+                1.5 * eps_perm) + 0.388888888888889 * np.exp(2 * eps_perm) + 0.311111111111111 * np.exp(
+                2.5 * eps_perm) + 0.155555555555556 * np.exp(3 * eps_perm) + 0.0444444444444444 * np.exp(
+                3.5 * eps_perm) + 0.00555555555555556 * np.exp(4 * eps_perm) - 0.222222222222222 * np.exp(
+                eps_1 + eps_perm) - 0.711111111111111 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
+                eps_1 + 2 * eps_perm) - 0.711111111111111 * np.exp(eps_1 + 2.5 * eps_perm) - 0.222222222222222 * np.exp(
+                eps_1 + 3 * eps_perm) + 0.0111111111111111 * np.exp(eps_1 + 4 * eps_perm) + 0.0444444444444444 * np.exp(
+                2 * eps_1 + 0.5 * eps_perm) + 0.155555555555556 * np.exp(2 * eps_1 + eps_perm) + 0.311111111111111 * np.exp(
+                2 * eps_1 + 1.5 * eps_perm) + 0.388888888888889 * np.exp(
+                2 * eps_1 + 2 * eps_perm) + 0.311111111111111 * np.exp(
+                2 * eps_1 + 2.5 * eps_perm) + 0.155555555555556 * np.exp(
+                2 * eps_1 + 3 * eps_perm) + 0.0444444444444444 * np.exp(
+                2 * eps_1 + 3.5 * eps_perm) + 0.00555555555555556 * np.exp(
+                2 * eps_1 + 4 * eps_perm) + 0.00555555555555556) - 0.25 * (
+                      np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
+                  eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)) * (
+                      np.exp(eps_1) + 4 * np.exp(0.5 * eps_perm) + 4 * np.exp(eps_perm) - np.exp(
+                  2 * eps_perm) - 4 * np.exp(eps_1 + eps_perm) - 4 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
+                  eps_1 + 2 * eps_perm) + 1)) / (
+                     (np.exp(eps_1) - 1) * (np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * (
+                     np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
+                 eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)))
 
-    # Number of reports
-    n = len(ue_reports)
+        if (np.array([p1, q1, p2, q2]) >= 0).all():
+            pass
+        else:
+            raise ValueError('Probabilities are negative.')
+
+        # Count how many times each bit has been reported
+        count_report = sum(reports)
 
-    # SUE parameters for round 1
-    p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
-    q1 = 1 - p1
-
-    # OUE parameters for round 2
-    p2 = 0.5
-    q2 = (3.35410196624968 * (np.exp(eps_1) - 1) * (
-            np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * np.sqrt(
-        0.0111111111111111 * np.exp(eps_1) + 0.00555555555555556 * np.exp(2 * eps_1) + 0.0444444444444444 * np.exp(
-            0.5 * eps_perm) + 0.155555555555556 * np.exp(eps_perm) + 0.311111111111111 * np.exp(
-            1.5 * eps_perm) + 0.388888888888889 * np.exp(2 * eps_perm) + 0.311111111111111 * np.exp(
-            2.5 * eps_perm) + 0.155555555555556 * np.exp(3 * eps_perm) + 0.0444444444444444 * np.exp(
-            3.5 * eps_perm) + 0.00555555555555556 * np.exp(4 * eps_perm) - 0.222222222222222 * np.exp(
-            eps_1 + eps_perm) - 0.711111111111111 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
-            eps_1 + 2 * eps_perm) - 0.711111111111111 * np.exp(eps_1 + 2.5 * eps_perm) - 0.222222222222222 * np.exp(
-            eps_1 + 3 * eps_perm) + 0.0111111111111111 * np.exp(eps_1 + 4 * eps_perm) + 0.0444444444444444 * np.exp(
-            2 * eps_1 + 0.5 * eps_perm) + 0.155555555555556 * np.exp(2 * eps_1 + eps_perm) + 0.311111111111111 * np.exp(
-            2 * eps_1 + 1.5 * eps_perm) + 0.388888888888889 * np.exp(
-            2 * eps_1 + 2 * eps_perm) + 0.311111111111111 * np.exp(
-            2 * eps_1 + 2.5 * eps_perm) + 0.155555555555556 * np.exp(
-            2 * eps_1 + 3 * eps_perm) + 0.0444444444444444 * np.exp(
-            2 * eps_1 + 3.5 * eps_perm) + 0.00555555555555556 * np.exp(
-            2 * eps_1 + 4 * eps_perm) + 0.00555555555555556) - 0.25 * (
-                  np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
-              eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)) * (
-                  np.exp(eps_1) + 4 * np.exp(0.5 * eps_perm) + 4 * np.exp(eps_perm) - np.exp(
-              2 * eps_perm) - 4 * np.exp(eps_1 + eps_perm) - 4 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
-              eps_1 + 2 * eps_perm) + 1)) / (
-                 (np.exp(eps_1) - 1) * (np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * (
-                 np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
-             eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)))
+        # Estimate with MI
+        norm_est_freq = MI_long(count_report, n, p1, q1, p2, q2)
+
+        return norm_est_freq
 
-    if (np.array([p1, q1, p2, q2]) >= 0).all():
-        pass
     else:
-        raise ValueError('Probabilities are negative.')
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
 
-    # Ensure non-negativity of estimated frequency
-    est_freq = ((sum(ue_reports) - n * q1 * (p2 - q2) - n * q2) / (n * (p1 - q1) * (p2 - q2))).clip(0)
 
-    # Re-normalized estimated frequency
-    if sum(est_freq) > 0:
-        norm_est_freq = np.nan_to_num(est_freq / sum(est_freq))
-    
+def L_SOUE_Aggregator_IBU(reports, k, eps_perm, eps_1, nb_iter=10000, tol=1e-12, err_func="max_abs"):
+    """
+    Estimator based on Iterative Bayesian Update[3,4].
+
+    :param reports: list of all L-SOUE UE-based vectors;
+    :param k: attribute's domain size;
+    :param eps_perm: upper bound of privacy guarantee (infinity reports);
+    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
+    :param nb_iter: number of iterations;
+    :param tol: tolerance;
+    :param err_func: early stopping function;
+    :return: frequency (histogram) estimation.
+    """
+
+    # Validations
+    if len(reports) == 0:
+        raise ValueError('List of reports is empty.')
+    if not isinstance(k, int) or not isinstance(nb_iter, int) or k < 2:
+        raise ValueError('k (>=2) and nb_iter need integer values.')
+    if nb_iter <= 0 or tol <= 0:
+        raise ValueError('nb_iter (int) and tol (float) need values greater than 0')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
+
+        # SUE parameters for round 1
+        p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
+        q1 = 1 - p1
+
+        # OUE parameters for round 2
+        p2 = 0.5
+        q2 = (3.35410196624968 * (np.exp(eps_1) - 1) * (
+                np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * np.sqrt(
+            0.0111111111111111 * np.exp(eps_1) + 0.00555555555555556 * np.exp(2 * eps_1) + 0.0444444444444444 * np.exp(
+                0.5 * eps_perm) + 0.155555555555556 * np.exp(eps_perm) + 0.311111111111111 * np.exp(
+                1.5 * eps_perm) + 0.388888888888889 * np.exp(2 * eps_perm) + 0.311111111111111 * np.exp(
+                2.5 * eps_perm) + 0.155555555555556 * np.exp(3 * eps_perm) + 0.0444444444444444 * np.exp(
+                3.5 * eps_perm) + 0.00555555555555556 * np.exp(4 * eps_perm) - 0.222222222222222 * np.exp(
+                eps_1 + eps_perm) - 0.711111111111111 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
+                eps_1 + 2 * eps_perm) - 0.711111111111111 * np.exp(eps_1 + 2.5 * eps_perm) - 0.222222222222222 * np.exp(
+                eps_1 + 3 * eps_perm) + 0.0111111111111111 * np.exp(eps_1 + 4 * eps_perm) + 0.0444444444444444 * np.exp(
+                2 * eps_1 + 0.5 * eps_perm) + 0.155555555555556 * np.exp(
+                2 * eps_1 + eps_perm) + 0.311111111111111 * np.exp(
+                2 * eps_1 + 1.5 * eps_perm) + 0.388888888888889 * np.exp(
+                2 * eps_1 + 2 * eps_perm) + 0.311111111111111 * np.exp(
+                2 * eps_1 + 2.5 * eps_perm) + 0.155555555555556 * np.exp(
+                2 * eps_1 + 3 * eps_perm) + 0.0444444444444444 * np.exp(
+                2 * eps_1 + 3.5 * eps_perm) + 0.00555555555555556 * np.exp(
+                2 * eps_1 + 4 * eps_perm) + 0.00555555555555556) - 0.25 * (
+                      np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
+                  eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)) * (
+                      np.exp(eps_1) + 4 * np.exp(0.5 * eps_perm) + 4 * np.exp(eps_perm) - np.exp(
+                  2 * eps_perm) - 4 * np.exp(eps_1 + eps_perm) - 4 * np.exp(eps_1 + 1.5 * eps_perm) - np.exp(
+                  eps_1 + 2 * eps_perm) + 1)) / (
+                     (np.exp(eps_1) - 1) * (np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm)) * (
+                     np.exp(0.5 * eps_perm) + 2 * np.exp(eps_perm) + np.exp(1.5 * eps_perm) - np.exp(
+                 eps_1 + 0.5 * eps_perm) - 2 * np.exp(eps_1 + eps_perm) - np.exp(eps_1 + 1.5 * eps_perm)))
+
+        if (np.array([p1, q1, p2, q2]) >= 0).all():
+            pass
+        else:
+            raise ValueError('Probabilities are negative.')
+
+        # Count how many times each bit has been reported
+        count_report = sum(reports)
+        obs_freq = count_report / sum(count_report)
+
+        # Estimate with IBU
+        p = p1 * p2 + (1 - p1) * q2  # cf [1]
+        q = (1 - q1) * q2 + q1 * p2  # cf [1]
+        A = np.eye(k)
+        A[A == 1] = p
+        A[A == 0] = q
+        est_freq = IBU(k, A, obs_freq, nb_iter, tol, err_func)
+
+        return est_freq
+
     else:
-        norm_est_freq = est_freq
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
 
-    return norm_est_freq
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/L_SUE.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/L_SUE.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 from numba import jit
+from multi_freq_ldpy.estimators.Histogram_estimator import MI_long, IBU
 
 # [1] Arcolezi et al (2021) "Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates" (arXiv:2111.04636).
 # [2] Erlingsson, Pihur, and Korolova (2014) "RAPPOR: Randomized aggregatable privacy-preserving ordinal response" (ACM CCS).
 # [3] Wang et al (2017) "Locally differentially private protocols for frequency estimation" (USENIX Security).
+# [4] Agrawal and Aggarwal (2001,) "On the design and quantification of privacy preserving data mining algorithms" (PODS).
+# [5] ElSalamouny and Palamidessi (2020) "Generalized iterative bayesian update and applications to mechanisms for privacy protection" (EuroS&P).
 
 # The analytical analysis of how to calculate parameters (p1, q2, p2, q2) is from: https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B4%5D/1_ALLOMFREE_Analysis.ipynb
 
 @jit(nopython=True)
 def L_SUE_Client(input_data, k, eps_perm, eps_1):
 
     """
@@ -15,19 +18,24 @@
 
     :param input_data: user's true value;
     :param k: attribute's domain size;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: sanitized UE vector.
     """
-    
-    if eps_1 >= eps_perm:
-        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
-    
-    else:
+
+    # Validations
+    if input_data < 0 or input_data >= k:
+        raise ValueError('input_data (integer) should be in the range [0, k-1].')
+    if not isinstance(k, int) or k < 2:
+        raise ValueError('k needs an integer value >=2.')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
+
         # SUE parameters for round 1
         p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
         q1 = 1 - p1
 
         # SUE parameters for round 2
         p2 = - (np.sqrt((4 * np.exp(7 * eps_perm / 2) - 4 * np.exp(5 * eps_perm / 2) - 4 * np.exp(
             3 * eps_perm / 2) + 4 * np.exp(eps_perm / 2) + np.exp(4 * eps_perm) + 4 * np.exp(3 * eps_perm) - 10 * np.exp(
@@ -74,58 +82,133 @@
             else:
                 rnd = np.random.random()
                 if rnd <= p2:
                     second_sanitization[ind] = 1
 
         return second_sanitization
 
-def L_SUE_Aggregator(ue_reports, eps_perm, eps_1):
+    else:
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
+
+
+def L_SUE_Aggregator_MI(reports, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) with post-processing to ensure non-negativity.
 
     :param reports: list of all L-SUE sanitized UE-based vectors;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation.
     """
 
-    if len(ue_reports) == 0:
+    # Validations
+    if len(reports) == 0:
+        raise ValueError('List of reports is empty.')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
+
+        # Number of reports
+        n = len(reports)
+
+        # SUE parameters for round 1
+        p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
+        q1 = 1 - p1
+
+        # SUE parameters for round 2
+        p2 = - (np.sqrt((4 * np.exp(7 * eps_perm / 2) - 4 * np.exp(5 * eps_perm / 2) - 4 * np.exp(
+            3 * eps_perm / 2) + 4 * np.exp(eps_perm / 2) + np.exp(4 * eps_perm) + 4 * np.exp(3 * eps_perm) - 10 * np.exp(
+            2 * eps_perm) + 4 * np.exp(eps_perm) + 1) * np.exp(eps_1)) * (np.exp(eps_1) - 1) * (
+                            np.exp(eps_perm) - 1) ** 2 - (
+                            np.exp(eps_1) - np.exp(2 * eps_perm) + 2 * np.exp(eps_perm) - 2 * np.exp(
+                        eps_1 + eps_perm) + np.exp(eps_1 + 2 * eps_perm) - 1) * (
+                            np.exp(3 * eps_perm / 2) - np.exp(eps_perm / 2) + np.exp(eps_perm) - np.exp(
+                        eps_1 + eps_perm / 2) - np.exp(eps_1 + eps_perm) + np.exp(eps_1 + 3 * eps_perm / 2) + np.exp(
+                        eps_1 + 2 * eps_perm) - 1)) / ((np.exp(eps_1) - 1) * (np.exp(eps_perm) - 1) ** 2 * (
+                    np.exp(eps_1) - np.exp(2 * eps_perm) + 2 * np.exp(eps_perm) - 2 * np.exp(eps_1 + eps_perm) + np.exp(
+                eps_1 + 2 * eps_perm) - 1))
+        q2 = 1 - p2
+
+        if (np.array([p1, q1, p2, q2]) >= 0).all():
+            pass
+        else:
+            raise ValueError('Probabilities are negative.')
+
+        # Count how many times each bit has been reported
+        count_report = sum(reports)
+
+        # Estimate with MI
+        norm_est_freq = MI_long(count_report, n, p1, q1, p2, q2)
+
+        return norm_est_freq
+
+    else:
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
+
+
+def L_SUE_Aggregator_IBU(reports, k, eps_perm, eps_1, nb_iter=10000, tol=1e-12, err_func="max_abs"):
+    """
+    Estimator based on Iterative Bayesian Update[3,4].
+
+    :param reports: list of all L-SUE UE-based vectors;
+    :param k: attribute's domain size;
+    :param eps_perm: upper bound of privacy guarantee (infinity reports);
+    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
+    :param nb_iter: number of iterations;
+    :param tol: tolerance;
+    :param err_func: early stopping function;
+    :return: frequency (histogram) estimation.
+    """
+
+    # Validations
+    if len(reports) == 0:
         raise ValueError('List of reports is empty.')
+    if not isinstance(k, int) or not isinstance(nb_iter, int) or k < 2:
+        raise ValueError('k (>=2) and nb_iter need integer values.')
+    if nb_iter <= 0 or tol <= 0:
+        raise ValueError('nb_iter (int) and tol (float) need values greater than 0')
+    if eps_perm < 0 or eps_1 < 0:
+        raise ValueError('Please ensure eps_perm and eps_1 have numerical values greater than 0.')
+    if eps_1 < eps_perm:
 
-    # Number of reports
-    n = len(ue_reports)
+        # SUE parameters for round 1
+        p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
+        q1 = 1 - p1
 
-    # SUE parameters for round 1
-    p1 = np.exp(eps_perm / 2) / (np.exp(eps_perm / 2) + 1)
-    q1 = 1 - p1
-
-    # SUE parameters for round 2
-    p2 = - (np.sqrt((4 * np.exp(7 * eps_perm / 2) - 4 * np.exp(5 * eps_perm / 2) - 4 * np.exp(
-        3 * eps_perm / 2) + 4 * np.exp(eps_perm / 2) + np.exp(4 * eps_perm) + 4 * np.exp(3 * eps_perm) - 10 * np.exp(
-        2 * eps_perm) + 4 * np.exp(eps_perm) + 1) * np.exp(eps_1)) * (np.exp(eps_1) - 1) * (
+        # SUE parameters for round 2
+        p2 = - (np.sqrt((4 * np.exp(7 * eps_perm / 2) - 4 * np.exp(5 * eps_perm / 2) - 4 * np.exp(
+            3 * eps_perm / 2) + 4 * np.exp(eps_perm / 2) + np.exp(4 * eps_perm) + 4 * np.exp(
+            3 * eps_perm) - 10 * np.exp(
+            2 * eps_perm) + 4 * np.exp(eps_perm) + 1) * np.exp(eps_1)) * (np.exp(eps_1) - 1) * (
                         np.exp(eps_perm) - 1) ** 2 - (
                         np.exp(eps_1) - np.exp(2 * eps_perm) + 2 * np.exp(eps_perm) - 2 * np.exp(
                     eps_1 + eps_perm) + np.exp(eps_1 + 2 * eps_perm) - 1) * (
                         np.exp(3 * eps_perm / 2) - np.exp(eps_perm / 2) + np.exp(eps_perm) - np.exp(
                     eps_1 + eps_perm / 2) - np.exp(eps_1 + eps_perm) + np.exp(eps_1 + 3 * eps_perm / 2) + np.exp(
                     eps_1 + 2 * eps_perm) - 1)) / ((np.exp(eps_1) - 1) * (np.exp(eps_perm) - 1) ** 2 * (
                 np.exp(eps_1) - np.exp(2 * eps_perm) + 2 * np.exp(eps_perm) - 2 * np.exp(eps_1 + eps_perm) + np.exp(
             eps_1 + 2 * eps_perm) - 1))
-    q2 = 1 - p2
+        q2 = 1 - p2
 
-    if (np.array([p1, q1, p2, q2]) >= 0).all():
-        pass
-    else:
-        raise ValueError('Probabilities are negative.')
+        if (np.array([p1, q1, p2, q2]) >= 0).all():
+            pass
+        else:
+            raise ValueError('Probabilities are negative.')
+
+        # Count how many times each bit has been reported
+        count_report = sum(reports)
+        obs_freq = count_report / sum(count_report)
+
+        # Estimate with IBU
+        p = p1 * p2 + (1 - p1) * q2  # cf [1]
+        q = (1 - q1) * q2 + q1 * p2  # cf [1]
+        A = np.eye(k)
+        A[A == 1] = p
+        A[A == 0] = q
+        est_freq = IBU(k, A, obs_freq, nb_iter, tol, err_func)
 
-    # Ensure non-negativity of estimated frequency
-    est_freq = ((sum(ue_reports) - n * q1 * (p2 - q2) - n * q2) / (n * (p1 - q1) * (p2 - q2))).clip(0)
+        return est_freq
 
-    # Re-normalized estimated frequency
-    if sum(est_freq) > 0:
-        norm_est_freq = np.nan_to_num(est_freq / sum(est_freq))
-    
     else:
-        norm_est_freq = est_freq
+        raise ValueError('Please set eps_1 (single report, i.e., lower bound) < eps_perm (infinity reports, i.e., upper bound)')
 
-    return norm_est_freq
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_freq_est/Variance_LONG_PURE.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_freq_est/Variance_LONG_PURE.py`

 * *Files identical despite different names*

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/L_SMP_Solution.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/L_SMP_Solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
-from multi_freq_ldpy.long_freq_est.L_GRR import L_GRR_Client, L_GRR_Aggregator
-from multi_freq_ldpy.long_freq_est.L_OUE import L_OUE_Client, L_OUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_OSUE import L_OSUE_Client, L_OSUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_SOUE import L_SOUE_Client, L_SOUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_ADP import L_ADP_Client, L_ADP_Aggregator
-from multi_freq_ldpy.long_freq_est.dBitFlipPM import dBitFlipPM_Client, dBitFlipPM_Aggregator
+from multi_freq_ldpy.long_freq_est.L_GRR import L_GRR_Client, L_GRR_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_OUE import L_OUE_Client, L_OUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_OSUE import L_OSUE_Client, L_OSUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_SOUE import L_SOUE_Client, L_SOUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_ADP import L_ADP_Client, L_ADP_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.dBitFlipPM import dBitFlipPM_Client, dBitFlipPM_Aggregator_MI
 
 # [1] Arcolezi et al (2021) "Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates" (arXiv:2111.04636).
 # [2] Erlingsson, Pihur, and Korolova (2014) "RAPPOR: Randomized aggregatable privacy-preserving ordinal response" (ACM CCS).
 # [3] Ding, Kulkarni, and Yekhanin (2017) "Collecting telemetry data privately." (NeurIPS).
 
 def SMP_L_GRR_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
@@ -111,59 +111,60 @@
     # Select an attribute at random
     rnd_att = np.random.randint(d)
 
     # Report the sampled attribute and its LDP value with L-SOUE protocol
     att_sanitized_value = (rnd_att, L_SOUE_Client(input_tuple[rnd_att], lst_k[rnd_att], eps_perm, eps_1))
 
     return att_sanitized_value
-    
-def SMP_dBitFlipPM_Client(input_tuple, lst_k, lst_b, d_bits, d, eps_perm):
+
+def SMP_L_ADP_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
     """
-    Sampling (SMP) a single attribute and using dBitFlipPM [3] protocol as local randomizer.
+    Sampling (SMP) a single attribute and using L-ADP [1] protocol as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param lst_k: list of attributes' domain size;
-    :param lst_b: list of attributes' new domain size (bucketized);
-    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
-    :return: tuple (sampled attribute, sanitized UE vector).
+    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
+    :return: tuple (sampled attribute, sanitized value or UE vector).
     """
 
     # Select an attribute at random
     rnd_att = np.random.randint(d)
 
-    # Report the sampled attribute and its LDP value with L-GRR protocol
-    att_sanitized_value = (rnd_att, dBitFlipPM_Client(input_tuple[rnd_att], lst_k[rnd_att], lst_b[rnd_att], d_bits, eps_perm))
+    # Report the sampled attribute and its LDP value with L-ADP protocol
+    att_sanitized_value = (rnd_att, L_ADP_Client(input_tuple[rnd_att], lst_k[rnd_att], eps_perm, eps_1))
 
-    return att_sanitized_value    
+    return att_sanitized_value
 
-def SMP_L_ADP_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
+def SMP_dBitFlipPM_Client(input_tuple, lst_k, lst_b, d_bits, d, eps_perm):
     """
-    Sampling (SMP) a single attribute and using L-ADP [1] protocol as local randomizer.
+    Sampling (SMP) a single attribute and using dBitFlipPM [3] protocol as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param lst_k: list of attributes' domain size;
+    :param lst_b: list of attributes' new domain size (bucketized);
+    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
-    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
-    :return: tuple (sampled attribute, sanitized value or UE vector).
+    :return: tuple (sampled attribute, sanitized UE vector).
     """
 
     # Select an attribute at random
     rnd_att = np.random.randint(d)
 
-    # Report the sampled attribute and its LDP value with L-ADP protocol
-    att_sanitized_value = (rnd_att, L_ADP_Client(input_tuple[rnd_att], lst_k[rnd_att], eps_perm, eps_1))
+    # Report the sampled attribute and its LDP value with L-GRR protocol
+    att_sanitized_value = (rnd_att, dBitFlipPM_Client(input_tuple[rnd_att], lst_k[rnd_att], lst_b[rnd_att], d_bits, eps_perm))
 
     return att_sanitized_value
 
-def SMP_L_GRR_Aggregator(reports_tuple, lst_k, d, eps_perm, eps_1):
+
+def SMP_L_GRR_Aggregator_MI(reports_tuple, lst_k, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized value);
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -180,19 +181,19 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_GRR_Aggregator(dic_rep_smp[idx], lst_k[idx], eps_perm, eps_1))
+        lst_freq_est.append(L_GRR_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], eps_perm, eps_1))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_L_OUE_Aggregator(reports_ue_tuple, d, eps_perm, eps_1):
+def SMP_L_OUE_Aggregator_MI(reports_ue_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -207,19 +208,19 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_OUE_Aggregator(dic_rep_smp[idx], eps_perm, eps_1))
+        lst_freq_est.append(L_OUE_Aggregator_MI(dic_rep_smp[idx], eps_perm, eps_1))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_L_OSUE_Aggregator(reports_ue_tuple, d, eps_perm, eps_1):
+def SMP_L_OSUE_Aggregator_MI(reports_ue_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -234,19 +235,19 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_OSUE_Aggregator(dic_rep_smp[idx], eps_perm, eps_1))
+        lst_freq_est.append(L_OSUE_Aggregator_MI(dic_rep_smp[idx], eps_perm, eps_1))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_L_SUE_Aggregator(reports_ue_tuple, d, eps_perm, eps_1):
+def SMP_L_SUE_Aggregator_MI(reports_ue_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -261,19 +262,19 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_SUE_Aggregator(dic_rep_smp[idx], eps_perm, eps_1))
+        lst_freq_est.append(L_SUE_Aggregator_MI(dic_rep_smp[idx], eps_perm, eps_1))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_L_SOUE_Aggregator(reports_ue_tuple, d, eps_perm, eps_1):
+def SMP_L_SOUE_Aggregator_MI(reports_ue_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -288,24 +289,25 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_SOUE_Aggregator(dic_rep_smp[idx], eps_perm, eps_1))
+        lst_freq_est.append(L_SOUE_Aggregator_MI(dic_rep_smp[idx], eps_perm, eps_1))
 
     return np.array(lst_freq_est, dtype='object')
     
-def SMP_dBitFlipPM_Aggregator(reports_ue_tuple, lst_b, d_bits, d, eps_perm):
+
+def SMP_L_ADP_Aggregator_MI(reports_ue_tuple, lst_k, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
-    :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
+    :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized value or UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation of all d attributes.
     """
 
     if len(reports_ue_tuple) == 0:
@@ -315,24 +317,24 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(dBitFlipPM_Aggregator(dic_rep_smp[idx], lst_b[idx], d_bits, eps_perm))
+        lst_freq_est.append(L_ADP_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], eps_perm, eps_1))
 
-    return np.array(lst_freq_est, dtype='object')    
+    return np.array(lst_freq_est, dtype='object')
 
-def SMP_L_ADP_Aggregator(reports_ue_tuple, lst_k, d, eps_perm, eps_1):
+def SMP_dBitFlipPM_Aggregator_MI(reports_ue_tuple, lst_b, d_bits, d, eps_perm):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
-    :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized value or UE vector);
+    :param reports_ue_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation of all d attributes.
     """
 
     if len(reports_ue_tuple) == 0:
@@ -342,10 +344,10 @@
     dic_rep_smp = {att: [] for att in range(d)}
     for val in reports_ue_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(L_ADP_Aggregator(dic_rep_smp[idx], lst_k[idx], eps_perm, eps_1))
+        lst_freq_est.append(dBitFlipPM_Aggregator_MI(dic_rep_smp[idx], lst_b[idx], d_bits, eps_perm))
 
-    return np.array(lst_freq_est, dtype='object')
+    return np.array(lst_freq_est, dtype='object')
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/long_mdim_freq_est/L_SPL_Solution.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/long_mdim_freq_est/L_SPL_Solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
-from multi_freq_ldpy.long_freq_est.L_GRR import L_GRR_Client, L_GRR_Aggregator
-from multi_freq_ldpy.long_freq_est.L_OUE import L_OUE_Client, L_OUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_OSUE import L_OSUE_Client, L_OSUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_SOUE import L_SOUE_Client, L_SOUE_Aggregator
-from multi_freq_ldpy.long_freq_est.L_ADP import L_ADP_Client, L_ADP_Aggregator
-from multi_freq_ldpy.long_freq_est.dBitFlipPM import dBitFlipPM_Client, dBitFlipPM_Aggregator
+from multi_freq_ldpy.long_freq_est.L_GRR import L_GRR_Client, L_GRR_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_OUE import L_OUE_Client, L_OUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_OSUE import L_OSUE_Client, L_OSUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_SOUE import L_SOUE_Client, L_SOUE_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.L_ADP import L_ADP_Client, L_ADP_Aggregator_MI
+from multi_freq_ldpy.long_freq_est.dBitFlipPM import dBitFlipPM_Client, dBitFlipPM_Aggregator_MI
 
 # [1] Arcolezi et al (2021) "Improving the Utility of Locally Differentially Private Protocols for Longitudinal and Multidimensional Frequency Estimates" (arXiv:2111.04636).
 # [2] Erlingsson, Pihur, and Korolova (2014) "RAPPOR: Randomized aggregatable privacy-preserving ordinal response" (ACM CCS).
 # [3] Ding, Kulkarni, and Yekhanin (2017) "Collecting telemetry data privately." (NeurIPS).
 
 def SPL_L_GRR_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
@@ -124,64 +124,65 @@
 
     # Sanitization of each value with L-SOUE protocol
     sanitized_tuple = []
     for idx in range(d):
         sanitized_tuple.append(L_SOUE_Client(input_tuple[idx], lst_k[idx], eps_perm_spl, eps_1_spl))
 
     return sanitized_tuple
-    
-def SPL_dBitFlipPM_Client(input_tuple, lst_k, lst_b, d_bits, d, eps_perm):
+
+def SPL_L_ADP_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
     """
-    Splitting (SPL) the privacy budget and using dBitFlipPM [3] protocol as local randomizer.
+    Splitting (SPL) the privacy budget and using L-ADP [1] protocol (a.k.a. ALLOMFREE [1]) as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param lst_k: list of attributes' domain size;
-    :param lst_b: list of attributes' new domain size (bucketized);
-    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
+    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: tuple of sanitized UE vectors.
     """
 
     # Splitting the privacy budget over the number of attributes d
     eps_perm_spl = eps_perm / d
+    eps_1_spl = eps_1 / d
 
-    # Sanitization of each value with L-GRR protocol
+    # Sanitization of each value with L-ADP protocol
     sanitized_tuple = []
     for idx in range(d):
-        sanitized_tuple.append(dBitFlipPM_Client(input_tuple[idx], lst_k[idx], lst_b[idx], d_bits, eps_perm_spl))
+        sanitized_tuple.append(L_ADP_Client(input_tuple[idx], lst_k[idx], eps_perm_spl, eps_1_spl))
 
-    return sanitized_tuple    
+    return sanitized_tuple
 
-def SPL_L_ADP_Client(input_tuple, lst_k, d, eps_perm, eps_1):
 
+def SPL_dBitFlipPM_Client(input_tuple, lst_k, lst_b, d_bits, d, eps_perm):
     """
-    Splitting (SPL) the privacy budget and using L-ADP [1] protocol (a.k.a. ALLOMFREE [1]) as local randomizer.
+    Splitting (SPL) the privacy budget and using dBitFlipPM [3] protocol as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param lst_k: list of attributes' domain size;
+    :param lst_b: list of attributes' new domain size (bucketized);
+    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
-    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: tuple of sanitized UE vectors.
     """
 
     # Splitting the privacy budget over the number of attributes d
     eps_perm_spl = eps_perm / d
-    eps_1_spl = eps_1 / d
 
-    # Sanitization of each value with L-ADP protocol
+    # Sanitization of each value with L-GRR protocol
     sanitized_tuple = []
     for idx in range(d):
-        sanitized_tuple.append(L_ADP_Client(input_tuple[idx], lst_k[idx], eps_perm_spl, eps_1_spl))
+        sanitized_tuple.append(dBitFlipPM_Client(input_tuple[idx], lst_k[idx], lst_b[idx], d_bits, eps_perm_spl))
 
     return sanitized_tuple
 
-def SPL_L_GRR_Aggregator(reports_tuple, lst_k, d, eps_perm, eps_1):
+
+def SPL_L_GRR_Aggregator_MI(reports_tuple, lst_k, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -196,19 +197,19 @@
     eps_perm_spl = eps_perm / d
     eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_GRR_Aggregator(reports, lst_k[idx], eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(L_GRR_Aggregator_MI(reports, lst_k[idx], eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_L_OUE_Aggregator(reports_tuple, d, eps_perm, eps_1):
+def SPL_L_OUE_Aggregator_MI(reports_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -222,19 +223,19 @@
     eps_perm_spl = eps_perm / d
     eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_OUE_Aggregator(reports, eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(L_OUE_Aggregator_MI(reports, eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_L_OSUE_Aggregator(reports_tuple, d, eps_perm, eps_1):
+def SPL_L_OSUE_Aggregator_MI(reports_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -248,45 +249,45 @@
     eps_perm_spl = eps_perm / d
     eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_OSUE_Aggregator(reports, eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(L_OSUE_Aggregator_MI(reports, eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
-    
-def SPL_dBitFlipPM_Aggregator(reports_tuple, lst_b, d_bits, d, eps_perm):
+
+def SPL_L_SUE_Aggregator_MI(reports_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
-    :param lst_b: list of attributes' new domain size (bucketized);
-    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
+    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation of all d attributes.
     """
 
     reports_tuple = np.array(reports_tuple, dtype='object')
 
     # Splitting the privacy budget over the number of attributes d
     eps_perm_spl = eps_perm / d
+    eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(dBitFlipPM_Aggregator(reports, lst_b[idx], d_bits, eps_perm_spl))
+        lst_freq_est.append(L_SUE_Aggregator_MI(reports, eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_L_SUE_Aggregator(reports_tuple, d, eps_perm, eps_1):
+def SPL_L_SOUE_Aggregator_MI(reports_tuple, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
@@ -300,24 +301,25 @@
     eps_perm_spl = eps_perm / d
     eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_SUE_Aggregator(reports, eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(L_SOUE_Aggregator_MI(reports, eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_L_SOUE_Aggregator(reports_tuple, d, eps_perm, eps_1):
+def SPL_L_ADP_Aggregator_MI(reports_tuple, lst_k, d, eps_perm, eps_1):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
+    :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
     :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation of all d attributes.
     """
 
     reports_tuple = np.array(reports_tuple, dtype='object')
@@ -326,37 +328,36 @@
     eps_perm_spl = eps_perm / d
     eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_SOUE_Aggregator(reports, eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(L_ADP_Aggregator_MI(reports, lst_k[idx], eps_perm_spl, eps_1_spl))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_L_ADP_Aggregator(reports_tuple, lst_k, d, eps_perm, eps_1):
 
+def SPL_dBitFlipPM_Aggregator_MI(reports_tuple, lst_b, d_bits, d, eps_perm):
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
-    :param lst_k: list of attributes' domain size;
+    :param lst_b: list of attributes' new domain size (bucketized);
+    :param d_bits: number of bits to report;
     :param d: number of attributes;
     :param eps_perm: upper bound of privacy guarantee (infinity reports);
-    :param eps_1: lower bound of privacy guarantee (a single report), thus, eps_1 < eps_perm;
     :return: normalized frequency (histogram) estimation of all d attributes.
     """
 
     reports_tuple = np.array(reports_tuple, dtype='object')
 
     # Splitting the privacy budget over the number of attributes d
     eps_perm_spl = eps_perm / d
-    eps_1_spl = eps_1 / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(L_ADP_Aggregator(reports, lst_k[idx], eps_perm_spl, eps_1_spl))
+        lst_freq_est.append(dBitFlipPM_Aggregator_MI(reports, lst_b[idx], d_bits, eps_perm_spl))
 
-    return np.array(lst_freq_est, dtype='object')
+    return np.array(lst_freq_est, dtype='object')
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/RSpFD_solution.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/RSpFD_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                 sanitized_tuple.append(GRR_Client(input_tuple[idx], k, amp_eps))
 
             else:
                 sanitized_tuple.append(UE_Client(input_tuple[idx], k, amp_eps, optimal))
 
     return sanitized_tuple
 
-def RSpFD_GRR_Aggregator(reports_tuple, lst_k, d, epsilon):
+def RSpFD_GRR_Aggregator_MI(reports_tuple, lst_k, d, epsilon):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all RS+FD[GRR]-based sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -212,15 +212,15 @@
         # Re-normalized estimated frequency
         norm_est_freq = est_freq / sum(est_freq)
 
         lst_freq_est.append(norm_est_freq)
 
     return np.array(lst_freq_est, dtype='object')
 
-def RSpFD_UE_zero_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def RSpFD_UE_zero_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all RS+FD[UE-zero]-based sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -261,15 +261,15 @@
         # Re-normalized estimated frequency
         norm_est_freq = est_freq / sum(est_freq)
 
         lst_freq_est.append(norm_est_freq)
 
     return np.array(lst_freq_est, dtype='object')
 
-def RSpFD_UE_rnd_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def RSpFD_UE_rnd_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all RS+FD[UE-rnd]-based sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -310,15 +310,15 @@
         # Re-normalized estimated frequency
         norm_est_freq = est_freq / sum(est_freq)
 
         lst_freq_est.append(norm_est_freq)
 
     return np.array(lst_freq_est, dtype='object')
 
-def RSpFD_ADP_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def RSpFD_ADP_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all RS+FD[GRR]- / RS+FD[UE-zero]-based sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/SMP_solution.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/SMP_solution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from multi_freq_ldpy.pure_frequency_oracles.GRR import GRR_Client, GRR_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.UE import UE_Client, UE_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.ADP import ADP_Client, ADP_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.LH import LH_Client, LH_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.SS import SS_Client, SS_Aggregator
+from multi_freq_ldpy.pure_frequency_oracles.GRR import GRR_Client, GRR_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.UE import UE_Client, UE_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.ADP import ADP_Client, ADP_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.LH import LH_Client, LH_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.SS import SS_Client, SS_Aggregator_MI
 
 # [1] Kairouz, Bonawitz, and Ramage (2016) "Discrete distribution estimation under local privacy" (ICML)
 # [2] Erlingsson, Pihur, and Korolova (2014) "RAPPOR: Randomized aggregatable privacy-preserving ordinal response" (ACM CCS).
 # [3] Wang et al (2017) "Locally differentially private protocols for frequency estimation" (USENIX Security).
 # [4] Ye and Barg (2018) "Optimal schemes for discrete distribution estimation under locally differential privacy" (IEEE Transactions on Information Theory)
 # [5] Wang et al (2016) "Mutual information optimally local private discrete distribution estimation" (arXiv:1607.08025).
 
@@ -48,15 +48,15 @@
     rnd_att = np.random.randint(d)
 
     # Report the sampled attribute and its LDP value with UE protocol
     att_sanitized_value = (rnd_att, UE_Client(input_tuple[rnd_att], lst_k[rnd_att], epsilon, optimal))
     
     return att_sanitized_value
 
-def SMP_LH_Client(input_tuple, d, epsilon, optimal=True):
+def SMP_LH_Client(input_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Sampling (SMP) a single attribute and using Local Hashing (LH) protocol [3] as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
@@ -64,15 +64,15 @@
     :return: tuple (sampled attribute and tuple of sanitized value and random seed).
     """
 
     # Select an attribute at random
     rnd_att = np.random.randint(d)
 
     # Report the sampled attribute and its LDP value with UE protocol
-    att_sanitized_value = (rnd_att, LH_Client(input_tuple[rnd_att], epsilon, optimal))
+    att_sanitized_value = (rnd_att, LH_Client(input_tuple[rnd_att], lst_k[rnd_att], epsilon, optimal))
     
     return att_sanitized_value
 
 def SMP_SS_Client(input_tuple, lst_k, d, epsilon):
 
     """
     Sampling (SMP) a single attribute and using Subset Selection (SS) [4,5] protocol as local randomizer.
@@ -109,15 +109,15 @@
     rnd_att = np.random.randint(d)
 
     # Report the sampled attribute and its LDP value with ADP protocol
     att_sanitized_value = (rnd_att, ADP_Client(input_tuple[rnd_att], lst_k[rnd_att], epsilon, optimal))
 
     return att_sanitized_value
 
-def SMP_GRR_Aggregator(reports_tuple, lst_k, d, epsilon):
+def SMP_GRR_Aggregator_MI(reports_tuple, lst_k, d, epsilon):
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized value);
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
@@ -132,19 +132,19 @@
     dic_rep_smp = {att:[] for att in range(d)}
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(GRR_Aggregator(dic_rep_smp[idx], lst_k[idx], epsilon))
+        lst_freq_est.append(GRR_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], epsilon))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_UE_Aggregator(reports_tuple, d, epsilon, optimal=True):
+def SMP_UE_Aggregator_MI(reports_tuple, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized UE vector);
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
@@ -160,19 +160,19 @@
     dic_rep_smp = {att:[] for att in range(d)}
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(UE_Aggregator(dic_rep_smp[idx], epsilon, optimal))
+        lst_freq_est.append(UE_Aggregator_MI(dic_rep_smp[idx], epsilon, optimal))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SMP_LH_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def SMP_LH_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized value, and random seed);
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -189,19 +189,19 @@
     dic_rep_smp = {att:[] for att in range(d)}
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(LH_Aggregator(dic_rep_smp[idx], lst_k[idx], epsilon, optimal))
+        lst_freq_est.append(LH_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], epsilon, optimal))
 
     return np.array(lst_freq_est, dtype='object')
     
-def SMP_SS_Aggregator(reports_tuple, lst_k, d, epsilon):
+def SMP_SS_Aggregator_MI(reports_tuple, lst_k, d, epsilon):
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized value);
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
@@ -216,19 +216,19 @@
     dic_rep_smp = {att:[] for att in range(d)}
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
-        lst_freq_est.append(SS_Aggregator(dic_rep_smp[idx], lst_k[idx], epsilon))
+        lst_freq_est.append(SS_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], epsilon))
 
     return np.array(lst_freq_est, dtype='object')    
 
-def SMP_ADP_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def SMP_ADP_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all tuples (sampled attribute, sanitized value or UE vector);
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
@@ -244,10 +244,10 @@
     for val in reports_tuple:
         dic_rep_smp[val[0]].append(val[-1])
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
 
-        lst_freq_est.append(ADP_Aggregator(dic_rep_smp[idx], lst_k[idx], epsilon, optimal))
+        lst_freq_est.append(ADP_Aggregator_MI(dic_rep_smp[idx], lst_k[idx], epsilon, optimal))
 
     return np.array(lst_freq_est, dtype='object')
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/SPL_solution.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/SPL_solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-from multi_freq_ldpy.pure_frequency_oracles.GRR import GRR_Client, GRR_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.UE import UE_Client, UE_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.ADP import ADP_Client, ADP_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.LH import LH_Client, LH_Aggregator
-from multi_freq_ldpy.pure_frequency_oracles.SS import SS_Client, SS_Aggregator
+from multi_freq_ldpy.pure_frequency_oracles.GRR import GRR_Client, GRR_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.UE import UE_Client, UE_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.ADP import ADP_Client, ADP_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.LH import LH_Client, LH_Aggregator_MI
+from multi_freq_ldpy.pure_frequency_oracles.SS import SS_Client, SS_Aggregator_MI
 
 # [1] Kairouz, Bonawitz, and Ramage (2016) "Discrete distribution estimation under local privacy" (ICML)
 # [2] Erlingsson, Pihur, and Korolova (2014) "RAPPOR: Randomized aggregatable privacy-preserving ordinal response" (ACM CCS).
 # [3] Wang et al (2017) "Locally differentially private protocols for frequency estimation" (USENIX Security).
 # [4] Ye and Barg (2018) "Optimal schemes for discrete distribution estimation under locally differential privacy" (IEEE Transactions on Information Theory)
 # [5] Wang et al (2016) "Mutual information optimally local private discrete distribution estimation" (arXiv:1607.08025).
 
@@ -53,15 +53,15 @@
 	sanitized_ue_tuple = []
 	for idx in range(d):
 
 		sanitized_ue_tuple.append(UE_Client(input_tuple[idx], lst_k[idx], eps_spl, optimal))
 
 	return sanitized_ue_tuple
 
-def SPL_LH_Client(input_tuple, d, epsilon, optimal=True):
+def SPL_LH_Client(input_tuple, lst_k, d, epsilon, optimal=True):
     """
     Splitting (SPL) the privacy budget and using Local Hashing (LH) [3] protocol as local randomizer.
 
     :param input_tuple: user's true tuple of values;
     :param d: number of attributes;
     :param epsilon: privacy guarantee;
     :param optimal: if True, it uses the Optimized LH (OLH) protocol from [3];
@@ -71,15 +71,15 @@
     # Splitting the privacy budget over the number of attributes d
     eps_spl = epsilon / d
 
     # Sanitization of each value with UE protocol
     sanitized_tuple = []
     for idx in range(d):
 
-        sanitized_tuple.append(LH_Client(input_tuple[idx], eps_spl, optimal))
+        sanitized_tuple.append(LH_Client(input_tuple[idx], lst_k[idx], eps_spl, optimal))
 
     return sanitized_tuple
 
 def SPL_SS_Client(input_tuple, lst_k, d, epsilon):
 
 	"""
 	Splitting (SPL) the privacy budget and using Subset Selection (SS) [4,5] protocol as local randomizer.
@@ -122,15 +122,15 @@
 	sanitized_tuple = []
 	for idx in range(d):
 
 		sanitized_tuple.append(ADP_Client(input_tuple[idx], lst_k[idx], eps_spl, optimal))
 
 	return sanitized_tuple
 
-def SPL_GRR_Aggregator(reports_tuple, lst_k, d, epsilon):
+def SPL_GRR_Aggregator_MI(reports_tuple, lst_k, d, epsilon):
 
 	"""
 	Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
 	:param reports_tuple: list of all sanitized tuples;
 	:param lst_k: list of attributes' domain size;
 	:param d: number of attributes;
@@ -147,19 +147,19 @@
 	eps_spl = epsilon / d
 
 	# Estimated frequency for all d attributes
 	lst_freq_est = []
 	for idx in range(d):
 		
 		reports = reports_tuple[:, idx]
-		lst_freq_est.append(GRR_Aggregator(reports, lst_k[idx], eps_spl))
+		lst_freq_est.append(GRR_Aggregator_MI(reports, lst_k[idx], eps_spl))
 
 	return np.array(lst_freq_est, dtype='object')
 
-def SPL_UE_Aggregator(reports_tuple, d, epsilon, optimal=True):
+def SPL_UE_Aggregator_MI(reports_tuple, d, epsilon, optimal=True):
 
 	"""
 	Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
 	:param reports_tuple: list of all sanitized tuples;
 	:param lst_k: list of attributes' domain size;
 	:param d: number of attributes;
@@ -177,19 +177,19 @@
 	eps_spl = epsilon / d
 
 	# Estimated frequency for all d attributes
 	lst_freq_est = []
 	for idx in range(d):
 		
 		reports_ue = reports_tuple[:, idx]
-		lst_freq_est.append(UE_Aggregator(reports_ue, eps_spl, optimal))
+		lst_freq_est.append(UE_Aggregator_MI(reports_ue, eps_spl, optimal))
 
 	return np.array(lst_freq_est, dtype='object')
 
-def SPL_LH_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def SPL_LH_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
     """
     Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
     :param reports_tuple: list of all sanitized tuples;
     :param lst_k: list of attributes' domain size;
     :param d: number of attributes;
@@ -207,19 +207,19 @@
     eps_spl = epsilon / d
 
     # Estimated frequency for all d attributes
     lst_freq_est = []
     for idx in range(d):
 
         reports = reports_tuple[:, idx]
-        lst_freq_est.append(LH_Aggregator(reports, lst_k[idx], eps_spl, optimal))
+        lst_freq_est.append(LH_Aggregator_MI(reports, lst_k[idx], eps_spl, optimal))
 
     return np.array(lst_freq_est, dtype='object')
 
-def SPL_SS_Aggregator(reports_tuple, lst_k, d, epsilon):
+def SPL_SS_Aggregator_MI(reports_tuple, lst_k, d, epsilon):
 
 	"""
 	Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
 	:param reports_tuple: list of all sanitized tuples;
 	:param lst_k: list of attributes' domain size;
 	:param d: number of attributes;
@@ -236,19 +236,19 @@
 	eps_spl = epsilon / d
 
 	# Estimated frequency for all d attributes
 	lst_freq_est = []
 	for idx in range(d):
 		
 		reports = reports_tuple[:, idx]
-		lst_freq_est.append(SS_Aggregator(reports, lst_k[idx], eps_spl))
+		lst_freq_est.append(SS_Aggregator_MI(reports, lst_k[idx], eps_spl))
 
 	return np.array(lst_freq_est, dtype='object')
 
-def SPL_ADP_Aggregator(reports_tuple, lst_k, d, epsilon, optimal=True):
+def SPL_ADP_Aggregator_MI(reports_tuple, lst_k, d, epsilon, optimal=True):
 
 	"""
 	Statistical Estimator for Normalized Frequency (0 -- 1) of all d attributes with post-processing to ensure non-negativity.
 
 	:param reports_tuple: list of all sanitized tuples;
 	:param lst_k: list of attributes' domain size;
 	:param d: number of attributes;
@@ -266,10 +266,10 @@
 	eps_spl = epsilon / d
 
 	# Estimated frequency for all d attributes
 	lst_freq_est = []
 	for idx in range(d):
 
 		reports = reports_tuple[:, idx]
-		lst_freq_est.append(ADP_Aggregator(reports, lst_k[idx], eps_spl, optimal))
+		lst_freq_est.append(ADP_Aggregator_MI(reports, lst_k[idx], eps_spl, optimal))
 
 	return np.array(lst_freq_est, dtype='object')
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/mdim_freq_est/Variance_RSpFD.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/mdim_freq_est/Variance_RSpFD.py`

 * *Files identical despite different names*

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy/pure_frequency_oracles/Variance_PURE.py` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy/pure_frequency_oracles/Variance_PURE.py`

 * *Files identical despite different names*

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/PKG-INFO` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,59 @@
 Metadata-Version: 2.1
 Name: multi-freq-ldpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Multiple Frequency Estimation Under Local Differential Privacy in Python
 Home-page: https://github.com/hharcolezi/multi-freq-ldpy
 Author: Héber H. Arcolezi
 Author-email: hh.arcolezi@gmail.com
 License: MIT
 Keywords: local-differential-privacy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python
 
-Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
+Multi-Freq-LDPy is a Python library for performing multiple frequency estimation tasks (one-time, multidimensional, longitudinal, and both) under local differential privacy (LDP) guarantees. The main goal is to provide an easy-to-use and fast execution toolkit to benchmark and experiment with state-of-the-art solutions and LDP protocols.
 
 Here's an introductory [Video_Presentation](https://screencast-o-matic.com/watch/c3hhQYVYNDi), [Slide_Presentation](http://hharcolezi.github.io/files/2022_Multi_Freq_LDPy_Presentation.pdf), and [arXived Demonstration Paper](https://arxiv.org/abs/2205.02648) of our package.
 
 If our codes and work are useful to you, we would appreciate a reference to:
 
 ```
-@article{arcolezi2022multi,
-  title={Multi-Freq-LDPy: Multiple Frequency Estimation Under Local Differential Privacy in Python},
-  author={Arcolezi, H{\'e}ber H and Couchot, Jean-Fran{\c{c}}ois and Gambs, S{\'e}bastien and Palamidessi, Catuscia and Zolfaghari, Majid},
-  journal={arXiv preprint arXiv:2205.02648},
-  year={2022}
+@incollection{Arcolezi2022,
+  doi = {10.1007/978-3-031-17143-7_40},
+  url = {https://doi.org/10.1007/978-3-031-17143-7_40},
+  year = {2022},
+  publisher = {Springer Nature Switzerland},
+  pages = {770--775},
+  author = {H{\'{e}}ber H. Arcolezi and Jean-Fran{\c{c}}ois Couchot and S{\'{e}}bastien Gambs and Catuscia Palamidessi and Majid Zolfaghari},
+  title = {Multi-Freq-{LDPy}: Multiple Frequency Estimation Under Local Differential Privacy in~Python},
+  booktitle = {Computer Security {\textendash} {ESORICS} 2022}
 }
 ```
 
+```
+@incollection{Arcolezi2023,
+  doi = {10.1007/978-3-031-37586-6_11},
+  url = {https://doi.org/10.1007/978-3-031-37586-6_11},
+  year = {2023},
+  publisher = {Springer Nature Switzerland},
+  pages = {165--183},
+  author = {H{\'{e}}ber H. Arcolezi and Selene Cerna and Catuscia Palamidessi},
+  title = {On the Utility Gain of Iterative Bayesian Update for Locally Differentially Private Mechanisms},
+  booktitle = {Data and Applications Security and Privacy {XXXVII}}
+}
+```
+
+
+
 ## Installation
 
 Please use the package manager [pip](https://pypi.org/project/multi-freq-ldpy/) to install multi-freq-ldpy.
 
 ```bash
 pip install multi-freq-ldpy
 ```
@@ -60,14 +79,17 @@
 multi-freq-ldpy package
 |
 |- pure_frequency_oracles (Single Frequency Estimation)
 |  |- GRR (Generalized Randomized Response[1,2] a.k.a. k-RR or Direct Encoding)
 |  |- UE (Unary Encoding)
 |  |  |- SUE (Symmetric UE[3] a.k.a. Basic One-Time RAPPOR[11])
 |  |  |- OUE (Optimized UE[3])
+|  |- HE (Histogram Encoding)
+|  |  |- SHE (Summation with HE[3])
+|  |  |- THE (Thresholding with HE[3])
 |  |- LH (Local Hashing)
 |  |  |- BLH (Binary LH[3,4])
 |  |  |- OLH (Optimized LH[3])
 |  |- SS (Subset Selection[5,6])
 |  |- ADP (Adaptive, i.e., GRR or OUE)
 |
 |- mdim_freq_est (Multidimensional Frequency Estimation)
@@ -81,89 +103,102 @@
 |  |  |- RSpFD_SUE_rnd (fake data generated with SUE applied to a random bit-vector)
 |  |  |- RSpFD_OUE_zero (fake data generated with OUE applied to a zero-vector)
 |  |  |- RSpFD_OUE_rnd (fake data generated with OUE applied to a random bit-vector)
 |  |  |- RSpFD_ADP (RSpFD_GRR or RSpFD_OUE_z)
 |
 |- long_freq_est (Longitudinal Single Frequency Estimation)
 |  |- L_GRR (Longitudinal GRR[10])
+|  |- L_LH (Longitudinal LH[12])
+|  |  |- L_BLH (Binary LH[12])
+|  |  |- L_OLH (Optimized LH[12])
 |  |- L_OUE (Longitudinal OUE[10])
 |  |- L_OSUE (Longitudinal OUE-SUE[10])
 |  |- L_SUE (Longitudinal SUE[10], a.k.a. Basic RAPPOR[11])
 |  |- L_SOUE (Longitudinal SUE-OUE[10])
 |  |- L_ADP (Longitudinal ADP[10], i.e., L-GRR or L-OSUE)
-|  |- dBitFlipPM[12]
+|  |- dBitFlipPM[13]
 |
 |- long_mdim_freq_est (Longitudinal Multidimensional Frequency Estimation)
 |  |- Longitudinal SPL (L_SPL_Solution[10]): Splits the privacy budget and sanitizes using long_freq_est LDP protocols
 |  |  |- SPL_L_GRR, SPL_L_OUE, SPL_L_OSUE, SPL_L_SUE, SPL_L_SOUE, SPL_L_ADP, SPL_dBitFlipPM
 |  |- Longitudinal SMP (L_SMP_Solution[10]): Samples a single attribute and sanitizes using long_freq_est LDP protocols
 |  |  |- SMP_L_GRR, SMP_L_OUE, SMP_L_OSUE, SMP_L_SUE, SMP_L_SOUE, SMP_L_ADP, SMP_dBitFlipPM
+|
+| - estimators (Distribution Estimator Methods)
+|  |- MI (Matrix Inverse)
+|  |- IBU (Iterative Bayesian Estimator[14])
 ```
 
 ## Usage
 This is a function-based package that simulates the LDP data collection pipeline of users and the server. For each functionality, there is always a ```Client``` and an ```Aggregator``` function. For more details, please refer to the [tutorials](https://github.com/hharcolezi/multi-freq-ldpy/tree/main/tutorials) folder, which covers all 1--4 tasks with real-world open datasets ([Adult](https://archive.ics.uci.edu/ml/datasets/adult), [Nursery](https://archive.ics.uci.edu/ml/datasets/nursery), [MS-FIMU](https://github.com/hharcolezi/OpenMSFIMU)).
 
 ```python
 # Common libraries
 import numpy as np
 import matplotlib.pyplot as plt
 
 # Multi-Freq-LDPy functions for L-SUE protocol (a.k.a. Basic RAPPOR[11])
-from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator
+from multi_freq_ldpy.long_freq_est.L_SUE import L_SUE_Client, L_SUE_Aggregator_MI, L_SUE_Aggregator_IBU
 
 # Parameters for simulation
 epsilon_perm = 2 # longitudinal privacy guarantee, i.e., upper bound (infinity reports)
 epsilon_1 = 0.5 * epsilon_perm # single report privacy guarantee, i.e., lower bound
 n = int(1e6) # number of users
 k = 5 # attribute's domain size
 
 # Simulation dataset where every user has a number between [0-k) with n users
 data = np.random.randint(k, size=n)
 
 # Simulation of client-side
 l_sue_reports = [L_SUE_Client(input_data, k, epsilon_perm, epsilon_1) for input_data in data]
 
-# Simulation of server-side aggregation
-l_sue_est_freq = L_SUE_Aggregator(l_sue_reports, epsilon_perm, epsilon_1)
+# Simulation of server-side aggregation with Matrix Inversion (MI)
+l_sue_est_freq_MI = L_SUE_Aggregator_MI(l_sue_reports, epsilon_perm, epsilon_1)
+
+# Simulation of server-side aggregation with Iterative Bayesian Updates (IBU)[14]
+l_sue_est_freq_IBU = L_SUE_Aggregator_IBU(l_sue_reports, k, epsilon_perm, epsilon_1)
 
 # Real frequency 
 real_freq = np.unique(data, return_counts=True)[-1] / n
 
 # Visualizing results
-barwidth = 0.45
-x_axis = np.arange(k)
+x = np.arange(k)  # the label locations
+barwidth = 0.3 # the width of the bars
 
-plt.bar(x_axis - barwidth/2, real_freq, label='Real Freq', width=barwidth)
-plt.bar(x_axis + barwidth/2 , l_sue_est_freq, label='Est Freq: L-SUE', width=barwidth)
+plt.bar(x - barwidth, real_freq, label='Real Freq', width=barwidth)
+plt.bar(x , l_sue_est_freq_MI, label='MI Est Freq: L-SUE', width=barwidth)
+plt.bar(x + barwidth, l_sue_est_freq_IBU, label='IBU Est Freq: L-SUE', width=barwidth)
 plt.ylabel('Normalized Frequency')
 plt.xlabel('Domain values')
-plt.legend(loc='upper right', bbox_to_anchor=(1.015, 1.15))
+plt.legend(ncol=3, loc='upper right', bbox_to_anchor=(1., 1.1))
 plt.show();
 ```
 
 ## Contributing
 Multi-Freq-LDPy is a work in progress, and we expect to release new versions frequently, incorporating feedback and code contributions from the community. Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Contact
-For any question, please contact [Heber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
+For any question, please contact [HÃ©ber H. Arcolezi](https://hharcolezi.github.io/): heber.hwang-arcolezi [at] inria.fr
 
 ## Acknowledgments
    * The Local Hashing (LH) functions were adapted from the [pure-LDP](https://github.com/Samuel-Maddock/pure-LDP) package, which covers a wider range of frequency oracles for single-frequency estimation.
-   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) repository. 
+   * Some codes were adapted from our [ldp-protocols-mobility-cdrs](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs) and [LOLOHA](https://github.com/hharcolezi/LOLOHA) repositories. 
 
 ## License
 [MIT](https://github.com/hharcolezi/multi-freq-ldpy/blob/main/LICENSE)
 
 
-## References
+## Main References
 - [1] Kairouz, Peter, Keith Bonawitz, and Daniel Ramage. "Discrete distribution estimation under local privacy." International Conference on Machine Learning. PMLR, 2016.
 - [2] Kairouz, Peter, Sewoong Oh, and Pramod Viswanath. "Extremal mechanisms for local differential privacy." Advances in neural information processing systems 27 (2014).
 - [3] Wang, Tianhao, et al. "Locally differentially private protocols for frequency estimation." 26th USENIX Security Symposium (USENIX Security 17). 2017.
 - [4] Bassily, Raef, and Adam Smith. "Local, private, efficient protocols for succinct histograms." Proceedings of the forty-seventh annual ACM symposium on Theory of computing. 2015.
 - [5] Ye, Min, and Alexander Barg. "Optimal schemes for discrete distribution estimation under locally differential privacy." IEEE Transactions on Information Theory 64.8 (2018): 5662-5676.
 - [6] Wang, Shaowei, et al. "Mutual information optimally local private discrete distribution estimation." arXiv preprint arXiv:1607.08025 (2016).
 - [7] NguyÃªn, ThÃ´ng T., et al. "Collecting and analyzing data from smart device users with local differential privacy." arXiv preprint arXiv:1606.05053 (2016).
 - [8] Wang, Ning, et al. "Collecting and analyzing multidimensional data with local differential privacy." 2019 IEEE 35th International Conference on Data Engineering (ICDE). IEEE, 2019.
 - [9] Arcolezi, HÃ©ber H., et al. "Random sampling plus fake data: Multidimensional frequency estimates with local differential privacy." Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021.
 - [10] Arcolezi, HÃ©ber H., et al. "Improving the utility of locally differentially private protocols for longitudinal and multidimensional frequency estimates." Digital Communications and Networks (2022).
 - [11] Erlingsson, Ãšlfar, Vasyl Pihur, and Aleksandra Korolova. "Rappor: Randomized aggregatable privacy-preserving ordinal response." Proceedings of the 2014 ACM SIGSAC conference on computer and communications security. 2014.
-- [12] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [12] Arcolezi, HÃ©ber H., et al. "Frequency Estimation of Evolving Data Under Local Differential Privacy." arXiv preprint arXiv:2210.00262 (2022).
+- [13] Ding, Bolin, Janardhan Kulkarni, and Sergey Yekhanin. "Collecting telemetry data privately." Advances in Neural Information Processing Systems 30 (2017).
+- [14] Agrawal, Dakshi, and Charu C. Aggarwal. "On the design and quantification of privacy preserving data mining algorithms." Proceedings of the twentieth ACM SIGMOD-SIGACT-SIGART symposium on Principles of database systems. 2001.
```

### Comparing `multi-freq-ldpy-0.2.4/src/multi_freq_ldpy.egg-info/SOURCES.txt` & `multi-freq-ldpy-0.2.5/src/multi_freq_ldpy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-LICENSE
+LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/multi_freq_ldpy/__init__.py
 src/multi_freq_ldpy.egg-info/PKG-INFO
 src/multi_freq_ldpy.egg-info/SOURCES.txt
 src/multi_freq_ldpy.egg-info/dependency_links.txt
 src/multi_freq_ldpy.egg-info/requires.txt
 src/multi_freq_ldpy.egg-info/top_level.txt
+src/multi_freq_ldpy/estimators/Histogram_estimator.py
+src/multi_freq_ldpy/estimators/__init__.py
 src/multi_freq_ldpy/long_freq_est/L_ADP.py
 src/multi_freq_ldpy/long_freq_est/L_GRR.py
+src/multi_freq_ldpy/long_freq_est/L_LH.py
 src/multi_freq_ldpy/long_freq_est/L_OSUE.py
 src/multi_freq_ldpy/long_freq_est/L_OUE.py
 src/multi_freq_ldpy/long_freq_est/L_SOUE.py
 src/multi_freq_ldpy/long_freq_est/L_SUE.py
 src/multi_freq_ldpy/long_freq_est/Variance_LONG_PURE.py
 src/multi_freq_ldpy/long_freq_est/__init__.py
 src/multi_freq_ldpy/long_freq_est/dBitFlipPM.py
@@ -24,12 +27,13 @@
 src/multi_freq_ldpy/mdim_freq_est/RSpFD_solution.py
 src/multi_freq_ldpy/mdim_freq_est/SMP_solution.py
 src/multi_freq_ldpy/mdim_freq_est/SPL_solution.py
 src/multi_freq_ldpy/mdim_freq_est/Variance_RSpFD.py
 src/multi_freq_ldpy/mdim_freq_est/__init__.py
 src/multi_freq_ldpy/pure_frequency_oracles/ADP.py
 src/multi_freq_ldpy/pure_frequency_oracles/GRR.py
+src/multi_freq_ldpy/pure_frequency_oracles/HE.py
 src/multi_freq_ldpy/pure_frequency_oracles/LH.py
 src/multi_freq_ldpy/pure_frequency_oracles/SS.py
 src/multi_freq_ldpy/pure_frequency_oracles/UE.py
 src/multi_freq_ldpy/pure_frequency_oracles/Variance_PURE.py
 src/multi_freq_ldpy/pure_frequency_oracles/__init__.py
```

