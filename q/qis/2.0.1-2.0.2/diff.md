# Comparing `tmp/qis-2.0.1.tar.gz` & `tmp/qis-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qis-2.0.1.tar", max compression
+gzip compressed data, was "qis-2.0.2.tar", max compression
```

## Comparing `qis-2.0.1.tar` & `qis-2.0.2.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.651210 qis-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1838 2023-07-08 19:40:06.554744 qis-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-03-30 08:29:12.943307 qis-2.0.1/qis/__init__.py
--rw-r--r--   0        0        0     4523 2023-02-04 11:08:31.167705 qis-2.0.1/qis/examples/constant_notional.py
--rw-r--r--   0        0        0     1861 2023-07-08 18:05:07.253134 qis-2.0.1/qis/examples/factsheets/multi_assets.py
--rw-r--r--   0        0        0     4990 2023-07-08 18:09:33.222905 qis-2.0.1/qis/examples/factsheets/multi_strategy.py
--rw-r--r--   0        0        0     7334 2023-07-08 18:05:35.120895 qis-2.0.1/qis/examples/factsheets/strategy.py
--rw-r--r--   0        0        0     5521 2023-07-08 18:08:30.345257 qis-2.0.1/qis/examples/factsheets/strategy_benchmark.py
--rw-r--r--   0        0        0  1640225 2023-07-08 18:11:37.205012 qis-2.0.1/qis/examples/figures/multi_strategy.PNG
--rw-r--r--   0        0        0  2049816 2023-07-08 17:49:42.548781 qis-2.0.1/qis/examples/figures/multiassets.PNG
--rw-r--r--   0        0        0   555317 2023-07-08 19:54:41.720622 qis-2.0.1/qis/examples/figures/perf1.PNG
--rw-r--r--   0        0        0   922873 2023-07-08 19:54:44.932256 qis-2.0.1/qis/examples/figures/perf2.PNG
--rw-r--r--   0        0        0   294749 2023-07-08 19:54:47.978979 qis-2.0.1/qis/examples/figures/perf3.PNG
--rw-r--r--   0        0        0  1109717 2023-07-08 18:06:43.873552 qis-2.0.1/qis/examples/figures/strategy.PNG
--rw-r--r--   0        0        0  1445665 2023-07-08 18:10:36.225831 qis-2.0.1/qis/examples/figures/strategy_benchmark.PNG
--rw-r--r--   0        0        0    15024 2023-07-07 16:38:16.408568 qis-2.0.1/qis/examples/move_index.py
--rw-r--r--   0        0        0     1827 2023-07-08 19:54:35.290079 qis-2.0.1/qis/examples/performances.py
--rw-r--r--   0        0        0     6183 2023-06-07 13:05:39.000000 qis-2.0.1/qis/examples/price_plots.py
--rw-r--r--   0        0        0    11025 2023-06-22 07:47:30.271035 qis-2.0.1/qis/examples/simulate_quant_strats.py
--rw-r--r--   0        0        0     8041 2023-04-04 08:32:09.000000 qis-2.0.1/qis/examples/test_ewm.py
--rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.000000 qis-2.0.1/qis/examples/test_scatter.py
--rw-r--r--   0        0        0     7071 2023-07-08 08:12:25.236850 qis-2.0.1/qis/examples/try_pybloqs.py
--rw-r--r--   0        0        0    35171 2023-05-08 10:03:55.923578 qis-2.0.1/qis/file_utils.py
--rw-r--r--   0        0        0      991 2023-01-15 20:14:44.057860 qis-2.0.1/qis/local_path.py
--rw-r--r--   0        0        0     2102 2023-05-22 20:18:38.000000 qis-2.0.1/qis/models/__init__.py
--rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-2.0.1/qis/models/linear/__init__.py
--rw-r--r--   0        0        0     5463 2023-04-04 20:06:31.216516 qis-2.0.1/qis/models/linear/auto_corr.py
--rw-r--r--   0        0        0     8692 2023-02-18 22:06:10.000000 qis-2.0.1/qis/models/linear/corr_cov_matrix.py
--rw-r--r--   0        0        0    41116 2023-04-04 08:36:31.000000 qis-2.0.1/qis/models/linear/ewm.py
--rw-r--r--   0        0        0     3620 2023-02-18 22:06:06.000000 qis-2.0.1/qis/models/linear/ewm_convolution.py
--rw-r--r--   0        0        0     5989 2023-02-18 22:06:09.000000 qis-2.0.1/qis/models/linear/ewm_factors.py
--rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.000000 qis-2.0.1/qis/models/linear/pca.py
--rw-r--r--   0        0        0     6192 2023-02-18 22:06:07.000000 qis-2.0.1/qis/models/linear/plot_correlations.py
--rw-r--r--   0        0        0    11519 2023-02-27 21:29:05.000000 qis-2.0.1/qis/models/linear/ra_returns.py
--rw-r--r--   0        0        0       24 2023-01-23 21:08:28.000000 qis-2.0.1/qis/models/README.md
--rw-r--r--   0        0        0        0 2021-12-04 12:08:05.446837 qis-2.0.1/qis/models/stats/__init__.py
--rw-r--r--   0        0        0    18914 2023-07-02 06:53:30.734832 qis-2.0.1/qis/models/stats/bootstrap.py
--rw-r--r--   0        0        0     2319 2023-01-08 14:55:40.643012 qis-2.0.1/qis/models/stats/ohlc_vol.py
--rw-r--r--   0        0        0     8556 2023-02-18 22:06:11.000000 qis-2.0.1/qis/models/stats/test_bootstrap.py
--rw-r--r--   0        0        0     2420 2023-03-02 15:20:10.000000 qis-2.0.1/qis/perfstats/__init__.py
--rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.000000 qis-2.0.1/qis/perfstats/cond_regression.py
--rw-r--r--   0        0        0    11407 2023-06-08 14:14:30.628944 qis-2.0.1/qis/perfstats/config.py
--rw-r--r--   0        0        0     6844 2023-02-18 22:06:08.000000 qis-2.0.1/qis/perfstats/desc_table.py
--rw-r--r--   0        0        0    21447 2023-06-06 14:51:04.000000 qis-2.0.1/qis/perfstats/perf_stats.py
--rw-r--r--   0        0        0       24 2023-01-23 21:09:51.000000 qis-2.0.1/qis/perfstats/README.md
--rw-r--r--   0        0        0    20191 2023-05-30 13:27:06.000000 qis-2.0.1/qis/perfstats/regime_classifier.py
--rw-r--r--   0        0        0    31157 2023-07-02 06:57:09.133529 qis-2.0.1/qis/perfstats/returns.py
--rw-r--r--   0        0        0     7920 2023-05-12 14:35:19.552286 qis-2.0.1/qis/perfstats/timeseries_bfill.py
--rw-r--r--   0        0        0     3812 2023-05-31 04:27:08.487324 qis-2.0.1/qis/plots/__init__.py
--rw-r--r--   0        0        0    17326 2023-02-18 22:06:04.000000 qis-2.0.1/qis/plots/bars.py
--rw-r--r--   0        0        0    23048 2023-05-31 04:27:08.517244 qis-2.0.1/qis/plots/boxplot.py
--rw-r--r--   0        0        0     3917 2023-02-18 22:06:06.000000 qis-2.0.1/qis/plots/contour.py
--rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-2.0.1/qis/plots/derived/__init__.py
--rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.686282 qis-2.0.1/qis/plots/derived/data_timeseries.py
--rw-r--r--   0        0        0     7464 2023-04-23 14:40:57.890091 qis-2.0.1/qis/plots/derived/drawdowns.py
--rw-r--r--   0        0        0    18685 2023-06-07 13:58:02.000000 qis-2.0.1/qis/plots/derived/perf_table.py
--rw-r--r--   0        0        0    22969 2023-06-06 13:07:17.000000 qis-2.0.1/qis/plots/derived/prices.py
--rw-r--r--   0        0        0     3489 2023-02-18 22:06:08.000000 qis-2.0.1/qis/plots/derived/regime_class_table.py
--rw-r--r--   0        0        0    11801 2023-04-23 15:39:47.885142 qis-2.0.1/qis/plots/derived/regime_data.py
--rw-r--r--   0        0        0     3519 2023-02-18 22:06:07.000000 qis-2.0.1/qis/plots/derived/regime_pdf.py
--rw-r--r--   0        0        0     6590 2023-02-18 22:06:08.000000 qis-2.0.1/qis/plots/derived/regime_scatter.py
--rw-r--r--   0        0        0    18010 2023-03-02 12:04:37.000000 qis-2.0.1/qis/plots/derived/returns_heatmap.py
--rw-r--r--   0        0        0     5173 2023-02-18 22:06:08.000000 qis-2.0.1/qis/plots/derived/returns_scatter.py
--rw-r--r--   0        0        0     4008 2023-02-18 22:06:13.000000 qis-2.0.1/qis/plots/errorbar.py
--rw-r--r--   0        0        0     3643 2023-02-18 22:06:09.000000 qis-2.0.1/qis/plots/heatmap.py
--rw-r--r--   0        0        0    10657 2023-05-24 20:20:57.000000 qis-2.0.1/qis/plots/histogram.py
--rw-r--r--   0        0        0     2917 2023-02-18 22:06:04.000000 qis-2.0.1/qis/plots/histplot2d.py
--rw-r--r--   0        0        0     5424 2023-02-18 22:06:07.000000 qis-2.0.1/qis/plots/lineplot.py
--rw-r--r--   0        0        0     1850 2023-03-21 14:30:08.000000 qis-2.0.1/qis/plots/pie.py
--rw-r--r--   0        0        0     5889 2023-02-18 22:06:10.000000 qis-2.0.1/qis/plots/qqplot.py
--rw-r--r--   0        0        0       24 2023-01-23 21:10:18.000000 qis-2.0.1/qis/plots/README.md
--rw-r--r--   0        0        0    15874 2023-03-14 11:00:14.000000 qis-2.0.1/qis/plots/scatter.py
--rw-r--r--   0        0        0     6009 2023-03-21 06:51:44.000000 qis-2.0.1/qis/plots/stackplot.py
--rw-r--r--   0        0        0    14403 2023-03-02 12:06:44.000000 qis-2.0.1/qis/plots/table.py
--rw-r--r--   0        0        0    21512 2023-05-31 09:52:23.000000 qis-2.0.1/qis/plots/time_series.py
--rw-r--r--   0        0        0    57015 2023-07-05 12:55:13.000000 qis-2.0.1/qis/plots/utils.py
--rw-r--r--   0        0        0      607 2023-07-08 08:04:21.844825 qis-2.0.1/qis/portfolio/__init__.py
--rw-r--r--   0        0        0    11646 2023-06-07 09:56:37.000000 qis-2.0.1/qis/portfolio/backtester.py
--rw-r--r--   0        0        0    27498 2023-07-08 08:04:21.808920 qis-2.0.1/qis/portfolio/multi_portfolio_data.py
--rw-r--r--   0        0        0    36972 2023-07-08 08:04:21.827870 qis-2.0.1/qis/portfolio/portfolio_data.py
--rw-r--r--   0        0        0       24 2023-01-23 21:10:46.000000 qis-2.0.1/qis/portfolio/README.md
--rw-r--r--   0        0        0        0 2023-06-22 07:59:37.604630 qis-2.0.1/qis/portfolio/reports/__init__.py
--rw-r--r--   0        0        0      906 2023-07-07 21:33:49.000000 qis-2.0.1/qis/portfolio/reports/config.py
--rw-r--r--   0        0        0    17485 2023-07-08 11:47:54.120055 qis-2.0.1/qis/portfolio/reports/multi_assets_factsheet.py
--rw-r--r--   0        0        0     7571 2023-07-08 08:11:22.704374 qis-2.0.1/qis/portfolio/reports/multi_strategy_factsheet.py
--rw-r--r--   0        0        0    12574 2023-07-08 05:53:59.904603 qis-2.0.1/qis/portfolio/reports/strategy_benchmark_factsheet.py
--rw-r--r--   0        0        0    12042 2023-07-08 06:56:25.597930 qis-2.0.1/qis/portfolio/reports/strategy_factsheet.py
--rw-r--r--   0        0        0        0 2022-12-17 17:53:19.519118 qis-2.0.1/qis/portfolio/strats/__init__.py
--rw-r--r--   0        0        0     5778 2023-02-18 22:06:12.000000 qis-2.0.1/qis/portfolio/strats/quant_strats_delta1.py
--rw-r--r--   0        0        0      202 2023-07-08 19:37:39.030412 qis-2.0.1/qis/settings.yaml
--rw-r--r--   0        0        0      443 2023-01-15 20:14:44.028937 qis-2.0.1/qis/sql_engine.py
--rw-r--r--   0        0        0     1261 2023-03-02 12:52:25.000000 qis-2.0.1/qis/test_data.py
--rw-r--r--   0        0        0     4752 2023-07-05 08:31:26.000000 qis-2.0.1/qis/utils/__init__.py
--rw-r--r--   0        0        0    41336 2023-06-22 14:34:38.084959 qis-2.0.1/qis/utils/dates.py
--rw-r--r--   0        0        0    11347 2023-06-07 09:35:59.000000 qis-2.0.1/qis/utils/df_agg.py
--rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.792219 qis-2.0.1/qis/utils/df_cut.py
--rw-r--r--   0        0        0     7848 2023-03-02 15:00:21.000000 qis-2.0.1/qis/utils/df_freq.py
--rw-r--r--   0        0        0    10992 2023-02-18 22:06:12.000000 qis-2.0.1/qis/utils/df_groups.py
--rw-r--r--   0        0        0     6819 2023-02-18 22:06:11.000000 qis-2.0.1/qis/utils/df_melt.py
--rw-r--r--   0        0        0    23956 2023-07-02 06:53:30.708901 qis-2.0.1/qis/utils/df_ops.py
--rw-r--r--   0        0        0     8905 2023-02-18 22:06:10.000000 qis-2.0.1/qis/utils/df_str.py
--rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.048573 qis-2.0.1/qis/utils/df_to_weights.py
--rw-r--r--   0        0        0    10640 2023-05-12 08:13:42.291695 qis-2.0.1/qis/utils/generic.py
--rw-r--r--   0        0        0    15848 2023-07-05 08:50:35.000000 qis-2.0.1/qis/utils/np_ops.py
--rw-r--r--   0        0        0     5576 2023-04-04 20:13:54.941670 qis-2.0.1/qis/utils/ols.py
--rw-r--r--   0        0        0       22 2023-01-23 21:14:19.000000 qis-2.0.1/qis/utils/README.md
--rw-r--r--   0        0        0     4589 2023-02-18 22:06:08.000000 qis-2.0.1/qis/utils/sampling.py
--rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.000000 qis-2.0.1/qis/utils/struct_ops.py
--rw-r--r--   0        0        0     8982 2023-07-08 19:58:17.094938 qis-2.0.1/README.md
--rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 qis-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35802 2022-12-30 16:28:55.651210 qis-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1838 2023-07-15 18:33:45.699934 qis-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-03-30 08:29:12.943307 qis-2.0.2/qis/__init__.py
+-rw-r--r--   0        0        0     8584 2023-07-15 18:37:45.571700 qis-2.0.2/qis/examples/bootstrap_analysis.py
+-rw-r--r--   0        0        0     4523 2023-02-04 11:08:31.167705 qis-2.0.2/qis/examples/constant_notional.py
+-rw-r--r--   0        0        0     1861 2023-07-08 18:05:07.253134 qis-2.0.2/qis/examples/factsheets/multi_assets.py
+-rw-r--r--   0        0        0     4990 2023-07-08 18:09:33.222905 qis-2.0.2/qis/examples/factsheets/multi_strategy.py
+-rw-r--r--   0        0        0     7334 2023-07-08 18:05:35.120895 qis-2.0.2/qis/examples/factsheets/strategy.py
+-rw-r--r--   0        0        0     5521 2023-07-08 18:08:30.345257 qis-2.0.2/qis/examples/factsheets/strategy_benchmark.py
+-rw-r--r--   0        0        0  1640225 2023-07-08 18:11:37.205012 qis-2.0.2/qis/examples/figures/multi_strategy.PNG
+-rw-r--r--   0        0        0  2049816 2023-07-08 17:49:42.548781 qis-2.0.2/qis/examples/figures/multiassets.PNG
+-rw-r--r--   0        0        0   555317 2023-07-08 19:54:41.720622 qis-2.0.2/qis/examples/figures/perf1.PNG
+-rw-r--r--   0        0        0   922873 2023-07-08 19:54:44.932256 qis-2.0.2/qis/examples/figures/perf2.PNG
+-rw-r--r--   0        0        0   294749 2023-07-08 19:54:47.978979 qis-2.0.2/qis/examples/figures/perf3.PNG
+-rw-r--r--   0        0        0  1109717 2023-07-08 18:06:43.873552 qis-2.0.2/qis/examples/figures/strategy.PNG
+-rw-r--r--   0        0        0  1445665 2023-07-08 18:10:36.225831 qis-2.0.2/qis/examples/figures/strategy_benchmark.PNG
+-rw-r--r--   0        0        0    15024 2023-07-07 16:38:16.408568 qis-2.0.2/qis/examples/move_index.py
+-rw-r--r--   0        0        0     1827 2023-07-08 19:54:35.290079 qis-2.0.2/qis/examples/performances.py
+-rw-r--r--   0        0        0     6183 2023-06-07 13:05:39.000000 qis-2.0.2/qis/examples/price_plots.py
+-rw-r--r--   0        0        0    11025 2023-06-22 07:47:30.271035 qis-2.0.2/qis/examples/simulate_quant_strats.py
+-rw-r--r--   0        0        0     8041 2023-04-04 08:32:09.000000 qis-2.0.2/qis/examples/test_ewm.py
+-rw-r--r--   0        0        0     1599 2023-01-22 21:54:41.000000 qis-2.0.2/qis/examples/test_scatter.py
+-rw-r--r--   0        0        0     7071 2023-07-08 08:12:25.236850 qis-2.0.2/qis/examples/try_pybloqs.py
+-rw-r--r--   0        0        0    35171 2023-05-08 10:03:55.923578 qis-2.0.2/qis/file_utils.py
+-rw-r--r--   0        0        0      991 2023-01-15 20:14:44.057860 qis-2.0.2/qis/local_path.py
+-rw-r--r--   0        0        0     2102 2023-05-22 20:18:38.000000 qis-2.0.2/qis/models/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:42:40.000000 qis-2.0.2/qis/models/linear/__init__.py
+-rw-r--r--   0        0        0     5515 2023-07-15 12:28:57.386631 qis-2.0.2/qis/models/linear/auto_corr.py
+-rw-r--r--   0        0        0     8692 2023-02-18 22:06:10.000000 qis-2.0.2/qis/models/linear/corr_cov_matrix.py
+-rw-r--r--   0        0        0    41116 2023-04-04 08:36:31.000000 qis-2.0.2/qis/models/linear/ewm.py
+-rw-r--r--   0        0        0     3620 2023-02-18 22:06:06.000000 qis-2.0.2/qis/models/linear/ewm_convolution.py
+-rw-r--r--   0        0        0     5989 2023-02-18 22:06:09.000000 qis-2.0.2/qis/models/linear/ewm_factors.py
+-rw-r--r--   0        0        0     4032 2023-01-23 14:52:48.000000 qis-2.0.2/qis/models/linear/pca.py
+-rw-r--r--   0        0        0     6192 2023-02-18 22:06:07.000000 qis-2.0.2/qis/models/linear/plot_correlations.py
+-rw-r--r--   0        0        0    11519 2023-02-27 21:29:05.000000 qis-2.0.2/qis/models/linear/ra_returns.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:08:28.000000 qis-2.0.2/qis/models/README.md
+-rw-r--r--   0        0        0        0 2021-12-04 12:08:05.446837 qis-2.0.2/qis/models/stats/__init__.py
+-rw-r--r--   0        0        0    19490 2023-07-15 18:32:45.862513 qis-2.0.2/qis/models/stats/bootstrap.py
+-rw-r--r--   0        0        0     2319 2023-01-08 14:55:40.643012 qis-2.0.2/qis/models/stats/ohlc_vol.py
+-rw-r--r--   0        0        0     8556 2023-02-18 22:06:11.000000 qis-2.0.2/qis/models/stats/test_bootstrap.py
+-rw-r--r--   0        0        0     2420 2023-03-02 15:20:10.000000 qis-2.0.2/qis/perfstats/__init__.py
+-rw-r--r--   0        0        0     7178 2023-01-23 14:52:48.000000 qis-2.0.2/qis/perfstats/cond_regression.py
+-rw-r--r--   0        0        0    11407 2023-06-08 14:14:30.628944 qis-2.0.2/qis/perfstats/config.py
+-rw-r--r--   0        0        0     6844 2023-02-18 22:06:08.000000 qis-2.0.2/qis/perfstats/desc_table.py
+-rw-r--r--   0        0        0    21447 2023-06-06 14:51:04.000000 qis-2.0.2/qis/perfstats/perf_stats.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:09:51.000000 qis-2.0.2/qis/perfstats/README.md
+-rw-r--r--   0        0        0    20191 2023-05-30 13:27:06.000000 qis-2.0.2/qis/perfstats/regime_classifier.py
+-rw-r--r--   0        0        0    31157 2023-07-02 06:57:09.133529 qis-2.0.2/qis/perfstats/returns.py
+-rw-r--r--   0        0        0     7920 2023-05-12 14:35:19.552286 qis-2.0.2/qis/perfstats/timeseries_bfill.py
+-rw-r--r--   0        0        0     3812 2023-05-31 04:27:08.487324 qis-2.0.2/qis/plots/__init__.py
+-rw-r--r--   0        0        0    17326 2023-02-18 22:06:04.000000 qis-2.0.2/qis/plots/bars.py
+-rw-r--r--   0        0        0    23159 2023-07-15 15:16:40.000000 qis-2.0.2/qis/plots/boxplot.py
+-rw-r--r--   0        0        0     3917 2023-02-18 22:06:06.000000 qis-2.0.2/qis/plots/contour.py
+-rw-r--r--   0        0        0        0 2021-03-12 13:47:34.000000 qis-2.0.2/qis/plots/derived/__init__.py
+-rw-r--r--   0        0        0     2196 2023-01-07 22:34:01.686282 qis-2.0.2/qis/plots/derived/data_timeseries.py
+-rw-r--r--   0        0        0     7464 2023-04-23 14:40:57.890091 qis-2.0.2/qis/plots/derived/drawdowns.py
+-rw-r--r--   0        0        0    18685 2023-06-07 13:58:02.000000 qis-2.0.2/qis/plots/derived/perf_table.py
+-rw-r--r--   0        0        0    22969 2023-06-06 13:07:17.000000 qis-2.0.2/qis/plots/derived/prices.py
+-rw-r--r--   0        0        0     3489 2023-02-18 22:06:08.000000 qis-2.0.2/qis/plots/derived/regime_class_table.py
+-rw-r--r--   0        0        0    11801 2023-04-23 15:39:47.885142 qis-2.0.2/qis/plots/derived/regime_data.py
+-rw-r--r--   0        0        0     3519 2023-02-18 22:06:07.000000 qis-2.0.2/qis/plots/derived/regime_pdf.py
+-rw-r--r--   0        0        0     6590 2023-02-18 22:06:08.000000 qis-2.0.2/qis/plots/derived/regime_scatter.py
+-rw-r--r--   0        0        0    18010 2023-03-02 12:04:37.000000 qis-2.0.2/qis/plots/derived/returns_heatmap.py
+-rw-r--r--   0        0        0     5173 2023-02-18 22:06:08.000000 qis-2.0.2/qis/plots/derived/returns_scatter.py
+-rw-r--r--   0        0        0     4008 2023-02-18 22:06:13.000000 qis-2.0.2/qis/plots/errorbar.py
+-rw-r--r--   0        0        0     3643 2023-02-18 22:06:09.000000 qis-2.0.2/qis/plots/heatmap.py
+-rw-r--r--   0        0        0    10657 2023-05-24 20:20:57.000000 qis-2.0.2/qis/plots/histogram.py
+-rw-r--r--   0        0        0     2917 2023-02-18 22:06:04.000000 qis-2.0.2/qis/plots/histplot2d.py
+-rw-r--r--   0        0        0     5424 2023-02-18 22:06:07.000000 qis-2.0.2/qis/plots/lineplot.py
+-rw-r--r--   0        0        0     1850 2023-03-21 14:30:08.000000 qis-2.0.2/qis/plots/pie.py
+-rw-r--r--   0        0        0     5889 2023-02-18 22:06:10.000000 qis-2.0.2/qis/plots/qqplot.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:18.000000 qis-2.0.2/qis/plots/README.md
+-rw-r--r--   0        0        0    15874 2023-03-14 11:00:14.000000 qis-2.0.2/qis/plots/scatter.py
+-rw-r--r--   0        0        0     6009 2023-03-21 06:51:44.000000 qis-2.0.2/qis/plots/stackplot.py
+-rw-r--r--   0        0        0    14403 2023-03-02 12:06:44.000000 qis-2.0.2/qis/plots/table.py
+-rw-r--r--   0        0        0    21512 2023-05-31 09:52:23.000000 qis-2.0.2/qis/plots/time_series.py
+-rw-r--r--   0        0        0    57385 2023-07-15 14:36:30.000000 qis-2.0.2/qis/plots/utils.py
+-rw-r--r--   0        0        0      607 2023-07-08 08:04:21.844825 qis-2.0.2/qis/portfolio/__init__.py
+-rw-r--r--   0        0        0    11646 2023-06-07 09:56:37.000000 qis-2.0.2/qis/portfolio/backtester.py
+-rw-r--r--   0        0        0    27498 2023-07-08 08:04:21.808920 qis-2.0.2/qis/portfolio/multi_portfolio_data.py
+-rw-r--r--   0        0        0    36972 2023-07-08 08:04:21.827870 qis-2.0.2/qis/portfolio/portfolio_data.py
+-rw-r--r--   0        0        0       24 2023-01-23 21:10:46.000000 qis-2.0.2/qis/portfolio/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 07:59:37.604630 qis-2.0.2/qis/portfolio/reports/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-07 21:33:49.000000 qis-2.0.2/qis/portfolio/reports/config.py
+-rw-r--r--   0        0        0    17485 2023-07-08 11:47:54.120055 qis-2.0.2/qis/portfolio/reports/multi_assets_factsheet.py
+-rw-r--r--   0        0        0     7571 2023-07-08 08:11:22.704374 qis-2.0.2/qis/portfolio/reports/multi_strategy_factsheet.py
+-rw-r--r--   0        0        0    12574 2023-07-08 05:53:59.904603 qis-2.0.2/qis/portfolio/reports/strategy_benchmark_factsheet.py
+-rw-r--r--   0        0        0    12042 2023-07-08 06:56:25.597930 qis-2.0.2/qis/portfolio/reports/strategy_factsheet.py
+-rw-r--r--   0        0        0        0 2022-12-17 17:53:19.519118 qis-2.0.2/qis/portfolio/strats/__init__.py
+-rw-r--r--   0        0        0     5778 2023-02-18 22:06:12.000000 qis-2.0.2/qis/portfolio/strats/quant_strats_delta1.py
+-rw-r--r--   0        0        0      202 2023-07-15 18:39:20.038525 qis-2.0.2/qis/settings.yaml
+-rw-r--r--   0        0        0      443 2023-01-15 20:14:44.028937 qis-2.0.2/qis/sql_engine.py
+-rw-r--r--   0        0        0     1261 2023-03-02 12:52:25.000000 qis-2.0.2/qis/test_data.py
+-rw-r--r--   0        0        0     4752 2023-07-05 08:31:26.000000 qis-2.0.2/qis/utils/__init__.py
+-rw-r--r--   0        0        0    41336 2023-06-22 14:34:38.084959 qis-2.0.2/qis/utils/dates.py
+-rw-r--r--   0        0        0    11347 2023-06-07 09:35:59.000000 qis-2.0.2/qis/utils/df_agg.py
+-rw-r--r--   0        0        0     8491 2023-01-08 13:32:37.792219 qis-2.0.2/qis/utils/df_cut.py
+-rw-r--r--   0        0        0     7848 2023-03-02 15:00:21.000000 qis-2.0.2/qis/utils/df_freq.py
+-rw-r--r--   0        0        0    10992 2023-02-18 22:06:12.000000 qis-2.0.2/qis/utils/df_groups.py
+-rw-r--r--   0        0        0     6819 2023-02-18 22:06:11.000000 qis-2.0.2/qis/utils/df_melt.py
+-rw-r--r--   0        0        0    23956 2023-07-02 06:53:30.708901 qis-2.0.2/qis/utils/df_ops.py
+-rw-r--r--   0        0        0     8905 2023-02-18 22:06:10.000000 qis-2.0.2/qis/utils/df_str.py
+-rw-r--r--   0        0        0    11344 2022-12-30 16:13:34.048573 qis-2.0.2/qis/utils/df_to_weights.py
+-rw-r--r--   0        0        0    10640 2023-05-12 08:13:42.291695 qis-2.0.2/qis/utils/generic.py
+-rw-r--r--   0        0        0    15848 2023-07-05 08:50:35.000000 qis-2.0.2/qis/utils/np_ops.py
+-rw-r--r--   0        0        0     5576 2023-04-04 20:13:54.941670 qis-2.0.2/qis/utils/ols.py
+-rw-r--r--   0        0        0       22 2023-01-23 21:14:19.000000 qis-2.0.2/qis/utils/README.md
+-rw-r--r--   0        0        0     4589 2023-02-18 22:06:08.000000 qis-2.0.2/qis/utils/sampling.py
+-rw-r--r--   0        0        0     5938 2022-12-16 21:08:07.000000 qis-2.0.2/qis/utils/struct_ops.py
+-rw-r--r--   0        0        0     8982 2023-07-08 19:58:17.094938 qis-2.0.2/README.md
+-rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 qis-2.0.2/PKG-INFO
```

### Comparing `qis-2.0.1/LICENSE.txt` & `qis-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/pyproject.toml` & `qis-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2271 6973 220d 0a76 6572  ame = "qis"..ver
-00000020: 7369 6f6e 203d 2022 322e 302e 3122 0d0a  sion = "2.0.1"..
+00000020: 7369 6f6e 203d 2022 322e 302e 3222 0d0a  sion = "2.0.2"..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 2249  description = "I
 00000040: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
 00000050: 2076 6973 7561 6c69 7361 7469 6f6e 2061   visualisation a
 00000060: 6e64 2072 6570 6f72 7469 6e67 2061 6e61  nd reporting ana
 00000070: 6c79 7469 6373 2066 6f72 2051 7561 6e74  lytics for Quant
 00000080: 6974 6174 6976 6520 496e 7665 7374 6d65  itative Investme
 00000090: 6e74 2053 7472 6174 6567 6965 7322 0d0a  nt Strategies"..
