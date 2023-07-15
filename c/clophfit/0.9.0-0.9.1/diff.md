# Comparing `tmp/clophfit-0.9.0.tar.gz` & `tmp/clophfit-0.9.1.tar.gz`

## Comparing `clophfit-0.9.0.tar` & `clophfit-0.9.1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.9.0/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.9.0/.darglint
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 clophfit-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 clophfit-0.9.0/.python-version
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 clophfit-0.9.0/.readthedocs.yml
--rw-r--r--   0        0        0    18712 2020-02-02 00:00:00.000000 clophfit-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.9.0/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.9.0/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.9.0/.github/dependabot.yml
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 clophfit-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.9.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/click.rst
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/conf.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/_static/csvtable.png
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/_static/file.png
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/_static/note_file.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/api/api.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/api/binding.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/api/prenspire.rst
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/api/prtecan.rst
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/contributing.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/description.rst
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/development.rst
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/older.rst
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/prenspire.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/prenspire.uml.rst
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/prtecan.rst
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/prtecan.uml.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/references/references.rst
--rw-r--r--   0        0        0  1428160 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/LMfit.ipynb
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/oldscripts.org
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/oldscripts.rst
--rw-r--r--   0        0        0   966128 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/prenspire.ipynb
--rw-r--r--   0        0        0  1137030 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 clophfit-0.9.0/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/__init__.py
--rw-r--r--   0        0        0    17122 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/py.typed
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/types.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/binding/fitting.py
--rw-r--r--   0        0        0    12140 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/binding/plotting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/__init__.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/prenspire/__init__.py
--rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/prenspire/prenspire.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    52882 2020-02-02 00:00:00.000000 clophfit-0.9.0/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/test_binding.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/test_oldscripts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/test_prenspire.py
--rw-r--r--   0        0        0    29864 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/test_prtecan.py
--rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/24well_clop0_95.csv
--rw-r--r--   0        0        0   679291 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/G10.csv
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/NTT-G10_note.csv
--rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/e2-T-without_sample_column.csv
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota-Err
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota-Err.csv
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota.csv
--rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/h148g-spettroC.csv
--rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/cli/NTT_37C_pKa.csv
--rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
--rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
--rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
--rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv
--rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
--rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
--rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
--rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
--rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/H04.dat
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0   530592 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/tmp/A04 Cl.csv
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 clophfit-0.9.0/tests/data/tmp/NTT-A04-Cl_note.csv
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 clophfit-0.9.0/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 clophfit-0.9.0/README.md
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 clophfit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 clophfit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.9.1/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.9.1/.darglint
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 clophfit-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 clophfit-0.9.1/.python-version
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 clophfit-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0    18850 2020-02-02 00:00:00.000000 clophfit-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.9.1/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.9.1/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 clophfit-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.9.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/click.rst
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/_static/csvtable.png
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/_static/file.png
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/_static/note_file.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/api/api.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/api/binding.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/api/prenspire.rst
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/api/prtecan.rst
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/contributing.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/description.rst
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/development.rst
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/older.rst
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/prenspire.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/prenspire.uml.rst
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/prtecan.rst
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/prtecan.uml.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/references/references.rst
+-rw-r--r--   0        0        0  1428160 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/LMfit.ipynb
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/oldscripts.org
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/oldscripts.rst
+-rw-r--r--   0        0        0   966128 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/prenspire.ipynb
+-rw-r--r--   0        0        0  1137030 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 clophfit-0.9.1/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/__init__.py
+-rw-r--r--   0        0        0    17122 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/py.typed
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/types.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/binding/fitting.py
+-rw-r--r--   0        0        0    12140 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/binding/plotting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/__init__.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/prenspire/__init__.py
+-rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/prenspire/prenspire.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    53047 2020-02-02 00:00:00.000000 clophfit-0.9.1/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/test_binding.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/test_cli.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/test_oldscripts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/test_prenspire.py
+-rw-r--r--   0        0        0    29864 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/test_prtecan.py
+-rw-r--r--   0        0        0    34305 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/24well_clop0_95.csv
+-rw-r--r--   0        0        0   679291 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/G10.csv
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/NTT-G10_note.csv
+-rw-r--r--   0        0        0   103231 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/e2-T-without_sample_column.csv
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota-Err
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota-Err.csv
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota.csv
+-rw-r--r--   0        0        0   373790 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/h148g-spettroC.csv
+-rw-r--r--   0        0        0    98464 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/cli/NTT_37C_pKa.csv
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv
+-rw-r--r--   0        0        0    68449 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv
+-rw-r--r--   0        0        0    53309 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv
+-rw-r--r--   0        0        0   103682 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv
+-rw-r--r--   0        0        0   104940 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv
+-rw-r--r--   0        0        0   104939 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv
+-rw-r--r--   0        0        0   344763 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv
+-rw-r--r--   0        0        0   373857 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv
+-rw-r--r--   0        0        0   344941 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/H04.dat
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0   530592 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/tmp/A04 Cl.csv
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 clophfit-0.9.1/tests/data/tmp/NTT-A04-Cl_note.csv
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 clophfit-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 clophfit-0.9.1/README.md
+-rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 clophfit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 clophfit-0.9.1/PKG-INFO
```

### Comparing `clophfit-0.9.0/.pre-commit-config.yaml` & `clophfit-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/CHANGELOG.md` & `clophfit-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.9.1 (2023-07-15)
+
+### Docs
+
+- Fix zenodo badge to auto-update
+
+### Refactor
+
+- Remove silencer noqa for merge_md and norm metadata
+
 ## v0.9.0 (2023-07-15)
 
 ### Feat
 
 - Change tecan and enspire as subcommands of `ppr`
 - pr.tecan exports png for each well
 - **prtecan**: new fit; sort results; add export_png
