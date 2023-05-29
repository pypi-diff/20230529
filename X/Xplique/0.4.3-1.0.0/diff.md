# Comparing `tmp/Xplique-0.4.3.tar.gz` & `tmp/Xplique-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xplique-0.4.3.tar", last modified: Wed Dec 14 09:26:18 2022, max compression
+gzip compressed data, was "Xplique-1.0.0.tar", last modified: Mon May 29 15:27:13 2023, max compression
```

## Comparing `Xplique-0.4.3.tar` & `Xplique-1.0.0.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.218879 Xplique-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2022-12-14 09:26:10.000000 Xplique-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    21904 2022-12-14 09:26:18.214879 Xplique-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21378 2022-12-14 09:26:10.000000 Xplique-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.206879 Xplique-0.4.3/Xplique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21904 2022-12-14 09:26:18.000000 Xplique-0.4.3/Xplique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3911 2022-12-14 09:26:18.000000 Xplique-0.4.3/Xplique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-14 09:26:18.000000 Xplique-0.4.3/Xplique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-12-14 09:26:18.000000 Xplique-0.4.3/Xplique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-14 09:26:18.000000 Xplique-0.4.3/Xplique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-14 09:26:18.218879 Xplique-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-12-14 09:26:10.000000 Xplique-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.206879 Xplique-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8146 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (122)     4955 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_deconvnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3019 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     3284 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_guided_backprop.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_hsic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_rise.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     4954 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_sobol.py
--rw-r--r--   0 runner    (1001) docker     (122)     5240 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/attributions/test_tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/commons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/commons/test_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/commons/test_model_override.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/concepts/test_cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/concepts/test_tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_preconditionning.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/features_visualizations/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/generic/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/metrics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/metrics/test_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/metrics/test_mege.py
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/metrics/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/plots/test_metric_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/plots/test_timeseries_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2022-12-14 09:26:10.000000 Xplique-0.4.3/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.210879 Xplique-0.4.3/xplique/
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5240 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/deconvnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)      781 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6536 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     4972 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/kernels.py
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2745 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     9897 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     7197 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/guided_backpropagation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6887 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     6525 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)    25822 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10436 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     8686 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/rise.py
--rw-r--r--   0 runner    (1001) docker     (122)     2766 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)     5656 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1711 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/square_grad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1521 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/attributions/vargrad.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/commons/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2584 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/commons/callable_operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/commons/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/commons/model_override.py
--rw-r--r--   0 runner    (1001) docker     (122)     5754 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/commons/tf_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4603 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/concepts/cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/concepts/tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)      410 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    11025 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     6520 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/optim.py
--rw-r--r--   0 runner    (1001) docker     (122)     5433 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/preconditioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5581 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/features_visualizations/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    29157 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/metrics/fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)     8702 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/metrics/representativity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/metrics/stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5389 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/plots/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    12877 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/plots/tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     5166 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/plots/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 09:26:18.214879 Xplique-0.4.3/xplique/types/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-12-14 09:26:10.000000 Xplique-0.4.3/xplique/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-29 15:27:01.000000 Xplique-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    21904 2023-05-29 15:27:13.355503 Xplique-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21378 2023-05-29 15:27:01.000000 Xplique-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/Xplique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21904 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-29 15:27:13.000000 Xplique-1.0.0/Xplique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 15:27:13.355503 Xplique-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-05-29 15:27:01.000000 Xplique-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_deconvnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_guided_backprop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_sobol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/attributions/test_tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/commons/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/test_cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/concepts/test_tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_preconditionning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/features_visualizations/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.347503 Xplique-1.0.0/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/generic/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5983 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_mege.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/metrics/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/test_metric_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/plots/test_timeseries_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-29 15:27:01.000000 Xplique-1.0.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/deconvnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.351503 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4972 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2317 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/guided_backpropagation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26149 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7484 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/square_grad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/attributions/vargrad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/callable_operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/commons/tf_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/concepts/tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6520 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5433 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/preconditioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/features_visualizations/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16580 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8702 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/representativity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/metrics/stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5830 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5389 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5166 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/plots/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:27:13.355503 Xplique-1.0.0/xplique/types/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-29 15:27:01.000000 Xplique-1.0.0/xplique/types/__init__.py
```

### Comparing `Xplique-0.4.3/LICENSE` & `Xplique-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/PKG-INFO` & `Xplique-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 0.4.3
+Version: 1.0.0
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 0.4.3 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.0 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
```

### Comparing `Xplique-0.4.3/README.md` & `Xplique-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/Xplique.egg-info/PKG-INFO` & `Xplique-1.0.0/Xplique.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 0.4.3
+Version: 1.0.0
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 0.4.3 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.0 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
```

### Comparing `Xplique-0.4.3/Xplique.egg-info/SOURCES.txt` & `Xplique-1.0.0/Xplique.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 tests/attributions/test_saliency.py
 tests/attributions/test_smoothgrad.py
 tests/attributions/test_sobol.py
 tests/attributions/test_tabular_data.py
 tests/commons/__init__.py
 tests/commons/test_data_conversion.py
 tests/commons/test_model_override.py
+tests/commons/test_operators.py
 tests/concepts/__init__.py
 tests/concepts/test_cav.py
 tests/concepts/test_tcav.py
 tests/features_visualizations/__init__.py
 tests/features_visualizations/test_losses.py
 tests/features_visualizations/test_objectives.py
 tests/features_visualizations/test_optim.py
@@ -77,15 +78,17 @@
 xplique/attributions/global_sensitivity_analysis/replicated_designs.py
 xplique/attributions/global_sensitivity_analysis/samplers.py
 xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
 xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
 xplique/commons/__init__.py
 xplique/commons/callable_operations.py
 xplique/commons/data_conversion.py
+xplique/commons/exceptions.py
 xplique/commons/model_override.py
+xplique/commons/operators.py
 xplique/commons/tf_operations.py
 xplique/concepts/__init__.py
 xplique/concepts/cav.py
 xplique/concepts/tcav.py
 xplique/features_visualizations/__init__.py
 xplique/features_visualizations/losses.py
 xplique/features_visualizations/objectives.py