```

### Comparing `qis-2.0.1/qis/__init__.py` & `qis-2.0.2/qis/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/constant_notional.py` & `qis-2.0.2/qis/examples/constant_notional.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/factsheets/multi_assets.py` & `qis-2.0.2/qis/examples/factsheets/multi_assets.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/factsheets/multi_strategy.py` & `qis-2.0.2/qis/examples/factsheets/multi_strategy.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/factsheets/strategy.py` & `qis-2.0.2/qis/examples/factsheets/strategy.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/factsheets/strategy_benchmark.py` & `qis-2.0.2/qis/examples/factsheets/strategy_benchmark.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/multi_strategy.PNG` & `qis-2.0.2/qis/examples/figures/multi_strategy.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/multiassets.PNG` & `qis-2.0.2/qis/examples/figures/multiassets.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/perf1.PNG` & `qis-2.0.2/qis/examples/figures/perf1.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/perf2.PNG` & `qis-2.0.2/qis/examples/figures/perf2.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/perf3.PNG` & `qis-2.0.2/qis/examples/figures/perf3.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/strategy.PNG` & `qis-2.0.2/qis/examples/figures/strategy.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/figures/strategy_benchmark.PNG` & `qis-2.0.2/qis/examples/figures/strategy_benchmark.PNG`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/move_index.py` & `qis-2.0.2/qis/examples/move_index.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/performances.py` & `qis-2.0.2/qis/examples/performances.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/price_plots.py` & `qis-2.0.2/qis/examples/price_plots.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/simulate_quant_strats.py` & `qis-2.0.2/qis/examples/simulate_quant_strats.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/test_ewm.py` & `qis-2.0.2/qis/examples/test_ewm.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/test_scatter.py` & `qis-2.0.2/qis/examples/test_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/examples/try_pybloqs.py` & `qis-2.0.2/qis/examples/try_pybloqs.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/file_utils.py` & `qis-2.0.2/qis/file_utils.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/local_path.py` & `qis-2.0.2/qis/local_path.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/__init__.py` & `qis-2.0.2/qis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/auto_corr.py` & `qis-2.0.2/qis/models/linear/auto_corr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # packages
 import numpy as np
 import pandas as pd
-from typing import Union
+from typing import Union, Tuple
 from numba import njit
 from statsmodels.tsa.stattools import pacf, acf
 
 # qis
 from qis.models.linear.ewm import MeanAdjType, compute_rolling_mean_adj
 
 
 def estimate_path_acf(paths: Union[np.ndarray, pd.DataFrame],
                       nlags: int = 10,
                       is_pacf: bool = True
-                      ):
+                      ) -> Tuple[pd.DataFrame, pd.Series, pd.Series]:
     if isinstance(paths, pd.DataFrame):
         columns = paths.columns
         paths = paths.to_numpy()
     else:
         columns = None
 
     nb_path = paths.shape[1]
```

