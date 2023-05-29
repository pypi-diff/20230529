# Comparing `tmp/psdm-analysis-0.1.3.tar.gz` & `tmp/psdm-analysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm-analysis-0.1.3.tar", max compression
+gzip compressed data, was "psdm-analysis-0.1.4.tar", max compression
```

## Comparing `psdm-analysis-0.1.3.tar` & `psdm-analysis-0.1.4.tar`

### file list

```diff
@@ -1,67 +1,71 @@
--rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.3/LICENSE
--rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.3/psdm_analysis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.3/psdm_analysis/analysis/__init__.py
--rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.3/psdm_analysis/analysis/calc.py
--rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.3/psdm_analysis/analysis/grid.py
--rw-r--r--   0        0        0        0 2023-04-28 08:49:33.826962 psdm-analysis-0.1.3/psdm_analysis/conversion/__init__.py
--rw-r--r--   0        0        0   254685 2023-04-28 08:32:26.669910 psdm-analysis-0.1.3/psdm_analysis/conversion/pandapower.ipynb
--rw-r--r--   0        0        0     3960 2023-04-28 08:49:33.827267 psdm-analysis-0.1.3/psdm_analysis/conversion/pandapower.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.3/psdm_analysis/io/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.3/psdm_analysis/io/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.3/psdm_analysis/models/__init__.py
--rw-r--r--   0        0        0     7232 2023-04-19 12:49:15.039262 psdm-analysis-0.1.3/psdm_analysis/models/entity.py
--rw-r--r--   0        0        0     5988 2023-04-19 12:49:15.039392 psdm-analysis-0.1.3/psdm_analysis/models/grid_with_results.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.3/psdm_analysis/models/input/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/__init__.py
--rw-r--r--   0        0        0     2126 2023-04-19 12:49:15.039712 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/lines.py
--rw-r--r--   0        0        0      578 2023-04-19 12:49:15.039922 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/switches.py
--rw-r--r--   0        0        0     2455 2023-04-19 12:49:15.040033 psdm-analysis-0.1.3/psdm_analysis/models/input/connector/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.3/psdm_analysis/models/input/container/__init__.py
--rw-r--r--   0        0        0     3925 2023-04-19 12:49:15.040286 psdm-analysis-0.1.3/psdm_analysis/models/input/container/grid_container.py
--rw-r--r--   0        0        0     3456 2023-04-19 12:49:15.040383 psdm-analysis-0.1.3/psdm_analysis/models/input/container/mixins.py
--rw-r--r--   0        0        0     6113 2023-04-19 12:49:15.040661 psdm-analysis-0.1.3/psdm_analysis/models/input/container/participants_container.py
--rw-r--r--   0        0        0     1884 2023-04-19 12:49:15.040834 psdm-analysis-0.1.3/psdm_analysis/models/input/enums.py
--rw-r--r--   0        0        0     1129 2023-04-19 12:49:15.041071 psdm-analysis-0.1.3/psdm_analysis/models/input/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/bm.py
--rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/charging.py
--rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/em.py
--rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evcs.py
--rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evs.py
--rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      814 2023-04-19 12:49:15.042128 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/hp.py
--rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/load.py
--rw-r--r--   0        0        0     1032 2023-04-19 12:49:15.042559 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/participant.py
--rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/pv.py
--rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/storage.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.3/psdm_analysis/models/input/participant/wec.py
--rw-r--r--   0        0        0     2887 2023-04-19 12:49:15.043116 psdm-analysis-0.1.3/psdm_analysis/models/primary_data.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.3/psdm_analysis/models/result/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.3/psdm_analysis/models/result/flex_option.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/__init__.py
--rw-r--r--   0        0        0     2314 2023-04-19 12:49:15.043655 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     3670 2023-04-19 12:49:15.043790 psdm-analysis-0.1.3/psdm_analysis/models/result/grid/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/__init__.py
--rw-r--r--   0        0        0     3645 2023-04-19 12:49:15.043937 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/dict.py
--rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     6261 2023-04-19 12:49:15.044315 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participant.py
--rw-r--r--   0        0        0     9664 2023-04-19 12:49:15.044458 psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participants_res_container.py
--rw-r--r--   0        0        0     5776 2023-04-19 12:49:15.044578 psdm-analysis-0.1.3/psdm_analysis/models/result/power.py
--rw-r--r--   0        0        0     2340 2023-04-19 12:49:15.044687 psdm-analysis-0.1.3/psdm_analysis/models/result/res_container.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.3/psdm_analysis/plots/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-20 07:54:56.450726 psdm-analysis-0.1.3/psdm_analysis/plots/grid.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.3/psdm_analysis/plots/results/__init__.py
--rw-r--r--   0        0        0     2431 2023-04-19 12:49:15.045086 psdm-analysis-0.1.3/psdm_analysis/plots/results/bar_plot.py
--rw-r--r--   0        0        0     3461 2023-04-19 12:49:15.045391 psdm-analysis-0.1.3/psdm_analysis/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1096 2023-04-19 12:49:15.045589 psdm-analysis-0.1.3/psdm_analysis/plots/results/line_plot.py
--rw-r--r--   0        0        0     2644 2023-04-28 08:49:33.827702 psdm-analysis-0.1.3/psdm_analysis/plots/results/node_plot.py
--rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.3/psdm_analysis/plots/results/nodes.py
--rw-r--r--   0        0        0    11954 2023-04-19 12:49:15.045955 psdm-analysis-0.1.3/psdm_analysis/plots/results/power_plot.py
--rw-r--r--   0        0        0     4318 2023-04-28 09:03:18.431942 psdm-analysis-0.1.3/psdm_analysis/plots/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.3/psdm_analysis/processing/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-19 12:49:15.046231 psdm-analysis-0.1.3/psdm_analysis/processing/dataframe.py
--rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.3/psdm_analysis/processing/series.py
--rw-r--r--   0        0        0      683 2023-04-28 09:04:17.744077 psdm-analysis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 psdm-analysis-0.1.3/setup.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 psdm-analysis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.4/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.4/psdm_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.4/psdm_analysis/analysis/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.4/psdm_analysis/analysis/calc.py
+-rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.4/psdm_analysis/analysis/grid.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:38:45.729757 psdm-analysis-0.1.4/psdm_analysis/conversion/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-02 07:38:45.730387 psdm-analysis-0.1.4/psdm_analysis/conversion/pandapower.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.4/psdm_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.4/psdm_analysis/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.4/psdm_analysis/models/__init__.py
+-rw-r--r--   0        0        0     9503 2023-05-23 11:13:37.867698 psdm-analysis-0.1.4/psdm_analysis/models/entity.py
+-rw-r--r--   0        0        0     6788 2023-05-26 10:45:12.995987 psdm-analysis-0.1.4/psdm_analysis/models/grid_with_results.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.4/psdm_analysis/models/input/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     1195 2023-05-23 11:13:37.868712 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/connector.py
+-rw-r--r--   0        0        0     1888 2023-05-23 11:13:37.869005 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/lines.py
+-rw-r--r--   0        0        0      674 2023-05-23 11:13:37.869378 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/switches.py
+-rw-r--r--   0        0        0     2240 2023-05-29 07:50:38.432624 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.4/psdm_analysis/models/input/container/__init__.py
+-rw-r--r--   0        0        0     6724 2023-05-29 07:47:15.753072 psdm-analysis-0.1.4/psdm_analysis/models/input/container/grid_container.py
+-rw-r--r--   0        0        0     3456 2023-05-04 10:09:12.848994 psdm-analysis-0.1.4/psdm_analysis/models/input/container/mixins.py
+-rw-r--r--   0        0        0     6312 2023-05-23 11:13:37.870997 psdm-analysis-0.1.4/psdm_analysis/models/input/container/participants_container.py
+-rw-r--r--   0        0        0     3134 2023-05-23 11:13:37.871280 psdm-analysis-0.1.4/psdm_analysis/models/input/enums.py
+-rw-r--r--   0        0        0     1365 2023-05-23 11:13:37.871527 psdm-analysis-0.1.4/psdm_analysis/models/input/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/charging.py
+-rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/em.py
+-rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evcs.py
+-rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evs.py
+-rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      813 2023-05-23 11:13:37.872710 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/hp.py
+-rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/load.py
+-rw-r--r--   0        0        0     1266 2023-05-23 11:13:37.873708 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/wec.py
+-rw-r--r--   0        0        0     4354 2023-05-23 11:13:37.874172 psdm-analysis-0.1.4/psdm_analysis/models/primary_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.4/psdm_analysis/models/result/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.4/psdm_analysis/models/result/flex_option.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-23 11:13:37.874372 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/connector.py
+-rw-r--r--   0        0        0     2284 2023-05-26 10:46:52.073721 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/enhanced_node.py
+-rw-r--r--   0        0        0     2626 2023-05-26 10:48:25.443146 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/node.py
+-rw-r--r--   0        0        0     1701 2023-05-23 11:13:37.875468 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/__init__.py
+-rw-r--r--   0        0        0     6696 2023-05-29 07:46:12.859811 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0     3619 2023-05-26 10:49:03.203272 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participant.py
+-rw-r--r--   0        0        0    10556 2023-05-26 09:57:21.675417 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participants_res_container.py
+-rw-r--r--   0        0        0     5842 2023-05-23 11:13:37.877331 psdm-analysis-0.1.4/psdm_analysis/models/result/power.py
+-rw-r--r--   0        0        0     4499 2023-05-23 11:13:37.878078 psdm-analysis-0.1.4/psdm_analysis/models/result/res_container.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.4/psdm_analysis/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:13:37.878152 psdm-analysis-0.1.4/psdm_analysis/plots/common/__init__.py
+-rw-r--r--   0        0        0     2431 2023-05-23 11:13:37.878287 psdm-analysis-0.1.4/psdm_analysis/plots/common/bar_plot.py
+-rw-r--r--   0        0        0     1103 2023-05-23 11:13:37.878583 psdm-analysis-0.1.4/psdm_analysis/plots/common/line_plot.py
+-rw-r--r--   0        0        0     5500 2023-05-25 08:03:08.060857 psdm-analysis-0.1.4/psdm_analysis/plots/common/utils.py
+-rw-r--r--   0        0        0     4128 2023-05-23 11:13:37.879462 psdm-analysis-0.1.4/psdm_analysis/plots/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.4/psdm_analysis/plots/results/__init__.py
+-rw-r--r--   0        0        0     6143 2023-05-23 11:13:37.879649 psdm-analysis-0.1.4/psdm_analysis/plots/results/connector_plot.py
+-rw-r--r--   0        0        0     3467 2023-05-23 11:13:37.880115 psdm-analysis-0.1.4/psdm_analysis/plots/results/flex_plot.py
+-rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.4/psdm_analysis/plots/results/nodes.py
+-rw-r--r--   0        0        0    11960 2023-05-23 11:13:37.880667 psdm-analysis-0.1.4/psdm_analysis/plots/results/power_plot.py
+-rw-r--r--   0        0        0     7726 2023-05-29 07:50:11.470993 psdm-analysis-0.1.4/psdm_analysis/plots/results/voltage_plot.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.4/psdm_analysis/processing/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-04 10:44:30.440027 psdm-analysis-0.1.4/psdm_analysis/processing/dataframe.py
+-rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.4/psdm_analysis/processing/series.py
+-rw-r--r--   0        0        0      789 2023-05-29 07:51:17.774103 psdm-analysis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 psdm-analysis-0.1.4/setup.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 psdm-analysis-0.1.4/PKG-INFO
```

### Comparing `psdm-analysis-0.1.3/LICENSE` & `psdm-analysis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/analysis/calc.py` & `psdm-analysis-0.1.4/psdm_analysis/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/analysis/grid.py` & `psdm-analysis-0.1.4/psdm_analysis/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/conversion/pandapower.py` & `psdm-analysis-0.1.4/psdm_analysis/conversion/pandapower.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/io/utils.py` & `psdm-analysis-0.1.4/psdm_analysis/io/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/entity.py` & `psdm-analysis-0.1.4/psdm_analysis/models/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List
+from typing import TYPE_CHECKING, List, Optional, Tuple, TypeVar, Union
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from psdm_analysis.io import utils
 from psdm_analysis.io.utils import df_to_csv, read_csv, to_date_time
 from psdm_analysis.models.input.enums import (
     EntitiesEnum,
     RawGridElementsEnum,
     SystemParticipantsEnum,
 )
 from psdm_analysis.models.input.participant.charging import parse_evcs_type_info
 from psdm_analysis.processing.dataframe import filter_data_for_time_interval
 