```

### Comparing `Xplique-0.4.3/setup.py` & `Xplique-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as fh:
     README = fh.read()
 
 setup(
     name="Xplique",
-    version="0.4.3",
+    version="1.0.0",
     description="Explanations toolbox for Tensorflow 2",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Thomas FEL",
     author_email="thomas_fel@brown.edu",
     license="MIT",
     install_requires=['tensorflow>=2.1.0', 'numpy', 'scikit-learn', 'scikit-image',
```

### Comparing `Xplique-0.4.3/tests/attributions/test_callable.py` & `Xplique-1.0.0/tests/attributions/test_callable.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import numpy as np
 import tensorflow as tf
 
 from sklearn.svm import SVC
 from sklearn.ensemble import RandomForestClassifier
 
 from xplique.attributions import (Occlusion, Rise, Lime, KernelShap, SobolAttributionMethod)
-from xplique.commons.tf_operations import predictions_one_hot, batch_predictions_one_hot
-from xplique.commons.callable_operations import predictions_one_hot_callable, \
+from xplique.commons.operators import predictions_operator, batch_predictions,\
     batch_predictions_one_hot_callable
+from xplique.commons.callable_operations import predictions_one_hot_callable
 
 from ..utils import generate_data, generate_model, generate_regression_model
 
 def _default_methods_tabular(model):
     return [
         Occlusion(model, patch_size = 1, patch_stride = 1),
         Lime(model),
@@ -161,16 +161,16 @@
     inputs, targets = generate_data((input_size,), nb_labels, samples)
     models = _default_tf_model_tabular(input_size, nb_labels)
 
     for model in models:
         explainers = _default_methods_tabular(model)
 
         for explainer in explainers:
-            assert explainer.inference_function is predictions_one_hot
-            assert explainer.batch_inference_function is batch_predictions_one_hot
+            assert explainer.inference_function is predictions_operator
+            assert explainer.batch_inference_function is batch_predictions
 
             explanations = explainer(inputs, targets)
 
             assert explanations.shape == (samples, input_size)
 
 def test_tf_models_images():
     """
@@ -185,16 +185,16 @@
         inputs, targets = generate_data(input_shape, nb_labels, samples)
         models = _default_tf_model_images(input_shape, nb_labels)
         for model in models:
 
             explainers = _default_methods_images(model)
 
             for explainer in explainers:
-                assert explainer.inference_function is predictions_one_hot
-                assert explainer.batch_inference_function is batch_predictions_one_hot
+                assert explainer.inference_function is predictions_operator
+                assert explainer.batch_inference_function is batch_predictions
 
                 explanations = explainer(inputs, targets)
 
                 assert explanations.shape == (samples, *input_shape[:2])
 
 def test_callable_models_tabular():
     """
```

### Comparing `Xplique-0.4.3/tests/attributions/test_common.py` & `Xplique-1.0.0/tests/attributions/test_common.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_deconvnet.py` & `Xplique-1.0.0/tests/attributions/test_deconvnet.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_grad_cam.py` & `Xplique-1.0.0/tests/attributions/test_grad_cam.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_grad_cam_pp.py` & `Xplique-1.0.0/tests/attributions/test_grad_cam_pp.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_gradient_input.py` & `Xplique-1.0.0/tests/attributions/test_gradient_input.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_guided_backprop.py` & `Xplique-1.0.0/tests/attributions/test_guided_backprop.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_hsic.py` & `Xplique-1.0.0/tests/attributions/test_hsic.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_integrated_gradients.py` & `Xplique-1.0.0/tests/attributions/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_kernel_shap.py` & `Xplique-1.0.0/tests/attributions/test_kernel_shap.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_lime.py` & `Xplique-1.0.0/tests/attributions/test_lime.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_object_detector.py` & `Xplique-1.0.0/tests/attributions/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_occlusion.py` & `Xplique-1.0.0/tests/attributions/test_occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             [0, 0],
             [1, 0]
         ],
         [
             [0, 0],
             [0, 1]
         ],
-    ], dtype=np.bool))
+    ], dtype=np.float32))
 
 
 def test_apply():
     """Ensure we apply correctly the masks"""
     x = np.ones((2, 2, 1), dtype=np.float32)
     applied_value = 49.0
```

### Comparing `Xplique-0.4.3/tests/attributions/test_rise.py` & `Xplique-1.0.0/tests/attributions/test_rise.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_saliency.py` & `Xplique-1.0.0/tests/attributions/test_saliency.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_smoothgrad.py` & `Xplique-1.0.0/tests/attributions/test_smoothgrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_sobol.py` & `Xplique-1.0.0/tests/attributions/test_sobol.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/attributions/test_tabular_data.py` & `Xplique-1.0.0/tests/attributions/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/commons/test_data_conversion.py` & `Xplique-1.0.0/tests/commons/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/commons/test_model_override.py` & `Xplique-1.0.0/tests/commons/test_model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/concepts/test_cav.py` & `Xplique-1.0.0/tests/concepts/test_cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/concepts/test_tcav.py` & `Xplique-1.0.0/tests/concepts/test_tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_losses.py` & `Xplique-1.0.0/tests/features_visualizations/test_losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_objectives.py` & `Xplique-1.0.0/tests/features_visualizations/test_objectives.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_optim.py` & `Xplique-1.0.0/tests/features_visualizations/test_optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_preconditionning.py` & `Xplique-1.0.0/tests/features_visualizations/test_preconditionning.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_regularizers.py` & `Xplique-1.0.0/tests/features_visualizations/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/features_visualizations/test_transformations.py` & `Xplique-1.0.0/tests/features_visualizations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/generic/test_wrapper.py` & `Xplique-1.0.0/tests/generic/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/metrics/test_common.py` & `Xplique-1.0.0/tests/metrics/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,10 +44,12 @@
     for explainer in explainers:
         explanations = explainer(x, y)
         for metric in metrics:
             assert hasattr(metric, 'evaluate')
             if isinstance(metric, ExplainerMetric):
                 score = metric(explainer)
             else:
+                assert hasattr(metric, 'inference_function')
+                assert hasattr(metric, 'batch_inference_function')
                 score = metric(explanations)
             print(f"\n\n\n {type(score)} \n\n\n")
             assert type(score) in [np.float32, np.float64, float]
```

### Comparing `Xplique-0.4.3/tests/metrics/test_fidelity.py` & `Xplique-1.0.0/tests/metrics/test_fidelity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tensorflow as tf
 import numpy as np
 
-from ..utils import generate_model, generate_timeseries_model, generate_regression_model, generate_data, almost_equal
-from xplique.metrics import Insertion, Deletion, MuFidelity, InsertionTS, DeletionTS, InsertionTab, DeletionTab
+from ..utils import (generate_model, generate_regression_model, generate_timeseries_model, 
+                     generate_data, almost_equal)
+from xplique.commons.operators import regression_operator
+from xplique.metrics import Insertion, Deletion, MuFidelity
 
 
 def test_mu_fidelity():
     # ensure we can compute the metric with consistents arguments
     input_shape, nb_labels, nb_samples = ((32, 32, 3), 10, 20)
     x, y = generate_data(input_shape, nb_labels, nb_samples)
     model = generate_model(input_shape, nb_labels)
@@ -40,72 +42,46 @@
                                       baseline_mode=baseline_mode,
                                       steps=step)(explanations)
 
             for score in [score_insertion, score_deletion]:
                 assert 0.0 <= score <= 1.0
 
 
