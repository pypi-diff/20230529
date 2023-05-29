# Comparing `tmp/financepy-0.290.tar.gz` & `tmp/financepy-0.300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financepy-0.290.tar", last modified: Wed May 10 16:52:55 2023, max compression
+gzip compressed data, was "financepy-0.300.tar", last modified: Mon May 29 09:50:24 2023, max compression
```

## Comparing `financepy-0.290.tar` & `financepy-0.300.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:55.134478 financepy-0.290/
--rw-rw-rw-   0        0        0    35823 2020-09-30 09:26:37.000000 financepy-0.290/LICENSE
--rw-rw-rw-   0        0        0     7284 2023-05-10 16:52:55.132487 financepy-0.290/PKG-INFO
--rw-rw-rw-   0        0        0     6687 2023-04-21 19:06:18.000000 financepy-0.290/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.211156 financepy-0.290/financepy/
--rw-rw-rw-   0        0        0      453 2023-05-10 16:52:52.000000 financepy-0.290/financepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.275505 financepy-0.290/financepy/market/
--rw-rw-rw-   0        0        0        0 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.306422 financepy-0.290/financepy/market/curves/
--rw-rw-rw-   0        0        0      308 2023-02-13 16:33:55.000000 financepy-0.290/financepy/market/curves/__init__.py
--rw-rw-rw-   0        0        0    17339 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve.py
--rw-rw-rw-   0        0        0     5170 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_flat.py
--rw-rw-rw-   0        0        0     6789 2023-02-13 16:33:55.000000 financepy-0.290/financepy/market/curves/discount_curve_ns.py
--rw-rw-rw-   0        0        0     7392 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_nss.py
--rw-rw-rw-   0        0        0     6281 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_poly.py
--rw-rw-rw-   0        0        0     5982 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_pwf.py
--rw-rw-rw-   0        0        0     5825 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_pwl.py
--rw-rw-rw-   0        0        0     5649 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_zeros.py
--rw-rw-rw-   0        0        0    12495 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/curves/interpolator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.308417 financepy-0.290/financepy/market/prices/
--rw-rw-rw-   0        0        0       25 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/prices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.336355 financepy-0.290/financepy/market/volatility/
--rw-rw-rw-   0        0        0      172 2021-12-22 21:07:08.000000 financepy-0.290/financepy/market/volatility/__init__.py
--rw-rw-rw-   0        0        0     2747 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/volatility/equity_vol_curve.py
--rw-rw-rw-   0        0        0    29961 2023-04-21 18:35:46.000000 financepy-0.290/financepy/market/volatility/equity_vol_surface.py
--rw-rw-rw-   0        0        0    47487 2022-08-31 19:10:11.000000 financepy-0.290/financepy/market/volatility/fx_vol_surface.py
--rw-rw-rw-   0        0        0    92029 2022-08-31 19:10:11.000000 financepy-0.290/financepy/market/volatility/fx_vol_surface_plus.py
--rw-rw-rw-   0        0        0     7343 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve.py
--rw-rw-rw-   0        0        0     1497 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve_fn.py
--rw-rw-rw-   0        0        0    36053 2023-04-21 18:35:56.000000 financepy-0.290/financepy/market/volatility/swaption_vol_surface.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.464063 financepy-0.290/financepy/models/
--rw-rw-rw-   0        0        0      837 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/__init__.py
--rw-rw-rw-   0        0        0     2299 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/bachelier.py
--rw-rw-rw-   0        0        0    30528 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/bdt_tree.py
--rw-rw-rw-   0        0        0    39920 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/bk_tree.py
--rw-rw-rw-   0        0        0    16639 2023-04-14 12:22:10.000000 financepy-0.290/financepy/models/black.py
--rw-rw-rw-   0        0        0    10633 2023-05-10 16:37:54.000000 financepy-0.290/financepy/models/black_scholes.py
--rw-rw-rw-   0        0        0    17933 2023-02-25 17:11:47.000000 financepy-0.290/financepy/models/black_scholes_analytic.py
--rw-rw-rw-   0        0        0     6944 2021-12-22 21:43:40.000000 financepy-0.290/financepy/models/black_scholes_mc.py
--rw-rw-rw-   0        0        0     3117 2021-12-22 21:35:15.000000 financepy-0.290/financepy/models/black_scholes_mc_tests.py
--rw-rw-rw-   0        0        0     2888 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/black_shifted.py
--rw-rw-rw-   0        0        0        0 2022-11-22 10:41:15.000000 financepy-0.290/financepy/models/bond_analytics.py
--rw-rw-rw-   0        0        0    10102 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/cir_mc.py
--rw-rw-rw-   0        0        0     8510 2023-03-12 16:15:39.000000 financepy-0.290/financepy/models/equity_barrier_models.py
--rw-rw-rw-   0        0        0     7178 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/equity_crr_tree.py
--rw-rw-rw-   0        0        0     5689 2023-05-10 16:33:55.000000 financepy-0.290/financepy/models/equity_lsmc.py
--rw-rw-rw-   0        0        0     7955 2023-04-21 18:55:08.000000 financepy-0.290/financepy/models/finite_difference.py
--rw-rw-rw-   0        0        0     4944 2023-04-14 12:22:10.000000 financepy-0.290/financepy/models/finite_difference_PSOR.py
--rw-rw-rw-   0        0        0     1725 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/gauss_copula.py
--rw-rw-rw-   0        0        0     6379 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gauss_copula_lhp.py
--rw-rw-rw-   0        0        0     5638 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gauss_copula_lhplus.py
--rw-rw-rw-   0        0        0    14108 2022-06-10 20:13:01.000000 financepy-0.290/financepy/models/gauss_copula_onefactor.py
--rw-rw-rw-   0        0        0     7254 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gbm_process_simulator.py
--rw-rw-rw-   0        0        0    14264 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/heston.py
--rw-rw-rw-   0        0        0    50919 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/hw_tree.py
--rw-rw-rw-   0        0        0    33901 2021-12-22 21:46:06.000000 financepy-0.290/financepy/models/lmm_mc.py
--rw-rw-rw-   0        0        0     4361 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/loss_dbn_builder.py
--rw-rw-rw-   0        0        0     5484 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/merton_firm.py
--rw-rw-rw-   0        0        0     6022 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/merton_firm_mkt.py
--rw-rw-rw-   0        0        0      434 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/model.py
--rw-rw-rw-   0        0        0     1985 2021-12-22 19:57:45.000000 financepy-0.290/financepy/models/option_implied_dbn.py
--rw-rw-rw-   0        0        0    14570 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/process_simulator.py
--rw-rw-rw-   0        0        0     3822 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/rates_ho_lee.py
--rw-rw-rw-   0        0        0    10574 2023-04-14 13:09:24.000000 financepy-0.290/financepy/models/sabr.py
--rw-rw-rw-   0        0        0     8306 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/sabr_shifted.py
--rw-rw-rw-   0        0        0     5321 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/sobol.py
--rw-rw-rw-   0        0        0   120492 2020-12-08 14:37:22.000000 financepy-0.290/financepy/models/sobolcoeff.npz
--rw-rw-rw-   0        0        0     1800 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/student_t_copula.py
--rw-rw-rw-   0        0        0     3303 2021-11-09 10:39:55.000000 financepy-0.290/financepy/models/vasicek_mc.py
--rw-rw-rw-   0        0        0     8210 2022-06-10 20:10:22.000000 financepy-0.290/financepy/models/volatility_fns.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.469048 financepy-0.290/financepy/products/
--rw-rw-rw-   0        0        0        0 2020-09-30 09:26:37.000000 financepy-0.290/financepy/products/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.525896 financepy-0.290/financepy/products/bonds/
--rw-rw-rw-   0        0        0      367 2023-04-23 13:18:26.000000 financepy-0.290/financepy/products/bonds/__init__.py
--rw-rw-rw-   0        0        0    40484 2023-04-23 13:34:35.000000 financepy-0.290/financepy/products/bonds/bond.py
--rw-rw-rw-   0        0        0     7744 2022-03-20 13:06:59.000000 financepy-0.290/financepy/products/bonds/bond_annuity.py
--rw-rw-rw-   0        0        0     9793 2022-03-20 13:01:16.000000 financepy-0.290/financepy/products/bonds/bond_callable.py
--rw-rw-rw-   0        0        0    26813 2022-03-20 13:14:56.000000 financepy-0.290/financepy/products/bonds/bond_convertible.py
--rw-rw-rw-   0        0        0    19575 2022-03-20 13:03:48.000000 financepy-0.290/financepy/products/bonds/bond_frn.py
--rw-rw-rw-   0        0        0     6067 2022-03-20 13:02:32.000000 financepy-0.290/financepy/products/bonds/bond_future.py
--rw-rw-rw-   0        0        0     5176 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/bond_market.py
--rw-rw-rw-   0        0        0     6495 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/bonds/bond_mortgage.py
--rw-rw-rw-   0        0        0     5841 2022-03-20 13:04:01.000000 financepy-0.290/financepy/products/bonds/bond_option.py
--rw-rw-rw-   0        0        0    11494 2022-03-20 13:04:21.000000 financepy-0.290/financepy/products/bonds/bond_portfolio.py
--rw-rw-rw-   0        0        0    28075 2023-02-24 13:55:17.000000 financepy-0.290/financepy/products/bonds/bond_zero.py
--rw-rw-rw-   0        0        0     6784 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/yield_curve.py
--rw-rw-rw-   0        0        0     5746 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/yield_curve_model.py
--rw-rw-rw-   0        0        0     7056 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/bonds/zero_curve.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.555346 financepy-0.290/financepy/products/credit/
--rw-rw-rw-   0        0        0      197 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/credit/__init__.py
--rw-rw-rw-   0        0        0    34584 2022-08-31 17:54:32.000000 financepy-0.290/financepy/products/credit/cds.py
--rw-rw-rw-   0        0        0    13492 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/credit/cds_basket.py
--rw-rw-rw-   0        0        0     8958 2022-08-31 18:05:32.000000 financepy-0.290/financepy/products/credit/cds_curve.py
--rw-rw-rw-   0        0        0    14463 2022-08-31 18:16:21.000000 financepy-0.290/financepy/products/credit/cds_index_option.py
--rw-rw-rw-   0        0        0    19440 2022-08-31 18:13:43.000000 financepy-0.290/financepy/products/credit/cds_index_portfolio.py
--rw-rw-rw-   0        0        0     6774 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/credit/cds_option.py
--rw-rw-rw-   0        0        0     8960 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/credit/cds_tranche.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.620179 financepy-0.290/financepy/products/equity/
--rw-rw-rw-   0        0        0      814 2023-03-12 15:30:43.000000 financepy-0.290/financepy/products/equity/__init__.py
--rw-rw-rw-   0        0        0     4523 2022-12-24 15:09:21.000000 financepy-0.290/financepy/products/equity/equity_american_option.py
--rw-rw-rw-   0        0        0    30586 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_asian_option.py
--rw-rw-rw-   0        0        0    11033 2023-03-12 16:16:22.000000 financepy-0.290/financepy/products/equity/equity_barrier_option.py
--rw-rw-rw-   0        0        0     9960 2023-04-21 18:57:50.000000 financepy-0.290/financepy/products/equity/equity_basket_option.py
--rw-rw-rw-   0        0        0     8409 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/equity/equity_binomial_tree.py
--rw-rw-rw-   0        0        0     9434 2022-06-10 19:55:23.000000 financepy-0.290/financepy/products/equity/equity_chooser_option.py
--rw-rw-rw-   0        0        0     7546 2022-06-10 19:56:04.000000 financepy-0.290/financepy/products/equity/equity_cliquet_option.py
--rw-rw-rw-   0        0        0    18066 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_compound_option.py
--rw-rw-rw-   0        0        0     7763 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_digital_option.py
--rw-rw-rw-   0        0        0    10384 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_fixed_lookback_option.py
--rw-rw-rw-   0        0        0     8866 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_float_lookback_option.py
--rw-rw-rw-   0        0        0     4868 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_forward.py
--rw-rw-rw-   0        0        0     9939 2023-04-14 12:22:10.000000 financepy-0.290/financepy/products/equity/equity_index_option.py
--rw-rw-rw-   0        0        0     1950 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/equity/equity_model_types.py
--rw-rw-rw-   0        0        0    19683 2021-12-25 18:48:58.000000 financepy-0.290/financepy/products/equity/equity_one_touch_option.py
--rw-rw-rw-   0        0        0     6735 2021-12-23 15:44:42.000000 financepy-0.290/financepy/products/equity/equity_option.py
--rw-rw-rw-   0        0        0    12100 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_rainbow_option.py
--rw-rw-rw-   0        0        0     8584 2023-04-21 18:30:04.000000 financepy-0.290/financepy/products/equity/equity_swap.py
--rw-rw-rw-   0        0        0    14016 2023-04-21 18:38:13.000000 financepy-0.290/financepy/products/equity/equity_swap_leg.py
--rw-rw-rw-   0        0        0    24907 2023-02-13 16:33:55.000000 financepy-0.290/financepy/products/equity/equity_vanilla_option.py
--rw-rw-rw-   0        0        0    10614 2021-12-22 21:00:14.000000 financepy-0.290/financepy/products/equity/equity_variance_swap.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.660595 financepy-0.290/financepy/products/fx/
--rw-rw-rw-   0        0        0      375 2021-12-25 19:13:13.000000 financepy-0.290/financepy/products/fx/__init__.py
--rw-rw-rw-   0        0        0    17295 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_barrier_option.py
--rw-rw-rw-   0        0        0     6174 2021-12-21 13:58:02.000000 financepy-0.290/financepy/products/fx/fx_digital_option.py
--rw-rw-rw-   0        0        0     9113 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_fixed_lookback_option.py
--rw-rw-rw-   0        0        0     7583 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_float_lookback_option.py
--rw-rw-rw-   0        0        0     7198 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_forward.py
--rw-rw-rw-   0        0        0     4868 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/fx/fx_mkt_conventions.py
--rw-rw-rw-   0        0        0    19515 2021-12-23 15:49:15.000000 financepy-0.290/financepy/products/fx/fx_one_touch_option.py
--rw-rw-rw-   0        0        0     5292 2021-12-23 15:43:21.000000 financepy-0.290/financepy/products/fx/fx_option.py
--rw-rw-rw-   0        0        0    11013 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_rainbow_option.py
--rw-rw-rw-   0        0        0    28014 2023-05-10 16:06:39.000000 financepy-0.290/financepy/products/fx/fx_vanilla_option.py
--rw-rw-rw-   0        0        0    10072 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_variance_swap.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.673555 financepy-0.290/financepy/products/inflation/
--rw-rw-rw-   0        0        0     6773 2023-02-24 13:55:17.000000 financepy-0.290/financepy/products/inflation/FinInflationBond.py
--rw-rw-rw-   0        0        0     4361 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/FinInflationIndexCurve.py
--rw-rw-rw-   0        0        0     6672 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/FinInflationSwap.py
--rw-rw-rw-   0        0        0    21176 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/inflation/FinInflationSwapCurve.py
--rw-rw-rw-   0        0        0       33 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.722432 financepy-0.290/financepy/products/rates/
--rw-rw-rw-   0        0        0      435 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/__init__.py
--rw-rw-rw-   0        0        0     9390 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/bermudan_swaption.py
--rw-rw-rw-   0        0        0    11427 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/callable_swap.py
--rw-rw-rw-   0        0        0    22970 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/dual_curve.py
--rw-rw-rw-   0        0        0     7979 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_basis_swap.py
--rw-rw-rw-   0        0        0    15095 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_cap_floor.py
--rw-rw-rw-   0        0        0     1246 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_conventions.py
--rw-rw-rw-   0        0        0     6722 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_deposit.py
--rw-rw-rw-   0        0        0     7139 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_fra.py
--rw-rw-rw-   0        0        0     5822 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_future.py
--rw-rw-rw-   0        0        0    17758 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ibor_lmm_products.py
--rw-rw-rw-   0        0        0    27170 2022-08-31 19:10:11.000000 financepy-0.290/financepy/products/rates/ibor_single_curve.py
--rw-rw-rw-   0        0        0    11620 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ibor_swap.py
--rw-rw-rw-   0        0        0    17602 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_swaption.py
--rw-rw-rw-   0        0        0    10266 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois.py
--rw-rw-rw-   0        0        0     7437 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois_basis_swap.py
--rw-rw-rw-   0        0        0    24892 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois_curve.py
--rw-rw-rw-   0        0        0    11327 2023-04-14 12:22:10.000000 financepy-0.290/financepy/products/rates/swap_fixed_leg.py
--rw-rw-rw-   0        0        0    12625 2023-03-12 15:30:43.000000 financepy-0.290/financepy/products/rates/swap_float_leg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.779804 financepy-0.290/financepy/utils/
--rw-rw-rw-   0        0        0      371 2021-10-05 08:15:43.000000 financepy-0.290/financepy/utils/__init__.py
--rw-rw-rw-   0        0        0     1553 2021-10-05 08:15:43.000000 financepy-0.290/financepy/utils/amount.py
--rw-rw-rw-   0        0        0    33935 2022-03-20 08:54:30.000000 financepy-0.290/financepy/utils/calendar.py
--rw-rw-rw-   0        0        0      630 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/currency.py
--rw-rw-rw-   0        0        0    32484 2023-02-13 16:33:55.000000 financepy-0.290/financepy/utils/date.py
--rw-rw-rw-   0        0        0    10541 2022-10-02 12:44:23.000000 financepy-0.290/financepy/utils/day_count.py
--rw-rw-rw-   0        0        0      888 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/distribution.py
--rw-rw-rw-   0        0        0     1956 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/error.py
--rw-rw-rw-   0        0        0     1601 2022-10-02 12:44:23.000000 financepy-0.290/financepy/utils/frequency.py
--rw-rw-rw-   0        0        0     2972 2023-03-12 15:57:49.000000 financepy-0.290/financepy/utils/global_types.py
--rw-rw-rw-   0        0        0      447 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/global_vars.py
--rw-rw-rw-   0        0        0    15898 2023-03-12 15:30:43.000000 financepy-0.290/financepy/utils/helpers.py
--rw-rw-rw-   0        0        0     2927 2022-03-20 08:29:25.000000 financepy-0.290/financepy/utils/latex.py
--rw-rw-rw-   0        0        0    20984 2023-04-14 12:22:10.000000 financepy-0.290/financepy/utils/math.py
--rw-rw-rw-   0        0        0     2301 2022-12-28 10:41:39.000000 financepy-0.290/financepy/utils/polyfit.py
--rw-rw-rw-   0        0        0    11970 2023-05-04 07:59:23.000000 financepy-0.290/financepy/utils/schedule.py
--rw-rw-rw-   0        0        0      498 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/singleton.py
--rw-rw-rw-   0        0        0    29377 2022-11-22 11:57:17.000000 financepy-0.290/financepy/utils/solver_1d.py
--rw-rw-rw-   0        0        0    21755 2023-04-21 18:36:04.000000 financepy-0.290/financepy/utils/solver_cg.py
--rw-rw-rw-   0        0        0    13278 2023-04-21 18:38:22.000000 financepy-0.290/financepy/utils/solver_nm.py
--rw-rw-rw-   0        0        0     2754 2022-06-24 08:40:16.000000 financepy-0.290/financepy/utils/stats.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.272513 financepy-0.290/financepy.egg-info/
--rw-rw-rw-   0        0        0     7284 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10686 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 16:52:55.135478 financepy-0.290/setup.cfg
--rw-rw-rw-   0        0        0     1996 2021-10-05 08:15:44.000000 financepy-0.290/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:52:55.127485 financepy-0.290/tests_golden/
--rw-rw-rw-   0        0        0    17690 2022-12-28 17:24:50.000000 financepy-0.290/tests_golden/FinTestCases.py
--rw-rw-rw-   0        0        0      890 2023-03-13 18:31:42.000000 financepy-0.290/tests_golden/TestFinAmount.py
--rw-rw-rw-   0        0        0    22862 2023-05-10 16:07:46.000000 financepy-0.290/tests_golden/TestFinBond.py
--rw-rw-rw-   0        0        0     7598 2022-03-20 13:10:36.000000 financepy-0.290/tests_golden/TestFinBondAnnuity.py
--rw-rw-rw-   0        0        0     4588 2022-06-24 08:59:58.000000 financepy-0.290/tests_golden/TestFinBondConvertible.py
--rw-rw-rw-   0        0        0     6956 2022-06-24 09:00:24.000000 financepy-0.290/tests_golden/TestFinBondEmbeddedOptionBK.py
--rw-rw-rw-   0        0        0     6942 2022-06-24 09:01:06.000000 financepy-0.290/tests_golden/TestFinBondEmbeddedOptionHW.py
--rw-rw-rw-   0        0        0    14054 2022-03-20 12:33:53.000000 financepy-0.290/tests_golden/TestFinBondFRN.py
--rw-rw-rw-   0        0        0     6176 2022-03-20 08:53:51.000000 financepy-0.290/tests_golden/TestFinBondFutures.py
--rw-rw-rw-   0        0        0     2041 2021-12-21 13:16:15.000000 financepy-0.290/tests_golden/TestFinBondMortgage.py
--rw-rw-rw-   0        0        0    15002 2022-06-24 09:01:30.000000 financepy-0.290/tests_golden/TestFinBondOptionBDTModel.py
--rw-rw-rw-   0        0        0    14962 2022-06-24 09:03:01.000000 financepy-0.290/tests_golden/TestFinBondOptionBKModel.py
--rw-rw-rw-   0        0        0    18901 2022-06-24 09:04:04.000000 financepy-0.290/tests_golden/TestFinBondOptionHWModel.py
--rw-rw-rw-   0        0        0     2152 2022-10-02 12:44:23.000000 financepy-0.290/tests_golden/TestFinBondPortfolio.py
--rw-rw-rw-   0        0        0     4514 2022-06-10 21:00:21.000000 financepy-0.290/tests_golden/TestFinBondYieldCurve.py
--rw-rw-rw-   0        0        0     2924 2022-11-22 09:47:45.000000 financepy-0.290/tests_golden/TestFinBondZeroCoupon.py
--rw-rw-rw-   0        0        0     2472 2022-08-11 21:00:13.000000 financepy-0.290/tests_golden/TestFinBondZeroCurve.py
--rw-rw-rw-   0        0        0    23600 2022-01-22 13:18:12.000000 financepy-0.290/tests_golden/TestFinCDS.py
--rw-rw-rw-   0        0        0    13736 2022-06-24 09:26:11.000000 financepy-0.290/tests_golden/TestFinCDSBasket.py
--rw-rw-rw-   0        0        0     5636 2022-08-31 20:01:33.000000 financepy-0.290/tests_golden/TestFinCDSCurve.py
--rw-rw-rw-   0        0        0     5374 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSIndex.py
--rw-rw-rw-   0        0        0    11357 2022-06-24 09:05:07.000000 financepy-0.290/tests_golden/TestFinCDSIndexAdjustHazards.py
--rw-rw-rw-   0        0        0    10646 2022-06-24 09:05:28.000000 financepy-0.290/tests_golden/TestFinCDSIndexAdjustSpreads.py
--rw-rw-rw-   0        0        0     8588 2022-06-24 09:12:38.000000 financepy-0.290/tests_golden/TestFinCDSIndexOption.py
--rw-rw-rw-   0        0        0     8138 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSIndexPortfolio.py
--rw-rw-rw-   0        0        0    10741 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSOption.py
--rw-rw-rw-   0        0        0    10942 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSTranche.py
--rw-rw-rw-   0        0        0     1720 2022-03-20 08:54:04.000000 financepy-0.290/tests_golden/TestFinCalendar.py
--rw-rw-rw-   0        0        0     8660 2022-02-14 09:19:14.000000 financepy-0.290/tests_golden/TestFinDate.py
--rw-rw-rw-   0        0        0     3513 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDateAdjust.py
--rw-rw-rw-   0        0        0     1335 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDayCount.py
--rw-rw-rw-   0        0        0     3504 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurve.py
--rw-rw-rw-   0        0        0     1857 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveFlat.py
--rw-rw-rw-   0        0        0     7352 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveNS.py
--rw-rw-rw-   0        0        0     4340 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveNSS.py
--rw-rw-rw-   0        0        0     1499 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurvePolynomial.py
--rw-rw-rw-   0        0        0     2873 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveZeros.py
--rw-rw-rw-   0        0        0     6743 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurves.py
--rw-rw-rw-   0        0        0    11033 2022-12-28 17:23:07.000000 financepy-0.290/tests_golden/TestFinEquityAmericanMC.py
--rw-rw-rw-   0        0        0     7143 2022-12-25 20:34:58.000000 financepy-0.290/tests_golden/TestFinEquityAmericanOption.py
--rw-rw-rw-   0        0        0    14048 2022-01-22 09:41:29.000000 financepy-0.290/tests_golden/TestFinEquityAsianOption.py
--rw-rw-rw-   0        0        0     6546 2023-03-12 16:16:54.000000 financepy-0.290/tests_golden/TestFinEquityBarrierOption.py
--rw-rw-rw-   0        0        0     7653 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityBasketOption.py
--rw-rw-rw-   0        0        0     6414 2022-06-24 09:08:30.000000 financepy-0.290/tests_golden/TestFinEquityBinomialTree.py
--rw-rw-rw-   0        0        0     5534 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityChooserOption.py
--rw-rw-rw-   0        0        0     1996 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityCliquetOption.py
--rw-rw-rw-   0        0        0     5917 2022-06-24 09:08:45.000000 financepy-0.290/tests_golden/TestFinEquityCompoundOption.py
--rw-rw-rw-   0        0        0     5086 2022-06-24 09:16:47.000000 financepy-0.290/tests_golden/TestFinEquityDigitalOption.py
--rw-rw-rw-   0        0        0     2134 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityForward.py
--rw-rw-rw-   0        0        0    16388 2022-01-22 09:40:51.000000 financepy-0.290/tests_golden/TestFinEquityLookbackOption.py
--rw-rw-rw-   0        0        0     6191 2022-01-22 09:44:19.000000 financepy-0.290/tests_golden/TestFinEquityOneTouchOption.py
--rw-rw-rw-   0        0        0    17897 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityRainbowOption.py
--rw-rw-rw-   0        0        0     7872 2023-04-14 13:24:43.000000 financepy-0.290/tests_golden/TestFinEquitySwap.py
--rw-rw-rw-   0        0        0    10841 2023-03-13 18:31:42.000000 financepy-0.290/tests_golden/TestFinEquityVanillaOption.py
--rw-rw-rw-   0        0        0     2341 2021-12-22 21:02:43.000000 financepy-0.290/tests_golden/TestFinEquityVarianceSwap.py
--rw-rw-rw-   0        0        0     4021 2021-12-22 21:03:03.000000 financepy-0.290/tests_golden/TestFinEquityVolSurface.py
--rw-rw-rw-   0        0        0     4803 2022-06-24 09:10:42.000000 financepy-0.290/tests_golden/TestFinFXAmericanOption.py
--rw-rw-rw-   0        0        0     6480 2022-06-24 09:10:55.000000 financepy-0.290/tests_golden/TestFinFXBarrierOption.py
--rw-rw-rw-   0        0        0     2644 2021-12-21 13:53:03.000000 financepy-0.290/tests_golden/TestFinFXDigitalOption.py
--rw-rw-rw-   0        0        0     3170 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXForward.py
--rw-rw-rw-   0        0        0    15254 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXLookbackOption.py
--rw-rw-rw-   0        0        0     6018 2021-12-25 19:11:30.000000 financepy-0.290/tests_golden/TestFinFXOneTouchOption.py
--rw-rw-rw-   0        0        0     5147 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXOptionSABR.py
--rw-rw-rw-   0        0        0    17551 2023-05-10 16:04:00.000000 financepy-0.290/tests_golden/TestFinFXVanillaOption.py
--rw-rw-rw-   0        0        0     9858 2021-12-22 21:05:30.000000 financepy-0.290/tests_golden/TestFinFXVolSurface.py
--rw-rw-rw-   0        0        0    18123 2021-12-22 19:19:05.000000 financepy-0.290/tests_golden/TestFinFXVolSurfacePlus.py
--rw-rw-rw-   0        0        0    28257 2021-12-22 19:15:39.000000 financepy-0.290/tests_golden/TestFinIborBermudanSwaption.py
--rw-rw-rw-   0        0        0    14266 2021-12-22 19:16:48.000000 financepy-0.290/tests_golden/TestFinIborCapFloor.py
--rw-rw-rw-   0        0        0     1921 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborCapVolCurve.py
--rw-rw-rw-   0        0        0    25121 2022-06-24 11:50:45.000000 financepy-0.290/tests_golden/TestFinIborDualCurve.py
--rw-rw-rw-   0        0        0     1044 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborFuture.py
--rw-rw-rw-   0        0        0     9516 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborLMMProducts.py
--rw-rw-rw-   0        0        0    27549 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborSingleCurve.py
--rw-rw-rw-   0        0        0    14159 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborSwap.py
--rw-rw-rw-   0        0        0    27393 2022-03-20 08:53:09.000000 financepy-0.290/tests_golden/TestFinIborSwaption.py
--rw-rw-rw-   0        0        0    14923 2022-03-20 08:57:37.000000 financepy-0.290/tests_golden/TestFinInflationBond.py
--rw-rw-rw-   0        0        0     1424 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInflationIndexCurve.py
--rw-rw-rw-   0        0        0     2269 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInterpolate.py
--rw-rw-rw-   0        0        0     2209 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInterpolatedForwards.py
--rw-rw-rw-   0        0        0     4299 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinLossDbnBuilder.py
--rw-rw-rw-   0        0        0     2850 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinMath.py
--rw-rw-rw-   0        0        0     1910 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinMathAccruedInterp.py
--rw-rw-rw-   0        0        0     3679 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelBlack.py
--rw-rw-rw-   0        0        0     4958 2021-12-22 20:18:30.000000 financepy-0.290/tests_golden/TestFinModelBlackScholes.py
--rw-rw-rw-   0        0        0     2586 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelBlack_SABR_HW.py
--rw-rw-rw-   0        0        0     2455 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelCIR.py
--rw-rw-rw-   0        0        0     6657 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelHeston.py
--rw-rw-rw-   0        0        0     3595 2022-01-22 13:54:49.000000 financepy-0.290/tests_golden/TestFinModelMerton.py
--rw-rw-rw-   0        0        0    10334 2022-03-20 13:11:37.000000 financepy-0.290/tests_golden/TestFinModelRatesBDT.py
--rw-rw-rw-   0        0        0     5310 2022-03-20 13:06:22.000000 financepy-0.290/tests_golden/TestFinModelRatesBK.py
--rw-rw-rw-   0        0        0    11763 2022-03-20 13:11:16.000000 financepy-0.290/tests_golden/TestFinModelRatesHW.py
--rw-rw-rw-   0        0        0    17835 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelRatesLMM.py
--rw-rw-rw-   0        0        0     3182 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelSABR.py
--rw-rw-rw-   0        0        0     2689 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelShiftedSABR.py
--rw-rw-rw-   0        0        0    12233 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinNumbaNumpySpeed.py
--rw-rw-rw-   0        0        0     2302 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinOIS.py
--rw-rw-rw-   0        0        0    19529 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinOISCurve.py
--rw-rw-rw-   0        0        0     3818 2021-12-22 20:46:18.000000 financepy-0.290/tests_golden/TestFinOptionImpliedDbn.py
--rw-rw-rw-   0        0        0     1018 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinPieceCurve.py
--rw-rw-rw-   0        0        0     6178 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinProcessSimulator.py
--rw-rw-rw-   0        0        0    18118 2023-05-03 16:37:45.000000 financepy-0.290/tests_golden/TestFinSchedule.py
--rw-rw-rw-   0        0        0     1669 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSobol.py
--rw-rw-rw-   0        0        0     2442 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinStatistics.py
--rw-rw-rw-   0        0        0     8851 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSwapLegs.py
--rw-rw-rw-   0        0        0     4678 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSwaptionVolSurface.py
--rw-rw-rw-   0        0        0     1341 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinVasicekRateModel.py
--rw-rw-rw-   0        0        0     1358 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinVolatilityCurve.py
--rw-rw-rw-   0        0        0       56 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/__init__.py
--rw-rw-rw-   0        0        0     2443 2023-03-13 10:28:21.000000 financepy-0.290/tests_golden/runAllTests.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:24.038200 financepy-0.300/
+-rw-rw-rw-   0        0        0    35823 2020-09-30 09:26:37.000000 financepy-0.300/LICENSE
+-rw-rw-rw-   0        0        0     7284 2023-05-29 09:50:24.037201 financepy-0.300/PKG-INFO
+-rw-rw-rw-   0        0        0     6687 2023-04-21 19:06:18.000000 financepy-0.300/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.346046 financepy-0.300/financepy/
+-rw-rw-rw-   0        0        0      453 2023-05-29 09:50:22.000000 financepy-0.300/financepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.381952 financepy-0.300/financepy/market/
+-rw-rw-rw-   0        0        0        0 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.400900 financepy-0.300/financepy/market/curves/
+-rw-rw-rw-   0        0        0      308 2023-02-13 16:33:55.000000 financepy-0.300/financepy/market/curves/__init__.py
+-rw-rw-rw-   0        0        0    17339 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve.py
+-rw-rw-rw-   0        0        0     5170 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_flat.py
+-rw-rw-rw-   0        0        0     6789 2023-02-13 16:33:55.000000 financepy-0.300/financepy/market/curves/discount_curve_ns.py
+-rw-rw-rw-   0        0        0     7392 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_nss.py
+-rw-rw-rw-   0        0        0     6281 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_poly.py
+-rw-rw-rw-   0        0        0     5982 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_pwf.py
+-rw-rw-rw-   0        0        0     5825 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_pwl.py
+-rw-rw-rw-   0        0        0     5649 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/curves/discount_curve_zeros.py
+-rw-rw-rw-   0        0        0    12495 2021-10-05 08:15:43.000000 financepy-0.300/financepy/market/curves/interpolator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.403892 financepy-0.300/financepy/market/prices/
+-rw-rw-rw-   0        0        0       25 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/prices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.423839 financepy-0.300/financepy/market/volatility/
+-rw-rw-rw-   0        0        0      172 2021-12-22 21:07:08.000000 financepy-0.300/financepy/market/volatility/__init__.py
+-rw-rw-rw-   0        0        0     2747 2021-10-05 08:15:43.000000 financepy-0.300/financepy/market/volatility/equity_vol_curve.py
+-rw-rw-rw-   0        0        0    29961 2023-04-21 18:35:46.000000 financepy-0.300/financepy/market/volatility/equity_vol_surface.py
+-rw-rw-rw-   0        0        0    47487 2022-08-31 19:10:11.000000 financepy-0.300/financepy/market/volatility/fx_vol_surface.py
+-rw-rw-rw-   0        0        0    92029 2022-08-31 19:10:11.000000 financepy-0.300/financepy/market/volatility/fx_vol_surface_plus.py
+-rw-rw-rw-   0        0        0     7343 2021-11-06 12:48:44.000000 financepy-0.300/financepy/market/volatility/ibor_cap_vol_curve.py
+-rw-rw-rw-   0        0        0     1497 2021-10-05 08:15:43.000000 financepy-0.300/financepy/market/volatility/ibor_cap_vol_curve_fn.py
+-rw-rw-rw-   0        0        0    36053 2023-04-21 18:35:56.000000 financepy-0.300/financepy/market/volatility/swaption_vol_surface.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.510606 financepy-0.300/financepy/models/
+-rw-rw-rw-   0        0        0      837 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/__init__.py
+-rw-rw-rw-   0        0        0     2299 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/bachelier.py
+-rw-rw-rw-   0        0        0    30528 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/bdt_tree.py
+-rw-rw-rw-   0        0        0    39920 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/bk_tree.py
+-rw-rw-rw-   0        0        0    16639 2023-04-14 12:22:10.000000 financepy-0.300/financepy/models/black.py
+-rw-rw-rw-   0        0        0    10633 2023-05-10 16:37:54.000000 financepy-0.300/financepy/models/black_scholes.py
+-rw-rw-rw-   0        0        0    17933 2023-02-25 17:11:47.000000 financepy-0.300/financepy/models/black_scholes_analytic.py
+-rw-rw-rw-   0        0        0     6944 2021-12-22 21:43:40.000000 financepy-0.300/financepy/models/black_scholes_mc.py
+-rw-rw-rw-   0        0        0     3117 2021-12-22 21:35:15.000000 financepy-0.300/financepy/models/black_scholes_mc_tests.py
+-rw-rw-rw-   0        0        0     2888 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/black_shifted.py
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:41:15.000000 financepy-0.300/financepy/models/bond_analytics.py
+-rw-rw-rw-   0        0        0    10102 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/cir_mc.py
+-rw-rw-rw-   0        0        0     8283 2023-05-22 12:02:11.000000 financepy-0.300/financepy/models/equity_barrier_models.py
+-rw-rw-rw-   0        0        0     7178 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/equity_crr_tree.py
+-rw-rw-rw-   0        0        0     5689 2023-05-10 16:33:55.000000 financepy-0.300/financepy/models/equity_lsmc.py
+-rw-rw-rw-   0        0        0     7955 2023-04-21 18:55:08.000000 financepy-0.300/financepy/models/finite_difference.py
+-rw-rw-rw-   0        0        0     4944 2023-04-14 12:22:10.000000 financepy-0.300/financepy/models/finite_difference_PSOR.py
+-rw-rw-rw-   0        0        0     1725 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/gauss_copula.py
+-rw-rw-rw-   0        0        0     6379 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/gauss_copula_lhp.py
+-rw-rw-rw-   0        0        0     5638 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/gauss_copula_lhplus.py
+-rw-rw-rw-   0        0        0    14108 2022-06-10 20:13:01.000000 financepy-0.300/financepy/models/gauss_copula_onefactor.py
+-rw-rw-rw-   0        0        0     7254 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/gbm_process_simulator.py
+-rw-rw-rw-   0        0        0    14264 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/heston.py
+-rw-rw-rw-   0        0        0    50919 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/hw_tree.py
+-rw-rw-rw-   0        0        0    33901 2021-12-22 21:46:06.000000 financepy-0.300/financepy/models/lmm_mc.py
+-rw-rw-rw-   0        0        0     4361 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/loss_dbn_builder.py
+-rw-rw-rw-   0        0        0     5484 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/merton_firm.py
+-rw-rw-rw-   0        0        0     6022 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/merton_firm_mkt.py
+-rw-rw-rw-   0        0        0      434 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/model.py
+-rw-rw-rw-   0        0        0     1985 2021-12-22 19:57:45.000000 financepy-0.300/financepy/models/option_implied_dbn.py
+-rw-rw-rw-   0        0        0    14570 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/process_simulator.py
+-rw-rw-rw-   0        0        0     3822 2021-11-06 12:48:44.000000 financepy-0.300/financepy/models/rates_ho_lee.py
+-rw-rw-rw-   0        0        0    10574 2023-04-14 13:09:24.000000 financepy-0.300/financepy/models/sabr.py
+-rw-rw-rw-   0        0        0     8306 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/sabr_shifted.py
+-rw-rw-rw-   0        0        0     5321 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/sobol.py
+-rw-rw-rw-   0        0        0   120492 2020-12-08 14:37:22.000000 financepy-0.300/financepy/models/sobolcoeff.npz
+-rw-rw-rw-   0        0        0     1800 2021-10-05 08:15:43.000000 financepy-0.300/financepy/models/student_t_copula.py
+-rw-rw-rw-   0        0        0     3303 2021-11-09 10:39:55.000000 financepy-0.300/financepy/models/vasicek_mc.py
+-rw-rw-rw-   0        0        0     8210 2022-06-10 20:10:22.000000 financepy-0.300/financepy/models/volatility_fns.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.512602 financepy-0.300/financepy/products/
+-rw-rw-rw-   0        0        0        0 2020-09-30 09:26:37.000000 financepy-0.300/financepy/products/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.546521 financepy-0.300/financepy/products/bonds/
+-rw-rw-rw-   0        0        0      367 2023-04-23 13:18:26.000000 financepy-0.300/financepy/products/bonds/__init__.py
+-rw-rw-rw-   0        0        0    40484 2023-04-23 13:34:35.000000 financepy-0.300/financepy/products/bonds/bond.py
+-rw-rw-rw-   0        0        0     7744 2022-03-20 13:06:59.000000 financepy-0.300/financepy/products/bonds/bond_annuity.py
+-rw-rw-rw-   0        0        0     9793 2022-03-20 13:01:16.000000 financepy-0.300/financepy/products/bonds/bond_callable.py
+-rw-rw-rw-   0        0        0    26813 2022-03-20 13:14:56.000000 financepy-0.300/financepy/products/bonds/bond_convertible.py
+-rw-rw-rw-   0        0        0    19575 2022-03-20 13:03:48.000000 financepy-0.300/financepy/products/bonds/bond_frn.py
+-rw-rw-rw-   0        0        0     6067 2022-03-20 13:02:32.000000 financepy-0.300/financepy/products/bonds/bond_future.py
+-rw-rw-rw-   0        0        0     5176 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/bonds/bond_market.py
+-rw-rw-rw-   0        0        0     6495 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/bonds/bond_mortgage.py
+-rw-rw-rw-   0        0        0     5841 2022-03-20 13:04:01.000000 financepy-0.300/financepy/products/bonds/bond_option.py
+-rw-rw-rw-   0        0        0    11494 2022-03-20 13:04:21.000000 financepy-0.300/financepy/products/bonds/bond_portfolio.py
+-rw-rw-rw-   0        0        0    28075 2023-02-24 13:55:17.000000 financepy-0.300/financepy/products/bonds/bond_zero.py
+-rw-rw-rw-   0        0        0     6784 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/bonds/yield_curve.py
+-rw-rw-rw-   0        0        0     5746 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/bonds/yield_curve_model.py
+-rw-rw-rw-   0        0        0     7056 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/bonds/zero_curve.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.567462 financepy-0.300/financepy/products/credit/
+-rw-rw-rw-   0        0        0      197 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/credit/__init__.py
+-rw-rw-rw-   0        0        0    34584 2022-08-31 17:54:32.000000 financepy-0.300/financepy/products/credit/cds.py
+-rw-rw-rw-   0        0        0    13492 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/credit/cds_basket.py
+-rw-rw-rw-   0        0        0     8958 2022-08-31 18:05:32.000000 financepy-0.300/financepy/products/credit/cds_curve.py
+-rw-rw-rw-   0        0        0    14463 2022-08-31 18:16:21.000000 financepy-0.300/financepy/products/credit/cds_index_option.py
+-rw-rw-rw-   0        0        0    19440 2022-08-31 18:13:43.000000 financepy-0.300/financepy/products/credit/cds_index_portfolio.py
+-rw-rw-rw-   0        0        0     6774 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/credit/cds_option.py
+-rw-rw-rw-   0        0        0     8960 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/credit/cds_tranche.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.626298 financepy-0.300/financepy/products/equity/
+-rw-rw-rw-   0        0        0      814 2023-03-12 15:30:43.000000 financepy-0.300/financepy/products/equity/__init__.py
+-rw-rw-rw-   0        0        0     4523 2022-12-24 15:09:21.000000 financepy-0.300/financepy/products/equity/equity_american_option.py
+-rw-rw-rw-   0        0        0    30586 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_asian_option.py
+-rw-rw-rw-   0        0        0    11074 2023-05-22 12:02:11.000000 financepy-0.300/financepy/products/equity/equity_barrier_option.py
+-rw-rw-rw-   0        0        0     9960 2023-04-21 18:57:50.000000 financepy-0.300/financepy/products/equity/equity_basket_option.py
+-rw-rw-rw-   0        0        0     8409 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/equity/equity_binomial_tree.py
+-rw-rw-rw-   0        0        0     9434 2022-06-10 19:55:23.000000 financepy-0.300/financepy/products/equity/equity_chooser_option.py
+-rw-rw-rw-   0        0        0     7546 2022-06-10 19:56:04.000000 financepy-0.300/financepy/products/equity/equity_cliquet_option.py
+-rw-rw-rw-   0        0        0    18066 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_compound_option.py
+-rw-rw-rw-   0        0        0     7763 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_digital_option.py
+-rw-rw-rw-   0        0        0    10384 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_fixed_lookback_option.py
+-rw-rw-rw-   0        0        0     8866 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_float_lookback_option.py
+-rw-rw-rw-   0        0        0     4868 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_forward.py
+-rw-rw-rw-   0        0        0     9939 2023-04-14 12:22:10.000000 financepy-0.300/financepy/products/equity/equity_index_option.py
+-rw-rw-rw-   0        0        0     1950 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/equity/equity_model_types.py
+-rw-rw-rw-   0        0        0    19683 2021-12-25 18:48:58.000000 financepy-0.300/financepy/products/equity/equity_one_touch_option.py
+-rw-rw-rw-   0        0        0     6735 2021-12-23 15:44:42.000000 financepy-0.300/financepy/products/equity/equity_option.py
+-rw-rw-rw-   0        0        0    12100 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/equity/equity_rainbow_option.py
+-rw-rw-rw-   0        0        0     8584 2023-04-21 18:30:04.000000 financepy-0.300/financepy/products/equity/equity_swap.py
+-rw-rw-rw-   0        0        0    14016 2023-04-21 18:38:13.000000 financepy-0.300/financepy/products/equity/equity_swap_leg.py
+-rw-rw-rw-   0        0        0    24907 2023-02-13 16:33:55.000000 financepy-0.300/financepy/products/equity/equity_vanilla_option.py
+-rw-rw-rw-   0        0        0    10614 2021-12-22 21:00:14.000000 financepy-0.300/financepy/products/equity/equity_variance_swap.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.655221 financepy-0.300/financepy/products/fx/
+-rw-rw-rw-   0        0        0      375 2021-12-25 19:13:13.000000 financepy-0.300/financepy/products/fx/__init__.py
+-rw-rw-rw-   0        0        0    17295 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_barrier_option.py
+-rw-rw-rw-   0        0        0     6174 2021-12-21 13:58:02.000000 financepy-0.300/financepy/products/fx/fx_digital_option.py
+-rw-rw-rw-   0        0        0     9113 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_fixed_lookback_option.py
+-rw-rw-rw-   0        0        0     7583 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_float_lookback_option.py
+-rw-rw-rw-   0        0        0     7198 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_forward.py
+-rw-rw-rw-   0        0        0     4868 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/fx/fx_mkt_conventions.py
+-rw-rw-rw-   0        0        0    19515 2021-12-23 15:49:15.000000 financepy-0.300/financepy/products/fx/fx_one_touch_option.py
+-rw-rw-rw-   0        0        0     5292 2021-12-23 15:43:21.000000 financepy-0.300/financepy/products/fx/fx_option.py
+-rw-rw-rw-   0        0        0    11013 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_rainbow_option.py
+-rw-rw-rw-   0        0        0    28014 2023-05-10 16:06:39.000000 financepy-0.300/financepy/products/fx/fx_vanilla_option.py
+-rw-rw-rw-   0        0        0    10072 2021-12-03 18:08:34.000000 financepy-0.300/financepy/products/fx/fx_variance_swap.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.667191 financepy-0.300/financepy/products/inflation/
+-rw-rw-rw-   0        0        0     6773 2023-02-24 13:55:17.000000 financepy-0.300/financepy/products/inflation/FinInflationBond.py
+-rw-rw-rw-   0        0        0     4361 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/inflation/FinInflationIndexCurve.py
+-rw-rw-rw-   0        0        0     6672 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/inflation/FinInflationSwap.py
+-rw-rw-rw-   0        0        0    21176 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/inflation/FinInflationSwapCurve.py
+-rw-rw-rw-   0        0        0       33 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/inflation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.713065 financepy-0.300/financepy/products/rates/
+-rw-rw-rw-   0        0        0      435 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/__init__.py
+-rw-rw-rw-   0        0        0     9390 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/bermudan_swaption.py
+-rw-rw-rw-   0        0        0    11427 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/callable_swap.py
+-rw-rw-rw-   0        0        0    22970 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/dual_curve.py
+-rw-rw-rw-   0        0        0     7979 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_basis_swap.py
+-rw-rw-rw-   0        0        0    15095 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_cap_floor.py
+-rw-rw-rw-   0        0        0     1246 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_conventions.py
+-rw-rw-rw-   0        0        0     6722 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_deposit.py
+-rw-rw-rw-   0        0        0     7139 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_fra.py
+-rw-rw-rw-   0        0        0     5822 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_future.py
+-rw-rw-rw-   0        0        0    17758 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/ibor_lmm_products.py
+-rw-rw-rw-   0        0        0    27170 2022-08-31 19:10:11.000000 financepy-0.300/financepy/products/rates/ibor_single_curve.py
+-rw-rw-rw-   0        0        0    11620 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/ibor_swap.py
+-rw-rw-rw-   0        0        0    17602 2021-10-05 08:15:43.000000 financepy-0.300/financepy/products/rates/ibor_swaption.py
+-rw-rw-rw-   0        0        0    10266 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/ois.py
+-rw-rw-rw-   0        0        0     7437 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/ois_basis_swap.py
+-rw-rw-rw-   0        0        0    24892 2021-11-06 12:48:44.000000 financepy-0.300/financepy/products/rates/ois_curve.py
+-rw-rw-rw-   0        0        0    11327 2023-04-14 12:22:10.000000 financepy-0.300/financepy/products/rates/swap_fixed_leg.py
+-rw-rw-rw-   0        0        0    12625 2023-03-12 15:30:43.000000 financepy-0.300/financepy/products/rates/swap_float_leg.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.763930 financepy-0.300/financepy/utils/
+-rw-rw-rw-   0        0        0      371 2021-10-05 08:15:43.000000 financepy-0.300/financepy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1553 2021-10-05 08:15:43.000000 financepy-0.300/financepy/utils/amount.py
+-rw-rw-rw-   0        0        0    33935 2022-03-20 08:54:30.000000 financepy-0.300/financepy/utils/calendar.py
+-rw-rw-rw-   0        0        0      630 2021-11-06 12:48:44.000000 financepy-0.300/financepy/utils/currency.py
+-rw-rw-rw-   0        0        0    32484 2023-02-13 16:33:55.000000 financepy-0.300/financepy/utils/date.py
+-rw-rw-rw-   0        0        0    10541 2022-10-02 12:44:23.000000 financepy-0.300/financepy/utils/day_count.py
+-rw-rw-rw-   0        0        0      888 2021-11-06 12:48:44.000000 financepy-0.300/financepy/utils/distribution.py
+-rw-rw-rw-   0        0        0     1956 2021-11-06 12:48:44.000000 financepy-0.300/financepy/utils/error.py
+-rw-rw-rw-   0        0        0     1601 2022-10-02 12:44:23.000000 financepy-0.300/financepy/utils/frequency.py
+-rw-rw-rw-   0        0        0     2972 2023-03-12 15:57:49.000000 financepy-0.300/financepy/utils/global_types.py
+-rw-rw-rw-   0        0        0      447 2021-11-06 12:48:44.000000 financepy-0.300/financepy/utils/global_vars.py
+-rw-rw-rw-   0        0        0    15898 2023-03-12 15:30:43.000000 financepy-0.300/financepy/utils/helpers.py
+-rw-rw-rw-   0        0        0     2927 2022-03-20 08:29:25.000000 financepy-0.300/financepy/utils/latex.py
+-rw-rw-rw-   0        0        0    20984 2023-04-14 12:22:10.000000 financepy-0.300/financepy/utils/math.py
+-rw-rw-rw-   0        0        0     2301 2022-12-28 10:41:39.000000 financepy-0.300/financepy/utils/polyfit.py
+-rw-rw-rw-   0        0        0    11970 2023-05-04 07:59:23.000000 financepy-0.300/financepy/utils/schedule.py
+-rw-rw-rw-   0        0        0      498 2021-11-06 12:48:44.000000 financepy-0.300/financepy/utils/singleton.py
+-rw-rw-rw-   0        0        0    29377 2022-11-22 11:57:17.000000 financepy-0.300/financepy/utils/solver_1d.py
+-rw-rw-rw-   0        0        0    21755 2023-04-21 18:36:04.000000 financepy-0.300/financepy/utils/solver_cg.py
+-rw-rw-rw-   0        0        0    13278 2023-04-21 18:38:22.000000 financepy-0.300/financepy/utils/solver_nm.py
+-rw-rw-rw-   0        0        0     2754 2022-06-24 08:40:16.000000 financepy-0.300/financepy/utils/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:23.379955 financepy-0.300/financepy.egg-info/
+-rw-rw-rw-   0        0        0     7284 2023-05-29 09:50:22.000000 financepy-0.300/financepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10686 2023-05-29 09:50:23.000000 financepy-0.300/financepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 09:50:22.000000 financepy-0.300/financepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-29 09:50:22.000000 financepy-0.300/financepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-29 09:50:22.000000 financepy-0.300/financepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 09:50:24.038200 financepy-0.300/setup.cfg
+-rw-rw-rw-   0        0        0     2058 2023-05-22 12:03:50.000000 financepy-0.300/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:50:24.035205 financepy-0.300/tests_golden/
+-rw-rw-rw-   0        0        0    17690 2022-12-28 17:24:50.000000 financepy-0.300/tests_golden/FinTestCases.py
+-rw-rw-rw-   0        0        0      890 2023-03-13 18:31:42.000000 financepy-0.300/tests_golden/TestFinAmount.py
+-rw-rw-rw-   0        0        0    22862 2023-05-10 16:07:46.000000 financepy-0.300/tests_golden/TestFinBond.py
+-rw-rw-rw-   0        0        0     7598 2022-03-20 13:10:36.000000 financepy-0.300/tests_golden/TestFinBondAnnuity.py
+-rw-rw-rw-   0        0        0     4588 2022-06-24 08:59:58.000000 financepy-0.300/tests_golden/TestFinBondConvertible.py
+-rw-rw-rw-   0        0        0     6956 2022-06-24 09:00:24.000000 financepy-0.300/tests_golden/TestFinBondEmbeddedOptionBK.py
+-rw-rw-rw-   0        0        0     6942 2022-06-24 09:01:06.000000 financepy-0.300/tests_golden/TestFinBondEmbeddedOptionHW.py
+-rw-rw-rw-   0        0        0    14054 2022-03-20 12:33:53.000000 financepy-0.300/tests_golden/TestFinBondFRN.py
+-rw-rw-rw-   0        0        0     6176 2022-03-20 08:53:51.000000 financepy-0.300/tests_golden/TestFinBondFutures.py
+-rw-rw-rw-   0        0        0     2041 2021-12-21 13:16:15.000000 financepy-0.300/tests_golden/TestFinBondMortgage.py
+-rw-rw-rw-   0        0        0    15002 2022-06-24 09:01:30.000000 financepy-0.300/tests_golden/TestFinBondOptionBDTModel.py
+-rw-rw-rw-   0        0        0    14962 2022-06-24 09:03:01.000000 financepy-0.300/tests_golden/TestFinBondOptionBKModel.py
+-rw-rw-rw-   0        0        0    18901 2022-06-24 09:04:04.000000 financepy-0.300/tests_golden/TestFinBondOptionHWModel.py
+-rw-rw-rw-   0        0        0     2152 2022-10-02 12:44:23.000000 financepy-0.300/tests_golden/TestFinBondPortfolio.py
+-rw-rw-rw-   0        0        0     4514 2022-06-10 21:00:21.000000 financepy-0.300/tests_golden/TestFinBondYieldCurve.py
+-rw-rw-rw-   0        0        0     2924 2022-11-22 09:47:45.000000 financepy-0.300/tests_golden/TestFinBondZeroCoupon.py
+-rw-rw-rw-   0        0        0     2472 2022-08-11 21:00:13.000000 financepy-0.300/tests_golden/TestFinBondZeroCurve.py
+-rw-rw-rw-   0        0        0    23600 2022-01-22 13:18:12.000000 financepy-0.300/tests_golden/TestFinCDS.py
+-rw-rw-rw-   0        0        0    13736 2022-06-24 09:26:11.000000 financepy-0.300/tests_golden/TestFinCDSBasket.py
+-rw-rw-rw-   0        0        0     5636 2022-08-31 20:01:33.000000 financepy-0.300/tests_golden/TestFinCDSCurve.py
+-rw-rw-rw-   0        0        0     5374 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinCDSIndex.py
+-rw-rw-rw-   0        0        0    11357 2022-06-24 09:05:07.000000 financepy-0.300/tests_golden/TestFinCDSIndexAdjustHazards.py
+-rw-rw-rw-   0        0        0    10646 2022-06-24 09:05:28.000000 financepy-0.300/tests_golden/TestFinCDSIndexAdjustSpreads.py
+-rw-rw-rw-   0        0        0     8588 2022-06-24 09:12:38.000000 financepy-0.300/tests_golden/TestFinCDSIndexOption.py
+-rw-rw-rw-   0        0        0     8138 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinCDSIndexPortfolio.py
+-rw-rw-rw-   0        0        0    10741 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinCDSOption.py
+-rw-rw-rw-   0        0        0    10942 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinCDSTranche.py
+-rw-rw-rw-   0        0        0     1720 2022-03-20 08:54:04.000000 financepy-0.300/tests_golden/TestFinCalendar.py
+-rw-rw-rw-   0        0        0     8660 2022-02-14 09:19:14.000000 financepy-0.300/tests_golden/TestFinDate.py
+-rw-rw-rw-   0        0        0     3513 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDateAdjust.py
+-rw-rw-rw-   0        0        0     1335 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDayCount.py
+-rw-rw-rw-   0        0        0     3504 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurve.py
+-rw-rw-rw-   0        0        0     1857 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurveFlat.py
+-rw-rw-rw-   0        0        0     7352 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurveNS.py
+-rw-rw-rw-   0        0        0     4340 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurveNSS.py
+-rw-rw-rw-   0        0        0     1499 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurvePolynomial.py
+-rw-rw-rw-   0        0        0     2873 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurveZeros.py
+-rw-rw-rw-   0        0        0     6743 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/TestFinDiscountCurves.py
+-rw-rw-rw-   0        0        0    11033 2022-12-28 17:23:07.000000 financepy-0.300/tests_golden/TestFinEquityAmericanMC.py
+-rw-rw-rw-   0        0        0     7143 2022-12-25 20:34:58.000000 financepy-0.300/tests_golden/TestFinEquityAmericanOption.py
+-rw-rw-rw-   0        0        0    14048 2022-01-22 09:41:29.000000 financepy-0.300/tests_golden/TestFinEquityAsianOption.py
+-rw-rw-rw-   0        0        0     6523 2023-05-22 12:02:11.000000 financepy-0.300/tests_golden/TestFinEquityBarrierOption.py
+-rw-rw-rw-   0        0        0     7653 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinEquityBasketOption.py
+-rw-rw-rw-   0        0        0     6414 2022-06-24 09:08:30.000000 financepy-0.300/tests_golden/TestFinEquityBinomialTree.py
+-rw-rw-rw-   0        0        0     5534 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinEquityChooserOption.py
+-rw-rw-rw-   0        0        0     1996 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinEquityCliquetOption.py
+-rw-rw-rw-   0        0        0     5917 2022-06-24 09:08:45.000000 financepy-0.300/tests_golden/TestFinEquityCompoundOption.py
+-rw-rw-rw-   0        0        0     5086 2022-06-24 09:16:47.000000 financepy-0.300/tests_golden/TestFinEquityDigitalOption.py
+-rw-rw-rw-   0        0        0     2134 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinEquityForward.py
+-rw-rw-rw-   0        0        0    16388 2022-01-22 09:40:51.000000 financepy-0.300/tests_golden/TestFinEquityLookbackOption.py
+-rw-rw-rw-   0        0        0     6191 2022-01-22 09:44:19.000000 financepy-0.300/tests_golden/TestFinEquityOneTouchOption.py
+-rw-rw-rw-   0        0        0    17897 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinEquityRainbowOption.py
+-rw-rw-rw-   0        0        0     7872 2023-04-14 13:24:43.000000 financepy-0.300/tests_golden/TestFinEquitySwap.py
+-rw-rw-rw-   0        0        0    10841 2023-03-13 18:31:42.000000 financepy-0.300/tests_golden/TestFinEquityVanillaOption.py
+-rw-rw-rw-   0        0        0     2341 2021-12-22 21:02:43.000000 financepy-0.300/tests_golden/TestFinEquityVarianceSwap.py
+-rw-rw-rw-   0        0        0     4021 2021-12-22 21:03:03.000000 financepy-0.300/tests_golden/TestFinEquityVolSurface.py
+-rw-rw-rw-   0        0        0     4803 2022-06-24 09:10:42.000000 financepy-0.300/tests_golden/TestFinFXAmericanOption.py
+-rw-rw-rw-   0        0        0     6480 2022-06-24 09:10:55.000000 financepy-0.300/tests_golden/TestFinFXBarrierOption.py
+-rw-rw-rw-   0        0        0     2644 2021-12-21 13:53:03.000000 financepy-0.300/tests_golden/TestFinFXDigitalOption.py
+-rw-rw-rw-   0        0        0     3170 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinFXForward.py
+-rw-rw-rw-   0        0        0    15254 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinFXLookbackOption.py
+-rw-rw-rw-   0        0        0     6018 2021-12-25 19:11:30.000000 financepy-0.300/tests_golden/TestFinFXOneTouchOption.py
+-rw-rw-rw-   0        0        0     5147 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinFXOptionSABR.py
+-rw-rw-rw-   0        0        0    17551 2023-05-10 16:04:00.000000 financepy-0.300/tests_golden/TestFinFXVanillaOption.py
+-rw-rw-rw-   0        0        0     9858 2021-12-22 21:05:30.000000 financepy-0.300/tests_golden/TestFinFXVolSurface.py
+-rw-rw-rw-   0        0        0    18123 2021-12-22 19:19:05.000000 financepy-0.300/tests_golden/TestFinFXVolSurfacePlus.py
+-rw-rw-rw-   0        0        0    28257 2021-12-22 19:15:39.000000 financepy-0.300/tests_golden/TestFinIborBermudanSwaption.py
+-rw-rw-rw-   0        0        0    14266 2021-12-22 19:16:48.000000 financepy-0.300/tests_golden/TestFinIborCapFloor.py
+-rw-rw-rw-   0        0        0     1921 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinIborCapVolCurve.py
+-rw-rw-rw-   0        0        0    25121 2022-06-24 11:50:45.000000 financepy-0.300/tests_golden/TestFinIborDualCurve.py
+-rw-rw-rw-   0        0        0     1044 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinIborFuture.py
+-rw-rw-rw-   0        0        0     9516 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinIborLMMProducts.py
+-rw-rw-rw-   0        0        0    27549 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinIborSingleCurve.py
+-rw-rw-rw-   0        0        0    14159 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinIborSwap.py
+-rw-rw-rw-   0        0        0    27393 2022-03-20 08:53:09.000000 financepy-0.300/tests_golden/TestFinIborSwaption.py
+-rw-rw-rw-   0        0        0    14923 2022-03-20 08:57:37.000000 financepy-0.300/tests_golden/TestFinInflationBond.py
+-rw-rw-rw-   0        0        0     1424 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinInflationIndexCurve.py
+-rw-rw-rw-   0        0        0     2269 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinInterpolate.py
+-rw-rw-rw-   0        0        0     2209 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinInterpolatedForwards.py
+-rw-rw-rw-   0        0        0     4299 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinLossDbnBuilder.py
+-rw-rw-rw-   0        0        0     2850 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinMath.py
+-rw-rw-rw-   0        0        0     1910 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinMathAccruedInterp.py
+-rw-rw-rw-   0        0        0     3679 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelBlack.py
+-rw-rw-rw-   0        0        0     4958 2021-12-22 20:18:30.000000 financepy-0.300/tests_golden/TestFinModelBlackScholes.py
+-rw-rw-rw-   0        0        0     2586 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelBlack_SABR_HW.py
+-rw-rw-rw-   0        0        0     2455 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelCIR.py
+-rw-rw-rw-   0        0        0     6657 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelHeston.py
+-rw-rw-rw-   0        0        0     3595 2022-01-22 13:54:49.000000 financepy-0.300/tests_golden/TestFinModelMerton.py
+-rw-rw-rw-   0        0        0    10334 2022-03-20 13:11:37.000000 financepy-0.300/tests_golden/TestFinModelRatesBDT.py
+-rw-rw-rw-   0        0        0     5310 2022-03-20 13:06:22.000000 financepy-0.300/tests_golden/TestFinModelRatesBK.py
+-rw-rw-rw-   0        0        0    11763 2022-03-20 13:11:16.000000 financepy-0.300/tests_golden/TestFinModelRatesHW.py
+-rw-rw-rw-   0        0        0    17835 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelRatesLMM.py
+-rw-rw-rw-   0        0        0     3182 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelSABR.py
+-rw-rw-rw-   0        0        0     2689 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinModelShiftedSABR.py
+-rw-rw-rw-   0        0        0    12233 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinNumbaNumpySpeed.py
+-rw-rw-rw-   0        0        0     2302 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinOIS.py
+-rw-rw-rw-   0        0        0    19529 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinOISCurve.py
+-rw-rw-rw-   0        0        0     3818 2021-12-22 20:46:18.000000 financepy-0.300/tests_golden/TestFinOptionImpliedDbn.py
+-rw-rw-rw-   0        0        0     1018 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinPieceCurve.py
+-rw-rw-rw-   0        0        0     6178 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinProcessSimulator.py
+-rw-rw-rw-   0        0        0    18118 2023-05-03 16:37:45.000000 financepy-0.300/tests_golden/TestFinSchedule.py
+-rw-rw-rw-   0        0        0     1669 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinSobol.py
+-rw-rw-rw-   0        0        0     2442 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinStatistics.py
+-rw-rw-rw-   0        0        0     8851 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinSwapLegs.py
+-rw-rw-rw-   0        0        0     4678 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinSwaptionVolSurface.py
+-rw-rw-rw-   0        0        0     1341 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinVasicekRateModel.py
+-rw-rw-rw-   0        0        0     1358 2021-12-03 18:08:34.000000 financepy-0.300/tests_golden/TestFinVolatilityCurve.py
+-rw-rw-rw-   0        0        0       56 2021-10-05 08:15:44.000000 financepy-0.300/tests_golden/__init__.py
+-rw-rw-rw-   0        0        0     2443 2023-03-13 10:28:21.000000 financepy-0.300/tests_golden/runAllTests.py
```

### Comparing `financepy-0.290/LICENSE` & `financepy-0.300/LICENSE`

 * *Files identical despite different names*

### Comparing `financepy-0.290/PKG-INFO` & `financepy-0.300/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financepy
-Version: 0.290
+Version: 0.300
 Summary: A Finance Securities Valuation Library
 Home-page: https://github.com/domokane/FinancePy
 Author: Dominic O'Kane
 Author-email: dominic.okane@edhec.edu
 Keywords: FINANCE,OPTIONS,BONDS,VALUATION,DERIVATIVES
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `financepy-0.290/README.md` & `financepy-0.300/README.md`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve.py` & `financepy-0.300/financepy/market/curves/discount_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_flat.py` & `financepy-0.300/financepy/market/curves/discount_curve_flat.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_ns.py` & `financepy-0.300/financepy/market/curves/discount_curve_ns.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_nss.py` & `financepy-0.300/financepy/market/curves/discount_curve_nss.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_poly.py` & `financepy-0.300/financepy/market/curves/discount_curve_poly.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_pwf.py` & `financepy-0.300/financepy/market/curves/discount_curve_pwf.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_pwl.py` & `financepy-0.300/financepy/market/curves/discount_curve_pwl.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/discount_curve_zeros.py` & `financepy-0.300/financepy/market/curves/discount_curve_zeros.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/curves/interpolator.py` & `financepy-0.300/financepy/market/curves/interpolator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/equity_vol_curve.py` & `financepy-0.300/financepy/market/volatility/equity_vol_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/equity_vol_surface.py` & `financepy-0.300/financepy/market/volatility/equity_vol_surface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/fx_vol_surface.py` & `financepy-0.300/financepy/market/volatility/fx_vol_surface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/fx_vol_surface_plus.py` & `financepy-0.300/financepy/market/volatility/fx_vol_surface_plus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve.py` & `financepy-0.300/financepy/market/volatility/ibor_cap_vol_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve_fn.py` & `financepy-0.300/financepy/market/volatility/ibor_cap_vol_curve_fn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/market/volatility/swaption_vol_surface.py` & `financepy-0.300/financepy/market/volatility/swaption_vol_surface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/__init__.py` & `financepy-0.300/financepy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/bachelier.py` & `financepy-0.300/financepy/models/bachelier.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/bdt_tree.py` & `financepy-0.300/financepy/models/bdt_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/bk_tree.py` & `financepy-0.300/financepy/models/bk_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black.py` & `financepy-0.300/financepy/models/black.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black_scholes.py` & `financepy-0.300/financepy/models/black_scholes.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black_scholes_analytic.py` & `financepy-0.300/financepy/models/black_scholes_analytic.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black_scholes_mc.py` & `financepy-0.300/financepy/models/black_scholes_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black_scholes_mc_tests.py` & `financepy-0.300/financepy/models/black_scholes_mc_tests.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/black_shifted.py` & `financepy-0.300/financepy/models/black_shifted.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/cir_mc.py` & `financepy-0.300/financepy/models/cir_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/equity_barrier_models.py` & `financepy-0.300/financepy/models/equity_barrier_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 ##############################################################################
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
 ##############################################################################
 
 import numpy as np
 
 from ..market.curves.discount_curve import DiscountCurve