### Comparing `qis-2.0.1/qis/models/linear/corr_cov_matrix.py` & `qis-2.0.2/qis/models/linear/corr_cov_matrix.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/ewm.py` & `qis-2.0.2/qis/models/linear/ewm.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/ewm_convolution.py` & `qis-2.0.2/qis/models/linear/ewm_convolution.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/ewm_factors.py` & `qis-2.0.2/qis/models/linear/ewm_factors.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/pca.py` & `qis-2.0.2/qis/models/linear/pca.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/plot_correlations.py` & `qis-2.0.2/qis/models/linear/plot_correlations.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/linear/ra_returns.py` & `qis-2.0.2/qis/models/linear/ra_returns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/stats/bootstrap.py` & `qis-2.0.2/qis/models/stats/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,32 @@
 
 class BootsrapOutput(Enum):
     SERIES_TO_DF = 1
     DF_TO_LIST_ARRAYS = 2
 
 
 @njit
+def set_seed(value):
+    """
+    set seed for numba space
+    """
+    np.random.seed(value)
+
+
+@njit
 def bootstrap_indices_iid(num_data_index: int,
                           num_samples: int = 10,
                           index_length: int = 1000,
                           seed: int = 1
                           ) -> np.ndarray:
     """
     generate iid bootstrap indices
     """
     np.random.seed(seed)