+if TYPE_CHECKING:
+    from psdm_analysis.models.input.node import Nodes
+
+EntityType = TypeVar("EntityType", bound="Entities")
+
 
 @dataclass(frozen=True)
 class Entities(ABC):
     data: DataFrame
 
     def __len__(self):
         return len(self.data)
@@ -134,38 +141,83 @@
         return ["uuid", "id", "operates_from", "operates_until", "operator"]
 
     @classmethod
     def create_empty(cls):
         data = pd.DataFrame(columns=cls.attributes())
         return cls(data)
 
+    def subset(self, uuids: Union[list[str], str]):
+        if isinstance(uuids, str):
+            uuids = [uuids]
+        return type(self)(self.data.loc[uuids])
+
+    def subset_split(self, uuids: list[str]):
+        rmd = set(self.uuids) - set(uuids)
+        return self.subset(uuids), self.subset(list(rmd))
+
+    @abstractmethod
+    def nodes(self):
+        pass
+
+    def filter_for_node(self, uuid: str):
+        data = self.data[self.nodes() == str(uuid)]
+        return type(self)(data)
+
+    def find_nodes(self, nodes: Nodes) -> Nodes:
+        return nodes.subset(self.nodes())
+
+
+ResultType = TypeVar("ResultType", bound="ResultEntities")
+
 
 @dataclass(frozen=True)
 class ResultEntities(ABC):
     # todo: type is a reserved keyword -> rename
     type: EntitiesEnum
-    name: str
     input_model: str
+    name: Optional[str]
     data: DataFrame
 
     def __repr__(self):
         return self.data
 
     def __len__(self):
         return len(self.data)
 
-    def __getitem__(self, slice_val: slice):
-        if not isinstance(slice_val, slice):
-            raise ValueError("Only slicing is supported!")
-        start, stop, step = slice_val.start, slice_val.stop, slice_val.step
-        if step is not None:
-            logging.warning("Step is not supported for slicing. Ignoring it.")
-        if not (isinstance(start, datetime) and isinstance(stop, datetime)):
-            raise ValueError("Only datetime slicing is supported")
-        return self.filter_for_time_interval(start, stop)
+    def __getitem__(self, where: Union[slice, datetime, list[datetime]]):
+        if isinstance(where, slice):
+            start, stop, step = where.start, where.stop, where.step
+            if step is not None:
+                logging.warning("Step is not supported for slicing. Ignoring it.")
+            if not (isinstance(start, datetime) and isinstance(stop, datetime)):
+                raise ValueError("Only datetime slicing is supported")
+            return self.filter_for_time_interval(start, stop)
+        elif isinstance(where, datetime):
+            filtered, dt = self._get_data_by_datetime(where)
+            data = pd.DataFrame(filtered).T
+            return self.build(self.type, self.input_model, data, dt, self.name)
+        elif isinstance(where, list):
+            filtered = [self._get_data_by_datetime(time)[0] for time in where]
+            data = pd.DataFrame(pd.concat(filtered, axis=1)).T
+            max_dt = sorted(data.index)[-1]
+            return self.build(self.type, self.input_model, data, max_dt, name=self.name)
+
+    def _get_data_by_datetime(self, dt: datetime) -> Tuple[Series, datetime]:
+        if dt > self.data.index[-1]:
+            logging.warning(
+                "Trying to access data after last time step. Returning last time step."
+            )
+            return self.data.iloc[-1], self.data.index[-1]
+        if dt < self.data.index[0]:
+            logging.warning(
+                "Trying to access data before first time step. Returning first time step."
+            )
+            return self.data.iloc[0], self.data.index[0]
+        else:
+            return self.data.asof(dt), dt
 
     @staticmethod
     @abstractmethod
     def attributes() -> List[str]:
         pass
 
     @classmethod
@@ -173,51 +225,60 @@
         return (
             pd.DataFrame(columns=cls.attributes(), index=index)
             if index
             else pd.DataFrame(columns=cls.attributes())
         )
 
     @classmethod
-    def create_empty(cls, entity_type: EntitiesEnum, name: str, input_model: str):
+    def create_empty(
+        cls, entity_type: EntitiesEnum, name: Optional[str], input_model: str
+    ):
         data = cls.empty_data()
-        return cls(entity_type, name, input_model, data)
+        return cls(entity_type, input_model, name, data)
 
     @classmethod
     def build(
         cls,
         entity_type: EntitiesEnum,
         input_model: str,
         data: DataFrame,
         end: datetime,
-        name: str = "",
+        name: Optional[str] = None,
     ) -> "ResultEntities":
         if data.empty:
             return cls.create_empty(entity_type, name, input_model)
 
         if "time" in data.columns:
             data["time"] = data["time"].apply(
                 lambda date_string: to_date_time(date_string)
             )
             data = data.set_index("time", drop=True)
+
         last_state = data.iloc[len(data) - 1]
         if last_state.name != end:
             last_state.name = end
             data = pd.concat([data, DataFrame(last_state).transpose()])
         # todo: deal with duplicate indexes -> take later one
         data = data[~data.index.duplicated(keep="last")]
-        return cls(entity_type, name, input_model, data)
+        data.sort_index(inplace=True)
+        return cls(entity_type, input_model, name, data)
 
     def filter_for_time_interval(self, start: datetime, end: datetime):
         filtered_data = filter_data_for_time_interval(self.data, start, end)
         return self.build(self.type, self.input_model, filtered_data, end, self.name)
 
     @classmethod
     # todo: find a way for parallel calculation
-    def sum(cls, results: List["ResultEntities"]) -> "ResultEntities":
+    def sum(cls, results: list[ResultType]) -> ResultType:
         if len(results) == 0:
             return cls.create_empty(SystemParticipantsEnum.PARTICIPANTS_SUM, "", "")
         if len(results) == 1:
             return results[0]
         agg = results[0]
         for result in results[1::]:
             agg += result
         return agg
+
+    def find_input_entity(self, input_model: EntityType):
+        if self.type != input_model.get_enum():
+            logging.warning("Input model type does not match result type!")
+        return input_model.subset([self.input_model])
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/grid_with_results.py` & `psdm-analysis-0.1.4/psdm_analysis/models/grid_with_results.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import concurrent
 import logging
+from concurrent.futures import ProcessPoolExecutor
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 from psdm_analysis.io.utils import check_filter
 from psdm_analysis.models.input.container.grid_container import GridContainer
 from psdm_analysis.models.input.container.participants_container import (
     SystemParticipantsContainer,
 )
 from psdm_analysis.models.input.enums import RawGridElementsEnum, SystemParticipantsEnum
+from psdm_analysis.models.result.grid.connector import ConnectorsResult
 from psdm_analysis.models.result.grid.enhanced_node import EnhancedNodesResult
 from psdm_analysis.models.result.grid.node import NodesResult
+from psdm_analysis.models.result.grid.transformer import Transformers2WResult
 from psdm_analysis.models.result.participant.participant import ParticipantsResult
 from psdm_analysis.models.result.participant.participants_res_container import (
     ParticipantsResultContainer,
 )
 from psdm_analysis.models.result.res_container import ResultContainer
 
 