-from ..utils.date import Date
 from ..utils.error import FinError
 from ..utils.global_types import EquityBarrierTypes
-from ..utils.global_vars import gDaysInYear
 from ..utils.math import N
 
 
 # Calculates the Barrier option price using an Analytical Approach
 # and the Black Scholes Model
-def value_bs(expiry_date: Date,
+def value_bs(time_to_expiry: float,  # time in years
               strike_price: float,
               option_type: int,
               barrier_level: float,
               num_observations,  # number of observations per year
               notional: float,
-              valuation_date: Date,
               stock_price: (float, np.ndarray),
               rf_rate: float,
               div_rate: float,
               model):
     """ This values a single option. Because of its structure it cannot
     easily be vectorised which is why it has been wrapped. """
-
-    t_exp = (expiry_date - valuation_date) / gDaysInYear
-
-    if t_exp < 0:
-        raise FinError("Option expires before value date.")
-
-    t_exp = max(t_exp, 1e-6)
+    t_exp = max(time_to_expiry, 1e-6)
 
     lnS0k = np.log(stock_price / strike_price)
     sqrtT = np.sqrt(t_exp)
 
     r = rf_rate
     q = div_rate
```

### Comparing `financepy-0.290/financepy/models/equity_crr_tree.py` & `financepy-0.300/financepy/models/equity_crr_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/equity_lsmc.py` & `financepy-0.300/financepy/models/equity_lsmc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/finite_difference.py` & `financepy-0.300/financepy/models/finite_difference.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/finite_difference_PSOR.py` & `financepy-0.300/financepy/models/finite_difference_PSOR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/gauss_copula.py` & `financepy-0.300/financepy/models/gauss_copula.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/gauss_copula_lhp.py` & `financepy-0.300/financepy/models/gauss_copula_lhp.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/gauss_copula_lhplus.py` & `financepy-0.300/financepy/models/gauss_copula_lhplus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/gauss_copula_onefactor.py` & `financepy-0.300/financepy/models/gauss_copula_onefactor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/gbm_process_simulator.py` & `financepy-0.300/financepy/models/gbm_process_simulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/heston.py` & `financepy-0.300/financepy/models/heston.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/hw_tree.py` & `financepy-0.300/financepy/models/hw_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/lmm_mc.py` & `financepy-0.300/financepy/models/lmm_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/loss_dbn_builder.py` & `financepy-0.300/financepy/models/loss_dbn_builder.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/merton_firm.py` & `financepy-0.300/financepy/models/merton_firm.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/merton_firm_mkt.py` & `financepy-0.300/financepy/models/merton_firm_mkt.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/option_implied_dbn.py` & `financepy-0.300/financepy/models/option_implied_dbn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/process_simulator.py` & `financepy-0.300/financepy/models/process_simulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/rates_ho_lee.py` & `financepy-0.300/financepy/models/rates_ho_lee.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/sabr.py` & `financepy-0.300/financepy/models/sabr.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/sabr_shifted.py` & `financepy-0.300/financepy/models/sabr_shifted.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/sobol.py` & `financepy-0.300/financepy/models/sobol.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/sobolcoeff.npz` & `financepy-0.300/financepy/models/sobolcoeff.npz`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/student_t_copula.py` & `financepy-0.300/financepy/models/student_t_copula.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/vasicek_mc.py` & `financepy-0.300/financepy/models/vasicek_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/models/volatility_fns.py` & `financepy-0.300/financepy/models/volatility_fns.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond.py` & `financepy-0.300/financepy/products/bonds/bond.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_annuity.py` & `financepy-0.300/financepy/products/bonds/bond_annuity.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_callable.py` & `financepy-0.300/financepy/products/bonds/bond_callable.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_convertible.py` & `financepy-0.300/financepy/products/bonds/bond_convertible.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_frn.py` & `financepy-0.300/financepy/products/bonds/bond_frn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_future.py` & `financepy-0.300/financepy/products/bonds/bond_future.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_market.py` & `financepy-0.300/financepy/products/bonds/bond_market.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_mortgage.py` & `financepy-0.300/financepy/products/bonds/bond_mortgage.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_option.py` & `financepy-0.300/financepy/products/bonds/bond_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_portfolio.py` & `financepy-0.300/financepy/products/bonds/bond_portfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/bond_zero.py` & `financepy-0.300/financepy/products/bonds/bond_zero.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/yield_curve.py` & `financepy-0.300/financepy/products/bonds/yield_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/yield_curve_model.py` & `financepy-0.300/financepy/products/bonds/yield_curve_model.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/bonds/zero_curve.py` & `financepy-0.300/financepy/products/bonds/zero_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds.py` & `financepy-0.300/financepy/products/credit/cds.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_basket.py` & `financepy-0.300/financepy/products/credit/cds_basket.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_curve.py` & `financepy-0.300/financepy/products/credit/cds_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_index_option.py` & `financepy-0.300/financepy/products/credit/cds_index_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_index_portfolio.py` & `financepy-0.300/financepy/products/credit/cds_index_portfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_option.py` & `financepy-0.300/financepy/products/credit/cds_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/credit/cds_tranche.py` & `financepy-0.300/financepy/products/credit/cds_tranche.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/__init__.py` & `financepy-0.300/financepy/products/equity/__init__.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_american_option.py` & `financepy-0.300/financepy/products/equity/equity_american_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_asian_option.py` & `financepy-0.300/financepy/products/equity/equity_asian_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_barrier_option.py` & `financepy-0.300/financepy/products/equity/equity_barrier_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,57 +85,59 @@
         if isinstance(stock_price, float):
             stock_prices = [stock_price]
         else:
             stock_prices = stock_price
 
         values = []
 
+        t_exp = (self._expiry_date - valuation_date) / gDaysInYear
+
+        if t_exp < 0:
+            raise FinError("Option expires before value date.")
+
         for stock_price in stock_prices:
 
-            v = value_bs(self._expiry_date, 
+            v = value_bs(t_exp,
                           self._strike_price, 
                           self._option_type.value, 
                           self._barrier_level,
                           self._num_observations_per_year, 
-                          self._notional, 
-                          valuation_date, 
+                          self._notional,
                           stock_price,
                           discount_curve.cc_rate(self._expiry_date),
                           dividend_curve.cc_rate(self._expiry_date), model)
 
             values.append(v)
 
         if isinstance(stock_price, float):
             return values[0]
         else:
             return np.array(values)
 
 ###############################################################################
 
     def value_mc(self, 
-                 expiry_date: Date,
+                 time_to_expiry: float,
                  strike_price,
                  option_type: int,
                  barrier_level,
                  notional,
-                 valuation_date: Date,
                  stock_price: float,
                  rf_rate: float,
                  process_type,
                  model_params,
                  numAnnObs: int = 252,
                  num_paths: int = 10000,
                  seed: int = 4242):
         """ A Monte-Carlo based valuation of the barrier option which simulates
         the evolution of the stock price of at a specified number of annual
         observation times until expiry to examine if the barrier has been
         crossed and the corresponding value of the final payoff, if any. It
         assumes a GBM model for the stock price. """
-    
-        texp = (expiry_date - valuation_date) / gDaysInYear
+        texp = max(time_to_expiry, 1e-6)
         num_time_steps = int(texp * numAnnObs)
         K = strike_price
         B = barrier_level
         option_type = option_type
     
         process = FinProcessSimulator()
```

### Comparing `financepy-0.290/financepy/products/equity/equity_basket_option.py` & `financepy-0.300/financepy/products/equity/equity_basket_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_binomial_tree.py` & `financepy-0.300/financepy/products/equity/equity_binomial_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_chooser_option.py` & `financepy-0.300/financepy/products/equity/equity_chooser_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_cliquet_option.py` & `financepy-0.300/financepy/products/equity/equity_cliquet_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_compound_option.py` & `financepy-0.300/financepy/products/equity/equity_compound_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_digital_option.py` & `financepy-0.300/financepy/products/equity/equity_digital_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_fixed_lookback_option.py` & `financepy-0.300/financepy/products/equity/equity_fixed_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_float_lookback_option.py` & `financepy-0.300/financepy/products/equity/equity_float_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_forward.py` & `financepy-0.300/financepy/products/equity/equity_forward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_index_option.py` & `financepy-0.300/financepy/products/equity/equity_index_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_model_types.py` & `financepy-0.300/financepy/products/equity/equity_model_types.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_one_touch_option.py` & `financepy-0.300/financepy/products/equity/equity_one_touch_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_option.py` & `financepy-0.300/financepy/products/equity/equity_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_rainbow_option.py` & `financepy-0.300/financepy/products/equity/equity_rainbow_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_swap.py` & `financepy-0.300/financepy/products/equity/equity_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_swap_leg.py` & `financepy-0.300/financepy/products/equity/equity_swap_leg.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_vanilla_option.py` & `financepy-0.300/financepy/products/equity/equity_vanilla_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/equity/equity_variance_swap.py` & `financepy-0.300/financepy/products/equity/equity_variance_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_barrier_option.py` & `financepy-0.300/financepy/products/fx/fx_barrier_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_digital_option.py` & `financepy-0.300/financepy/products/fx/fx_digital_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_fixed_lookback_option.py` & `financepy-0.300/financepy/products/fx/fx_fixed_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_float_lookback_option.py` & `financepy-0.300/financepy/products/fx/fx_float_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_forward.py` & `financepy-0.300/financepy/products/fx/fx_forward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_mkt_conventions.py` & `financepy-0.300/financepy/products/fx/fx_mkt_conventions.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_one_touch_option.py` & `financepy-0.300/financepy/products/fx/fx_one_touch_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_option.py` & `financepy-0.300/financepy/products/fx/fx_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_rainbow_option.py` & `financepy-0.300/financepy/products/fx/fx_rainbow_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_vanilla_option.py` & `financepy-0.300/financepy/products/fx/fx_vanilla_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/fx/fx_variance_swap.py` & `financepy-0.300/financepy/products/fx/fx_variance_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/inflation/FinInflationBond.py` & `financepy-0.300/financepy/products/inflation/FinInflationBond.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/inflation/FinInflationIndexCurve.py` & `financepy-0.300/financepy/products/inflation/FinInflationIndexCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/inflation/FinInflationSwap.py` & `financepy-0.300/financepy/products/inflation/FinInflationSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/inflation/FinInflationSwapCurve.py` & `financepy-0.300/financepy/products/inflation/FinInflationSwapCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/bermudan_swaption.py` & `financepy-0.300/financepy/products/rates/bermudan_swaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/callable_swap.py` & `financepy-0.300/financepy/products/rates/callable_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/dual_curve.py` & `financepy-0.300/financepy/products/rates/dual_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_basis_swap.py` & `financepy-0.300/financepy/products/rates/ibor_basis_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_cap_floor.py` & `financepy-0.300/financepy/products/rates/ibor_cap_floor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_conventions.py` & `financepy-0.300/financepy/products/rates/ibor_conventions.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_deposit.py` & `financepy-0.300/financepy/products/rates/ibor_deposit.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_fra.py` & `financepy-0.300/financepy/products/rates/ibor_fra.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_future.py` & `financepy-0.300/financepy/products/rates/ibor_future.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_lmm_products.py` & `financepy-0.300/financepy/products/rates/ibor_lmm_products.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_single_curve.py` & `financepy-0.300/financepy/products/rates/ibor_single_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_swap.py` & `financepy-0.300/financepy/products/rates/ibor_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ibor_swaption.py` & `financepy-0.300/financepy/products/rates/ibor_swaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ois.py` & `financepy-0.300/financepy/products/rates/ois.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ois_basis_swap.py` & `financepy-0.300/financepy/products/rates/ois_basis_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/ois_curve.py` & `financepy-0.300/financepy/products/rates/ois_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/swap_fixed_leg.py` & `financepy-0.300/financepy/products/rates/swap_fixed_leg.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/products/rates/swap_float_leg.py` & `financepy-0.300/financepy/products/rates/swap_float_leg.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/amount.py` & `financepy-0.300/financepy/utils/amount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/calendar.py` & `financepy-0.300/financepy/utils/calendar.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/currency.py` & `financepy-0.300/financepy/utils/currency.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/date.py` & `financepy-0.300/financepy/utils/date.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/day_count.py` & `financepy-0.300/financepy/utils/day_count.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/distribution.py` & `financepy-0.300/financepy/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/error.py` & `financepy-0.300/financepy/utils/error.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/frequency.py` & `financepy-0.300/financepy/utils/frequency.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/global_types.py` & `financepy-0.300/financepy/utils/global_types.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/helpers.py` & `financepy-0.300/financepy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/latex.py` & `financepy-0.300/financepy/utils/latex.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/math.py` & `financepy-0.300/financepy/utils/math.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/polyfit.py` & `financepy-0.300/financepy/utils/polyfit.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/schedule.py` & `financepy-0.300/financepy/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/solver_1d.py` & `financepy-0.300/financepy/utils/solver_1d.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/solver_cg.py` & `financepy-0.300/financepy/utils/solver_cg.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/solver_nm.py` & `financepy-0.300/financepy/utils/solver_nm.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy/utils/stats.py` & `financepy-0.300/financepy/utils/stats.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/financepy.egg-info/PKG-INFO` & `financepy-0.300/financepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financepy
-Version: 0.290
+Version: 0.300
 Summary: A Finance Securities Valuation Library
 Home-page: https://github.com/domokane/FinancePy
 Author: Dominic O'Kane
 Author-email: dominic.okane@edhec.edu
 Keywords: FINANCE,OPTIONS,BONDS,VALUATION,DERIVATIVES
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `financepy-0.290/financepy.egg-info/SOURCES.txt` & `financepy-0.300/financepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `financepy-0.290/setup.py` & `financepy-0.300/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     author="Dominic O'Kane",
     author_email="dominic.okane@edhec.edu",
     description="A Finance Securities Valuation Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/domokane/FinancePy",
     keywords=['FINANCE', 'OPTIONS', 'BONDS', 'VALUATION', 'DERIVATIVES'],
-    install_requires=['numpy', 'numba', 'scipy'],
+    install_requires=['numpy', 'numba', 'scipy', 'llvmlite', 'ipython', 'matplotlib', 'pandas', 'prettytable'],
     package_data={'': ['*.npz'], },
     include_package_date=True,
     packages=setuptools.find_packages(),
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `financepy-0.290/tests_golden/FinTestCases.py` & `financepy-0.300/tests_golden/FinTestCases.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinAmount.py` & `financepy-0.300/tests_golden/TestFinAmount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBond.py` & `financepy-0.300/tests_golden/TestFinBond.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondAnnuity.py` & `financepy-0.300/tests_golden/TestFinBondAnnuity.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondConvertible.py` & `financepy-0.300/tests_golden/TestFinBondConvertible.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondEmbeddedOptionBK.py` & `financepy-0.300/tests_golden/TestFinBondEmbeddedOptionBK.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondEmbeddedOptionHW.py` & `financepy-0.300/tests_golden/TestFinBondEmbeddedOptionHW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondFRN.py` & `financepy-0.300/tests_golden/TestFinBondFRN.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondFutures.py` & `financepy-0.300/tests_golden/TestFinBondFutures.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondMortgage.py` & `financepy-0.300/tests_golden/TestFinBondMortgage.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondOptionBDTModel.py` & `financepy-0.300/tests_golden/TestFinBondOptionBDTModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondOptionBKModel.py` & `financepy-0.300/tests_golden/TestFinBondOptionBKModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondOptionHWModel.py` & `financepy-0.300/tests_golden/TestFinBondOptionHWModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondPortfolio.py` & `financepy-0.300/tests_golden/TestFinBondPortfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondYieldCurve.py` & `financepy-0.300/tests_golden/TestFinBondYieldCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondZeroCoupon.py` & `financepy-0.300/tests_golden/TestFinBondZeroCoupon.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinBondZeroCurve.py` & `financepy-0.300/tests_golden/TestFinBondZeroCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDS.py` & `financepy-0.300/tests_golden/TestFinCDS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSBasket.py` & `financepy-0.300/tests_golden/TestFinCDSBasket.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSCurve.py` & `financepy-0.300/tests_golden/TestFinCDSCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSIndex.py` & `financepy-0.300/tests_golden/TestFinCDSIndex.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSIndexAdjustHazards.py` & `financepy-0.300/tests_golden/TestFinCDSIndexAdjustHazards.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSIndexAdjustSpreads.py` & `financepy-0.300/tests_golden/TestFinCDSIndexAdjustSpreads.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSIndexOption.py` & `financepy-0.300/tests_golden/TestFinCDSIndexOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSIndexPortfolio.py` & `financepy-0.300/tests_golden/TestFinCDSIndexPortfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSOption.py` & `financepy-0.300/tests_golden/TestFinCDSOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCDSTranche.py` & `financepy-0.300/tests_golden/TestFinCDSTranche.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinCalendar.py` & `financepy-0.300/tests_golden/TestFinCalendar.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDate.py` & `financepy-0.300/tests_golden/TestFinDate.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDateAdjust.py` & `financepy-0.300/tests_golden/TestFinDateAdjust.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDayCount.py` & `financepy-0.300/tests_golden/TestFinDayCount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurve.py` & `financepy-0.300/tests_golden/TestFinDiscountCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurveFlat.py` & `financepy-0.300/tests_golden/TestFinDiscountCurveFlat.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurveNS.py` & `financepy-0.300/tests_golden/TestFinDiscountCurveNS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurveNSS.py` & `financepy-0.300/tests_golden/TestFinDiscountCurveNSS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurvePolynomial.py` & `financepy-0.300/tests_golden/TestFinDiscountCurvePolynomial.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurveZeros.py` & `financepy-0.300/tests_golden/TestFinDiscountCurveZeros.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinDiscountCurves.py` & `financepy-0.300/tests_golden/TestFinDiscountCurves.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityAmericanMC.py` & `financepy-0.300/tests_golden/TestFinEquityAmericanMC.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityAmericanOption.py` & `financepy-0.300/tests_golden/TestFinEquityAmericanOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityAsianOption.py` & `financepy-0.300/tests_golden/TestFinEquityAsianOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityBarrierOption.py` & `financepy-0.300/tests_golden/TestFinEquityBarrierOption.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ###############################################################################
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
 ###############################################################################
 
 import sys
+
+from financepy.utils import gDaysInYear
+
 sys.path.append("..")
 
 from FinTestCases import FinTestCases, globalTestCaseMode
 
 from financepy.utils.date import Date
 
 from financepy.models.black_scholes import BlackScholes
@@ -22,14 +25,15 @@
 ###############################################################################
 
 
 def test_EquityBarrierOption():
 
     valuation_date = Date(1, 1, 2015)
     expiry_date = Date(1, 1, 2016)
+    t_exp = (expiry_date - valuation_date) / gDaysInYear
     stock_price = 100.0
     volatility = 0.20
     interest_rate = 0.05
     dividend_yield = 0.02
     option_type = EquityBarrierTypes.DOWN_AND_OUT_CALL
     notional = 1.0
 
@@ -75,20 +79,19 @@
                                  discount_curve,
                                  dividend_curve,
                                  model)
             
             start = time.time()
             model_params = (stock_price, drift, volatility, scheme)
 
-            test_value_mc = option.value_mc(expiry_date, 
+            test_value_mc = option.value_mc(t_exp,
                                      K, 
                                      option_type.value, 
                                      B, 
-                                     notional, 
-                                     valuation_date, 
+                                     notional,
                                      stock_price,
                                      discount_curve.cc_rate(expiry_date), 
                                      process_type, 
                                      model_params)
 
             end = time.time()
             time_elapsed = round(end - start, 3)
@@ -116,20 +119,19 @@
                 stock_price,
                 discount_curve,
                 dividend_curve,
                 model)
             start = time.time()
             model_params = (stock_price, drift, volatility, scheme)
 
-            test_value_mc = option.value_mc(expiry_date, 
+            test_value_mc = option.value_mc(t_exp,
                                      K, 
                                      option_type.value, 
                                      B, 
-                                     notional, 
-                                     valuation_date, 
+                                     notional,
                                      stock_price,
                                      discount_curve.cc_rate(expiry_date), 
                                      process_type, 
                                      model_params)
 
             end = time.time()
             time_elapsed = round(end - start, 3)
```

### Comparing `financepy-0.290/tests_golden/TestFinEquityBasketOption.py` & `financepy-0.300/tests_golden/TestFinEquityBasketOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityBinomialTree.py` & `financepy-0.300/tests_golden/TestFinEquityBinomialTree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityChooserOption.py` & `financepy-0.300/tests_golden/TestFinEquityChooserOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityCliquetOption.py` & `financepy-0.300/tests_golden/TestFinEquityCliquetOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityCompoundOption.py` & `financepy-0.300/tests_golden/TestFinEquityCompoundOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityDigitalOption.py` & `financepy-0.300/tests_golden/TestFinEquityDigitalOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityForward.py` & `financepy-0.300/tests_golden/TestFinEquityForward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityLookbackOption.py` & `financepy-0.300/tests_golden/TestFinEquityLookbackOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityOneTouchOption.py` & `financepy-0.300/tests_golden/TestFinEquityOneTouchOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityRainbowOption.py` & `financepy-0.300/tests_golden/TestFinEquityRainbowOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquitySwap.py` & `financepy-0.300/tests_golden/TestFinEquitySwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityVanillaOption.py` & `financepy-0.300/tests_golden/TestFinEquityVanillaOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityVarianceSwap.py` & `financepy-0.300/tests_golden/TestFinEquityVarianceSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinEquityVolSurface.py` & `financepy-0.300/tests_golden/TestFinEquityVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXAmericanOption.py` & `financepy-0.300/tests_golden/TestFinFXAmericanOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXBarrierOption.py` & `financepy-0.300/tests_golden/TestFinFXBarrierOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXDigitalOption.py` & `financepy-0.300/tests_golden/TestFinFXDigitalOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXForward.py` & `financepy-0.300/tests_golden/TestFinFXForward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXLookbackOption.py` & `financepy-0.300/tests_golden/TestFinFXLookbackOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXOneTouchOption.py` & `financepy-0.300/tests_golden/TestFinFXOneTouchOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXOptionSABR.py` & `financepy-0.300/tests_golden/TestFinFXOptionSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXVanillaOption.py` & `financepy-0.300/tests_golden/TestFinFXVanillaOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXVolSurface.py` & `financepy-0.300/tests_golden/TestFinFXVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinFXVolSurfacePlus.py` & `financepy-0.300/tests_golden/TestFinFXVolSurfacePlus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborBermudanSwaption.py` & `financepy-0.300/tests_golden/TestFinIborBermudanSwaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborCapFloor.py` & `financepy-0.300/tests_golden/TestFinIborCapFloor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborCapVolCurve.py` & `financepy-0.300/tests_golden/TestFinIborCapVolCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborDualCurve.py` & `financepy-0.300/tests_golden/TestFinIborDualCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborFuture.py` & `financepy-0.300/tests_golden/TestFinIborFuture.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborLMMProducts.py` & `financepy-0.300/tests_golden/TestFinIborLMMProducts.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborSingleCurve.py` & `financepy-0.300/tests_golden/TestFinIborSingleCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborSwap.py` & `financepy-0.300/tests_golden/TestFinIborSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinIborSwaption.py` & `financepy-0.300/tests_golden/TestFinIborSwaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinInflationBond.py` & `financepy-0.300/tests_golden/TestFinInflationBond.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinInflationIndexCurve.py` & `financepy-0.300/tests_golden/TestFinInflationIndexCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinInterpolate.py` & `financepy-0.300/tests_golden/TestFinInterpolate.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinInterpolatedForwards.py` & `financepy-0.300/tests_golden/TestFinInterpolatedForwards.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinLossDbnBuilder.py` & `financepy-0.300/tests_golden/TestFinLossDbnBuilder.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinMath.py` & `financepy-0.300/tests_golden/TestFinMath.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinMathAccruedInterp.py` & `financepy-0.300/tests_golden/TestFinMathAccruedInterp.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelBlack.py` & `financepy-0.300/tests_golden/TestFinModelBlack.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelBlackScholes.py` & `financepy-0.300/tests_golden/TestFinModelBlackScholes.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelBlack_SABR_HW.py` & `financepy-0.300/tests_golden/TestFinModelBlack_SABR_HW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelCIR.py` & `financepy-0.300/tests_golden/TestFinModelCIR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelHeston.py` & `financepy-0.300/tests_golden/TestFinModelHeston.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelMerton.py` & `financepy-0.300/tests_golden/TestFinModelMerton.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelRatesBDT.py` & `financepy-0.300/tests_golden/TestFinModelRatesBDT.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelRatesBK.py` & `financepy-0.300/tests_golden/TestFinModelRatesBK.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelRatesHW.py` & `financepy-0.300/tests_golden/TestFinModelRatesHW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelRatesLMM.py` & `financepy-0.300/tests_golden/TestFinModelRatesLMM.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelSABR.py` & `financepy-0.300/tests_golden/TestFinModelSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinModelShiftedSABR.py` & `financepy-0.300/tests_golden/TestFinModelShiftedSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinNumbaNumpySpeed.py` & `financepy-0.300/tests_golden/TestFinNumbaNumpySpeed.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinOIS.py` & `financepy-0.300/tests_golden/TestFinOIS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinOISCurve.py` & `financepy-0.300/tests_golden/TestFinOISCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinOptionImpliedDbn.py` & `financepy-0.300/tests_golden/TestFinOptionImpliedDbn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinPieceCurve.py` & `financepy-0.300/tests_golden/TestFinPieceCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinProcessSimulator.py` & `financepy-0.300/tests_golden/TestFinProcessSimulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinSchedule.py` & `financepy-0.300/tests_golden/TestFinSchedule.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinSobol.py` & `financepy-0.300/tests_golden/TestFinSobol.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinStatistics.py` & `financepy-0.300/tests_golden/TestFinStatistics.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinSwapLegs.py` & `financepy-0.300/tests_golden/TestFinSwapLegs.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinSwaptionVolSurface.py` & `financepy-0.300/tests_golden/TestFinSwaptionVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinVasicekRateModel.py` & `financepy-0.300/tests_golden/TestFinVasicekRateModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/TestFinVolatilityCurve.py` & `financepy-0.300/tests_golden/TestFinVolatilityCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.290/tests_golden/runAllTests.py` & `financepy-0.300/tests_golden/runAllTests.py`

 * *Files identical despite different names*