+    set_seed(seed)
     bootstrapped_indices = np.zeros((index_length, num_samples), dtype=np.int64)
     for idx in np.arange(num_samples):
         previous_index, next_index = 0, 0
         while next_index < index_length-1:
             ran_indices = np.random.randint(low=0, high=num_data_index, size=num_data_index)
             next_index = np.minimum(previous_index+num_data_index, index_length-1)
             required_fill = next_index - previous_index
@@ -247,39 +256,52 @@
                          bootsrap_type: BootsrapType = BootsrapType.STATIONARY,
                          bootsrap_output: BootsrapOutput = BootsrapOutput.DF_TO_LIST_ARRAYS,
                          num_samples: int = 10,
                          index_length: int = 1000,
                          block_size: int = 20,
                          is_log_returns: bool = False,
                          seed: int = 1,
-                         bootstrapped_indices: np.ndarray = None
+                         bootstrapped_indices: np.ndarray = None,
+                         init_to_end: bool = True
                          ) -> Union[List[np.ndarray], pd.DataFrame]:
-
+    """
+    bootstrap price data
+    for pd.Dataframe use bootsrap_output = BootsrapOutput.DF_TO_LIST_ARRAYS to get list of nd.arrays
+    block_size = 1 corresponds to iid sampling
+    """
     returns = ret.to_returns(prices=prices, is_log_returns=is_log_returns, drop_first=True)
 
     bootstrap_returns = bootstrap_data(data=returns,
                                        bootsrap_type=bootsrap_type,
                                        bootsrap_output=bootsrap_output,
                                        num_samples=num_samples,
                                        index_length=index_length,
                                        block_size=block_size,
                                        seed=seed,
                                        bootstrapped_indices=bootstrapped_indices)
 
     if bootsrap_output == BootsrapOutput.DF_TO_LIST_ARRAYS:
-        init_value = prices.iloc[-1, :].to_numpy()
+        if init_to_end:
+            init_value = prices.iloc[-1, :].to_numpy()
+        else:
+            init_value = prices.iloc[0, :].to_numpy()
+
         bootstrap_sample = List()
         for returns in bootstrap_returns:
             if is_log_returns:
                 bootstrap_sample.append(ret.log_returns_to_nav(log_returns=returns, init_value=init_value))
             else:
                 bootstrap_sample.append(ret.returns_to_nav(returns=returns, init_value=init_value))
 
     elif bootsrap_output == BootsrapOutput.SERIES_TO_DF:
-        init_value = prices[-1]*np.ones(num_samples)
+        if init_to_end:
+            init_value = prices[-1]*np.ones(num_samples)
+        else:
+            init_value = prices[0]*np.ones(num_samples)
+
         if is_log_returns:
             bootstrap_sample = ret.log_returns_to_nav(log_returns=bootstrap_returns, init_value=init_value)
         else:
             bootstrap_sample = ret.returns_to_nav(returns=bootstrap_returns, init_value=init_value)
     else:
         raise ValueError(f"not implemented")
```

### Comparing `qis-2.0.1/qis/models/stats/ohlc_vol.py` & `qis-2.0.2/qis/models/stats/ohlc_vol.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/models/stats/test_bootstrap.py` & `qis-2.0.2/qis/models/stats/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/__init__.py` & `qis-2.0.2/qis/perfstats/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/cond_regression.py` & `qis-2.0.2/qis/perfstats/cond_regression.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/config.py` & `qis-2.0.2/qis/perfstats/config.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/desc_table.py` & `qis-2.0.2/qis/perfstats/desc_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/perf_stats.py` & `qis-2.0.2/qis/perfstats/perf_stats.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/regime_classifier.py` & `qis-2.0.2/qis/perfstats/regime_classifier.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/returns.py` & `qis-2.0.2/qis/perfstats/returns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/perfstats/timeseries_bfill.py` & `qis-2.0.2/qis/perfstats/timeseries_bfill.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/__init__.py` & `qis-2.0.2/qis/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/bars.py` & `qis-2.0.2/qis/plots/bars.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/boxplot.py` & `qis-2.0.2/qis/plots/boxplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,31 +187,33 @@
     # need to add line for legend with hues
     lines = None
     if labels is not None:
         lines = []
         for label, color in zip(labels, palette):
             lines.append((label, {'color': color}))
 