-def test_perturbation_metrics():
-    # ensure we can compute insertion/deletion metric with consistent arguments
-    input_shape, nb_labels, nb_samples = ((20, 10), 5, 50)
-    x, y = generate_data(input_shape, nb_labels, nb_samples)
-    model = generate_timeseries_model(input_shape, nb_labels)
-    explanations = np.random.uniform(0, 1, x.shape)
-
-    def inverse(x):
-        maximums = x.max(axis=1)
-        maximums = np.expand_dims(maximums, axis=1)
-        maximums = np.repeat(maximums, x.shape[1], axis=1)
-        baselines = maximums - x
-        return baselines
-
-    for step in [-1, 10]:
-        for baseline_mode in [0.0, inverse]:
-            for metric in ["loss", "accuracy"]:
-                score_insertion = InsertionTS(
-                    model, x, y, metric=metric, baseline_mode=baseline_mode,
-                    steps=step, max_percentage_perturbed=0.2,
-                ).evaluate(explanations)
-                score_deletion = DeletionTS(
-                    model, x, y, metric=metric, baseline_mode=baseline_mode,
-                    steps=step, max_percentage_perturbed=0.2,
-                ).evaluate(explanations)
-
-                for score in [score_insertion, score_deletion]:
-                    if metric == "loss":
-                        assert 0.0 < score
-                    elif metric == "accuracy":
-                        assert 0.0 <= score <= 1.0
-
-
-def test_regression_metrics():
-    # ensure we can compute insertion/deletion metric with consistent arguments
-    input_shape, nb_labels, nb_samples = ((20, 10), 5, 50)
-    x, y = generate_data(input_shape, nb_labels, nb_samples)
-    model = generate_regression_model(input_shape, nb_labels)
-    explanations = np.random.uniform(0, 1, x.shape)
-
-    for step in [5, 10]:
-        for baseline_mode in [0.0, lambda x: x-0.5]:
-            for metric in ["loss", "accuracy"]:
-                score_insertion = InsertionTab(
-                    model, x, y, metric=metric, baseline_mode=baseline_mode,
-                    steps=step, max_percentage_perturbed=0.2,
-                ).evaluate(explanations)
-                score_deletion = DeletionTab(
-                    model, x, y, metric=metric, baseline_mode=baseline_mode,
-                    steps=step, max_percentage_perturbed=0.2,
-                ).evaluate(explanations)
-
-                for score in [score_insertion, score_deletion]:
-                    if metric == "loss":
-                        assert 0.0 < score
-
-                    elif metric == "accuracy":
-                        assert 0.0 <= score <= 1.0
+def test_data_types_with_regression():
+    # ensure that the different metrics are robust to several data types with regression
+    # test several data types
+    data_types = {
+        "tabular": (16,),
+        "time-series": (16, 8),
+        "images": (16, 16, 3)
+    }
+
+    for type, input_shape in data_types.items():
+        nb_labels, samples = 10, 20
+        x, y = generate_data(input_shape, nb_labels, samples)
+        model = generate_regression_model(input_shape, nb_labels)
+
+        explanations = np.random.uniform(0, 1, x.shape[:-1])
+
+    score_insertion = Insertion(
+        model, x, y, operator=regression_operator, steps=3,
+    ).evaluate(explanations)
+
+    score_deletion = Deletion(
+        model, x, y, operator=regression_operator, steps=3,
+    ).evaluate(explanations)
+
+    for score in [score_insertion, score_deletion]:
+        assert 0.0 < score
+
+    score_mufidelity = MuFidelity(
+        model, x, y, operator=regression_operator, nb_samples=3
+    ).evaluate(explanations)
+            
+    assert -1.0 < score_mufidelity < 1.0
 
 
 def test_perfect_correlation():
     """Ensure we get perfect score if the correlation is perfect"""
     # we ensure perfect correlation if the model return the sum of the input,
     # and the input is the explanations: corr( sum(phi), sum(x) - sum(x-phi) )
     # to do so we define f(x) -> sum(x) and phi = x
```

### Comparing `Xplique-0.4.3/tests/metrics/test_mege.py` & `Xplique-1.0.0/tests/metrics/test_mege.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/metrics/test_stability.py` & `Xplique-1.0.0/tests/metrics/test_stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/plots/test_metric_plots.py` & `Xplique-1.0.0/tests/plots/test_metric_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/plots/test_timeseries_plots.py` & `Xplique-1.0.0/tests/plots/test_timeseries_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/tests/utils.py` & `Xplique-1.0.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/__init__.py` & `Xplique-1.0.0/xplique/attributions/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/base.py` & `Xplique-1.0.0/xplique/attributions/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from abc import ABC, abstractmethod
 import warnings
 
 import tensorflow as tf
 import numpy as np
 
 from ..types import Callable, Dict, Tuple, Union, Optional
-from ..commons import find_layer, tensor_sanitize, batch_predictions_one_hot, \
-                      predictions_one_hot, batch_predictions_one_hot_callable, \
-                      predictions_one_hot_callable
-
+from ..commons import (find_layer, tensor_sanitize, get_inference_function,
+                      get_gradient_functions, no_gradients_available)
 
 
 def sanitize_input_output(explanation_method: Callable):
     """
     Wrap a method explanation function to ensure tf.Tensor as inputs,
     and as output
 
@@ -40,39 +38,46 @@
 
     Parameters
     ----------
     model
         The model from which we want to obtain explanations
     batch_size
         Number of pertubed samples to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     # in order to avoid re-tracing at each tf.function call,
     # share the reconfigured models between the methods if possible
     _cache_models: Dict[Tuple[int, int], tf.keras.Model] = {}
 
-    def __init__(self, model: Callable, batch_size: Optional[int] = 64):
+    def __init__(self, model: Callable, batch_size: Optional[int] = 64,
+                operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None):
+
         if isinstance(model, tf.keras.Model):
             model_key = (id(model.input), id(model.output))
             if model_key not in BlackBoxExplainer._cache_models:
                 BlackBoxExplainer._cache_models[model_key] = model
             self.model = BlackBoxExplainer._cache_models[model_key]
-            self.inference_function = predictions_one_hot
-            self.batch_inference_function = batch_predictions_one_hot
-        elif isinstance(model, (tf.Module, tf.keras.layers.Layer)):
-            self.model = model
-            self.inference_function = predictions_one_hot
-            self.batch_inference_function = batch_predictions_one_hot
         else:
             self.model = model
-            self.inference_function = predictions_one_hot_callable
-            self.batch_inference_function = batch_predictions_one_hot_callable
 
         self.batch_size = batch_size
 
+        # define the inference function according to the model type
+        self.inference_function, self.batch_inference_function = \
+            get_inference_function(model, operator)
+
+        # black box method don't have access to the model's gradients
+        self.gradient = no_gradients_available
+        self.batch_gradient = no_gradients_available
+
+
     @abstractmethod
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.array],
                 targets: Optional[Union[tf.Tensor, np.array]] = None) -> tf.Tensor:
         """
         Compute the explanations of the given inputs.
         Accept Tensor, numpy array or tf.data.Dataset (in that case targets is None)