@@ -29,15 +33,14 @@
         name: str,
         grid_path: str,
         grid_delimiter: str,
         result_path: str,
         result_delimiter: str,
         primary_data_delimiter: Optional[str] = None,
         simulation_end: Optional[datetime] = None,
-        from_agg_results: bool = False,
         filter_start: Optional[datetime] = None,
         filter_end: Optional[datetime] = None,
     ) -> "GridWithResults":
         check_filter(filter_start, filter_end)
 
         if not primary_data_delimiter:
             primary_data_delimiter = grid_delimiter
@@ -50,15 +53,15 @@
             raise ValueError(f"Grid is empty. Is the path correct? {grid_path}")
 
         results = ResultContainer.from_csv(
             name,
             result_path,
             result_delimiter,
             simulation_end,
-            from_agg_results,
+            grid_container=grid,
             filter_start=filter_start,
             filter_end=filter_end,
         )
 
         if not results:
             raise ValueError(f"Results are empty. Is the path correct? {result_path}")
 
@@ -88,14 +91,18 @@
         participants = self.results.participants.subset(participants_uuids)
         return ResultContainer(
             name=node_uuid,
             nodes=NodesResult(
                 RawGridElementsEnum.NODE,
                 {node_uuid: self.results.nodes.entities[node_uuid]},
             ),
+            lines=ConnectorsResult.create_empty(RawGridElementsEnum.LINE),
+            transformers_2w=Transformers2WResult.create_empty(
+                RawGridElementsEnum.TRANSFORMER_2_W
+            ),
             participants=participants,
         )
 
     # todo: this is not used so might be deleted
     @staticmethod
     def _safe_get_result(
         participant: SystemParticipantsEnum,
@@ -134,24 +141,41 @@
                 self.grid.participants.subset(connected_assets + [em_uuid]),
                 self.results.participants.subset(connected_assets + [em_uuid]),
             )
             for (em_uuid, connected_assets) in uuid_to_connected_asset.items()
         ]
 
     def build_enhanced_nodes_result(self):
-        ps, qs = {}, {}
-        for uuid, nodal_result in self.nodal_results().items():
-            ps[uuid] = nodal_result.participants.p_sum()
-            qs[uuid] = nodal_result.participants.q_sum()
-        return EnhancedNodesResult.from_nodes_result(self.results.nodes, ps, qs)
+        nodal_results = self.nodal_results()
+
+        with ProcessPoolExecutor() as executor:
+            futures = {
+                executor.submit(self.calc_pq, uuid, nodal_result)
+                for uuid, nodal_result in nodal_results.items()
+            }
+
+            nodal_pq = {}
+            for future in concurrent.futures.as_completed(futures):
+                uuid, pq = future.result()
+                nodal_pq[uuid] = pq
+
+        return EnhancedNodesResult.from_nodes_result(self.results.nodes, nodal_pq)
+
+    @staticmethod
+    def calc_pq(uuid, nodal_result: ResultContainer):
+        pq = nodal_result.participants.sum()
+        return uuid, pq
 
     def find_participant_result_pair(self, uuid: str):
         return self.grid.participants.find_participant(
             uuid
         ), self.results.participants.find_participant_result(uuid)
 
+    def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
+        return GridWithResults(
+            self.grid.filter_by_date_time(time), self.results.filter_by_date_time(time)
+        )
+
     def filter_for_time_interval(self, start: datetime, end: datetime):
-        nodes_res = self.results.nodes.filter_for_time_interval(start, end)
-        participant_res = self.results.participants.filter_for_time_interval(start, end)
         return GridWithResults(
-            self.grid, ResultContainer(self.results.name, nodes_res, participant_res)
+            self.grid, self.results.filter_for_time_interval(start, end)
         )
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/lines.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/connector/lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 from dataclasses import dataclass
 from typing import List
 
 from pandas import DataFrame, Series
 
-from psdm_analysis.models.entity import Entities
+from psdm_analysis.models.input.connector.connector import Connector
 from psdm_analysis.models.input.container.mixins import HasTypeMixin
 from psdm_analysis.models.input.enums import RawGridElementsEnum
 
 
 @dataclass(frozen=True)
-class Lines(Entities, HasTypeMixin):
+class Lines(Connector, HasTypeMixin):
     data: DataFrame
 
     @staticmethod
     def get_enum() -> RawGridElementsEnum:
         return RawGridElementsEnum.LINE
 
     @property
-    def node_a(self) -> Series:
-        return self.data["node_a"]
-
-    @property
-    def node_b(self) -> Series:
-        return self.data["node_b"]
-
-    @property
-    def parallel_devices(self) -> Series:
-        return self.data["parallel_devices"]
-
-    @property
     def length(self) -> Series:
         return self.data["length"]
 
     @property
     def geo_position(self) -> Series:
         return self.data["geo_position"]
 
@@ -78,10 +66,10 @@
     def aggregated_line_length(self) -> float:
         return self.data["length"].sum()
 
     def relative_line_length(self) -> float:
         return self.data["length"] / len(self.data)
 
     def find_lines_by_nodes(self, node_uuids):
-        return self.data[
-            (self.node_a.isin(node_uuids)) | (self.node_b.isin(node_uuids))
-        ]
+        return Lines(
+            self.data[(self.node_a.isin(node_uuids)) | (self.node_b.isin(node_uuids))]
+        )
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/switches.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,65 @@
 from dataclasses import dataclass
+from typing import List
 
 from pandas import DataFrame
 
 from psdm_analysis.models.entity import Entities
-from psdm_analysis.models.input.enums import EntitiesEnum, RawGridElementsEnum
+from psdm_analysis.models.input.enums import RawGridElementsEnum
 
 
 @dataclass(frozen=True)
-class Switches(Entities):
+class Nodes(Entities):
     data: DataFrame
 
     @staticmethod
-    def get_enum() -> EntitiesEnum:
-        return RawGridElementsEnum.SWITCH
+    def get_enum() -> RawGridElementsEnum:
+        return RawGridElementsEnum.NODE
+
+    @staticmethod
+    def attributes() -> List[str]:
+        return Entities.attributes() + [
+            "v_rated",
+            "v_target",
+            "slack",
+            "geo_position",
+            "volt_lvl",
+            "subnet",
+        ]
+
+    @property
+    def geo_position(self):
+        return self.data["geo_position"]
+
+    @property
+    def longitude(self):
+        return self.data["longitude"]
+
+    @property
+    def latitude(self):
+        return self.data["latitude"]
+
+    @property
+    def slack(self):
+        return self.data["slack"]
 
     @property
-    def node_a(self):
-        return self.data["node_a"]
+    def subnet(self):
+        return self.data["subnet"]
 
     @property
-    def node_b(self):
-        return self.data["node_b"]
+    def v_rated(self):
+        return self.data["v_rated"]
 
     @property
-    def closed(self):
-        return self.data["closed"]
+    def v_target(self):  # in kV
+        return self.data["v_target"]
+
+    @property
+    def volt_lvl(self):
+        return self.data["volt_lvl"]
+
+    def get_slack_nodes(self):
+        return Nodes(self.data[self.slack])
+
+    def nodes(self):
+        return self.data.index
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/connector/transformer.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/connector/transformer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 from dataclasses import dataclass
 
 from pandas import DataFrame
 
-from psdm_analysis.models.entity import Entities
+from psdm_analysis.models.input.connector.connector import Connector
 from psdm_analysis.models.input.container.mixins import HasTypeMixin
 from psdm_analysis.models.input.enums import RawGridElementsEnum
 
 
 @dataclass(frozen=True)
-class Transformers2W(Entities, HasTypeMixin):
+class Transformers2W(Connector, HasTypeMixin):
     data: DataFrame
 
     @property
-    def node_a(self):
-        return self.data["node_a"]
-
-    @property
-    def node_b(self):
-        return self.data["node_b"]
-
-    @property
-    def parallel_devices(self):
-        return self.data["parallel_devices"]
-
-    @property
     def type_id(self):
         return self.data["type_id"]
 
     @property
     def tap_pos(self):
         return self.data["tap_pos"]
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/container/mixins.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/container/mixins.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/container/participants_container.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/container/participants_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from dataclasses import dataclass
 
 import pandas as pd
 
 from psdm_analysis.models.input.container.mixins import ContainerMixin
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.bm import BiomassPlants
@@ -98,30 +99,33 @@
         )
 
     def get_participants(self, sp_type: SystemParticipantsEnum):
         if sp_type == SystemParticipantsEnum.ENERGY_MANAGEMENT:
             return self.ems
         elif sp_type == SystemParticipantsEnum.LOAD:
             return self.loads
+        elif sp_type == SystemParticipantsEnum.BIOMASS_PLANT:
+            return self.biomass_plants
         elif sp_type == SystemParticipantsEnum.FIXED_FEED_IN:
             return self.fixed_feed_ins
         elif sp_type == SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
             return self.pvs
         elif sp_type == SystemParticipantsEnum.WIND_ENERGY_CONVERTER:
             return self.wecs
         elif sp_type == SystemParticipantsEnum.STORAGE:
             return self.storages
         elif sp_type == SystemParticipantsEnum.EV_CHARGING_STATION:
             return self.evcs
-        elif sp_type == SystemParticipantsEnum.HEATP_PUMP:
+        elif sp_type == SystemParticipantsEnum.ELECTRIC_VEHICLE:
+            return self.evs
+        elif sp_type == SystemParticipantsEnum.HEAT_PUMP:
             return self.hps
         else:
-            raise ValueError(
-                f"No return value for system participant of type: {sp_type}"
-            )
+            logging.error(f"No return value for system participant of type: {sp_type}")
+            return None
 
     def find_participant(self, uuid: str):
         if uuid in self.loads:
             return self.loads.get(uuid)
         elif uuid in self.fixed_feed_ins:
             return self.fixed_feed_ins.get(uuid)
         elif uuid in self.pvs:
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/node.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/load.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 from dataclasses import dataclass
 from typing import List
 
-from pandas import DataFrame
-
-from psdm_analysis.models.entity import Entities
-from psdm_analysis.models.input.enums import RawGridElementsEnum
+from psdm_analysis.models.input.enums import SystemParticipantsEnum
+from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
-class Nodes(Entities):
-    data: DataFrame
-
+class Loads(SystemParticipants):
     @staticmethod
-    def get_enum() -> RawGridElementsEnum:
-        return RawGridElementsEnum.NODE
-
-    @staticmethod
-    def attributes() -> List[str]:
-        return super().attributes() + [
-            "v_target",
-            "slack",
-            "geo_position",
-            "volt_lvl",
-            "subnet",
-        ]
+    def get_enum() -> SystemParticipantsEnum:
+        return SystemParticipantsEnum.LOAD
 
     @property
-    def geo_position(self):
-        return self.data["geo_position"]
+    def s_rated(self):
+        return self.data["s_rated"]
 
     @property
-    def longitude(self):
-        return self.data["longitude"]
+    def standard_load_profile(self):
+        return self.data["standard_load_profile"]
 
     @property
-    def latitude(self):
-        return self.data["latitude"]
+    def e_cons_annual(self):
+        return self.data["e_cons_annual"]
 
     @property
-    def slack(self):
-        return self.data["slack"]
+    def cosphi_rated(self):
+        return self.data["cosphi_rated"]
 
-    @property
-    def subnet(self):
-        return self.data["subnet"]
-
-    @property
-    def volt_lvl(self):
-        return self.data["volt_lvl"]
-
-    def get_slack_nodes(self):
-        return Nodes(self.data[self.slack])
+    @staticmethod
+    def attributes() -> List[str]:
+        return SystemParticipants.attributes() + [
+            "standard_load_profile",
+            "e_cons_annual",
+            "s_rated",
+            "cosphi_rated",
+        ]
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/bm.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/bm.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/charging.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/charging.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/em.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/em.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evcs.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evcs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/evs.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/fixed_feed_in.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/fixed_feed_in.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/hp.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/hp.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class HeatPumps(SystemParticipants, SpTypeMixin):
     @staticmethod
     def get_enum() -> SystemParticipantsEnum:
-        return SystemParticipantsEnum.HEATP_PUMP
+        return SystemParticipantsEnum.HEAT_PUMP
 
     @property
     def thermal_bus(self):
         return self.data["thermal_bus"]
 
     @property
     def p_thermal(self):
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/load.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/pv.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,55 @@
 from typing import List
 
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
-class Loads(SystemParticipants):
+class PhotovoltaicPowerPlants(SystemParticipants):
     @staticmethod
     def get_enum() -> SystemParticipantsEnum:
-        return SystemParticipantsEnum.LOAD
+        return SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT
 
     @property
     def s_rated(self):
         return self.data["s_rated"]
 
     @property
-    def standard_load_profile(self):
-        return self.data["standard_load_profile"]
+    def albedo(self):
+        return self.data["albedo"]
 
     @property
-    def e_cons_annual(self):
-        return self.data["e_cons_annual"]
+    def azimuth(self):
+        return self.data["azimuth"]
 
     @property
-    def cosphi_rated(self):
-        return self.data["cosphi_rated"]
+    def elevation_angle(self):
+        return self.data["elevation_angle"]
+
+    @property
+    def k_g(self):
+        return self.data["k_g"]
+
+    @property
+    def k_t(self):
+        return self.data["k_t"]
+
+    @property
+    def market_reaction(self):
+        return self.data["market_reaction"]
+
+    @property
+    def cos_phi_rated(self):
+        return self.data["cos_phi_rated"]
 
     @staticmethod
     def attributes() -> List[str]:
         return SystemParticipants.attributes() + [
-            "standard_load_profile",
-            "e_cons_annual",
-            "s_rated",
-            "cosphi_rated",
+            "albedo",
+            "azimuth",
+            "elevation_angle",
+            "k_g",
+            "k_t",
+            "market_reaction",
+            "cos_phi_rated",
         ]
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/participant.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/participant.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 from psdm_analysis.models.entity import Entities
+from psdm_analysis.models.input.node import Nodes
 
 
 @dataclass(frozen=True)
-class SystemParticipants(Entities):
+class SystemParticipants(Entities, ABC):
     @staticmethod
     def attributes():
         return Entities.attributes() + ["node", "q_characteristics"]
 
     def nodes(self):
         return self.data["node"]
 
     def q_characteristics(self):
         return self.data["q_characteristic"]
 
-    def filter_for_node(self, uuid: str):
-        data = self.data[self.nodes() == str(uuid)]
-        return type(self)(data)
-
-    def subset(self, uuids: [str]):
+    def subset(self, uuids: list[str]):
         data = self.data.loc[self.data.index.intersection(uuids)]
         return type(self)(data)
 
+    def insert_node_id_columns(self, nodes: Nodes) -> None:
+        index_to_id = nodes.ids.to_dict()
+
+        if "node_id" not in self.data.columns:
+            self.data.insert(self.data.columns.get_loc("node") + 1, "node_id", None)
+        self.data["node_id"] = self.nodes().map(index_to_id)
+
 
 @dataclass(frozen=True)
 class SystemParticipantsWithCapacity(SystemParticipants):
     @staticmethod
     @abstractmethod
     def capacity_attribute() -> str:
         pass
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/storage.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/storage.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/input/participant/wec.py` & `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/wec.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/flex_option.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/flex_option.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/grid/enhanced_node.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/grid/connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,106 @@
+from __future__ import annotations
+
+import math
 from dataclasses import dataclass
+from typing import List
 
+import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 
-from psdm_analysis.models.input.enums import RawGridElementsEnum
-from psdm_analysis.models.result.grid.node import NodeResult, NodesResult
+from psdm_analysis.models.entity import ResultEntities
+from psdm_analysis.models.result.grid.node import NodeResult
+from psdm_analysis.models.result.participant.dict import ResultDict
 
 
 @dataclass(frozen=True)
-class EnhancedNodeResult(NodeResult):
-    def __eq__(self, other):
-        if not isinstance(other, EnhancedNodeResult):
-            return False
-        return (
-            (self.input_model == other.input_model)
-            & (self.name == other.name)
-            & (self.data.equals(other.data))
-        )
+class ConnectorResult(ResultEntities):
+    @staticmethod
+    def attributes() -> List[str]:
+        return ["i_a_ang", "i_a_mag", "i_b_ang", "i_b_mag"]
 
-    @classmethod
-    def from_node_result(
-        cls, node_res: NodeResult, p: Series, q: Series = None
-    ) -> "EnhancedNodeResult":
-        return cls(
-            RawGridElementsEnum.NODE,
-            node_res.name,
-            node_res.input_model,
-            pd.concat(
-                [node_res.data, p.rename("p"), q.rename("q")], axis=1
-            ).sort_index(),
-        )
+    @property
+    def i_a_ang(self) -> Series:
+        return self.data["i_a_ang"]
+
+    @property
+    def i_a_mag(self) -> Series:
+        return self.data["i_a_mag"]
+
+    @property
+    def i_a_complex(self) -> Series:
+        return self.i_a_mag * np.exp(1j * np.radians(self.i_a_ang))
 
     @property
-    def p(self) -> Series:
-        return self.data["p"]
+    def i_b_ang(self) -> Series:
+        return self.data["i_b_ang"]
 
     @property
-    def q(self) -> Series:
-        return self.data["q"]
+    def i_b_mag(self) -> Series:
+        return self.data["i_b_mag"]
+
+    @property
+    def i_b_complex(self) -> Series:
+        return self.i_b_mag * np.exp(1j * np.radians(self.i_b_ang))
+
+    # todo: Check if calculation is correct
+    def calc_rated_power(
+        self, node_res: NodeResult, voltage_level_kv: float, node="a", absolute=True
+    ):  # in kVA
+        s_rated_fn = (
+            lambda i_complex: math.sqrt(3)
+            * node_res.v_complex(voltage_level_kv)
+            * np.conj(i_complex)
+        )
+        if node == "a":
+            res = s_rated_fn(self.i_a_complex)
+        elif node == "b":
+            res = s_rated_fn(self.i_b_complex)
+        else:
+            raise ValueError("Node must be either hv or lv")
+        return np.absolute(res) if absolute else res
 
 
 @dataclass(frozen=True)
-class EnhancedNodesResult(NodesResult):
-    entities: dict[str, EnhancedNodeResult]
+class ConnectorsResult(ResultDict):
+    entities: dict[str, ConnectorResult]
 