-    put.set_legend(ax=ax,
-                   legend_title=hue,
-                   legend_loc=legend_loc,
-                   fontsize=fontsize,
-                   lines=lines,
-                   **kwargs)
+    if legend_loc is not None:
+        put.set_legend(ax=ax,
+                       legend_title=hue,
+                       legend_loc=legend_loc,
+                       fontsize=fontsize,
+                       lines=lines,
+                       **kwargs)
 
     if title is not None:
         put.set_title(ax=ax, title=title, fontsize=fontsize)
     put.set_spines(ax=ax)
 
     return fig
 
 
 def df_boxplot_by_index(df: Union[pd.Series, pd.DataFrame],
                         index_var_name: str = 'date',
                         ylabel: str = 'returns',
+                        xlabel: str = None,
                         show_ylabel: bool = True,
                         title: str = None,
                         colors: Optional[List[str]] = None,
                         ax: plt.Subplot = None,
                         **kwargs
                         ) -> Optional[plt.Figure]:
     """
@@ -228,15 +230,15 @@
     fig = plot_box(df=box_data,
                    x=index_var_name,
                    y=ylabel,
                    continuous_x_col=ylabel,
                    ylabel=ylabel if show_ylabel else None,
                    original_index=df.index,
                    colors=colors,
-                   xlabel=False,
+                   xlabel=xlabel or False,
                    title=title,
                    ax=ax,
                    **kwargs)
     return fig
 
 
 def df_boxplot_by_columns(df: Union[pd.Series, pd.DataFrame],
```

### Comparing `qis-2.0.1/qis/plots/contour.py` & `qis-2.0.2/qis/plots/contour.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/data_timeseries.py` & `qis-2.0.2/qis/plots/derived/data_timeseries.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/drawdowns.py` & `qis-2.0.2/qis/plots/derived/drawdowns.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/perf_table.py` & `qis-2.0.2/qis/plots/derived/perf_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/prices.py` & `qis-2.0.2/qis/plots/derived/prices.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/regime_class_table.py` & `qis-2.0.2/qis/plots/derived/regime_class_table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/regime_data.py` & `qis-2.0.2/qis/plots/derived/regime_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/regime_pdf.py` & `qis-2.0.2/qis/plots/derived/regime_pdf.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/regime_scatter.py` & `qis-2.0.2/qis/plots/derived/regime_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/returns_heatmap.py` & `qis-2.0.2/qis/plots/derived/returns_heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/derived/returns_scatter.py` & `qis-2.0.2/qis/plots/derived/returns_scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/errorbar.py` & `qis-2.0.2/qis/plots/errorbar.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/heatmap.py` & `qis-2.0.2/qis/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/histogram.py` & `qis-2.0.2/qis/plots/histogram.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/histplot2d.py` & `qis-2.0.2/qis/plots/histplot2d.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/lineplot.py` & `qis-2.0.2/qis/plots/lineplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/pie.py` & `qis-2.0.2/qis/plots/pie.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/qqplot.py` & `qis-2.0.2/qis/plots/qqplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/scatter.py` & `qis-2.0.2/qis/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/stackplot.py` & `qis-2.0.2/qis/plots/stackplot.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/table.py` & `qis-2.0.2/qis/plots/table.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/time_series.py` & `qis-2.0.2/qis/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/plots/utils.py` & `qis-2.0.2/qis/plots/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1367,31 +1367,38 @@
         n_hue = len(df[hue].unique())
         # colorise = [elem for _ in range(n_hue) for elem in colorise]  # extend colors n times
         colorise = [elem for elem in colorise for _ in range(n_hue) ]  # extend colors n times
     return colorise
 
 
 def add_scatter_points(ax: plt.Subplot,
-                       label_x_y: Dict[str, Tuple[Any, float]],
+                       label_x_y: Union[Dict[str, Tuple[Any, float]], List[Tuple[Any, float]]],
                        fontsize: int = 12,
                        color: str = 'steelblue',
                        colors: List[str] = None,
                        linewidth: int = 3,
+                       size: int = 3,
                        **kwargs
                        ) -> None:
-
+    """
+    add scatter points to ax
+    """
     if colors is None:
-        colors = len(label_x_y.keys()) * [color]
-    for (key, (x, y)), color in zip(label_x_y.items(), colors):
-        ax.annotate(key,
-                    xy=(x, y), xytext=(2, 2),
-                    textcoords='offset points', ha='left', va='bottom',
-                    color=color,
-                    fontsize=fontsize)
-        ax.scatter(x=x, y=y, marker='*', color=color, s=3, linewidth=linewidth)
+        if isinstance(label_x_y, dict):
+            colors = len(label_x_y.keys()) * [color]
+        else:
+            colors = len(label_x_y) * [color]
+    if isinstance(label_x_y, dict):
+        for (key, (x, y)), color in zip(label_x_y.items(), colors):
+            ax.annotate(key, xy=(x, y), xytext=(2, 2), color=color,
+                        textcoords='offset points', ha='left', va='bottom', fontsize=fontsize)
+            ax.scatter(x=x, y=y, marker='*', color=color, s=size, linewidth=linewidth)
+    else:
+        for (x, y), color in zip(label_x_y, colors):
+            ax.scatter(x=x, y=y, marker='*', color=color, s=size, linewidth=linewidth)
 
 
 def calc_table_height(num_rows: int,
                       row_height: float = ROW_HIGHT,
                       first_row_height: float = None,
                       scale: float = 0.225
                       ) -> float:
```

### Comparing `qis-2.0.1/qis/portfolio/__init__.py` & `qis-2.0.2/qis/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/backtester.py` & `qis-2.0.2/qis/portfolio/backtester.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/multi_portfolio_data.py` & `qis-2.0.2/qis/portfolio/multi_portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/portfolio_data.py` & `qis-2.0.2/qis/portfolio/portfolio_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/reports/config.py` & `qis-2.0.2/qis/portfolio/reports/config.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/reports/multi_assets_factsheet.py` & `qis-2.0.2/qis/portfolio/reports/multi_assets_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/reports/multi_strategy_factsheet.py` & `qis-2.0.2/qis/portfolio/reports/multi_strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/reports/strategy_benchmark_factsheet.py` & `qis-2.0.2/qis/portfolio/reports/strategy_benchmark_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/reports/strategy_factsheet.py` & `qis-2.0.2/qis/portfolio/reports/strategy_factsheet.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/portfolio/strats/quant_strats_delta1.py` & `qis-2.0.2/qis/portfolio/strats/quant_strats_delta1.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/test_data.py` & `qis-2.0.2/qis/test_data.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/__init__.py` & `qis-2.0.2/qis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/dates.py` & `qis-2.0.2/qis/utils/dates.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_agg.py` & `qis-2.0.2/qis/utils/df_agg.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_cut.py` & `qis-2.0.2/qis/utils/df_cut.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_freq.py` & `qis-2.0.2/qis/utils/df_freq.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_groups.py` & `qis-2.0.2/qis/utils/df_groups.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_melt.py` & `qis-2.0.2/qis/utils/df_melt.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_ops.py` & `qis-2.0.2/qis/utils/df_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_str.py` & `qis-2.0.2/qis/utils/df_str.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/df_to_weights.py` & `qis-2.0.2/qis/utils/df_to_weights.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/generic.py` & `qis-2.0.2/qis/utils/generic.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/np_ops.py` & `qis-2.0.2/qis/utils/np_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/ols.py` & `qis-2.0.2/qis/utils/ols.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/sampling.py` & `qis-2.0.2/qis/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/qis/utils/struct_ops.py` & `qis-2.0.2/qis/utils/struct_ops.py`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/README.md` & `qis-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qis-2.0.1/PKG-INFO` & `qis-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qis
-Version: 2.0.1
+Version: 2.0.2
 Summary: Implementation of visualisation and reporting analytics for Quantitative Investment Strategies
 Home-page: https://github.com/ArturSepp/QuantInvestStrats
 License: LICENSE.txt
 Keywords: quantitative,investing,portfolio optimization,systematic strategies,volatility
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