@@ -117,28 +122,34 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Operator to use to compute the explanation, if None use standard predictions.
     """
 
     def __init__(self,
-                 model: tf.keras.Model,
-                 output_layer: Optional[Union[str, int]] = None,
-                 batch_size: Optional[int] = 64):
+                model: tf.keras.Model,
+                output_layer: Optional[Union[str, int]] = None,
+                batch_size: Optional[int] = 64,
+                operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None):
+
+        super().__init__(model, batch_size, operator)
 
         if output_layer is not None:
             # reconfigure the model (e.g skip softmax to target logits)
             target_layer = find_layer(model, output_layer)
             model = tf.keras.Model(model.input, target_layer.output)
 
             # sanity check, output layer before softmax
             try:
                 if target_layer.activation.__name__ == tf.keras.activations.softmax.__name__:
                     warnings.warn("Output is after softmax, it is recommended to "
                                   "use the layer before.")
             except AttributeError:
                 pass
 
-        super().__init__(model, batch_size)
+        # check and get gradient function from model and operator
+        self.gradient, self.batch_gradient = get_gradient_functions(model, operator)
```

### Comparing `Xplique-0.4.3/xplique/attributions/deconvnet.py` & `Xplique-1.0.0/xplique/attributions/deconvnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Module related to DeconvNet method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import override_relu_gradient, deconv_relu_policy, batch_gradient
-from ..types import Union, Optional
+from ..commons import override_relu_gradient, deconv_relu_policy
+from ..types import Union, Optional, Callable
 
 
 class DeconvNet(WhiteBoxExplainer):
     """
     Used to compute the DeconvNet method, which modifies the classic Saliency procedure on
     ReLU's non linearities, allowing only the positive gradients (even from negative inputs) to
     pass through.
@@ -23,26 +23,30 @@
     ----------
     model
         The model from which we want to obtain explanations
     output_layer
         Layer to target for the outputs (e.g logits or after softmax).
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
-
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     def __init__(self,
-                 model: tf.keras.Model,
-                 output_layer: Optional[Union[str, int]] = None,
-                 batch_size: Optional[int] = 32):
-        super().__init__(model, output_layer, batch_size)
+                model: tf.keras.Model,
+                output_layer: Optional[Union[str, int]] = None,
+                batch_size: Optional[int] = 32,
+                operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None):
+        super().__init__(model, output_layer, batch_size, operator)
         self.model = override_relu_gradient(self.model, deconv_relu_policy)
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
         """
@@ -63,9 +67,9 @@
             More information in the documentation.
 
         Returns
         -------
         explanations
             Deconv maps.
         """
-        gradients = batch_gradient(self.model, inputs, targets, self.batch_size)
+        gradients = self.batch_gradient(self.model, inputs, targets, self.batch_size)
         return gradients
```

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/__init__.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,28 +71,33 @@
     estimator
         Estimator used to compute the attribution score, e.g Sobol or HSIC estimator.
     perturbation_function
         Function to call to apply the perturbation on the input. Can also be string in
         'inpainting', 'blur'.
     batch_size
         Batch size to use for the forwards.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     def __init__(
         self,
         model: tf.keras.Model,
         sampler: Callable,
         estimator: Callable,
         grid_size: int = 7,
         nb_design: int = 32,
         perturbation_function: Optional[Union[Callable, str]] = "inpainting",
         batch_size=256,
+        operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
     ):
 
-        super().__init__(model, batch_size)
+        super().__init__(model, batch_size, operator)
 
         self.grid_size = grid_size
         self.nb_design = nb_design
 
         if isinstance(perturbation_function, str):
             self.perturbation_function = PerturbationFunction.from_string(
                 perturbation_function
```

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Hsic Attribution Method explainer
 """
 
+import tensorflow as tf
+
 from ...types import Callable, Union, Optional
 from .gsa_attribution_method import GSABaseAttributionMethod
 from .samplers import Sampler, TFSobolSequence
 from .hsic_estimators import (
     BinaryEstimator,
     HsicEstimator,
 )
@@ -36,25 +38,30 @@
     estimator
         Estimator used to compute the HSIC score.
     perturbation_function
         Function to call to apply the perturbation on the input. Can also be string in
         'inpainting', 'blur'.
     batch_size
         Batch size to use for the forwards.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     def __init__(
         self,
         model,
         grid_size: int = 8,
         nb_design: int = 500,
         sampler: Optional[Sampler] = None,
         estimator: Optional[HsicEstimator] = None,
         perturbation_function: Optional[Union[Callable, str]] = "inpainting",
         batch_size=256,
+        operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
     ):
 
         sampler = sampler if sampler is not None else TFSobolSequence(binary=True)
         estimator = (
             estimator if estimator is not None else BinaryEstimator(output_kernel="rbf")
         )
 
@@ -62,11 +69,12 @@
         assert isinstance(
             estimator, HsicEstimator
         ), "The estimator must be a valid HsicEstimator."
 
         if isinstance(estimator, BinaryEstimator):
             assert sampler.binary, "The sampler must be binary for BinaryEstimator."
 
-        super().__init__(model = model, sampler = sampler, estimator = estimator,
+        super().__init__(model = model, operator = operator,
+                         sampler = sampler, estimator = estimator,
                          grid_size = grid_size, nb_design = nb_design,
                          perturbation_function = perturbation_function, batch_size = batch_size,
         )
```

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/kernels.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/kernels.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/perturbations.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/perturbations.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/replicated_designs.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/replicated_designs.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/samplers.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/samplers.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Sobol Attribution Method explainer
 """
 
+import tensorflow as tf
+
 from ...types import Callable, Union, Optional
 from .gsa_attribution_method import GSABaseAttributionMethod
 from .sobol_estimators import SobolEstimator, JansenEstimator
 from .replicated_designs import ReplicatedSampler, TFSobolSequenceRS
 
 
 class SobolAttributionMethod(GSABaseAttributionMethod):