```

### Comparing `clophfit-0.9.0/cz_customize_info.txt` & `clophfit-0.9.1/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/.github/workflows/ci.yml` & `clophfit-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/.github/workflows/docs.yml` & `clophfit-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/Makefile` & `clophfit-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/conf.py` & `clophfit-0.9.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2023, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
-release = "0.9.0"
+release = "0.9.1"
 html_title = "ClopHfit"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `clophfit-0.9.0/docs/index.rst` & `clophfit-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/make.bat` & `clophfit-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/_static/csvtable.png` & `clophfit-0.9.1/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/_static/file.png` & `clophfit-0.9.1/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/_static/note_file.png` & `clophfit-0.9.1/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/contributing.rst` & `clophfit-0.9.1/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/development.rst` & `clophfit-0.9.1/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/older.rst` & `clophfit-0.9.1/docs/references/older.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/prenspire.uml.rst` & `clophfit-0.9.1/docs/references/prenspire.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/prtecan.rst` & `clophfit-0.9.1/docs/references/prtecan.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/references/prtecan.uml.rst` & `clophfit-0.9.1/docs/references/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/tutorials/LMfit.ipynb` & `clophfit-0.9.1/docs/tutorials/LMfit.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/tutorials/oldscripts.org` & `clophfit-0.9.1/docs/tutorials/oldscripts.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/tutorials/oldscripts.rst` & `clophfit-0.9.1/docs/tutorials/oldscripts.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/tutorials/prenspire.ipynb` & `clophfit-0.9.1/docs/tutorials/prenspire.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/docs/tutorials/prtecan.ipynb` & `clophfit-0.9.1/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/__main__.py` & `clophfit-0.9.1/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/binding/fitting.py` & `clophfit-0.9.1/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/binding/plotting.py` & `clophfit-0.9.1/src/clophfit/binding/plotting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/dil_buffer.py` & `clophfit-0.9.1/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/dil_correction.py` & `clophfit-0.9.1/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/fit_titration.py` & `clophfit-0.9.1/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/fit_titration_global.py` & `clophfit-0.9.1/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/merge.py` & `clophfit-0.9.1/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/plot_tecan.py` & `clophfit-0.9.1/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.9.1/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/prenspire/prenspire.py` & `clophfit-0.9.1/src/clophfit/prenspire/prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/prtecan/__init__.py` & `clophfit-0.9.1/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/src/clophfit/prtecan/prtecan.py` & `clophfit-0.9.1/src/clophfit/prtecan/prtecan.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,18 +206,26 @@
 
     return md
 
 
 def merge_md(mds: list[dict[str, Metadata]]) -> dict[str, Metadata]:
     """Merge a list of metadata dict if the key value is the same in the list."""
     mmd = {k: v for k, v in mds[0].items() if all(v == md[k] for md in mds[1:])}
+
     # To account for the case 93"Optimal" and 93"Manual" in lb metadata
-    if mmd.get("Gain") is None and mds[0].get("Gain") is not None:  # noqa: SIM102
-        if all(mds[0]["Gain"].value == md["Gain"].value for md in mds[1:]):
-            mmd["Gain"] = Metadata(mds[0]["Gain"].value)
+    def all_same_gain(mds: list[dict[str, Metadata]]) -> bool:
+        return all(md["Gain"].value == mds[0]["Gain"].value for md in mds[1:])
+
+    if (
+        mmd.get("Gain") is None
+        and mds[0].get("Gain") is not None
+        and all_same_gain(mds)
+    ):
+        mmd["Gain"] = Metadata(mds[0]["Gain"].value)
+
     return mmd
 
 
 def calculate_conc(
     additions: Sequence[float], conc_stock: float, conc_ini: float = 0.0
 ) -> ArrayF:
     """Calculate concentration values.
@@ -454,15 +462,17 @@
     @property
     def data_norm(self) -> dict[str, float]:
         """Normalize data by number of flashes, integration time and gain."""
         if self._data_norm is None:
             try:
                 norm = 1000.0
                 for k in Labelblock._NORM_KEYS:
-                    norm /= self.metadata[k].value  # type: ignore # FIXME: D
+                    val = self.metadata[k].value
+                    if isinstance(val, (float, int)):
+                        norm /= val
             except TypeError:
                 warnings.warn(
                     "Could not normalize for non numerical Gain, Number of Flashes or Integration time.",
                     stacklevel=2,
                 )  # pragma: no cover
             self._data_norm = {k: v * norm for k, v in self.data.items()}
         return self._data_norm
```