-    @classmethod
-    def from_nodes_result(
-        cls, nodes_result: NodesResult, ps: dict[str, Series], qs: dict[str, Series]
-    ):
-        return cls(
-            RawGridElementsEnum.NODE,
-            {
-                uuid: EnhancedNodeResult.from_node_result(result, ps[uuid], qs[uuid])
-                for uuid, result in nodes_result.entities.items()
-            },
+    @property
+    def i_a_ang(self) -> DataFrame:
+        return pd.concat(
+            [
+                node_res.i_a_ang.rename(node_res.input_model)
+                for node_res in self.entities.values()
+            ],
+            axis=1,
+        )
+
+    @property
+    def i_a_mag(self) -> DataFrame:
+        return pd.concat(
+            [
+                node_res.i_a_mag.rename(node_res.input_model)
+                for node_res in self.entities.values()
+            ],
+            axis=1,
         )
 
     @property
-    def p(self) -> DataFrame:
-        return (
-            pd.concat(
-                [
-                    node_res.p.rename(node_res.input_model)
-                    for node_res in self.entities.values()
-                ],
-                axis=1,
-            )
-            .sort_index()
-            .ffill()
-            .fillna(0)
+    def i_b_ang(self) -> DataFrame:
+        return pd.concat(
+            [
+                node_res.i_b_ang.rename(node_res.input_model)
+                for node_res in self.entities.values()
+            ],
+            axis=1,
         )
 
     @property
-    def q(self) -> DataFrame:
-        return (
-            pd.concat(
-                [
-                    node_res.q.rename(node_res.input_model)
-                    for node_res in self.entities.values()
-                ],
-                axis=1,
-            )
-            .sort_index()
-            .ffill()
-            .fillna(0)
+    def i_b_mag(self) -> DataFrame:
+        return pd.concat(
+            [
+                node_res.i_b_mag.rename(node_res.input_model)
+                for node_res in self.entities.values()
+            ],
+            axis=1,
         )
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/flex_options.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/flex_options.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participant.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/power.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,193 +1,178 @@
-import logging
-import os.path
-import uuid
+import dataclasses
+import os
+import re
 from dataclasses import dataclass
-from datetime import datetime
-from typing import Dict
+from functools import reduce
+from typing import List, Tuple, Union
 
 import pandas as pd
-from pandas import DataFrame, Series
+from pandas import Series
 
-from psdm_analysis.models.input.enums import SystemParticipantsEnum
-from psdm_analysis.models.input.participant.participant import (
-    SystemParticipantsWithCapacity,
+from psdm_analysis.io.utils import get_absolute_path
+from psdm_analysis.models.entity import ResultEntities
+from psdm_analysis.models.input.enums import EntitiesEnum, SystemParticipantsEnum
+from psdm_analysis.processing.dataframe import divide_positive_negative
+from psdm_analysis.processing.series import (
+    add_series,
+    duration_weighted_sum,
+    hourly_mean_resample,
+    load_and_generation,
 )
-from psdm_analysis.models.result.participant.dict import ResultDict
-from psdm_analysis.models.result.power import PQResult, PQWithSocResult
-from psdm_analysis.processing.dataframe import join_dataframes
 
 
 @dataclass(frozen=True)
-class ParticipantsResult(ResultDict):
-    entities: Dict[str, PQResult]
+class PQResult(ResultEntities):
+    def __add__(self, other: "PQResult"):
+        p_sum = add_series(self.p, other.p, "p")
+        q_sum = add_series(self.q, other.q, "q")
+        summed_data = p_sum.to_frame().join(q_sum)
+        return PQResult(
+            self.type
+            if self.type == other.type
+            else SystemParticipantsEnum.PARTICIPANTS_SUM,
+            "PQResult - Sum",
+            "PQResult - Sum",
+            summed_data,
+        )
 
-    @classmethod
-    def from_csv(
-        cls,
-        entity_type: SystemParticipantsEnum,
-        simulation_data_path: str,
-        delimiter: str,
-        simulation_end: datetime,
-        from_agg_res: bool = False,
-    ) -> "ParticipantsResult":
-        if from_agg_res:
-            path = ResultDict.safe_get_path(entity_type, simulation_data_path)
-            if not path:
-                return cls.create_empty(entity_type)
-            agg_res = pd.read_csv(path)
-            agg_res["time"] = pd.to_datetime(agg_res["time"])
-            agg_res = agg_res.set_index("time", drop=True)
-            if "q" not in agg_res.columns:
-                agg_res["q"] = 0
-            agg_pq = PQResult(
-                entity_type, "aggregated_result", "aggregated_result", agg_res
-            )
-            return ParticipantsResult(entity_type, {"aggregated": agg_pq})
+    def __sub__(self, other: "PQResult"):
+        return self + (other * -1)
 
+    def __mul__(self, other: Union[float, int]):
+        if isinstance(other, float) or isinstance(other, int):
+            updated_data = self.data * other
+            return PQResult(self.type, self.input_model, self.name, updated_data)
         else:
-            participant_grpd_df = ResultDict.get_grpd_df(
-                entity_type,
-                simulation_data_path,
-                delimiter,
-            )
-            if not participant_grpd_df:
-                logging.debug("There are no " + str(cls))
-                return cls.create_empty(entity_type)
-            entities = dict(
-                participant_grpd_df.apply(
-                    lambda grp: PQResult.build(
-                        entity_type,
-                        grp.name,
-                        grp.drop(columns=["input_model"]),
-                        simulation_end,
-                    )
-                )
-            )
-            return cls(
-                entity_type,
-                entities,
+            raise ValueError(
+                f"Multiplication with type {type(other)} not or not yet supported"
             )
 
-    def to_csv(self, path: str, resample_rate: str = None):
-        file_name = self.entity_type.get_csv_result_file_name()
+    # commutative multiplication (a*b=b*a)
+    __rmul__ = __mul__
 
-        def resample(data: DataFrame, input_model: str):
-            data = (
-                data.resample("60s").ffill().resample(resample_rate).mean()
-                if resample_rate
-                else data
-            )
-            data["uuid"] = data.apply(lambda _: uuid.uuid4(), axis=1)
-            data["input_model"] = input_model
-            return data
-
-        resampled = [
-            resample(participant.data, input_model)
-            for input_model, participant in self.entities.items()
-        ]
-        df = join_dataframes(resampled)
-        df.to_csv(os.path.join(path, file_name))
-
-    def nodal_results(self, node_uuid: str) -> "ParticipantsResult":
-        pass
-
-    def get(self, key: str) -> PQResult:
-        return self.entities[key]
-
-    def subset(self, uuids):
-        return type(self)(
-            self.entity_type,
-            {uuid: self.entities[uuid] for uuid in self.entities.keys() & uuids},
+    def __eq__(self, other):
+        if not isinstance(other, PQResult):
+            return False
+        return (self.data == other.data).all()
+
+    @classmethod
+    def from_csv(cls, file_path: str, sp_type: EntitiesEnum, name: str = None):
+        file_path = get_absolute_path(file_path)
+        data = pd.read_csv(file_path)
+        data["time"] = pd.to_datetime(data["time"])
+        data = data.set_index("time", drop=True)
+        file_name = os.path.basename(file_path)
+        is_default_file_name = re.match(
+            f"{sp_type.get_csv_result_file_name()}_.*", file_name
         )
+        input_model = file_name.split("_")[-1] if is_default_file_name else file_name
+        return cls(sp_type, name if name else input_model, input_model, data)
+
+    def to_csv(self, path: str, file_name: str = None, delimiter: str = ","):
+        file_name = file_name if file_name else self.get_default_output_name()
+        self.data.to_csv(os.path.join(path, file_name), sep=delimiter)
+
+    def get_default_output_name(self):
+        return self.input_model + "_" + self.type.get_csv_result_file_name()
 
     @property
     def p(self):
-        if not self.entities.values():
-            return None
-        return (
-            pd.DataFrame({p_uuid: res.p for p_uuid, res in self.entities.items()})
-            .fillna(method="ffill")
-            .sort_index()
-        )
-
-    def sum(self) -> PQResult:
-        return PQResult.sum(list(self.entities.values()))
-
-    def p_sum(self) -> Series:
-        if not self.entities:
-            return Series(dtype=float)
-        return self.p.fillna(method="ffill").sum(axis=1).rename("p_sum")
+        return self.data["p"]
 
     @property
     def q(self):
+        return self.data["q"]
+
+    @staticmethod
+    def attributes() -> List[str]:
+        return ["p", "q"]
+
+    @classmethod
+    # todo: find a way for parallel calculation
+    def sum(cls, results: List["PQResult"]) -> "PQResult":
+        if len(results) == 0:
+            return PQResult.create_empty(
+                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
+            )
+        if len(results) == 1:
+            return results[0]
+        return reduce(lambda a, b: a + b, results)
+
+    def energy(self) -> float:
+        return duration_weighted_sum(self.p)
+
+    def load_and_generation(self) -> Tuple[float, float]:
+        return load_and_generation(self.p)
+
+    def divide_load_generation(self):
+        load, generation = divide_positive_negative(self.data)
+        return dataclasses.replace(self, data=load), dataclasses.replace(
+            self, data=generation
+        )
+
+    def daily_usage(self, device_power_mw):
         return (
-            pd.DataFrame({p_uuid: res.q for p_uuid, res in self.entities.items()})
-            .fillna(method="ffill")
-            .sort_index()
-        )
-
-    def q_sum(self):
-        if not self.entities:
-            return Series(dtype=float)
-        return self.q.fillna(method="ffill").sum(axis=1).rename("q_sum")
-
-    def energy(self):
-        # todo make concurrent
-        sum = 0
-        for participant in self.entities.values():
-            sum += participant.energy()
-        return sum
+            self.p()
+            .groupby(self.p.index.date)
+            .apply(lambda series: duration_weighted_sum(series.abs()))
+            / device_power_mw
+        )
 
-    def load_and_generation(self):
-        return self.sum().load_and_generation()
+    def annual_duration_series(self, drop_index=True):
+        return (
+            hourly_mean_resample(self.p)
+            .sort_values(ascending=False)
+            .reset_index(drop=drop_index)
+        )
 
+    def hourly_resample(self):
+        updated_data = self.data.apply(lambda col: hourly_mean_resample(col), axis=0)
+        return PQResult(self.type, self.input_model, self.name, updated_data)
 
-@dataclass(frozen=True)
-class ParticipantsWithSocResult(ParticipantsResult):
-    entity_type: SystemParticipantsEnum
-    entities: Dict[str, PQWithSocResult]
+    def complex_power(self):
+        return self.p + 1j * self.q
 
-    @classmethod
-    def from_csv(
-        cls,
-        sp_type: SystemParticipantsEnum,
-        simulation_data_path: str,
-        delimiter: str,
-        simulation_end: datetime,
-        from_agg_res: bool = False,
-    ) -> "ParticipantsWithSocResult":
-        if from_agg_res:
-            raise ValueError(
-                "Aggregated results do not contain SOC information. Consider reading as `ParticipantsResult`"
-            )
 
-        participant_grpd_df = ResultDict.get_grpd_df(
-            sp_type,
-            simulation_data_path,
-            delimiter,
-        )
-
-        if not participant_grpd_df:
-            logging.debug(f"There are no {sp_type.value} results.")
-            return cls.create_empty(sp_type)
-
-        entities = dict(
-            participant_grpd_df.apply(
-                lambda grp: PQWithSocResult.build(
-                    sp_type,
-                    grp.name,
-                    grp.drop(columns=["input_model"]),
-                    simulation_end,
-                )
-            )
+@dataclass(frozen=True)
+class PQWithSocResult(PQResult):
+    def add_with_soc(
+        self, this_capacity: float, other: "PQWithSocResult", other_capacity: float
+    ):
+        p_sum = add_series(self.p, other.p, "p")
+        q_sum = add_series(self.q, other.q, "q")
+        total_capacity = this_capacity + other_capacity
+        soc = add_series(
+            self.soc() * this_capacity / total_capacity,
+            other.soc() * other_capacity / total_capacity,
+            "soc",
+        )
+        summed_data = p_sum.to_frame().join([q_sum, soc])
+        return PQWithSocResult(
+            self.type,
+            "PQResult - Sum",
+            "PQResult - Sum",
+            summed_data,
         )
-        return cls(sp_type, entities)
 
-    def sum_with_soc(self, inputs: SystemParticipantsWithCapacity) -> PQWithSocResult:
-        if not self.entities:
-            return PQWithSocResult.create_empty(self.entity_type, "", "")
-        capacity_participant = []
-        for participant_uuid, res in self.entities.items():
-            capacity = inputs.get(participant_uuid)[inputs.capacity_attribute()]
-            capacity_participant.append((capacity, res))
-        return PQWithSocResult.sum_with_soc(capacity_participant)
+    @staticmethod
+    # todo: find a way for parallel calculation
+    def sum_with_soc(
+        results: list[Tuple[float, "PQWithSocResult"]]
+    ) -> "PQWithSocResult":
+        if len(results) == 0:
+            return PQWithSocResult.create_empty(
+                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
+            )
+        if len(results) == 1:
+            return results[0][1]
+        this_capacity, agg = results[0]
+        for other_capacity, result in results[1::]:
+            agg = agg.add_with_soc(this_capacity, result, other_capacity)
+        return agg
+
+    def soc(self) -> Series:
+        return self.data["soc"]
+
+    @staticmethod
+    def attributes() -> List[str]:
+        return ["p", "q", "capacity"]
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/participant/participants_res_container.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participants_res_container.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import concurrent.futures
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
-from typing import Optional
+from typing import Optional, Union
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from psdm_analysis.io.utils import check_filter
+from psdm_analysis.models.input.container.grid_container import GridContainer
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.result.participant.flex_options import FlexOptionsResult
 from psdm_analysis.models.result.participant.participant import (
     ParticipantsResult,
     ParticipantsWithSocResult,
 )
 from psdm_analysis.models.result.power import PQResult
@@ -44,27 +45,27 @@
 
     @classmethod
     def from_csv(
         cls,
         simulation_data_path: str,
         delimiter: str,
         simulation_end: datetime,
-        from_agg_results: bool = False,
+        grid_container: Optional[GridContainer] = None,
         filter_start: Optional[datetime] = None,
         filter_end: Optional[datetime] = None,
     ):
         check_filter(filter_start, filter_end)
         with concurrent.futures.ProcessPoolExecutor() as executor:
             # warning: Breakpoints in the underlying method might not work when started from ipynb
             pa_from_csv_for_participant = partial(
                 ParticipantsResultContainer.from_csv_for_participant,
                 simulation_data_path,
                 delimiter,
                 simulation_end,
-                from_agg_results,
+                grid_container,
             )
             participant_results = executor.map(
                 pa_from_csv_for_participant,
                 filter(
                     lambda x: x != SystemParticipantsEnum.FLEX_OPTIONS,
                     SystemParticipantsEnum.values(),
                 ),
@@ -80,15 +81,15 @@
             fixed_feed_ins=participant_result_map[SystemParticipantsEnum.FIXED_FEED_IN],
             pvs=participant_result_map[SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT],
             wecs=participant_result_map[SystemParticipantsEnum.WIND_ENERGY_CONVERTER],
             storages=participant_result_map[SystemParticipantsEnum.STORAGE],
             ems=participant_result_map[SystemParticipantsEnum.ENERGY_MANAGEMENT],
             evcs=participant_result_map[SystemParticipantsEnum.EV_CHARGING_STATION],
             evs=participant_result_map[SystemParticipantsEnum.ELECTRIC_VEHICLE],
-            hps=participant_result_map[SystemParticipantsEnum.HEATP_PUMP],
+            hps=participant_result_map[SystemParticipantsEnum.HEAT_PUMP],
             flex=FlexOptionsResult.from_csv(
                 SystemParticipantsEnum.FLEX_OPTIONS,
                 simulation_data_path,
                 delimiter,
                 simulation_end,
             ),
         )
@@ -99,32 +100,36 @@
         )
 
     @staticmethod
     def from_csv_for_participant(
         simulation_data_path: str,
         delimiter: str,
         simulation_end: datetime,
-        from_agg_results: bool,
+        grid_container: Optional[GridContainer],
         participant: SystemParticipantsEnum,
     ):
-        if participant.has_soc() and not from_agg_results:
+        if grid_container:
+            input_entities = grid_container.participants.get_participants(participant)
+        else:
+            input_entities = None
+        if participant.has_soc():
             return ParticipantsWithSocResult.from_csv(
                 participant,
                 simulation_data_path,
                 delimiter,
                 simulation_end,
-                from_agg_results,
+                input_entities,
             )
         else:
             return ParticipantsResult.from_csv(
                 participant,
                 simulation_data_path,
                 delimiter,
                 simulation_end,
-                from_agg_results,
+                input_entities=input_entities,
             )
 
     def to_list(
         self, include_em: bool = True, include_flex=True, include_empty=True
     ) -> list[ParticipantsResult]:
         optional = []
         if include_em:
@@ -174,15 +179,15 @@
             return self.pvs
         elif sp_type == SystemParticipantsEnum.WIND_ENERGY_CONVERTER:
             return self.wecs
         elif sp_type == SystemParticipantsEnum.STORAGE:
             return self.storages
         elif sp_type == SystemParticipantsEnum.EV_CHARGING_STATION:
             return self.evcs
-        elif sp_type == SystemParticipantsEnum.HEATP_PUMP:
+        elif sp_type == SystemParticipantsEnum.HEAT_PUMP:
             return self.hps
         else:
             raise ValueError(
                 f"No return value for system participant of type: {sp_type}"
             )
 
     @property
@@ -236,14 +241,28 @@
 
     def sum(self) -> PQResult:
         participant_res = []
         for participant in self.to_list(include_em=False, include_flex=False):
             participant_res.append(participant.sum())
         return PQResult.sum(participant_res)
 
+    def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
+        return ParticipantsResultContainer(
+            self.ems.filter_by_date_time(time),
+            self.loads.filter_by_date_time(time),
+            self.fixed_feed_ins.filter_by_date_time(time),
+            self.pvs.filter_by_date_time(time),
+            self.wecs.filter_by_date_time(time),
+            self.storages.filter_by_date_time(time),
+            self.evcs.filter_by_date_time(time),
+            self.evs.filter_by_date_time(time),
+            self.hps.filter_by_date_time(time),
+            self.flex.filter_by_date_time(time),
+        )
+
     def filter_for_time_interval(self, start: datetime, end: datetime):
         return ParticipantsResultContainer(
             self.ems.filter_for_time_interval(start, end),
             self.loads.filter_for_time_interval(start, end),
             self.fixed_feed_ins.filter_for_time_interval(start, end),
             self.pvs.filter_for_time_interval(start, end),
             self.wecs.filter_for_time_interval(start, end),
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/models/result/power.py` & `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/dict.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,175 +1,200 @@
-import dataclasses
-import os
-import re
+import logging
+from abc import ABC
 from dataclasses import dataclass
-from functools import reduce
-from typing import List, Tuple, Union
+from datetime import datetime
+from typing import Dict, Optional, Type, TypeVar, Union
 
-import pandas as pd
-from pandas import Series
+from pandas import DataFrame
+from pandas.core.groupby import DataFrameGroupBy
 
-from psdm_analysis.io.utils import get_absolute_path
-from psdm_analysis.models.entity import ResultEntities
-from psdm_analysis.models.input.enums import EntitiesEnum, SystemParticipantsEnum
-from psdm_analysis.processing.dataframe import divide_positive_negative
-from psdm_analysis.processing.series import (
-    add_series,
-    duration_weighted_sum,
-    hourly_mean_resample,
-    load_and_generation,
+from psdm_analysis.io.utils import (
+    check_filter,
+    csv_to_grpd_df,
+    get_file_path,
+    to_date_time,
 )
+from psdm_analysis.models.entity import Entities, ResultEntities
+from psdm_analysis.models.input.enums import EntitiesEnum, EntityEnumType
 
+ResultDictType = TypeVar("ResultDictType", bound="ResultDict")
 
-@dataclass(frozen=True)
-class PQResult(ResultEntities):
-    def __add__(self, other: "PQResult"):
-        p_sum = add_series(self.p, other.p, "p")
-        q_sum = add_series(self.q, other.q, "q")
-        summed_data = p_sum.to_frame().join(q_sum)
-        return PQResult(
-            self.type
-            if self.type == other.type
-            else SystemParticipantsEnum.PARTICIPANTS_SUM,
-            "PQResult - Sum",
-            "PQResult - Sum",
-            summed_data,
-        )
-
-    def __sub__(self, other: "PQResult"):
-        return self + (other * -1)
-
-    def __mul__(self, other: Union[float, int]):
-        if isinstance(other, float) or isinstance(other, int):
-            updated_data = self.data * other
-            return PQResult(self.type, self.name, self.input_model, updated_data)
-        else:
-            raise ValueError(
-                f"Multiplication with type {type(other)} not or not yet supported"
-            )
-
-    # commutative multiplication (a*b=b*a)
-    __rmul__ = __mul__
-
-    def __eq__(self, other):
-        if not isinstance(other, PQResult):
-            return False
-        return (self.data == other.data).all()
-
-    @classmethod
-    def from_csv(cls, file_path: str, sp_type: EntitiesEnum, name: str = None):
-        file_path = get_absolute_path(file_path)
-        data = pd.read_csv(file_path)
-        data["time"] = pd.to_datetime(data["time"])
-        data = data.set_index("time", drop=True)
-        file_name = os.path.basename(file_path)
-        is_default_file_name = re.match(
-            f"{sp_type.get_csv_result_file_name()}_.*", file_name
-        )
-        input_model = file_name.split("_")[-1] if is_default_file_name else file_name
-        return cls(sp_type, name if name else input_model, input_model, data)
-
-    def to_csv(self, path: str, file_name: str = None, delimiter: str = ","):
-        file_name = file_name if file_name else self.get_default_output_name()
-        self.data.to_csv(os.path.join(path, file_name), sep=delimiter)
-
-    def get_default_output_name(self):
-        return self.input_model + "_" + self.type.get_csv_result_file_name()
-
-    @property
-    def p(self):
-        return self.data["p"]
-
-    @property
-    def q(self):
-        return self.data["q"]
 
-    @staticmethod
-    def attributes() -> List[str]:
-        return ["p", "q"]
+@dataclass(frozen=True)
+class ResultDict(ABC):
+    entity_type: EntitiesEnum
+    entities: Dict[str, ResultEntities]
+
+    def __len__(self):
+        return len(self.entities)
+
+    def __contains__(self, uuid):
+        return uuid in self.entities
+
+    def __getitem__(self, get):
+        match get:
+            case str():
+                return self.entities[get]
+            case slice():
+                start, stop, step = get.start, get.stop, get.step
+                if step is not None:
+                    logging.warning("Step is not supported for slicing. Ignoring it.")
+                if not (isinstance(start, datetime) and isinstance(stop, datetime)):
+                    raise ValueError("Only datetime slicing is supported")
+                entities = {
+                    key: e.filter_for_time_interval(start, stop)
+                    for key, e in self.entities.items()
+                }
+                return type(self)(self.entity_type, entities)
+            case _:
+                raise ValueError(
+                    "Only get by uuid or datetime slice for filtering is supported."
+                )
 
     @classmethod
-    # todo: find a way for parallel calculation
-    def sum(cls, results: List["PQResult"]) -> "PQResult":
-        if len(results) == 0:
-            return PQResult.create_empty(
-                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
+    def from_csv(
+        cls: Type[ResultDictType],
+        entity_type: EntityEnumType,
+        simulation_data_path: str,
+        delimiter: str,
+        simulation_end: Optional[datetime] = None,
+        input_entities: Optional[Entities] = None,
+        filter_start: Optional[datetime] = None,
+        filter_end: Optional[datetime] = None,
+    ) -> ResultDictType:
+        check_filter(filter_start, filter_end)
+        grpd_df = ResultDict.get_grpd_df(
+            entity_type,
+            simulation_data_path,
+            delimiter,
+        )
+        if not grpd_df:
+            logging.debug("There are no " + str(cls))
+            return cls.create_empty(entity_type)
+        if simulation_end is None:
+            simulation_end = to_date_time(grpd_df["time"].max().max())
+        entities = dict(
+            grpd_df.apply(
+                lambda grp: ResultDict.build_for_entity(
+                    entity_type,
+                    grp.name,
+                    grp.drop(columns=["input_model"]),
+                    simulation_end,
+                    input_entities=input_entities,
+                )
             )
-        if len(results) == 1:
-            return results[0]
-        return reduce(lambda a, b: a + b, results)
-
-    def energy(self) -> float:
-        return duration_weighted_sum(self.p)
-
-    def load_and_generation(self) -> Tuple[float, float]:
-        return load_and_generation(self.p)
-
-    def divide_load_generation(self):
-        load, generation = divide_positive_negative(self.data)
-        return dataclasses.replace(self, data=load), dataclasses.replace(
-            self, data=generation
         )
-
-    def daily_usage(self, device_power_mw):
-        return (
-            self.p()
-            .groupby(self.p.index.date)
-            .apply(lambda series: duration_weighted_sum(series.abs()))
-            / device_power_mw
+        res = cls(
+            entity_type,
+            entities,
         )
-
-    def annual_duration_series(self, drop_index=True):
         return (
-            hourly_mean_resample(self.p)
-            .sort_values(ascending=False)
-            .reset_index(drop=drop_index)
+            res
+            if not filter_start
+            else res.filter_for_time_interval(filter_start, filter_end)
         )
 
-    def hourly_resample(self):
-        updated_data = self.data.apply(lambda col: hourly_mean_resample(col), axis=0)
-        return PQResult(self.type, self.name, self.input_model, updated_data)
-
+    @staticmethod
+    def build_for_entity(
+        entity_type: EntityEnumType,
+        input_model: str,
+        data: DataFrame,
+        simulation_end: datetime,
+        input_entities=Optional[Entities],
+    ) -> ResultDictType:
+        name = None
+        if input_entities is not None:
+            if input_model not in input_entities.ids.index:
+                logging.debug(
+                    f"Input model {input_model} of type {entity_type} not found in input entities. It seems like the wrong input_entities have been passed. Not assigning a name to the result."
+                )
+            else:
+                name = input_entities.ids.loc[input_model]
 
-@dataclass(frozen=True)
-class PQWithSocResult(PQResult):
-    def add_with_soc(
-        self, this_capacity: float, other: "PQWithSocResult", other_capacity: float
-    ):
-        p_sum = add_series(self.p, other.p, "p")
-        q_sum = add_series(self.q, other.q, "q")
-        total_capacity = this_capacity + other_capacity
-        soc = add_series(
-            self.soc() * this_capacity / total_capacity,
-            other.soc() * other_capacity / total_capacity,
-            "soc",
-        )
-        summed_data = p_sum.to_frame().join([q_sum, soc])
-        return PQWithSocResult(
-            self.type,
-            "PQResult - Sum",
-            "PQResult - Sum",
-            summed_data,
+        return entity_type.get_result_type().build(
+            entity_type, input_model, data, simulation_end, name=name
         )
 
     @staticmethod
-    # todo: find a way for parallel calculation
-    def sum_with_soc(
-        results: list[Tuple[float, "PQWithSocResult"]]
-    ) -> "PQWithSocResult":
-        if len(results) == 0:
-            return PQWithSocResult.create_empty(
-                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
+    def get_grpd_df(
+        entity_type: EntityEnumType,
+        simulation_data_path: str,
+        delimiter: str,
+    ) -> Optional[DataFrameGroupBy]:
+        file_name = entity_type.get_csv_result_file_name()
+        path = get_file_path(simulation_data_path, file_name)
+
+        if not path.exists():
+            logging.info(
+                "No results built for {} since {} does not exist".format(
+                    file_name, str(path)
+                )
             )
-        if len(results) == 1:
-            return results[0][1]
-        this_capacity, agg = results[0]
-        for other_capacity, result in results[1::]:
-            agg = agg.add_with_soc(this_capacity, result, other_capacity)
-        return agg
+            return None
 
-    def soc(self) -> Series:
-        return self.data["soc"]
+        return csv_to_grpd_df(file_name, simulation_data_path, delimiter)
 
     @staticmethod
-    def attributes() -> List[str]:
-        return ["p", "q", "capacity"]
+    def safe_get_path(entity_type: EntityEnumType, data_path: str) -> Optional[str]:
+        file_name = entity_type.get_csv_result_file_name()
+        path = get_file_path(data_path, file_name)
+        if path.exists():
+            return path
+        else:
+            logging.info(
+                "No results built for {} since {} does not exist".format(
+                    file_name, str(path)
+                )
+            )
+            return None
+
+    @classmethod
+    def create_empty(cls, sp_type):
+        return cls(sp_type, dict())
+
+    def uuids(self):
+        return list(self.entities.keys())
+
+    def results(self):
+        return list(self.entities.values())
+
+    # noinspection PyArgumentList
+    def subset(self, uuids):
+        matched_participants = {
+            uuid: self.entities[uuid] for uuid in self.entities.keys() & uuids
+        }
+
+        return type(self)(self.entity_type, matched_participants)
+
+    def subset_split(self, uuids: list[str]):
+        """
+        Returns a results result containing the given uuids and a results result containing the remaining uuids.
+        :param uuids: the uuids with which to split the result
+        :return:
+        """
+
+        rmd_uuids = self.entities.keys() - uuids
+        return self.subset(uuids), self.subset(rmd_uuids)
+
+    def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
+        """
+        Filters the result by the given datetime or list of datetimes.
+        :param time: the time or list of times to filter by
+        :return: a new result containing only the given time or times
+        """
+        return type(self)(
+            self.entity_type,
+            {uuid: result[time] for uuid, result in self.entities.items()},
+        )
+
+    # noinspection PyArgumentList
+    def filter_for_time_interval(self, start: datetime, end: datetime):
+        return type(self)(
+            self.entity_type,
+            {
+                uuid: result.filter_for_time_interval(start, end)
+                for uuid, result in self.entities.items()
+            },
+        )
+
+    def uuid_to_id_map(self) -> dict[str, Optional[str]]:
+        return {uuid: result.name for uuid, result in self.entities.items()}
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/results/bar_plot.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/common/bar_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/results/flex_plot.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/results/flex_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from psdm_analysis.models.input.enums import SystemParticipantsEnum
 from psdm_analysis.models.result.flex_option import FlexOptionResult
 from psdm_analysis.models.result.participant.participants_res_container import (
     ParticipantsResultContainer,
 )
 from psdm_analysis.models.result.power import PQResult
-from psdm_analysis.plots.results.line_plot import ax_plot_time_series
-from psdm_analysis.plots.results.power_plot import ax_plot_active_power
-from psdm_analysis.plots.utils import (
+from psdm_analysis.plots.common.line_plot import ax_plot_time_series
+from psdm_analysis.plots.common.utils import (
     FIGSIZE,
     FLEX_MAX,
     FLEX_MIN,
     FLEX_REF,
     ORANGE,
     set_style,
     set_title,
 )
+from psdm_analysis.plots.results.power_plot import ax_plot_active_power
 
 set_style()
 
 
 def plot_all_participants_flex_range(
     participants_res_container: ParticipantsResultContainer,
     title: str,
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/results/line_plot.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/common/line_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from matplotlib.axes import Axes
 from pandas import Series
 
 from psdm_analysis.models.input.enums import EntitiesEnum
-from psdm_analysis.plots.utils import (
+from psdm_analysis.plots.common.utils import (
     FILL_ALPHA,
     add_to_kwargs_if_not_exist,
     get_label_and_color_dict,
     plot_resample,
     set_date_format_and_label,
 )
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/results/nodes.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/results/nodes.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/results/power_plot.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/results/power_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     ParticipantsResult,
     ParticipantsWithSocResult,
 )
 from psdm_analysis.models.result.participant.participants_res_container import (
     ParticipantsResultContainer,
 )
 from psdm_analysis.models.result.power import PQResult, PQWithSocResult
-from psdm_analysis.plots.results.line_plot import ax_plot_time_series
-from psdm_analysis.plots.utils import (
+from psdm_analysis.plots.common.line_plot import ax_plot_time_series
+from psdm_analysis.plots.common.utils import (
     FIGSIZE,
     FILL_ALPHA,
     LOAD_COLOR,
     PV_COLOR,
     add_to_kwargs_if_not_exist,
     get_label_and_color,
     get_label_and_color_dict,
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/plots/utils.py` & `psdm-analysis-0.1.4/psdm_analysis/plots/common/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 GREY = COLOR_PALETTE[7]
 YELLOW = COLOR_PALETTE[8]
 LIGHT_BLUE = COLOR_PALETTE[9]
 
 # === COLOR MATCHING ===
 
 NODE_COLOR = BLUE
+TRANSFORMER_COLOR = BLUE
+LINE_COLOR = BLUE
 LOAD_COLOR = BLUE
 PV_COLOR = GREEN
 BS_COLOR = ORANGE
 HP_COLOR = PURPLE
 EVCS_COLOR = YELLOW
 RESIDUAL_LOAD_COLOR = LIGHT_BLUE
 UNKNOWN_COLOR = GREY
@@ -51,30 +53,36 @@
     sns.set_context(context)
 
 
 def get_label_and_color(sp_type: EntitiesEnum) -> Tuple[str, RGB]:
     match sp_type:
         case RawGridElementsEnum.NODE:
             return "Node", NODE_COLOR
+        case RawGridElementsEnum.TRANSFORMER_2_W:
+            return "Transformer", TRANSFORMER_COLOR
+        case RawGridElementsEnum.LINE:
+            return "Line", LINE_COLOR
         case SystemParticipantsEnum.LOAD:
             return "Load", LOAD_COLOR
         case SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
             return "PV", PV_COLOR
         case SystemParticipantsEnum.STORAGE:
             return "Battery", BS_COLOR
         case SystemParticipantsEnum.EV_CHARGING_STATION:
             return "EV Charging Station", EVCS_COLOR
         case SystemParticipantsEnum.ELECTRIC_VEHICLE:
             return "Electric Vehicle", EVCS_COLOR
-        case SystemParticipantsEnum.HEATP_PUMP:
+        case SystemParticipantsEnum.HEAT_PUMP:
             return "Heat Pump", HP_COLOR
         case SystemParticipantsEnum.ENERGY_MANAGEMENT:
             return "Energy Management", LOAD_COLOR
         case SystemParticipantsEnum.PARTICIPANTS_SUM:
             return "Participants Sum", LOAD_COLOR
+        case SystemParticipantsEnum.PRIMARY_DATA:
+            return "Primary Data", LOAD_COLOR
         case _:
             return sp_type.value, UNKNOWN_COLOR
 
 
 def get_label_and_color_dict(sp_type: EntitiesEnum):
     label, color = get_label_and_color(sp_type)
     return {"label": label, "color": color}
@@ -89,14 +97,15 @@
 # === FONT DEFAULTS ===
 
 TITLE_FONT_SIZE = 14
 
 # === SPACING ===
 
 TITLE_PAD = 15
+LABEL_PAD = 10
 
 # === SHADING ===
 
 FILL_ALPHA = 0.2
 
 
 def save_fig(figure: Figure, path: str, file_name: str, format="svg"):
@@ -137,14 +146,29 @@
         return "%b", "Month"
 
 
 def set_title(ax: Axes, title: str):
     ax.set_title(title, pad=TITLE_PAD, fontsize=TITLE_FONT_SIZE)
 
 
+def set_subplot_title(ax: Axes, title: str):
+    ax.set_title(title, pad=TITLE_PAD)
+
+
+def set_ylabel(ax: Axes, ylabel: str):
+    ax.set_ylabel(ylabel, labelpad=LABEL_PAD)
+
+
+def set_xlabels_rotated(
+    ax: Axes, labels: list[str], rotation: int = 45, ha: str = "center"
+):
+    ax.set_xticks(range(1, len(labels) + 1))
+    ax.set_xticklabels(labels, rotation=rotation, ha=ha)
+
+
 def legend_with_distinct_labels(ax: Axes):
     handles, labels = ax.get_legend_handles_labels()
     by_label = dict(zip(labels, handles))
     ax.legend(by_label.values(), by_label.keys())
 
 
 def rgb_to_hex(rgb):
@@ -152,7 +176,21 @@
 
 
 def add_to_kwargs_if_not_exist(kwargs: Dict, to_add: Dict):
     for key, value in to_add.items():
         if key not in kwargs:
             kwargs[key] = value
     return kwargs
+
+
+def ax_plot_secondary_axis(
+    ax: Axes, series: Series, ax_y_label: str, show_secondary_grid_lines: bool = False
+):
+    ax2 = ax.twinx()
+    (line_plot,) = ax2.plot(series)
+    line_plot.set_visible(False)
+    ax2.set_zorder(ax.get_zorder() - 1)
+    ax2.set_ylabel(ax_y_label, labelpad=10)
+    if show_secondary_grid_lines:
+        # Make the background of the original y-axis transparent so the gridlines are visible
+        ax.patch.set_visible(False)
+    return ax2
```

### Comparing `psdm-analysis-0.1.3/psdm_analysis/processing/dataframe.py` & `psdm-analysis-0.1.4/psdm_analysis/processing/dataframe.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/psdm_analysis/processing/series.py` & `psdm-analysis-0.1.4/psdm_analysis/processing/series.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.3/pyproject.toml` & `psdm-analysis-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psdm-analysis"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
 pandas = "2.0.1"
@@ -13,21 +13,24 @@
 seaborn = "^0.12.1"
 plotly = "^5.6.0"
 requests = "^2.27.1"
 numpy = "^1.24.1"
 scipy = "^1.10.0"
 pyarrow = "^11.0.0"
 openpyxl = "^3.1.2"
+python-dotenv = "^1.0.0" # Can probably be removed in the future
+shapely = "^2.0.1"
+networkx = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 flake8-isort = "^6.0.0"
-pre-commit = "^2.21.0"
+pre-commit = ">=2.21,<4.0"
 PyYAML = "^6.0"
 
 [tool.isort]
 profile= "black"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `psdm-analysis-0.1.3/setup.py` & `psdm-analysis-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,35 +11,39 @@
  'psdm_analysis.models.input.connector',
  'psdm_analysis.models.input.container',
  'psdm_analysis.models.input.participant',
  'psdm_analysis.models.result',
  'psdm_analysis.models.result.grid',
  'psdm_analysis.models.result.participant',
  'psdm_analysis.plots',
+ 'psdm_analysis.plots.common',
  'psdm_analysis.plots.results',
  'psdm_analysis.processing']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jupyter>=1.0.0,<2.0.0',
  'matplotlib>=3.6.0,<4.0.0',
+ 'networkx>=3.1,<4.0',
  'numpy>=1.24.1,<2.0.0',
  'openpyxl>=3.1.2,<4.0.0',
  'pandas==2.0.1',
  'plotly>=5.6.0,<6.0.0',
  'pyarrow>=11.0.0,<12.0.0',
+ 'python-dotenv>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
- 'seaborn>=0.12.1,<0.13.0']
+ 'seaborn>=0.12.1,<0.13.0',
+ 'shapely>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'psdm-analysis',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# psdm-analysis\n\nThe psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.\n\nIt is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.',
     'author': 'Thomas Oberliessen',
     'author_email': 'thomas.oberliessen@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psdm-analysis-0.1.3/PKG-INFO` & `psdm-analysis-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: psdm-analysis
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
 Requires-Python: >3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (==2.0.1)
 Requires-Dist: plotly (>=5.6.0,<6.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # psdm-analysis
 
 The psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.
 
 It is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.
```