@@ -33,25 +35,30 @@
         Estimator used to compute the total order sobol' indices, Jansen recommended. For more
         option, see the estimator module.
     perturbation_function
         Function to call to apply the perturbation on the input. Can also be string in
         'inpainting', 'blur'.
     batch_size
         Batch size to use for the forwards.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     def __init__(
         self,
         model,
         grid_size: int = 8,
         nb_design: int = 32,
         sampler: Optional[ReplicatedSampler] = None,
         estimator: Optional[SobolEstimator] = None,
         perturbation_function: Optional[Union[Callable, str]] = "inpainting",
         batch_size=256,
+        operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
     ):
 
         assert (
             nb_design & (nb_design - 1) == 0
         ) and nb_design != 0, "The number of design must be a power of two."
 
         sampler = sampler if sampler is not None else TFSobolSequenceRS()
@@ -62,14 +69,15 @@
         )
         assert isinstance(estimator, SobolEstimator), (
             "The estimator must be a" " valid Sobol estimator."
         )
 
         super().__init__(
             model=model,
+            operator=operator,
             sampler=sampler,
             estimator=estimator,
             grid_size=grid_size,
             nb_design=nb_design,
             perturbation_function=perturbation_function,
             batch_size=batch_size,
         )
```

### Comparing `Xplique-0.4.3/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py` & `Xplique-1.0.0/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/attributions/grad_cam.py` & `Xplique-1.0.0/xplique/attributions/grad_cam.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tensorflow as tf
 import numpy as np
 import cv2
 
 from .base import WhiteBoxExplainer, sanitize_input_output
 from ..commons import find_layer
-from ..types import Tuple, Union, Optional
+from ..types import Tuple, Union, Optional, Callable
 
 
 class GradCAM(WhiteBoxExplainer):
     """
     Used to compute the Grad-CAM visualization method.
 
     Only for Convolutional Networks.
@@ -30,26 +30,31 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     conv_layer
         Layer to target for Grad-CAM algorithm.
         If an int is provided it will be interpreted as a layer index.
         If a string is provided it will look for the layer name.
     """
 
     def __init__(self,
                  model: tf.keras.Model,
                  output_layer: Optional[Union[str, int]] = None,
                  batch_size: Optional[int] = 32,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  conv_layer: Optional[Union[str, int]] = None):
