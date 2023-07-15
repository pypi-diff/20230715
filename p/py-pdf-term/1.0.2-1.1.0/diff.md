# Comparing `tmp/py_pdf_term-1.0.2.tar.gz` & `tmp/py_pdf_term-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pdf_term-1.0.2.tar", max compression
+gzip compressed data, was "py_pdf_term-1.1.0.tar", max compression
```

## Comparing `py_pdf_term-1.0.2.tar` & `py_pdf_term-1.1.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py_pdf_term-1.0.2/LICENSE
--rw-r--r--   0        0        0      558 2023-04-22 03:34:12.853470 py_pdf_term-1.0.2/README.md
--rw-r--r--   0        0        0      325 2023-05-28 07:03:53.593903 py_pdf_term-1.0.2/py_pdf_term/__init__.py
--rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py_pdf_term-1.0.2/py_pdf_term/_common/__init__.py
--rw-r--r--   0        0        0     2445 2023-04-30 07:57:40.302941 py_pdf_term-1.0.2/py_pdf_term/_common/consts.py
--rw-r--r--   0        0        0      371 2023-05-28 06:39:10.015087 py_pdf_term-1.0.2/py_pdf_term/_common/data.py
--rw-r--r--   0        0        0      279 2023-05-07 09:38:40.928433 py_pdf_term-1.0.2/py_pdf_term/_common/utils.py
--rw-r--r--   0        0        0       89 2023-04-23 12:35:30.854867 py_pdf_term-1.0.2/py_pdf_term/analysis/__init__.py
--rw-r--r--   0        0        0      442 2023-05-21 10:48:35.970334 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/__init__.py
--rw-r--r--   0        0        0      168 2023-05-21 10:48:35.871081 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/__init__.py
--rw-r--r--   0        0        0     4013 2023-05-28 06:39:10.015976 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/lr.py
--rw-r--r--   0        0        0      151 2023-05-21 10:48:35.871055 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
--rw-r--r--   0        0        0     3159 2023-05-28 06:39:10.017254 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/container.py
--rw-r--r--   0        0        0      146 2023-05-21 10:48:35.888277 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/__init__.py
--rw-r--r--   0        0        0     3653 2023-05-28 06:39:10.017958 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/term.py
--rw-r--r--   0        0        0     2210 2023-05-07 09:38:40.931460 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/runner.py
--rw-r--r--   0        0        0       92 2023-04-23 12:35:30.855657 py_pdf_term-1.0.2/py_pdf_term/candidates/__init__.py
--rw-r--r--   0        0        0      287 2023-05-21 10:48:35.963075 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/__init__.py
--rw-r--r--   0        0        0      315 2023-05-21 10:48:35.923659 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/__init__.py
--rw-r--r--   0        0        0      965 2023-05-28 06:39:10.018630 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/base.py
--rw-r--r--   0        0        0     1405 2023-05-28 06:39:10.019389 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/combiner.py
--rw-r--r--   0        0        0     3479 2023-05-28 06:39:10.019839 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/separation.py
--rw-r--r--   0        0        0      315 2023-05-21 10:48:35.928200 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/__init__.py
--rw-r--r--   0        0        0     3433 2023-05-28 06:39:10.020224 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/base.py
--rw-r--r--   0        0        0      583 2023-05-28 06:39:10.020907 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/english.py
--rw-r--r--   0        0        0      620 2023-05-28 06:39:10.021358 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/japanese.py
--rw-r--r--   0        0        0     1370 2023-05-28 06:39:10.022872 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/marker.py
--rw-r--r--   0        0        0     4462 2023-05-28 06:39:10.024023 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/data.py
--rw-r--r--   0        0        0     8744 2023-05-28 06:39:10.024603 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/extractor.py
--rw-r--r--   0        0        0      985 2023-05-21 10:48:35.957866 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/__init__.py
--rw-r--r--   0        0        0     3368 2023-05-28 06:39:10.025867 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/combiner.py
--rw-r--r--   0        0        0      816 2023-05-21 10:48:35.959032 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/__init__.py
--rw-r--r--   0        0        0     1840 2023-05-28 06:39:10.026666 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/base.py
--rw-r--r--   0        0        0      192 2023-05-21 10:48:36.026802 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
--rw-r--r--   0        0        0     3747 2023-05-28 06:39:10.027407 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
--rw-r--r--   0        0        0     5444 2023-05-28 06:39:10.027800 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
--rw-r--r--   0        0        0      168 2023-05-21 10:48:35.977851 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
--rw-r--r--   0        0        0      761 2023-05-28 06:39:10.028185 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
--rw-r--r--   0        0        0     1140 2023-05-28 06:39:10.028662 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
--rw-r--r--   0        0        0      180 2023-05-21 10:48:35.985218 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
--rw-r--r--   0        0        0      353 2023-05-28 06:39:10.029476 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
--rw-r--r--   0        0        0     1051 2023-05-28 06:39:10.030704 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
--rw-r--r--   0        0        0      180 2023-05-21 10:48:35.994920 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
--rw-r--r--   0        0        0     2252 2023-05-28 06:39:10.031302 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
--rw-r--r--   0        0        0     2355 2023-05-28 06:39:10.031818 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
--rw-r--r--   0        0        0      231 2023-05-21 10:48:36.028806 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/__init__.py
--rw-r--r--   0        0        0     1222 2023-05-28 06:39:10.032322 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/base.py
--rw-r--r--   0        0        0     2006 2023-05-28 06:39:10.032986 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/english.py
--rw-r--r--   0        0        0     2899 2023-05-28 06:39:10.033582 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/japanese.py
--rw-r--r--   0        0        0      254 2023-05-21 10:48:36.025521 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-28 06:39:10.034019 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/base.py
--rw-r--r--   0        0        0     1189 2023-05-28 06:39:10.034514 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/combiner.py
--rw-r--r--   0        0        0     2964 2023-05-28 06:39:10.034987 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/repeat.py
--rw-r--r--   0        0        0     1434 2023-05-28 06:39:10.035785 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/symname.py
--rw-r--r--   0        0        0     1693 2023-05-28 06:39:10.036377 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/utils.py
--rw-r--r--   0        0        0      115 2023-04-23 12:35:30.856299 py_pdf_term-1.0.2/py_pdf_term/candidates/augmenters.py
--rw-r--r--   0        0        0      117 2023-04-23 12:35:30.857009 py_pdf_term-1.0.2/py_pdf_term/candidates/classifiers.py
--rw-r--r--   0        0        0      109 2023-04-23 12:35:30.858941 py_pdf_term-1.0.2/py_pdf_term/candidates/filters.py
--rw-r--r--   0        0        0      113 2023-04-23 12:35:30.859936 py_pdf_term-1.0.2/py_pdf_term/candidates/splitters.py
--rw-r--r--   0        0        0      430 2023-05-21 10:48:36.041965 py_pdf_term-1.0.2/py_pdf_term/configs.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.860623 py_pdf_term-1.0.2/py_pdf_term/endtoend/__init__.py
--rw-r--r--   0        0        0      333 2023-05-21 10:48:36.055901 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/__init__.py
--rw-r--r--   0        0        0     1024 2023-05-21 10:48:36.093130 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/__init__.py
--rw-r--r--   0        0        0      254 2023-05-21 10:48:36.054361 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
--rw-r--r--   0        0        0     2176 2023-05-28 06:39:10.036961 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
--rw-r--r--   0        0        0     2351 2023-05-28 06:39:10.037466 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
--rw-r--r--   0        0        0      754 2023-05-28 06:39:10.038609 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
--rw-r--r--   0        0        0      184 2023-04-30 03:53:53.377462 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/consts.py
--rw-r--r--   0        0        0      448 2023-05-21 10:48:36.076321 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
--rw-r--r--   0        0        0     5886 2023-05-28 06:39:10.039426 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/base.py
--rw-r--r--   0        0        0     4853 2023-05-28 06:39:10.040018 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/file.py
--rw-r--r--   0        0        0     1742 2023-05-28 06:39:10.040618 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
--rw-r--r--   0        0        0      227 2023-05-21 10:48:36.069449 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
--rw-r--r--   0        0        0     2153 2023-05-28 06:39:10.041172 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
--rw-r--r--   0        0        0     2340 2023-05-28 06:39:10.041835 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
--rw-r--r--   0        0        0      736 2023-05-28 06:39:10.042586 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
--rw-r--r--   0        0        0      678 2023-05-28 06:39:10.043501 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/util.py
--rw-r--r--   0        0        0      203 2023-05-21 10:48:36.064385 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
--rw-r--r--   0        0        0     2043 2023-05-28 06:39:10.045020 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
--rw-r--r--   0        0        0     2299 2023-05-28 06:39:10.045547 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
--rw-r--r--   0        0        0      655 2023-05-28 06:39:10.046204 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
--rw-r--r--   0        0        0      586 2023-05-21 10:48:36.206572 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/__init__.py
--rw-r--r--   0        0        0      695 2023-05-28 06:39:10.047362 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/base.py
--rw-r--r--   0        0        0     3226 2023-05-28 06:39:10.048833 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/candidate.py
--rw-r--r--   0        0        0     1803 2023-05-28 06:39:10.049262 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/method.py
--rw-r--r--   0        0        0      715 2023-05-28 06:39:10.049650 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/styling.py
--rw-r--r--   0        0        0      748 2023-05-28 06:39:10.050003 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/techterm.py
--rw-r--r--   0        0        0      964 2023-05-28 06:39:10.050616 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/xml.py
--rw-r--r--   0        0        0      611 2023-05-28 06:39:10.051234 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/data.py
--rw-r--r--   0        0        0    17896 2023-05-28 06:39:10.053349 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/extractor.py
--rw-r--r--   0        0        0      480 2023-05-21 10:48:36.091002 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/__init__.py
--rw-r--r--   0        0        0     6065 2023-05-28 06:39:10.053907 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/candidate.py
--rw-r--r--   0        0        0     9692 2023-05-28 06:39:10.054462 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/method.py
--rw-r--r--   0        0        0     2778 2023-05-28 06:39:10.054879 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/styling.py
--rw-r--r--   0        0        0     5323 2023-05-28 06:39:10.055258 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/techterm.py
--rw-r--r--   0        0        0     2646 2023-05-28 06:39:10.055631 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/xml.py
--rw-r--r--   0        0        0     1077 2023-05-21 10:48:36.178877 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-28 06:39:10.056042 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/base.py
--rw-r--r--   0        0        0      407 2023-05-21 10:48:36.215373 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
--rw-r--r--   0        0        0      660 2023-05-28 06:39:10.057414 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
--rw-r--r--   0        0        0     1382 2023-05-28 06:39:10.057887 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
--rw-r--r--   0        0        0      625 2023-05-28 06:39:10.059023 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
--rw-r--r--   0        0        0      589 2023-05-28 06:39:10.059813 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
--rw-r--r--   0        0        0      446 2023-05-21 10:48:36.239199 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
--rw-r--r--   0        0        0      747 2023-05-28 06:39:10.061164 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
--rw-r--r--   0        0        0      756 2023-05-28 06:39:10.062123 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
--rw-r--r--   0        0        0     1698 2023-05-28 06:39:10.063009 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
--rw-r--r--   0        0        0      715 2023-05-28 06:39:10.065667 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
--rw-r--r--   0        0        0      617 2023-05-28 06:39:10.066128 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
--rw-r--r--   0        0        0      204 2023-05-21 10:48:36.187774 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
--rw-r--r--   0        0        0      683 2023-05-28 06:39:10.066509 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
--rw-r--r--   0        0        0      767 2023-05-28 06:39:10.066879 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
--rw-r--r--   0        0        0       97 2023-05-21 10:48:36.192351 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
--rw-r--r--   0        0        0      627 2023-05-28 06:39:10.068665 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py
--rw-r--r--   0        0        0       93 2023-05-21 10:48:36.200466 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
--rw-r--r--   0        0        0      653 2023-05-28 06:39:10.069219 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
--rw-r--r--   0        0        0      102 2023-04-23 12:35:30.862807 py_pdf_term-1.0.2/py_pdf_term/endtoend/caches.py
--rw-r--r--   0        0        0      976 2023-05-21 10:48:36.271106 py_pdf_term-1.0.2/py_pdf_term/mappers.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.863506 py_pdf_term-1.0.2/py_pdf_term/methods/__init__.py
--rw-r--r--   0        0        0      536 2023-05-21 10:48:36.254137 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/__init__.py
--rw-r--r--   0        0        0     8473 2023-05-28 06:39:10.069816 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/base.py
--rw-r--r--   0        0        0      567 2023-05-21 10:48:36.245483 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/__init__.py
--rw-r--r--   0        0        0      981 2023-05-28 06:39:10.070484 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/base.py
--rw-r--r--   0        0        0      998 2023-05-28 06:39:10.070879 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flr.py
--rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.071286 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flrh.py
--rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.072142 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/hits.py
--rw-r--r--   0        0        0     1008 2023-05-28 06:39:10.072766 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mcvalue.py
--rw-r--r--   0        0        0      738 2023-05-28 06:39:10.073246 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mdp.py
--rw-r--r--   0        0        0      891 2023-05-28 06:39:10.073711 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/tfidf.py
--rw-r--r--   0        0        0      924 2023-05-28 06:39:10.074373 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/data.py
--rw-r--r--   0        0        0      583 2023-05-28 06:39:10.074916 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flr.py
--rw-r--r--   0        0        0      939 2023-05-28 06:39:10.075329 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flrh.py
--rw-r--r--   0        0        0     1170 2023-05-28 06:39:10.075719 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/hits.py
--rw-r--r--   0        0        0      624 2023-05-28 06:39:10.076208 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mcvalue.py
--rw-r--r--   0        0        0      581 2023-05-28 06:39:10.076805 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mdp.py
--rw-r--r--   0        0        0      447 2023-05-21 10:48:36.254929 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/__init__.py
--rw-r--r--   0        0        0     2087 2023-05-28 06:39:10.077795 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/base.py
--rw-r--r--   0        0        0     2027 2023-05-28 06:39:10.078289 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flr.py
--rw-r--r--   0        0        0     2847 2023-05-28 06:39:10.079027 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flrh.py
--rw-r--r--   0        0        0     6308 2023-05-28 06:39:10.080583 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/hits.py
--rw-r--r--   0        0        0     1966 2023-05-28 06:39:10.081142 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mcvalue.py
--rw-r--r--   0        0        0     3145 2023-05-28 06:39:10.081601 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mdp.py
--rw-r--r--   0        0        0     1983 2023-05-28 06:39:10.083388 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/tfidf.py
--rw-r--r--   0        0        0      473 2023-05-21 10:48:36.275731 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/__init__.py
--rw-r--r--   0        0        0      555 2023-05-28 06:39:10.083958 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/base.py
--rw-r--r--   0        0        0      946 2023-05-28 06:39:10.084499 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flr.py
--rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085207 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flrh.py
--rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085888 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/hits.py
--rw-r--r--   0        0        0     1429 2023-05-28 06:39:10.086461 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
--rw-r--r--   0        0        0     1182 2023-05-28 07:03:53.594747 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mdp.py
--rw-r--r--   0        0        0      836 2023-05-28 06:39:10.087863 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/tfidf.py
--rw-r--r--   0        0        0      602 2023-05-28 06:39:10.088395 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/tfidf.py
--rw-r--r--   0        0        0      110 2023-04-23 12:35:30.865641 py_pdf_term-1.0.2/py_pdf_term/methods/collectors.py
--rw-r--r--   0        0        0      104 2023-04-23 12:35:30.866294 py_pdf_term-1.0.2/py_pdf_term/methods/rankers.py
--rw-r--r--   0        0        0      112 2023-04-23 12:35:30.866995 py_pdf_term-1.0.2/py_pdf_term/methods/rankingdata.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.867710 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/__init__.py
--rw-r--r--   0        0        0      174 2023-05-21 10:48:36.260616 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
--rw-r--r--   0        0        0      155 2023-05-21 10:48:36.285807 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/__init__.py
--rw-r--r--   0        0        0      573 2023-05-28 06:39:10.089345 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py
--rw-r--r--   0        0        0      367 2023-05-28 06:39:10.089829 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/standard.py
--rw-r--r--   0        0        0     4054 2023-05-28 06:39:10.090619 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/converter.py
--rw-r--r--   0        0        0     1415 2023-05-28 06:39:10.091183 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/data.py
--rw-r--r--   0        0        0     5980 2023-05-28 06:39:10.092194 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/textful.py
--rw-r--r--   0        0        0      824 2023-05-28 06:39:10.093197 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/utils.py
--rw-r--r--   0        0        0      111 2023-04-30 07:57:40.332098 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/binopeners.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.870578 py_pdf_term-1.0.2/py_pdf_term/stylings/__init__.py
--rw-r--r--   0        0        0      260 2023-05-21 10:48:36.286348 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/__init__.py
--rw-r--r--   0        0        0     2475 2023-05-28 06:39:10.094712 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/data.py
--rw-r--r--   0        0        0     3418 2023-05-28 06:39:10.095399 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scorer.py
--rw-r--r--   0        0        0      185 2023-05-21 10:48:36.278288 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/__init__.py
--rw-r--r--   0        0        0     1213 2023-05-28 06:39:10.096359 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/base.py
--rw-r--r--   0        0        0     1185 2023-05-28 06:39:10.096968 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/color.py
--rw-r--r--   0        0        0     1510 2023-05-28 06:39:10.097427 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/fontsize.py
--rw-r--r--   0        0        0      102 2023-04-23 12:35:30.871198 py_pdf_term-1.0.2/py_pdf_term/stylings/scores.py
--rw-r--r--   0        0        0       91 2023-04-23 12:35:30.872290 py_pdf_term-1.0.2/py_pdf_term/techterms/__init__.py
--rw-r--r--   0        0        0      287 2023-05-21 10:48:36.292986 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/__init__.py
--rw-r--r--   0        0        0     2403 2023-05-28 06:39:10.098467 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/data.py
--rw-r--r--   0        0        0     6067 2023-05-28 06:39:10.099038 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/extractor.py
--rw-r--r--   0        0        0      450 2023-05-28 06:39:10.099699 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/utils.py
--rw-r--r--   0        0        0       92 2023-04-30 07:57:40.332522 py_pdf_term-1.0.2/py_pdf_term/tokenizers/__init__.py
--rw-r--r--   0        0        0      337 2023-05-21 10:48:36.294274 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/__init__.py
--rw-r--r--   0        0        0     1482 2023-05-28 06:39:10.101451 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/base.py
--rw-r--r--   0        0        0     2533 2023-05-28 06:39:10.102033 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/data.py
--rw-r--r--   0        0        0     1417 2023-05-28 06:39:10.102730 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/english.py
--rw-r--r--   0        0        0     2864 2023-05-28 06:39:10.103262 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/japanese.py
--rw-r--r--   0        0        0     1350 2023-05-28 06:39:10.103860 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/tokenizer.py
--rw-r--r--   0        0        0     1185 2023-05-28 07:03:53.595227 py_pdf_term-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_pdf_term-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py_pdf_term-1.1.0/LICENSE
+-rw-r--r--   0        0        0      558 2023-07-15 03:22:17.553848 py_pdf_term-1.1.0/README.md
+-rw-r--r--   0        0        0      325 2023-07-15 03:22:17.561159 py_pdf_term-1.1.0/py_pdf_term/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py_pdf_term-1.1.0/py_pdf_term/_common/__init__.py
+-rw-r--r--   0        0        0     2445 2023-04-30 07:57:40.302941 py_pdf_term-1.1.0/py_pdf_term/_common/consts.py
+-rw-r--r--   0        0        0      371 2023-05-28 06:39:10.015087 py_pdf_term-1.1.0/py_pdf_term/_common/data.py
+-rw-r--r--   0        0        0      279 2023-05-07 09:38:40.928433 py_pdf_term-1.1.0/py_pdf_term/_common/utils.py
+-rw-r--r--   0        0        0       89 2023-04-23 12:35:30.854867 py_pdf_term-1.1.0/py_pdf_term/analysis/__init__.py
+-rw-r--r--   0        0        0      442 2023-05-21 10:48:35.970334 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.871081 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/concats/__init__.py
+-rw-r--r--   0        0        0     4013 2023-05-28 06:39:10.015976 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/concats/lr.py
+-rw-r--r--   0        0        0      151 2023-05-21 10:48:35.871055 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
+-rw-r--r--   0        0        0     3159 2023-05-28 06:39:10.017254 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py
+-rw-r--r--   0        0        0      146 2023-05-21 10:48:35.888277 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/occurrences/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-28 06:39:10.017958 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/occurrences/term.py
+-rw-r--r--   0        0        0     2210 2023-05-07 09:38:40.931460 py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/runner.py
+-rw-r--r--   0        0        0       92 2023-04-23 12:35:30.855657 py_pdf_term-1.1.0/py_pdf_term/candidates/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:35.963075 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.923659 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/__init__.py
+-rw-r--r--   0        0        0      965 2023-05-28 06:39:10.018630 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/base.py
+-rw-r--r--   0        0        0     1405 2023-05-28 06:39:10.019389 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/combiner.py
+-rw-r--r--   0        0        0     3479 2023-05-28 06:39:10.019839 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/separation.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.928200 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/__init__.py
+-rw-r--r--   0        0        0     3433 2023-05-28 06:39:10.020224 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/base.py
+-rw-r--r--   0        0        0      583 2023-05-28 06:39:10.020907 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/english.py
+-rw-r--r--   0        0        0      620 2023-05-28 06:39:10.021358 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py
+-rw-r--r--   0        0        0     1370 2023-05-28 06:39:10.022872 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/marker.py
+-rw-r--r--   0        0        0     4462 2023-05-28 06:39:10.024023 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/data.py
+-rw-r--r--   0        0        0     8744 2023-05-28 06:39:10.024603 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/extractor.py
+-rw-r--r--   0        0        0      985 2023-05-21 10:48:35.957866 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-28 06:39:10.025867 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/combiner.py
+-rw-r--r--   0        0        0      816 2023-05-21 10:48:35.959032 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-28 06:39:10.026666 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/base.py
+-rw-r--r--   0        0        0      192 2023-05-21 10:48:36.026802 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
+-rw-r--r--   0        0        0     3747 2023-05-28 06:39:10.027407 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
+-rw-r--r--   0        0        0     5444 2023-05-28 06:39:10.027800 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.977851 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-28 06:39:10.028185 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
+-rw-r--r--   0        0        0     1140 2023-05-28 06:39:10.028662 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.985218 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
+-rw-r--r--   0        0        0      353 2023-05-28 06:39:10.029476 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
+-rw-r--r--   0        0        0     1051 2023-05-28 06:39:10.030704 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.994920 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
+-rw-r--r--   0        0        0     2252 2023-05-28 06:39:10.031302 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
+-rw-r--r--   0        0        0     2355 2023-05-28 06:39:10.031818 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
+-rw-r--r--   0        0        0      231 2023-05-21 10:48:36.028806 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-28 06:39:10.032322 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/base.py
+-rw-r--r--   0        0        0     2006 2023-05-28 06:39:10.032986 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/english.py
+-rw-r--r--   0        0        0     2899 2023-05-28 06:39:10.033582 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.025521 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-28 06:39:10.034019 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/base.py
+-rw-r--r--   0        0        0     1189 2023-05-28 06:39:10.034514 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/combiner.py
+-rw-r--r--   0        0        0     2964 2023-05-28 06:39:10.034987 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/repeat.py
+-rw-r--r--   0        0        0     1434 2023-05-28 06:39:10.035785 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/symname.py
+-rw-r--r--   0        0        0     1693 2023-05-28 06:39:10.036377 py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/utils.py
+-rw-r--r--   0        0        0      115 2023-04-23 12:35:30.856299 py_pdf_term-1.1.0/py_pdf_term/candidates/augmenters.py
+-rw-r--r--   0        0        0      117 2023-04-23 12:35:30.857009 py_pdf_term-1.1.0/py_pdf_term/candidates/classifiers.py
+-rw-r--r--   0        0        0      109 2023-04-23 12:35:30.858941 py_pdf_term-1.1.0/py_pdf_term/candidates/filters.py
+-rw-r--r--   0        0        0      113 2023-04-23 12:35:30.859936 py_pdf_term-1.1.0/py_pdf_term/candidates/splitters.py
+-rw-r--r--   0        0        0      430 2023-05-21 10:48:36.041965 py_pdf_term-1.1.0/py_pdf_term/configs.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.860623 py_pdf_term-1.1.0/py_pdf_term/endtoend/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-21 10:48:36.055901 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/__init__.py
+-rw-r--r--   0        0        0     1024 2023-05-21 10:48:36.093130 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.054361 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
+-rw-r--r--   0        0        0     2176 2023-05-28 06:39:10.036961 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
+-rw-r--r--   0        0        0     2351 2023-05-28 06:39:10.037466 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
+-rw-r--r--   0        0        0      754 2023-05-28 06:39:10.038609 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
+-rw-r--r--   0        0        0      184 2023-04-30 03:53:53.377462 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/consts.py
+-rw-r--r--   0        0        0      448 2023-05-21 10:48:36.076321 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
+-rw-r--r--   0        0        0     5886 2023-05-28 06:39:10.039426 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/base.py
+-rw-r--r--   0        0        0     4853 2023-05-28 06:39:10.040018 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py
+-rw-r--r--   0        0        0     1742 2023-05-28 06:39:10.040618 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
+-rw-r--r--   0        0        0      227 2023-05-21 10:48:36.069449 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
+-rw-r--r--   0        0        0     2153 2023-05-28 06:39:10.041172 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
+-rw-r--r--   0        0        0     2340 2023-05-28 06:39:10.041835 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
+-rw-r--r--   0        0        0      736 2023-05-28 06:39:10.042586 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
+-rw-r--r--   0        0        0      678 2023-05-28 06:39:10.043501 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/util.py
+-rw-r--r--   0        0        0      203 2023-05-21 10:48:36.064385 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
+-rw-r--r--   0        0        0     2043 2023-05-28 06:39:10.045020 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
+-rw-r--r--   0        0        0     2299 2023-05-28 06:39:10.045547 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
+-rw-r--r--   0        0        0      655 2023-05-28 06:39:10.046204 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
+-rw-r--r--   0        0        0      586 2023-05-21 10:48:36.206572 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-28 06:39:10.047362 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/base.py
+-rw-r--r--   0        0        0     3226 2023-05-28 06:39:10.048833 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/candidate.py
+-rw-r--r--   0        0        0     1803 2023-05-28 06:39:10.049262 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/method.py
+-rw-r--r--   0        0        0      715 2023-05-28 06:39:10.049650 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/styling.py
+-rw-r--r--   0        0        0      748 2023-05-28 06:39:10.050003 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/techterm.py
+-rw-r--r--   0        0        0      964 2023-05-28 06:39:10.050616 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/xml.py
+-rw-r--r--   0        0        0      611 2023-05-28 06:39:10.051234 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/data.py
+-rw-r--r--   0        0        0    17896 2023-05-28 06:39:10.053349 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/extractor.py
+-rw-r--r--   0        0        0      480 2023-05-21 10:48:36.091002 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/__init__.py
+-rw-r--r--   0        0        0     6065 2023-05-28 06:39:10.053907 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py
+-rw-r--r--   0        0        0     9692 2023-05-28 06:39:10.054462 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/method.py
+-rw-r--r--   0        0        0     2778 2023-05-28 06:39:10.054879 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/styling.py
+-rw-r--r--   0        0        0     5323 2023-05-28 06:39:10.055258 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/techterm.py
+-rw-r--r--   0        0        0     2646 2023-05-28 06:39:10.055631 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/xml.py
+-rw-r--r--   0        0        0     1077 2023-05-21 10:48:36.178877 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-28 06:39:10.056042 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/base.py
+-rw-r--r--   0        0        0      407 2023-05-21 10:48:36.215373 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-28 06:39:10.057414 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
+-rw-r--r--   0        0        0     1382 2023-05-28 06:39:10.057887 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
+-rw-r--r--   0        0        0      625 2023-05-28 06:39:10.059023 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
+-rw-r--r--   0        0        0      589 2023-05-28 06:39:10.059813 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
+-rw-r--r--   0        0        0      446 2023-05-21 10:48:36.239199 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-28 06:39:10.061164 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
+-rw-r--r--   0        0        0      756 2023-05-28 06:39:10.062123 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
+-rw-r--r--   0        0        0     1698 2023-05-28 06:39:10.063009 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
+-rw-r--r--   0        0        0      715 2023-05-28 06:39:10.065667 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
+-rw-r--r--   0        0        0      617 2023-05-28 06:39:10.066128 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
+-rw-r--r--   0        0        0      204 2023-05-21 10:48:36.187774 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-28 06:39:10.066509 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
+-rw-r--r--   0        0        0      767 2023-05-28 06:39:10.066879 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
+-rw-r--r--   0        0        0       97 2023-05-21 10:48:36.192351 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-28 06:39:10.068665 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py
+-rw-r--r--   0        0        0       93 2023-05-21 10:48:36.200466 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
+-rw-r--r--   0        0        0      653 2023-05-28 06:39:10.069219 py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.862807 py_pdf_term-1.1.0/py_pdf_term/endtoend/caches.py
+-rw-r--r--   0        0        0      976 2023-05-21 10:48:36.271106 py_pdf_term-1.1.0/py_pdf_term/mappers.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.863506 py_pdf_term-1.1.0/py_pdf_term/methods/__init__.py
+-rw-r--r--   0        0        0      536 2023-05-21 10:48:36.254137 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-28 06:39:10.069816 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/base.py
+-rw-r--r--   0        0        0      567 2023-05-21 10:48:36.245483 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-28 06:39:10.070484 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/base.py
+-rw-r--r--   0        0        0      998 2023-05-28 06:39:10.070879 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/flr.py
+-rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.071286 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/flrh.py
+-rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.072142 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/hits.py
+-rw-r--r--   0        0        0     1008 2023-05-28 06:39:10.072766 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/mcvalue.py
+-rw-r--r--   0        0        0      738 2023-05-28 06:39:10.073246 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/mdp.py
+-rw-r--r--   0        0        0      891 2023-05-28 06:39:10.073711 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/tfidf.py
+-rw-r--r--   0        0        0      924 2023-05-28 06:39:10.074373 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/data.py
+-rw-r--r--   0        0        0      583 2023-05-28 06:39:10.074916 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/flr.py
+-rw-r--r--   0        0        0      939 2023-05-28 06:39:10.075329 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/flrh.py
+-rw-r--r--   0        0        0     1170 2023-05-28 06:39:10.075719 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/hits.py
+-rw-r--r--   0        0        0      624 2023-05-28 06:39:10.076208 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/mcvalue.py
+-rw-r--r--   0        0        0      581 2023-05-28 06:39:10.076805 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/mdp.py
+-rw-r--r--   0        0        0      447 2023-05-21 10:48:36.254929 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-28 06:39:10.077795 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/base.py
+-rw-r--r--   0        0        0     2027 2023-05-28 06:39:10.078289 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/flr.py
+-rw-r--r--   0        0        0     2847 2023-05-28 06:39:10.079027 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/flrh.py
+-rw-r--r--   0        0        0     6308 2023-05-28 06:39:10.080583 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/hits.py
+-rw-r--r--   0        0        0     1966 2023-05-28 06:39:10.081142 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/mcvalue.py
+-rw-r--r--   0        0        0     3145 2023-05-28 06:39:10.081601 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/mdp.py
+-rw-r--r--   0        0        0     1983 2023-05-28 06:39:10.083388 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/tfidf.py
+-rw-r--r--   0        0        0      473 2023-05-21 10:48:36.275731 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/__init__.py
+-rw-r--r--   0        0        0      555 2023-05-28 06:39:10.083958 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/base.py
+-rw-r--r--   0        0        0      946 2023-05-28 06:39:10.084499 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/flr.py
+-rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085207 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/flrh.py
+-rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085888 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/hits.py
+-rw-r--r--   0        0        0     1429 2023-05-28 06:39:10.086461 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
+-rw-r--r--   0        0        0     1182 2023-05-28 07:03:53.594747 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/mdp.py
+-rw-r--r--   0        0        0      836 2023-05-28 06:39:10.087863 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py
+-rw-r--r--   0        0        0      602 2023-05-28 06:39:10.088395 py_pdf_term-1.1.0/py_pdf_term/methods/_methods/tfidf.py
+-rw-r--r--   0        0        0      110 2023-04-23 12:35:30.865641 py_pdf_term-1.1.0/py_pdf_term/methods/collectors.py
+-rw-r--r--   0        0        0      104 2023-04-23 12:35:30.866294 py_pdf_term-1.1.0/py_pdf_term/methods/rankers.py
+-rw-r--r--   0        0        0      112 2023-04-23 12:35:30.866995 py_pdf_term-1.1.0/py_pdf_term/methods/rankingdata.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.867710 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-21 10:48:36.260616 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-21 10:48:36.285807 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/__init__.py
+-rw-r--r--   0        0        0      573 2023-05-28 06:39:10.089345 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py
+-rw-r--r--   0        0        0      367 2023-05-28 06:39:10.089829 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/standard.py
+-rw-r--r--   0        0        0     4054 2023-05-28 06:39:10.090619 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/converter.py
+-rw-r--r--   0        0        0     1415 2023-05-28 06:39:10.091183 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/data.py
+-rw-r--r--   0        0        0     5980 2023-05-28 06:39:10.092194 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py
+-rw-r--r--   0        0        0      824 2023-05-28 06:39:10.093197 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py
+-rw-r--r--   0        0        0      111 2023-04-30 07:57:40.332098 py_pdf_term-1.1.0/py_pdf_term/pdftoxml/binopeners.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.870578 py_pdf_term-1.1.0/py_pdf_term/stylings/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-21 10:48:36.286348 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-28 06:39:10.094712 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/data.py
+-rw-r--r--   0        0        0     3418 2023-05-28 06:39:10.095399 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scorer.py
+-rw-r--r--   0        0        0      185 2023-05-21 10:48:36.278288 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/__init__.py
+-rw-r--r--   0        0        0     1213 2023-05-28 06:39:10.096359 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/base.py
+-rw-r--r--   0        0        0     1185 2023-05-28 06:39:10.096968 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/color.py
+-rw-r--r--   0        0        0     1510 2023-05-28 06:39:10.097427 py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/fontsize.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.871198 py_pdf_term-1.1.0/py_pdf_term/stylings/scores.py
+-rw-r--r--   0        0        0       91 2023-04-23 12:35:30.872290 py_pdf_term-1.1.0/py_pdf_term/techterms/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:36.292986 py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/__init__.py
+-rw-r--r--   0        0        0     2403 2023-05-28 06:39:10.098467 py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/data.py
+-rw-r--r--   0        0        0     6067 2023-05-28 06:39:10.099038 py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/extractor.py
+-rw-r--r--   0        0        0      450 2023-05-28 06:39:10.099699 py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/utils.py
+-rw-r--r--   0        0        0       92 2023-04-30 07:57:40.332522 py_pdf_term-1.1.0/py_pdf_term/tokenizers/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-21 10:48:36.294274 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/__init__.py
+-rw-r--r--   0        0        0     1482 2023-05-28 06:39:10.101451 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/base.py
+-rw-r--r--   0        0        0     2533 2023-05-28 06:39:10.102033 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/data.py
+-rw-r--r--   0        0        0     1417 2023-05-28 06:39:10.102730 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/english.py
+-rw-r--r--   0        0        0     2864 2023-05-28 06:39:10.103262 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/japanese.py
+-rw-r--r--   0        0        0     1350 2023-05-28 06:39:10.103860 py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     1185 2023-07-15 03:22:17.561701 py_pdf_term-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_pdf_term-1.1.0/PKG-INFO
```

### Comparing `py_pdf_term-1.0.2/LICENSE` & `py_pdf_term-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/README.md` & `py_pdf_term-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 ```
 pip install py-pdf-term
 ```
 
 You also need to install spaCy models `ja_core_news_sm` and `en_core_web_sm`, which this module depends on.
 
 ```
-pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz
-pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.6.0/ja_core_news_sm-3.6.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.6.0/en_core_web_sm-3.6.0.tar.gz
 ```
 
 ## Documentation
 
 https://kumachan-mis.github.io/py-pdf-term