### Comparing `clophfit-0.9.0/tests/test_binding.py` & `clophfit-0.9.1/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/test_cli.py` & `clophfit-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/test_oldscripts.py` & `clophfit-0.9.1/tests/test_oldscripts.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/test_prenspire.py` & `clophfit-0.9.1/tests/test_prenspire.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/test_prtecan.py` & `clophfit-0.9.1/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/24well_clop0_95.csv` & `clophfit-0.9.1/tests/EnSpire/24well_clop0_95.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/G10.csv` & `clophfit-0.9.1/tests/EnSpire/G10.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/NTT-G10_note.csv` & `clophfit-0.9.1/tests/EnSpire/NTT-G10_note.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/e2-T-without_sample_column.csv` & `clophfit-0.9.1/tests/EnSpire/e2-T-without_sample_column.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota` & `clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota-Err` & `clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota-Err`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota-Err.csv` & `clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota-Err.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/h148g-spettroC-nota.csv` & `clophfit-0.9.1/tests/EnSpire/h148g-spettroC-nota.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/h148g-spettroC.csv` & `clophfit-0.9.1/tests/EnSpire/h148g-spettroC.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/cli/NTT_37C_pKa.csv` & `clophfit-0.9.1/tests/EnSpire/cli/NTT_37C_pKa.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv` & `clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_A.png` & `clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv` & `clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/cli/output/NTT_37C_pKa_B.png` & `clophfit-0.9.1/tests/EnSpire/cli/output/NTT_37C_pKa_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_11columns.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_fin.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/M1-A6-G12_missing_emptyline_ini.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-emwavelength.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-emwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelength.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelength.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelength2.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelength2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/e2dan-exwavelengthstrange.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/h148g-spettroC-idx0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv` & `clophfit-0.9.1/tests/EnSpire/exceptions/h148g-spettroC-idx2.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv` & `clophfit-0.9.1/tests/EnSpire/warnings/h148g-spettroC-incomplete.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_100.xls` & `clophfit-0.9.1/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_150.xls` & `clophfit-0.9.1/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_20.xls` & `clophfit-0.9.1/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_5.78.xls` & `clophfit-0.9.1/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_50.xls` & `clophfit-0.9.1/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_6.38.xls` & `clophfit-0.9.1/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_6.83.xls` & `clophfit-0.9.1/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_7.24.xls` & `clophfit-0.9.1/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_7.67.xls` & `clophfit-0.9.1/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_8.23.xls` & `clophfit-0.9.1/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_8.82.xls` & `clophfit-0.9.1/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290212_9.31.xls` & `clophfit-0.9.1/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290513_5.5.xls` & `clophfit-0.9.1/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.9.1/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290513_7.2.xls` & `clophfit-0.9.1/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/290513_8.8.xls` & `clophfit-0.9.1/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.9.1/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.9.1/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/fit0.csv` & `clophfit-0.9.1/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.9.1/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/fit1.csv` & `clophfit-0.9.1/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.9.1/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.9.1/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.9.1/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.9.1/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.9.1/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/A01-20140311a.dat` & `clophfit-0.9.1/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/A01.dat` & `clophfit-0.9.1/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/NTT-A04-Cl_note` & `clophfit-0.9.1/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.9.1/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/k/D05.dat-bs.png` & `clophfit-0.9.1/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/k/D05.dat.png` & `clophfit-0.9.1/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.9.1/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.9.1/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.9.1/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.9.1/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.9.1/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.9.1/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/tmp/A04 Cl.csv` & `clophfit-0.9.1/tests/data/tmp/A04 Cl.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/tests/data/tmp/NTT-A04-Cl_note.csv` & `clophfit-0.9.1/tests/data/tmp/NTT-A04-Cl_note.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/.gitignore` & `clophfit-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/LICENSE.txt` & `clophfit-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.9.0/README.md` & `clophfit-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ClopHfit
 
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8108468.svg)](https://doi.org/10.5281/zenodo.8108468)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6354111.svg)](https://doi.org/10.5281/zenodo.6354111)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.9.0"
+- Version: "0.9.1"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
 using `pip`:
 
     pip install clophfit
```

### Comparing `clophfit-0.9.0/pyproject.toml` & `clophfit-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "README.md"
 requires-python = ">=3.9, <3.12"
-version = "0.9.0"
+version = "0.9.1"
 
 [project.optional-dependencies]
 dev = [
   "commitizen < 3.5.3",
   "ipykernel",
   "jupyter",
   "jupyterlab",
@@ -111,15 +111,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.9.0"
+version = "0.9.1"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
@@ -253,15 +253,14 @@
 
 [tool.hatch.envs.typeguard]
 features = ["tests"]
 python = "3.11"
 template = "typeguard"
 
 [tool.hatch.envs.typeguard.scripts]
-# guard = "pytest", f"--typeguard-packages={package} {args}" see also {env:}  # XXX:
 run = "pytest --typeguard-packages=clophfit {args}"
 
 [tool.isort]
 combine_as_imports = true
 force_single_line = false
 include_trailing_comma = true
 known_first_party = "clophfit"
```

### Comparing `clophfit-0.9.0/PKG-INFO` & `clophfit-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://github.com/darosio/ClopHfit/blob/main/CHANGELOG.md
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -66,21 +66,21 @@
 
 # ClopHfit
 
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8108468.svg)](https://doi.org/10.5281/zenodo.8108468)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6354111.svg)](https://doi.org/10.5281/zenodo.6354111)
 
 This package provides a command line interface for fitting pH titration or
 binding assay data for macromolecules, such as fluorescence spectra. With this
 tool, users can easily analyze their data and obtain accurate fitting results.
 
-- Version: "0.9.0"
+- Version: "0.9.1"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/ClopHfit/)
 using `pip`:
 
     pip install clophfit
```