-        super().__init__(model, output_layer, batch_size)
+        super().__init__(model, output_layer, batch_size, operator)
 
         # find the layer to apply grad-cam
         if conv_layer is not None:
             self.conv_layer = find_layer(model, conv_layer)
         else:
             # no conv_layer specified, assuming default procedure : the last conv layer
             self.conv_layer = next(
```

### Comparing `Xplique-0.4.3/xplique/attributions/grad_cam_pp.py` & `Xplique-1.0.0/xplique/attributions/grad_cam_pp.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     conv_layer
         Layer to target for Grad-CAM++ algorithm.
         If an int is provided it will be interpreted as a layer index.
         If a string is provided it will look for the layer name.
     """
 
     # Avoid zero division during procedure. (the value is not important, as if the denominator is
```

### Comparing `Xplique-0.4.3/xplique/attributions/gradient_input.py` & `Xplique-1.0.0/xplique/attributions/gradient_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Module related to Gradient x Input method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import batch_gradient
 from ..types import Optional, Union
 
 
 class GradientInput(WhiteBoxExplainer):
     """
     Used to compute elementwise product between the saliency maps of Simonyan et al. and the
     input (Gradient x Input).
@@ -24,14 +23,18 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
         """
@@ -51,11 +54,11 @@
             More information in the documentation.
 
         Returns
         -------
         explanations
             Gradients x Inputs, with the same shape as the inputs.
         """
-        gradients = batch_gradient(self.model, inputs, targets, self.batch_size)
+        gradients = self.batch_gradient(self.model, inputs, targets, self.batch_size)
         gradients_inputs = tf.multiply(gradients, inputs)
 
         return gradients_inputs
```

### Comparing `Xplique-0.4.3/xplique/attributions/guided_backpropagation.py` & `Xplique-1.0.0/xplique/attributions/guided_backpropagation.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Module related to Guided Backpropagation method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import guided_relu_policy, override_relu_gradient, batch_gradient
-from ..types import Union, Optional
+from ..commons import guided_relu_policy, override_relu_gradient
+from ..types import Union, Optional, Callable
 
 
 class GuidedBackprop(WhiteBoxExplainer):
     """
     Used to compute the Guided Backpropagation, which modifies the classic Saliency procedure on
     ReLU's non linearities, allowing only the positive gradients from positive activations to pass
     through.
@@ -28,21 +28,26 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     def __init__(self,
-                 model: tf.keras.Model,
-                 output_layer: Optional[Union[str, int]] = None,
-                 batch_size: Optional[int] = 32):
-        super().__init__(model, output_layer, batch_size)
+                model: tf.keras.Model,
+                output_layer: Optional[Union[str, int]] = None,
+                batch_size: Optional[int] = 32,
+                operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None):
+        super().__init__(model, output_layer, batch_size, operator)
         self.model = override_relu_gradient(self.model, guided_relu_policy)
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
         """
@@ -62,9 +67,9 @@
             More information in the documentation.
 
         Returns
         -------
         explanations
             Guided Backpropagation maps.
         """
-        gradients = batch_gradient(self.model, inputs, targets, self.batch_size)
+        gradients = self.batch_gradient(self.model, inputs, targets, self.batch_size)
         return gradients
```

### Comparing `Xplique-0.4.3/xplique/attributions/integrated_gradients.py` & `Xplique-1.0.0/xplique/attributions/integrated_gradients.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Module related to Integrated Gradients method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import repeat_labels, batch_gradient, batch_tensor
-from ..types import Tuple, Union, Optional
+from ..commons import repeat_labels, batch_tensor
+from ..types import Tuple, Union, Optional, Callable
 
 
 class IntegratedGradients(WhiteBoxExplainer):
     """
     Used to compute the Integrated Gradients, by cumulating the gradients along a path from a
     baseline to the desired point.
 
@@ -34,27 +34,32 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     steps
         Number of points to interpolate between the baseline and the desired point.
     baseline_value
         Scalar used to create the the baseline point.
     """
 
     def __init__(self,
                  model: tf.keras.Model,
                  output_layer: Optional[Union[str, int]] = None,
                  batch_size: Optional[int] = 32,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  steps: int = 50,
                  baseline_value: float = .0):
-        super().__init__(model, output_layer, batch_size)
+        super().__init__(model, output_layer, batch_size, operator)
         self.steps = steps
         self.baseline_value = baseline_value
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
@@ -88,16 +93,16 @@
                                              max(batch_size // self.steps, 1)):
             # create the paths for every sample (interpolated points from baseline to sample)
             interpolated_inputs = IntegratedGradients._get_interpolated_points(
                 x_batch, self.steps, baseline)
             repeated_targets = repeat_labels(y_batch, self.steps)
 
             # compute the gradient for each paths
-            interpolated_gradients = batch_gradient(self.model, interpolated_inputs,
-                                                    repeated_targets, batch_size)
+            interpolated_gradients = self.batch_gradient(self.model, interpolated_inputs,
+                                                         repeated_targets, batch_size)
             interpolated_gradients = tf.reshape(interpolated_gradients,
                                                 (-1, self.steps, *interpolated_gradients.shape[1:]))
 
             # average the gradient using trapezoidal rule
             averaged_gradients = IntegratedGradients._average_gradients(interpolated_gradients)
             batch_integrated_gradients = (x_batch - baseline) * averaged_gradients
```

### Comparing `Xplique-0.4.3/xplique/attributions/kernel_shap.py` & `Xplique-1.0.0/xplique/attributions/kernel_shap.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     ----------
     model
         The model from which we want to obtain explanations.
     batch_size
         Number of perturbed samples to process at once, mandatory when nb_samples is huge.
         Notice, it is different compare to WhiteBox explainers which batch the inputs.
         Here inputs are process one by one.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     map_to_interpret_space
         Function which group features of an input corresponding to the same interpretable
         feature (e.g super-pixel).
         It allows to transpose from (resp. to) the original input space to (resp. from)
         the interpretable space.
     nb_samples
         The number of perturbed samples you want to generate for each input sample.
@@ -42,22 +46,24 @@
         and (C,) otherwise.
         The default ref value is set to (0.5,0.5,0.5) for inputs with 3 channels (corresponding
         to a grey pixel when inputs are normalized by 255) and to 0 otherwise.
     """
     def __init__(self,
                  model: Callable,
                  batch_size: int = 64,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  map_to_interpret_space: Optional[Callable] = None,
                  nb_samples: int = 800,
                  ref_value: Optional[np.ndarray] = None):
 
         Lime.__init__(
             self,
             model,
             batch_size,
+            operator,
             interpretable_model = linear_model.LinearRegression(),
             similarity_kernel = KernelShap._kernel_shap_similarity_kernel,
             pertub_func = KernelShap._kernel_shap_pertub_func,
             ref_value = ref_value,
             map_to_interpret_space = map_to_interpret_space,
             nb_samples = nb_samples,
             )
```

### Comparing `Xplique-0.4.3/xplique/attributions/lime.py` & `Xplique-1.0.0/xplique/attributions/lime.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     ----------
     model
         The model from which we want to obtain explanations
     batch_size
         Number of perturbed samples to process at once, mandatory when nb_samples is huge.
         Notice, it is different compare to WhiteBox explainers which batch the inputs.
         Here inputs are process one by one.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     interpretable_model
         Model object to train interpretable model.
         See the documentation for more information.
     similarity_kernel
         Function which considering an input, perturbed instances of these input and
         the interpretable version of those perturbed samples compute the similarities between
         the input and the perturbed samples.
@@ -91,14 +95,15 @@
         values.
         Default to 45 (i.e adapted for RGB images).
     """
     def __init__(
         self,
         model: Callable,
         batch_size: Optional[int] = None,
+        operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
         interpretable_model: Any = linear_model.Ridge(alpha=2),
         similarity_kernel: Optional[Callable[[tf.Tensor, tf.Tensor, tf.Tensor], tf.Tensor]] = None,
         pertub_func: Optional[Callable[[Union[int, tf.Tensor],int], tf.Tensor]] = None,
         map_to_interpret_space: Optional[Callable[[tf.Tensor], tf.Tensor]] = None,
         ref_value: Optional[np.ndarray] = None,
         nb_samples: int = 150,
         distance_mode: str = "euclidean",
@@ -125,15 +130,15 @@
                 "batch_size is set to None"
                 "This mean that you will ask your model to handle more than 500"
                 " perturbed samples per input at once."
                 "This can lead to OOM issue. To avoid it you can set the"
                 " batch_size argument."
             )
 
-        super().__init__(model, batch_size)
+        super().__init__(model, batch_size, operator)
 
         self.map_to_interpret_space = map_to_interpret_space
         self.interpretable_model = interpretable_model
         self.similarity_kernel = similarity_kernel
         self.pertub_func = pertub_func
         self.ref_value = ref_value
         self.nb_samples = nb_samples
```

### Comparing `Xplique-0.4.3/xplique/attributions/object_detector.py` & `Xplique-1.0.0/xplique/attributions/object_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Iterable, Tuple, Union, Optional
 import abc
 
 import tensorflow as tf
 import numpy as np
 
 from xplique.attributions.base import BlackBoxExplainer
-from xplique.commons.tf_operations import inference_batching
+from xplique.commons import operator_batching
 
 
 class IouCalculator:
     """
     Used to compute the Intersection Over Union (IOU).
     """
     @abc.abstractmethod
@@ -105,15 +105,15 @@
 
         intersection_area = tf.math.maximum(right - left, 0) * tf.math.maximum(top - bottom, 0)
 
         # determine the areas of the prediction and ground-truth rectangles
         a_area = (boxes_a[..., 2] - boxes_a[..., 0]) * (boxes_a[..., 3] - boxes_a[..., 1])
         b_area = (boxes_b[..., 2] - boxes_b[..., 0]) * (boxes_b[..., 3] - boxes_b[..., 1])
 
-        union_area = (a_area + b_area - intersection_area)
+        union_area = a_area + b_area - intersection_area
 
         iou_score = intersection_area / (union_area + BoxIouCalculator.EPSILON)
 
         return iou_score
 
 
 class IObjectFormater:
@@ -146,30 +146,15 @@
     """
     Class to compute batch score
     """
     def __init__(self, object_formater: IObjectFormater, iou_calculator: IouCalculator):
         self.object_formater = object_formater
         self.iou_calculator = iou_calculator
 
-    def batch_score(self, model, inputs, targets, batch_size):
-        """
-        Compute batch score
-
-        Parameters
-        ----------
-        model
-            the model used for the object detection
-        inputs
-            Input samples to be explained.
-        targets
-            model outputs
-        batch_size
-            number of masked samples to explain at once, if None process all at once.
-        """
-        return inference_batching(self.score, model, inputs, targets, batch_size)
+        self.batch_score = operator_batching(self.score)
 
     def score(self, model, inp, object_ref) -> tf.Tensor:
         """
         Compute the matching score between prediction and a given object
 
         Parameters
         ----------
```

### Comparing `Xplique-0.4.3/xplique/attributions/occlusion.py` & `Xplique-1.0.0/xplique/attributions/occlusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,34 @@
     Parameters
     ----------
     model
         The model from which we want to obtain explanations
     batch_size
         Number of pertubed samples to explain at once.
         Default to 32.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     patch_size
         Size of the patches to apply, if integer then assume an hypercube.
     patch_stride
         Stride between two patches, if integer then assume an hypercube.
     occlusion_value
         Value used as occlusion.
     """
 
     def __init__(self,
                  model: Callable,
                  batch_size: Optional[int] = 32,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  patch_size: Union[int, Tuple[int, int]] = 3,
                  patch_stride: Union[int, Tuple[int, int]] = 3,
                  occlusion_value: float = 0.0):
-        super().__init__(model, batch_size)
+        super().__init__(model, batch_size, operator)
 
         self.patch_size = patch_size
         self.patch_stride = patch_stride
         self.occlusion_value = occlusion_value
 
     @sanitize_input_output
     def explain(self,
```

### Comparing `Xplique-0.4.3/xplique/attributions/rise.py` & `Xplique-1.0.0/xplique/attributions/rise.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     Parameters
     ----------
     model
         The model from which we want to obtain explanations
     batch_size
         Number of pertubed samples to explain at once.
         Default to 32.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     nb_samples
         Number of masks generated for Monte Carlo sampling.
     grid_size
         Size of the grid used to generate the scaled-down masks. Masks are then rescale to
         and cropped to input_size. Can be a tuple for different cutting depending on the dimension.
     preservation_probability
         Probability of preservation for each pixel (or the percentage of non-masked pixels in
@@ -38,18 +42,19 @@
     # Avoid zero division during procedure. (the value is not important, as if the denominator is
     # zero, then the nominator will also be zero).
     EPSILON = tf.constant(1e-4)
 
     def __init__(self,
                  model: Callable,
                  batch_size: Optional[int] = 32,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  nb_samples: int = 4000,
                  grid_size: Union[int, Tuple[int]] = 7,
                  preservation_probability: float = .5):
-        super().__init__(model, batch_size)
+        super().__init__(model, batch_size, operator)
 
         self.nb_samples = nb_samples
         self.grid_size = grid_size
         self.preservation_probability = preservation_probability
         self.binary_masks = Rise._get_masks(self.nb_samples, self.grid_size,
                                             self.preservation_probability)
```

### Comparing `Xplique-0.4.3/xplique/attributions/saliency.py` & `Xplique-1.0.0/xplique/attributions/saliency.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Module related to Saliency maps method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import batch_gradient
 from ..types import Optional, Union
 
 
 class Saliency(WhiteBoxExplainer):
     """
     Used to compute the absolute gradient of the output relative to the input.
 
@@ -34,14 +33,18 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
         """
@@ -61,15 +64,15 @@
             More information in the documentation.
 
         Returns
         -------
         explanations
             Saliency maps.
         """
-        gradients = batch_gradient(self.model, inputs, targets, self.batch_size)
+        gradients = self.batch_gradient(self.model, inputs, targets, self.batch_size)
         gradients = tf.abs(gradients)
 
         # if the image is a RGB, take the maximum magnitude across the channels (see Ref.)
         if len(gradients.shape) == 4:
             gradients = tf.reduce_max(gradients, axis=-1)
 
         return gradients
```

### Comparing `Xplique-0.4.3/xplique/attributions/smoothgrad.py` & `Xplique-1.0.0/xplique/attributions/smoothgrad.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Module related to SmoothGrad method
 """
 
 import tensorflow as tf
 import numpy as np
 
 from .base import WhiteBoxExplainer, sanitize_input_output
-from ..commons import repeat_labels, batch_gradient, batch_tensor
-from ..types import Tuple, Union, Optional
+from ..commons import repeat_labels, batch_tensor
+from ..types import Tuple, Union, Optional, Callable
 
 
 class SmoothGrad(WhiteBoxExplainer):
     """
     Used to compute the SmoothGrad, by averaging Saliency maps of noisy samples centered on the
     original sample.
 
@@ -27,27 +27,32 @@
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     nb_samples
         Number of noisy samples generated for the smoothing procedure.
     noise
         Scalar, noise used as standard deviation of a normal law centered on zero.
     """
 
     def __init__(self,
                  model: tf.keras.Model,
                  output_layer: Optional[Union[str, int]] = None,
                  batch_size: Optional[int] = 32,
+                 operator: Optional[Callable[[tf.keras.Model, tf.Tensor, tf.Tensor], float]] = None,
                  nb_samples: int = 50,
                  noise: float = 0.2):
-        super().__init__(model, output_layer, batch_size)
+        super().__init__(model, output_layer, batch_size, operator)
         self.nb_samples = nb_samples
         self.noise = noise
 
     @sanitize_input_output
     def explain(self,
                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None) -> tf.Tensor:
@@ -78,15 +83,15 @@
         noisy_mask = SmoothGrad._get_noisy_mask((self.nb_samples, *inputs.shape[1:]), self.noise)
 
         for x_batch, y_batch in batch_tensor((inputs, targets),
                                              max(batch_size // self.nb_samples, 1)):
             noisy_inputs = SmoothGrad._apply_noise(x_batch, noisy_mask)
             repeated_targets = repeat_labels(y_batch, self.nb_samples)
             # compute the gradient of each noisy samples generated
-            gradients = batch_gradient(self.model, noisy_inputs, repeated_targets, batch_size)
+            gradients = self.batch_gradient(self.model, noisy_inputs, repeated_targets, batch_size)
             # group by inputs and compute the average gradient
             gradients = tf.reshape(gradients, (-1, self.nb_samples, *gradients.shape[1:]))
             reduced_gradients = self._reduce_gradients(gradients)
 
             smoothed_gradients = reduced_gradients if smoothed_gradients is None else tf.concat(
                 [smoothed_gradients, reduced_gradients], axis=0)
```

### Comparing `Xplique-0.4.3/xplique/attributions/square_grad.py` & `Xplique-1.0.0/xplique/attributions/vargrad.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 """
-Module related to SquareGrad method
+Module related to VarGrad method
 """
 
 import tensorflow as tf
 
 from .smoothgrad import SmoothGrad
 
 
-class SquareGrad(SmoothGrad):
+class VarGrad(SmoothGrad):
     """
-    SquareGrad (or SmoothGrad^2) is an unpublished variant of classic SmoothGrad which squares
-    each gradients of the noisy inputs before averaging.
+     VarGrad is a variance analog to SmoothGrad.
 
-    Ref. Hooker & al., A Benchmark for Interpretability Methods in Deep Neural Networks (2019).
-    https://papers.nips.cc/paper/9167-a-benchmark-for-interpretability-methods-in-deep-neural-networks.pdf
+    Ref. Adebayo & al., Sanity check for Saliency map (2018).
+    https://papers.nips.cc/paper/8160-sanity-checks-for-saliency-maps.pdf
 
     Parameters
     ----------
     model
         The model from which we want to obtain explanations
     output_layer
         Layer to target for the outputs (e.g logits or after softmax).
         If an `int` is provided it will be interpreted as a layer index.
         If a `string` is provided it will look for the layer name.
 
         Default to the last layer.
         It is recommended to use the layer before Softmax.
     batch_size
         Number of inputs to explain at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     nb_samples
         Number of noisy samples generated for the smoothing procedure.
     noise
         Scalar, noise used as standard deviation of a normal law centered on zero.
     """
 
     @staticmethod
     @tf.function
     def _reduce_gradients(gradients: tf.Tensor) -> tf.Tensor:
         """
-        Reduce the gradients using the square of the gradients obtained on each noisy samples.
+        Reduce the gradients using the variance obtained on each noisy samples.
 
         Parameters
         ----------
         gradients
             Gradients to reduce the sampling dimension for each inputs.
 
         Returns
         -------
         reduced_gradients
             Single saliency map for each input.
         """
-        return tf.math.reduce_mean(gradients**2, axis=1)
+        return tf.math.reduce_variance(gradients, axis=1)
```

### Comparing `Xplique-0.4.3/xplique/commons/callable_operations.py` & `Xplique-1.0.0/xplique/commons/callable_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Custom callable operations
 """
 
 import tensorflow as tf
 
-from .tf_operations import inference_batching
-from ..types import Callable, Optional
+from ..types import Callable
 
 def predictions_one_hot_callable(
     model: Callable,
     inputs: tf.Tensor,
     targets: tf.Tensor) -> tf.Tensor:
     """
     Compute predictions scores, only for the label class, for a batch of samples.
@@ -51,34 +50,7 @@
             # The prediction dimension disappeared
             pred = tf.expand_dims(pred, axis=1)
 
     pred = tf.cast(pred, dtype=tf.float32)
     scores = tf.reduce_sum(pred * targets, axis=-1)
 
     return scores
-
-
-def batch_predictions_one_hot_callable(model: Callable,
-                              inputs: tf.Tensor,
-                              targets: tf.Tensor,
-                              batch_size: Optional[int] = None) -> tf.Tensor:
-    """
-    Compute predictions scores, only for the label class, for the samples passed. Take
-    care of splitting in multiple batches if batch_size is specified.
-
-    Parameters
-    ----------
-    model
-        Model used for computing predictions score.
-    inputs
-        Input samples to be explained.
-    targets
-        One-hot encoded labels or regression target (e.g {+1, -1}), one for each sample.
-    batch_size
-        Number of samples to predict at once, if None compute all at once.
-
-    Returns
-    -------
-    scores
-        Predictions scores computed, only for the label class.
-    """
-    return inference_batching(predictions_one_hot_callable, model, inputs, targets, batch_size)
```

### Comparing `Xplique-0.4.3/xplique/commons/data_conversion.py` & `Xplique-1.0.0/xplique/commons/data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/commons/model_override.py` & `Xplique-1.0.0/xplique/commons/model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/concepts/cav.py` & `Xplique-1.0.0/xplique/concepts/cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/concepts/tcav.py` & `Xplique-1.0.0/xplique/concepts/tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/features_visualizations/losses.py` & `Xplique-1.0.0/xplique/features_visualizations/losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/features_visualizations/objectives.py` & `Xplique-1.0.0/xplique/features_visualizations/objectives.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
         """
         # the number of inputs will be the number of combinations possible
         # of the objectives, the mask are used to take into account
         # these combinations
         nb_sub_objectives = len(self.multipliers)
 
         # re-arrange to match the different objectives with the model outputs
-        masks = np.array([np.array(m) for m in itertools.product(*self.masks)])
-        masks = [tf.cast(tf.stack(masks[:, i]), tf.float32) for i in
+        masks = np.array([np.array(m, dtype=object) for m in itertools.product(*self.masks)])
+        masks = [tf.cast(tf.stack(list(masks[:, i])), tf.float32) for i in
                  range(nb_sub_objectives)]
 
         # the name of each combination is the concatenation of each objectives
         names = np.array([' & '.join(names) for names in
                            itertools.product(*self.names)])
         # one multiplier by sub-objective
         multipliers = tf.constant(self.multipliers)
```

### Comparing `Xplique-0.4.3/xplique/features_visualizations/optim.py` & `Xplique-1.0.0/xplique/features_visualizations/optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/features_visualizations/preconditioning.py` & `Xplique-1.0.0/xplique/features_visualizations/preconditioning.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/features_visualizations/regularizers.py` & `Xplique-1.0.0/xplique/features_visualizations/regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/features_visualizations/transformations.py` & `Xplique-1.0.0/xplique/features_visualizations/transformations.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/metrics/base.py` & `Xplique-1.0.0/xplique/metrics/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from abc import ABC, abstractmethod
 
 import tensorflow as tf
 import numpy as np
 
-from ..commons import numpy_sanitize
+from ..commons import numpy_sanitize, get_inference_function
 from ..types import Callable, Optional, Union
 
 
 class BaseAttributionMetric(ABC):
     """
     Base class for Attribution Metric.
 
@@ -87,16 +87,34 @@
         Model used for computing explanations.
     inputs
         Input samples to be explained.
     targets
         One-hot encoded labels or regression target (e.g {+1, -1}), one for each sample.
     batch_size
         Number of samples to evaluate at once, if None compute all at once.
+    operator
+        Function g to explain, g take 3 parameters (f, x, y) and should return a scalar,
+        with f the model, x the inputs and y the targets. If None, use the standard
+        operator g(f, x, y) = f(x)[y].
     """
 
+    def __init__(self,
+                 model: tf.keras.Model,
+                 inputs: Union[tf.data.Dataset, tf.Tensor, np.ndarray],
+                 targets: Optional[Union[tf.Tensor, np.ndarray]] = None,
+                 batch_size: Optional[int] = 64,
+                 operator: Optional[Callable] = None,
+                 ):
+        # pylint: disable=R0913
+        super().__init__(model, inputs, targets, batch_size)
+
+        # define the inference function according to the model type
+        self.inference_function, self.batch_inference_function = \
+            get_inference_function(model, operator)
+
     @abstractmethod
     def evaluate(self,
                  explanations: Union[tf.Tensor, np.array]) -> float:
         """
         Compute the score of the given explanations.
 
         Parameters
```

### Comparing `Xplique-0.4.3/xplique/metrics/representativity.py` & `Xplique-1.0.0/xplique/metrics/representativity.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/metrics/stability.py` & `Xplique-1.0.0/xplique/metrics/stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/plots/image.py` & `Xplique-1.0.0/xplique/plots/image.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/plots/metrics.py` & `Xplique-1.0.0/xplique/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/plots/tabular.py` & `Xplique-1.0.0/xplique/plots/tabular.py`

 * *Files identical despite different names*

### Comparing `Xplique-0.4.3/xplique/plots/timeseries.py` & `Xplique-1.0.0/xplique/plots/timeseries.py`

 * *Files identical despite different names*