```

### Comparing `py_pdf_term-1.0.2/py_pdf_term/_common/consts.py` & `py_pdf_term-1.1.0/py_pdf_term/_common/consts.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/lr.py` & `py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/concats/lr.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/container.py` & `py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/term.py` & `py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/occurrences/term.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/runner.py` & `py_pdf_term-1.1.0/py_pdf_term/analysis/_analysis/runner.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/base.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/combiner.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/combiner.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/separation.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/augmenters/separation.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/base.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/english.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/marker.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/classifiers/marker.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/data.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/extractor.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/extractor.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/combiner.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/combiner.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/base.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/base.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/english.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/base.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/combiner.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/combiner.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/repeat.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/repeat.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/symname.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/splitters/symname.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/utils.py` & `py_pdf_term-1.1.0/py_pdf_term/candidates/_candidates/utils.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/file.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/file.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/util.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/util.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/file.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/candidate.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/candidate.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/method.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/method.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/styling.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/styling.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/techterm.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/techterm.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/xml.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/configs/xml.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/data.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/extractor.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/extractor.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/candidate.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/method.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/method.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/styling.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/styling.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/techterm.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/techterm.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/xml.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/layers/xml.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/base.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py` & `py_pdf_term-1.1.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/mappers.py` & `py_pdf_term-1.1.0/py_pdf_term/mappers.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/base.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/__init__.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/base.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flr.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/flr.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flrh.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/flrh.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/hits.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/hits.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mcvalue.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/mcvalue.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mdp.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/mdp.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/tfidf.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/collectors/tfidf.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/data.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flr.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/flr.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flrh.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/flrh.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/hits.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/hits.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mcvalue.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/mcvalue.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mdp.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/mdp.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/base.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flr.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/flr.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flrh.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/flrh.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/hits.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/hits.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mcvalue.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/mcvalue.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mdp.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/mdp.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/tfidf.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankers/tfidf.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/base.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flr.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/flr.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flrh.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/flrh.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/hits.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/hits.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mcvalue.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mdp.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/mdp.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/tfidf.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/tfidf.py` & `py_pdf_term-1.1.0/py_pdf_term/methods/_methods/tfidf.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py` & `py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/converter.py` & `py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/converter.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/data.py` & `py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/textful.py` & `py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/utils.py` & `py_pdf_term-1.1.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/data.py` & `py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scorer.py` & `py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scorer.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/base.py` & `py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/color.py` & `py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/color.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/fontsize.py` & `py_pdf_term-1.1.0/py_pdf_term/stylings/_stylings/scores/fontsize.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/data.py` & `py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/extractor.py` & `py_pdf_term-1.1.0/py_pdf_term/techterms/_techterms/extractor.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/base.py` & `py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/data.py` & `py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/data.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/english.py` & `py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/english.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/japanese.py` & `py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/japanese.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/tokenizer.py` & `py_pdf_term-1.1.0/py_pdf_term/tokenizers/_tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.2/pyproject.toml` & `py_pdf_term-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "py-pdf-term"
-version = "1.0.2"
+version = "1.1.0"
 description = "A fully-configurable terminology extraction module written in Python"
 authors = ["Yuya Suwa"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/kumachan-mis/py-pdf-term"
 repository = "https://github.com/kumachan-mis/py-pdf-term"
 keywords = ["terminology extraction", "technical term", "pdf"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 "pdfminer.six" = "^20221105"
-spacy = "^3.5.3"
+spacy = "^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+black = "^23.7.0"
 flake8 = "^6.0.0"
 flake8-quotes = "^3.3.2"
 ghp-import = "^2.1.0"
 isort = "^5.12.0"
 pep8-naming = "^0.13.3"
-pre-commit = "^3.3.2"
-pytest-mock = "^3.10.0"
-pytest = "^7.3.1"
+pre-commit = "^3.3.3"
+pytest-mock = "^3.11.1"
+pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 Sphinx = "^7.0.1"
 
 [tool.poetry.group.dev.dependencies.en_core_web_sm]
-url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz"
+url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.6.0/en_core_web_sm-3.6.0.tar.gz"
 
 [tool.poetry.group.dev.dependencies.ja_core_news_sm]
-url = "https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz"
+url = "https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.6.0/ja_core_news_sm-3.6.0.tar.gz"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_pdf_term-1.0.2/PKG-INFO` & `py_pdf_term-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: py-pdf-term
-Version: 1.0.2
+Version: 1.1.0
 Summary: A fully-configurable terminology extraction module written in Python
 Home-page: https://github.com/kumachan-mis/py-pdf-term
 License: MIT
 Keywords: terminology extraction,technical term,pdf
 Author: Yuya Suwa
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pdfminer.six (>=20221105,<20221106)
-Requires-Dist: spacy (>=3.5.3,<4.0.0)
+Requires-Dist: spacy (>=3.6.0,<4.0.0)
 Project-URL: Repository, https://github.com/kumachan-mis/py-pdf-term
 Description-Content-Type: text/markdown
 
 # py-pdf-term
 
 A fully-configurable terminology extraction module written in Python
 
@@ -25,15 +25,15 @@
 ```
 pip install py-pdf-term
 ```
 
 You also need to install spaCy models `ja_core_news_sm` and `en_core_web_sm`, which this module depends on.
 
 ```
-pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz
-pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.6.0/ja_core_news_sm-3.6.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.6.0/en_core_web_sm-3.6.0.tar.gz
 ```
 
 ## Documentation
 
 https://kumachan-mis.github.io/py-pdf-term
```

