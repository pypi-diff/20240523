# Comparing `tmp/financetoolkit-1.9.0.tar.gz` & `tmp/financetoolkit-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.9.0.tar", max compression
+gzip compressed data, was "financetoolkit-1.9.1.tar", max compression
```

## Comparing `financetoolkit-1.9.0.tar` & `financetoolkit-1.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.9.0/LICENSE.txt
--rw-r--r--   0        0        0   247121 2024-04-29 18:24:37.870076 financetoolkit-1.9.0/README.md
--rw-r--r--   0        0        0      260 2024-04-29 18:23:59.825558 financetoolkit-1.9.0/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.9.0/financetoolkit/discovery/__init__.py
--rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.9.0/financetoolkit/discovery/discovery_controller.py
--rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.9.0/financetoolkit/discovery/discovery_model.py
--rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.9.0/financetoolkit/economics/__init__.py
--rw-r--r--   0        0        0   108131 2024-04-29 18:23:59.826104 financetoolkit-1.9.0/financetoolkit/economics/economics_controller.py
--rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.9.0/financetoolkit/economics/oecd_model.py
--rw-r--r--   0        0        0        0 2024-04-29 18:23:59.826176 financetoolkit-1.9.0/financetoolkit/fixedincome/__init__.py
--rw-r--r--   0        0        0    13245 2024-04-29 18:23:59.844627 financetoolkit-1.9.0/financetoolkit/fixedincome/bond_model.py
--rw-r--r--   0        0        0     4000 2024-04-29 18:23:59.961651 financetoolkit-1.9.0/financetoolkit/fixedincome/derivative_model.py
--rw-r--r--   0        0        0     2224 2024-04-29 18:23:59.961882 financetoolkit-1.9.0/financetoolkit/fixedincome/ecb_model.py
--rw-r--r--   0        0        0     1042 2024-04-29 18:23:59.962023 financetoolkit-1.9.0/financetoolkit/fixedincome/euribor_model.py
--rw-r--r--   0        0        0     5924 2024-04-29 18:23:59.827045 financetoolkit-1.9.0/financetoolkit/fixedincome/fed_model.py
--rw-r--r--   0        0        0    66392 2024-04-29 18:24:37.794605 financetoolkit-1.9.0/financetoolkit/fixedincome/fixedincome_controller.py
--rw-r--r--   0        0        0     7889 2024-04-29 18:23:59.827689 financetoolkit-1.9.0/financetoolkit/fixedincome/fred_model.py
--rw-r--r--   0        0        0      851 2024-04-29 18:23:59.962735 financetoolkit-1.9.0/financetoolkit/fixedincome/helpers.py
--rw-r--r--   0        0        0    47381 2024-01-26 13:56:45.140582 financetoolkit-1.9.0/financetoolkit/fundamentals_model.py
--rw-r--r--   0        0        0    18368 2024-04-02 15:17:03.310710 financetoolkit-1.9.0/financetoolkit/helpers.py
--rw-r--r--   0        0        0    43761 2024-04-29 18:22:33.320011 financetoolkit-1.9.0/financetoolkit/historical_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.9.0/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.9.0/financetoolkit/models/altman_model.py
--rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.9.0/financetoolkit/models/dupont_model.py
--rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.9.0/financetoolkit/models/enterprise_model.py
--rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.9.0/financetoolkit/models/growth_model.py
--rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.9.0/financetoolkit/models/helpers.py
--rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.9.0/financetoolkit/models/intrinsic_model.py
--rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.9.0/financetoolkit/models/models_controller.py
--rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.9.0/financetoolkit/models/piotroski_model.py
--rw-r--r--   0        0        0     7264 2024-04-29 18:22:33.320375 financetoolkit-1.9.0/financetoolkit/models/wacc_model.py
--rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.9.0/financetoolkit/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.9.0/financetoolkit/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.9.0/financetoolkit/normalization/income.csv
--rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.9.0/financetoolkit/normalization/statistics.csv
--rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.9.0/financetoolkit/normalization_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.9.0/financetoolkit/options/__init__.py
--rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.9.0/financetoolkit/options/binomial_trees_model.py
--rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.9.0/financetoolkit/options/black_scholes_model.py
--rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.9.0/financetoolkit/options/greeks_model.py
--rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.9.0/financetoolkit/options/helpers.py
--rw-r--r--   0        0        0   211062 2024-04-29 18:22:33.321511 financetoolkit-1.9.0/financetoolkit/options/options_controller.py
--rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.9.0/financetoolkit/options/options_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.9.0/financetoolkit/performance/__init__.py
--rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.9.0/financetoolkit/performance/helpers.py
--rw-r--r--   0        0        0    70539 2024-04-27 10:10:54.618662 financetoolkit-1.9.0/financetoolkit/performance/performance_controller.py
--rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.9.0/financetoolkit/performance/performance_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.9.0/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.9.0/financetoolkit/ratios/efficiency_model.py
--rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.9.0/financetoolkit/ratios/liquidity_model.py
--rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.9.0/financetoolkit/ratios/profitability_model.py
--rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.9.0/financetoolkit/ratios/ratios_controller.py
--rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.9.0/financetoolkit/ratios/solvency_model.py
--rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.9.0/financetoolkit/ratios/valuation_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.9.0/financetoolkit/risk/__init__.py
--rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.9.0/financetoolkit/risk/cvar_model.py
--rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.9.0/financetoolkit/risk/evar_model.py
--rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.9.0/financetoolkit/risk/garch_model.py
--rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.9.0/financetoolkit/risk/helpers.py
--rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.9.0/financetoolkit/risk/risk_controller.py
--rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.9.0/financetoolkit/risk/risk_model.py
--rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.9.0/financetoolkit/risk/var_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.9.0/financetoolkit/technicals/__init__.py
--rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.9.0/financetoolkit/technicals/breadth_model.py
--rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.9.0/financetoolkit/technicals/helpers.py
--rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.9.0/financetoolkit/technicals/momentum_model.py
--rw-r--r--   0        0        0     2761 2024-01-17 13:13:01.202897 financetoolkit-1.9.0/financetoolkit/technicals/overlap_model.py
--rw-r--r--   0        0        0    14582 2024-04-29 18:22:33.321927 financetoolkit-1.9.0/financetoolkit/technicals/statistic_model.py
--rw-r--r--   0        0        0   134139 2024-01-26 13:56:45.143730 financetoolkit-1.9.0/financetoolkit/technicals/technicals_controller.py
--rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.9.0/financetoolkit/technicals/volatility_model.py
--rw-r--r--   0        0        0   164184 2024-04-29 18:23:59.845946 financetoolkit-1.9.0/financetoolkit/toolkit_controller.py
--rw-r--r--   0        0        0     2497 2024-04-29 18:24:49.034852 financetoolkit-1.9.0/pyproject.toml
--rw-r--r--   0        0        0   248270 1970-01-01 00:00:00.000000 financetoolkit-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.9.1/LICENSE.txt
+-rw-r--r--   0        0        0   264049 2024-05-23 18:07:46.755315 financetoolkit-1.9.1/README.md
+-rw-r--r--   0        0        0      260 2024-04-29 18:23:59.825558 financetoolkit-1.9.1/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.9.1/financetoolkit/discovery/__init__.py
+-rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.9.1/financetoolkit/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.9.1/financetoolkit/discovery/discovery_model.py
+-rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.9.1/financetoolkit/economics/__init__.py
+-rw-r--r--   0        0        0   108131 2024-04-29 18:23:59.826104 financetoolkit-1.9.1/financetoolkit/economics/economics_controller.py
+-rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.9.1/financetoolkit/economics/oecd_model.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:23:59.826176 financetoolkit-1.9.1/financetoolkit/fixedincome/__init__.py
+-rw-r--r--   0        0        0    13245 2024-04-29 18:23:59.844627 financetoolkit-1.9.1/financetoolkit/fixedincome/bond_model.py
+-rw-r--r--   0        0        0     4000 2024-04-29 18:23:59.961651 financetoolkit-1.9.1/financetoolkit/fixedincome/derivative_model.py
+-rw-r--r--   0        0        0     2224 2024-04-29 18:23:59.961882 financetoolkit-1.9.1/financetoolkit/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     1042 2024-04-29 18:23:59.962023 financetoolkit-1.9.1/financetoolkit/fixedincome/euribor_model.py
+-rw-r--r--   0        0        0     5924 2024-04-29 18:23:59.827045 financetoolkit-1.9.1/financetoolkit/fixedincome/fed_model.py
+-rw-r--r--   0        0        0    68469 2024-05-23 18:08:21.583871 financetoolkit-1.9.1/financetoolkit/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0     7889 2024-04-29 18:23:59.827689 financetoolkit-1.9.1/financetoolkit/fixedincome/fred_model.py
+-rw-r--r--   0        0        0      851 2024-04-29 18:23:59.962735 financetoolkit-1.9.1/financetoolkit/fixedincome/helpers.py
+-rw-r--r--   0        0        0    47938 2024-05-23 18:06:15.608955 financetoolkit-1.9.1/financetoolkit/fundamentals_model.py
+-rw-r--r--   0        0        0    18368 2024-04-02 15:17:03.310710 financetoolkit-1.9.1/financetoolkit/helpers.py
+-rw-r--r--   0        0        0    43761 2024-05-23 18:04:30.298997 financetoolkit-1.9.1/financetoolkit/historical_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.9.1/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.9.1/financetoolkit/models/altman_model.py
+-rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.9.1/financetoolkit/models/dupont_model.py
+-rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.9.1/financetoolkit/models/enterprise_model.py
+-rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.9.1/financetoolkit/models/growth_model.py
+-rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.9.1/financetoolkit/models/helpers.py
+-rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.9.1/financetoolkit/models/intrinsic_model.py
+-rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.9.1/financetoolkit/models/models_controller.py
+-rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.9.1/financetoolkit/models/piotroski_model.py
+-rw-r--r--   0        0        0     7264 2024-05-23 18:04:30.299252 financetoolkit-1.9.1/financetoolkit/models/wacc_model.py
+-rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.9.1/financetoolkit/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.9.1/financetoolkit/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.9.1/financetoolkit/normalization/income.csv
+-rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.9.1/financetoolkit/normalization/statistics.csv
+-rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.9.1/financetoolkit/normalization_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.9.1/financetoolkit/options/__init__.py
+-rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.9.1/financetoolkit/options/binomial_trees_model.py
+-rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.9.1/financetoolkit/options/black_scholes_model.py
+-rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.9.1/financetoolkit/options/greeks_model.py
+-rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.9.1/financetoolkit/options/helpers.py
+-rw-r--r--   0        0        0   211062 2024-05-23 18:04:30.299969 financetoolkit-1.9.1/financetoolkit/options/options_controller.py
+-rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.9.1/financetoolkit/options/options_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.9.1/financetoolkit/performance/__init__.py
+-rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.9.1/financetoolkit/performance/helpers.py
+-rw-r--r--   0        0        0    70539 2024-04-27 10:10:54.618662 financetoolkit-1.9.1/financetoolkit/performance/performance_controller.py
+-rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.9.1/financetoolkit/performance/performance_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.9.1/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.9.1/financetoolkit/ratios/efficiency_model.py
+-rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.9.1/financetoolkit/ratios/liquidity_model.py
+-rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.9.1/financetoolkit/ratios/profitability_model.py
+-rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.9.1/financetoolkit/ratios/ratios_controller.py
+-rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.9.1/financetoolkit/ratios/solvency_model.py
+-rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.9.1/financetoolkit/ratios/valuation_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.9.1/financetoolkit/risk/__init__.py
+-rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.9.1/financetoolkit/risk/cvar_model.py
+-rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.9.1/financetoolkit/risk/evar_model.py
+-rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.9.1/financetoolkit/risk/garch_model.py
+-rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.9.1/financetoolkit/risk/helpers.py
+-rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.9.1/financetoolkit/risk/risk_controller.py
+-rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.9.1/financetoolkit/risk/risk_model.py
+-rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.9.1/financetoolkit/risk/var_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.9.1/financetoolkit/technicals/__init__.py
+-rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.9.1/financetoolkit/technicals/breadth_model.py
+-rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.9.1/financetoolkit/technicals/helpers.py
+-rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.9.1/financetoolkit/technicals/momentum_model.py
+-rw-r--r--   0        0        0     5496 2024-05-23 18:06:15.609233 financetoolkit-1.9.1/financetoolkit/technicals/overlap_model.py
+-rw-r--r--   0        0        0    14582 2024-05-23 18:04:30.300778 financetoolkit-1.9.1/financetoolkit/technicals/statistic_model.py
+-rw-r--r--   0        0        0   138478 2024-05-23 18:06:15.609743 financetoolkit-1.9.1/financetoolkit/technicals/technicals_controller.py
+-rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.9.1/financetoolkit/technicals/volatility_model.py
+-rw-r--r--   0        0        0   164876 2024-05-23 18:06:15.610492 financetoolkit-1.9.1/financetoolkit/toolkit_controller.py
+-rw-r--r--   0        0        0     2497 2024-05-23 18:06:53.457347 financetoolkit-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0   265198 1970-01-01 00:00:00.000000 financetoolkit-1.9.1/PKG-INFO
```

### Comparing `financetoolkit-1.9.0/LICENSE.txt` & `financetoolkit-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/README.md` & `financetoolkit-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 
 # a Technical example
 ichimoku_cloud = companies.technicals.get_ichimoku_cloud()
 
 # a Fixed Income example
 corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
 
+# a Fixed Income example
+corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
+
 # an Economics example
 unemployment_rates = companies.economics.get_unemployment_rate()
 ````
 
 Generally, the functions return a DataFrame with a multi-index in which all tickers, in this case Apple and Microsoft, are presented. To keep things manageable for this README, I select just Apple but in essence the list of tickers can be endless as I've seen DataFrames with thousands of tickers. The filtering is done through `.loc['AAPL']` and `.xs('AAPL', level=1, axis=1)` based on whether it's fundamental data or historical data respectively.
 
 ### Obtaining Historical Data
@@ -257,17 +260,17 @@
 |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
 | 2024-04-19 | 0.0518 | 0.0532 | 0.0561 | 0.0594 | 0.0678 | 0.0804 | 0.1385 |
 | 2024-04-22 | 0.0517 | 0.0532 | 0.056  | 0.0593 | 0.0671 | 0.0793 | 0.1377 |
 | 2024-04-23 | 0.0514 | 0.0528 | 0.0556 | 0.0589 | 0.066  | 0.0777 | 0.1364 |
 | 2024-04-24 | 0.0518 | 0.0531 | 0.0559 | 0.0592 | 0.0664 | 0.0778 | 0.1361 |
 | 2024-04-25 | 0.0524 | 0.0537 | 0.0564 | 0.0598 | 0.0673 | 0.079  | 0.1368 |
 
-And below Effective Yields, Option-Adjusted Spreads (OAS), Yield to Worst and Total Returns are plotted over time for the different maturity periods.
+And below a variety of Fixed Income metrics are shown all acquired from the Fixed Income module.
 
-![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/816cf251-4152-4341-a08e-a36268f5f721)
+![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/dfe2a819-87d8-46be-892c-f90663bc177d)
 
 ### Understanding Key Economic Indicators
 
 Get insights for 60+ countries into key economic indicators such as the Consumer Price Index (CPI), Gross Domestic Product (GDP), Unemployment Rates and 3-month and 10-year Government Interest Rates. This is done through the `economics` module and can be used as a standalone module as well by using `from financetoolkit import Economics`. For example see a selection of the countries below:
 
 |      |   Colombia |   United States |   Sweden |   Japan |   Germany |
 |:-----|-----------:|----------------:|---------:|--------:|----------:|
@@ -277,14 +280,15 @@
 | 2020 |     0.1586 |          0.0809 |   0.0848 |  0.0278 |    0.0362 |
 | 2021 |     0.1381 |          0.0537 |   0.0889 |  0.0282 |    0.0358 |
 | 2022 |     0.1122 |          0.0365 |   0.0748 |  0.026  |    0.0307 |
 
 And below these Unemployment Rates are plotted over time:
 
 ![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
+![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
 
 # Core Functionality and Metrics
 
 The Finance Toolkit has the ability to collect 30+ years of financial statements and calculate 150+ financial metrics. The following list shows all of the available functionality and metrics.
 
 Each ratio and indicator has a corresponding function that can be called directly for example `ratios.get_return_on_equity` or `technicals.get_relative_strength_index`. However, there are also functions that collect multiple ratios or indicators at once such as `ratios.collect_profitability_ratios`. These functions are useful when you want to collect a large amount of ratios or indicators at once.
 
@@ -2551,14 +2555,231 @@
 
 </details>
 
 ## Fixed Income
 
 The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
 
+<details>
+    <summary><b>Bond Valuations</b></summary>
+The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
+
+All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_present_value()
+```
+
+> **Bond Statistics**
+
+The bond statistics contains a variety of different metrics to evaluate a bond. These include:
+
+- **Par Value:** The face value of the bond.
+- **Coupon Rate:** The annual coupon rate (in decimal).
+- **Years to Maturity:** The number of years until the bond matures.
+- **Yield to Maturity:** The yield to maturity of the bond (in decimal).
+- **Frequency:** The number of coupon payments per year.
+- **Present Value:** The present value of the bond.
+- **Current Yield:** The annual coupon payment divided by the bond price.
+- **Effective Yield:** The return on a bond that has its interest payments (or coupons) reinvested at the same rate by the bondholder.
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+- **DV01:** The dollar value of a 0.01% change in yield to maturity.
+- **Convexity:** The second derivative of the bond price with respect to the yield to maturity.
+
+It gives a complete overview of the bond's performance. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_statistics) and an example below which shows the bond statistics for six different bonds using this functionality.
+
+|                     |   Bond 1 |   Bond 2 |   Bond 3 |    Bond 4 |   Bond 5 |   Bond 6 |
+|:--------------------|---------:|---------:|---------:|----------:|---------:|---------:|
+| Par Value           | 100      | 250      |  50      | 1000      |  85      | 320      |
+| Coupon Rate         |   0.05   |   0.02   |   0.075  |    0      |   0.15   |   0.015  |
+| Years to Maturity   |   5      |  10      |   2      |   10      |   3      |   1      |
+| Yield to Maturity   |   0.08   |   0.021  |   0.03   |    0      |   0.16   |   0.04   |
+| Frequency           |   1      |   1      |   4      |    1      |   2      |  12      |
+| Present Value       |  88.0219 | 247.766  |  54.3518 | 1000      |  83.0353 | 312.171  |
+| Current Yield       |   0.0568 |   0.0202 |   0.069  |    0      |   0.1535 |   0.0154 |
+| Effective Yield     |   0.05   |   0.02   |   0.0771 |    0      |   0.1556 |   0.0151 |
+| Macaulay's Duration |   4.5116 |   9.1576 |   1.8849 |   10      |   2.5667 |   0.9932 |
+| Modified Duration   |   4.1774 |   8.9693 |   1.8709 |   10      |   2.3766 |   0.9899 |
+| Effective Duration  |   4.0677 |   8.5181 |   1.8477 |    9.4713 |   2.2952 |   0.9844 |
+| Dollar Duration     |   3.677  |  22.2228 |   1.0168 |  100      |   1.9734 |   3.0902 |
+| DV01                |   0.0004 |   0.0022 |   0      |    0.01   |   0.0001 |   0      |
+| Convexity           |  22.4017 |  93.7509 |   4.0849 |  110      |   7.0923 |   1.0662 |
+
+> **Present Value**
+
+The bond price is the present value of the bond's future cash flows. It is calculated by discounting the bond's coupon payments and principal repayment to the present value using the bond's yield to maturity. The present value is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_price).
+
+> **Duration**
+
+The bond duration is a measure of the bond's sensitivity to changes in interest rates. It is the weighted average of the bond's cash flows, where the weights are the present value of each cash flow divided by the bond's price. It is possible to calculate the following durations:
+
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+
+The duration values are depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_duration).
+
+> **Yield to Maturity**
+
+The Yield to Maturity (YTM) is the total return anticipated on a bond if it is held until it matures. It is the internal rate of return of an investment in a bond if the investor holds the bond until maturity and receives all payments as scheduled. The yield to maturity is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_yield_to_maturity).
+
+</details>
+
+<details>
+    <summary><b>Derivative Valuations</b></summary>
+The Derivative Valuations section contains a variety of models that can be used to value derivative instruments such as Swaptions. These models include the Black Model and the Bachelier Model.
+
+All derivative valuations can be called by using `get_` to get a single valuation. E.g. `get_derivative_price`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_derivative_price(model_type="black")
+```
+
+> **Black Model**
+
+The Black Model is a mathematical model used to calculate the price of European-style options. It is based on the Black-Scholes model but is used for interest rate options. The Black Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+> **Bachelier Model**
+
+The Bachelier Model is a mathematical model used to calculate the price of European-style options. It is based on the normal distribution and is used for interest rate options as opposed to the Black model which uses a log-normal distribution. The Bachelier Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+</details>
+
+<details>
+    <summary><b>Central Banks</b></summary>
+
+The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
+
+All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_european_central_bank_rates()
+```
+
+> **Main Refinancing Operations**
+
+The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+
+> **Marginal Lending Facility**
+
+The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Deposit Facility**
+
+The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Euribor Rates**
+
+The Euro Interbank Offered Rate (Euribor) is a daily reference rate based on the averaged interest rates at which Eurozone banks offer to lend unsecured funds to other banks in the euro wholesale money market. It is widely used as the base rate for a variety of financial products, including mortgages, savings accounts, and derivatives. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_euribor_rates).
+
+> **Effective Federal Funds Rate**
+
+The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Overnight Bank Funding Rate**
+
+The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Tri-Party General Collateral Rate**
+
+The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Broad General Collateral Rate**
+
+The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Secured Overnight Financing Rate (SOFR)**
+
+The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+</details>
+
+<details>
+    <summary><b>Government Bonds</b></summary>
+
+It is possible to view both short-term (3-month) and long-term (10-year) interest rates for each of the available countries. These rates relate to the interest rates at which countries issue government bonds and are used as a benchmark for other interest rates in the economy. For example, the German government bond yield is an overall indicator of the European economy.
+
+These interest rates can be obtained with `get_government_bond_yield`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_government_bond_yield()
+```
+
+> **Long Term Interest Rates (10 year)**
+
+Long-term interest rates refer to government bonds maturing in ten years. Rates are mainly determined by the price charged by the lender, the risk from the borrower and the fall in the capital value. Long-term interest rates are generally averages of daily rates, measured as a percentage. These interest rates are implied by the prices at which the government bonds are traded on financial markets, not the interest rates at which the loans were issued.
+
+In all cases, they refer to bonds whose capital repayment is guaranteed by governments. Long-term interest rates are one of the determinants of business investment. Low long term interest rates encourage investment in new equipment and high interest rates discourage it. Investment is, in turn, a major source of economic growth. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+> **Short Term Interest Rates (3 month)**
+
+Short-term interest rates are the rates at which short-term borrowings are effected between financial institutions or the rate at which short-term government paper is issued or traded in the market. Short-term interest rates are generally averages of daily rates, measured as a percentage.
+
+Short-term interest rates are based on three-month money market rates where available. Typical standardised names are “money market rate” and “treasury bill rate”. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+</details>
+
+<details>
+    <summary><b>Corporate Bonds</b></summary>
+
+The Corporate Bonds section features the widely used ICE BofA benchmarks which include option-adjusted spreads, effective yields and the total returns. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All corporate bond metrics can be called by using `get_` to get a single metric. E.g. `get_ice_bofa_option_adjusted_spread` or `get_ice_bofa_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_ice_bofa_option_adjusted_spread()
+```
+
+> **Option-Adjusted Spread (OAS)**
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_option_adjusted_spread).
+
+> **Effective Yield**
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_effective_yield).
+
+> **Total Return**
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_total_return).
+
+> **Yield to Worst**
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_yield_to_worst).
+
+</details>
+
+## Fixed Income
+
+The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
+
 <details>
     <summary><b>Bond Valuations</b></summary>
 The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
 
 All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
 
 ```python
```

### Comparing `financetoolkit-1.9.0/financetoolkit/discovery/discovery_controller.py` & `financetoolkit-1.9.1/financetoolkit/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/discovery/discovery_model.py` & `financetoolkit-1.9.1/financetoolkit/discovery/discovery_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/economics/economics_controller.py` & `financetoolkit-1.9.1/financetoolkit/economics/economics_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/economics/oecd_model.py` & `financetoolkit-1.9.1/financetoolkit/economics/oecd_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/bond_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/bond_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/derivative_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/derivative_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/ecb_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/ecb_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/euribor_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/euribor_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/fed_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/fed_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/fixedincome_controller.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/fixedincome_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,51 @@
             years_to_maturity (int): The number of years until the bond matures. Defaults to 5.
             yield_to_maturity (float): The yield to maturity of the bond (in decimal). Defaults to 0.08.
             frequency (int): The number of coupon payments per year. Defaults to 1.
             show_input_info (bool, optional): Whether to display input information. Defaults to True.
 
         Returns:
             pd.Series: A pandas Series containing the bond statistics.
+
+        As an example:
+
+        ```python
+        from financetoolkit import FixedIncome
+
+        fixedincome = FixedIncome()
+
+        # This is one example and below a collection of different bonds
+        # is shown with different characteristics
+        fixedincome.collect_bond_statistics(
+            par_value=100,
+            coupon_rate=0.05,
+            years_to_maturity=5,
+            yield_to_maturity=0.08,
+            frequency=1,
+        )
+        ```
+
+        Which returns:
+
+        |                     |   Bond 1 |   Bond 2 |   Bond 3 |    Bond 4 |   Bond 5 |   Bond 6 |
+        |:--------------------|---------:|---------:|---------:|----------:|---------:|---------:|
+        | Par Value           | 100      | 250      |  50      | 1000      |  85      | 320      |
+        | Coupon Rate         |   0.05   |   0.02   |   0.075  |    0      |   0.15   |   0.015  |
+        | Years to Maturity   |   5      |  10      |   2      |   10      |   3      |   1      |
+        | Yield to Maturity   |   0.08   |   0.021  |   0.03   |    0      |   0.16   |   0.04   |
+        | Frequency           |   1      |   1      |   4      |    1      |   2      |  12      |
+        | Present Value       |  88.0219 | 247.766  |  54.3518 | 1000      |  83.0353 | 312.171  |
+        | Current Yield       |   0.0568 |   0.0202 |   0.069  |    0      |   0.1535 |   0.0154 |
+        | Effective Yield     |   0.05   |   0.02   |   0.0771 |    0      |   0.1556 |   0.0151 |
+        | Macaulay's Duration |   4.5116 |   9.1576 |   1.8849 |   10      |   2.5667 |   0.9932 |
+        | Modified Duration   |   4.1774 |   8.9693 |   1.8709 |   10      |   2.3766 |   0.9899 |
+        | Effective Duration  |   4.0677 |   8.5181 |   1.8477 |    9.4713 |   2.2952 |   0.9844 |
+        | Dollar Duration     |   3.677  |  22.2228 |   1.0168 |  100      |   1.9734 |   3.0902 |
+        | DV01                |   0.0004 |   0.0022 |   0      |    0.01   |   0.0001 |   0      |
+        | Convexity           |  22.4017 |  93.7509 |   4.0849 |  110      |   7.0923 |   1.0662 |
         """
         bond_statistics = {
             "Par Value": par_value,
             "Coupon Rate": coupon_rate,
             "Years to Maturity": years_to_maturity,
             "Yield to Maturity": yield_to_maturity,
             "Frequency": frequency,
@@ -832,285 +869,14 @@
 
         government_bond_yield = government_bond_yield.loc[
             self._start_date : None if forecast else self._end_date
         ]
 
         return government_bond_yield.round(rounding if rounding else self._rounding)
 
-    def get_european_central_bank_rates(
-        self, rate: str | None = None, rounding: int | None = None
-    ):
-        """
-        The Governing Council of the ECB sets the key interest rates for the
-        euro area. The available rates are:
-
-        - Main refinancing operations (refinancing)
-        - Marginal lending facility (lending)
-        - Deposit facility (deposit)
-
-        The main refinancing operations (MRO) rate is the interest rate banks
-        pay when they borrow money from the ECB for one week. When they do this,
-        they have to provide collateral to guarantee that the money will be paid back.
-
-        The marginal lending facility rate is the interest rate banks pay when they
-        borrow from the ECB overnight. When they do this, they have to provide collateral,
-        for example securities, to guarantee that the money will be paid back.
-
-        The deposit facility rate is one of the three interest rates the ECB sets every
-        six weeks as part of its monetary policy. The rate defines the interest banks
-        receive for depositing money with the central bank overnight.
-
-        See source: https://data.ecb.europa.eu/main-figures/
-
-        Args:
-            rate (str, optional): The rate to return. Defaults to None, which returns all rates.
-                Choose between 'refinancing', 'lending' or 'deposit'.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the ECB rates.
-
-        As an example:
-
-        ```python
-        from financetoolkit import FixedIncome
-
-        fixedincome = FixedIncome(start_date='2023-12-01')
-
-        fixedincome.get_european_central_bank_rates()
-        ```
-
-        Which returns:
-
-        |            |   Refinancing |   Lending |   Deposit |
-        |:-----------|--------------:|----------:|----------:|
-        | 2023-12-01 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-02 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-03 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-04 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-05 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-06 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-07 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-08 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-09 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-10 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-11 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-12 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-13 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-14 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-15 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-16 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-17 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-18 |         0.045 |    0.0475 |      0.04 |
-        """
-        ecb_rates = pd.DataFrame()
-
-        if rate and rate not in ["refinancing", "lending", "deposit"]:
-            raise ValueError(
-                "Rate must be one of 'refinancing', 'lending' or 'deposit' or left empty for all."
-            )
-
-        if not rate or rate == "refinancing":
-            ecb_rates["Refinancing"] = ecb_model.get_main_refinancing_operations()
-        if not rate or rate == "lending":
-            ecb_rates["Lending"] = ecb_model.get_marginal_lending_facility()
-        if not rate or rate == "deposit":
-            ecb_rates["Deposit"] = ecb_model.get_deposit_facility()
-
-        ecb_rates = ecb_rates.loc[self._start_date : self._end_date]
-
-        ecb_rates = ecb_rates.round(rounding if rounding else self._rounding)
-
-        return ecb_rates
-
-    def get_federal_reserve_rates(
-        self, rate: str = "EFFR", rounding: int | None = None
-    ):
-        """
-        Get the Federal Reserve rates as published by the Federal Reserve Bank of New York.
-        The federal funds market consists of domestic unsecured borrowings in U.S. dollars
-        by depository institutions from other depository institutions and certain other
-        entities, primarily government-sponsored enterprises.
-
-        The following rates are available:
-
-        - Effective Federal Funds Rate (EFFR)
-        - Overnight Bank Funding Rate (OBFR)
-        - Tri-Party General Collateral Rate (TGCR)
-        - Broad General Collateral Rate (BGCR)
-        - Secured Overnight Financing Rate (SOFR)
-
-        The effective federal funds rate (EFFR) is calculated as a volume-weighted median
-        of overnight federal funds transactions reported in the FR 2420 Report of Selected
-        Money Market Rates.
-
-        The overnight bank funding rate (OBFR) is calculated as a volume-weighted median
-        of overnight federal funds transactions, Eurodollar transactions, and the
-        domestic deposits reported as “Selected Deposits” in the FR 2420 Report.
-
-        The TGCR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon.
-
-        The BGCR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon as well
-        as GCF Repo transaction data obtained from the U.S. Department of the
-        Treasury’s Office of Financial Research (OFR).
-
-        The SOFR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon as well as
-        GCF Repo transaction data and data on bilateral Treasury repo transactions
-        cleared through FICC's DVP service, which are obtained from the U.S.
-        Department of the Treasury’s Office of Financial Research (OFR).
-
-        The New York Fed publishes the rates for the prior business day on the New
-        York Fed’s website between 8:00 and 9:00 a.m.
-
-        See source: https://www.newyorkfed.org/markets/reference-rates/
-
-        Args:
-            rate (str): The rate to return. Defaults to 'EFFR' (Effective Federal Funds Rate).
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Federal Reserve rates including the rate,
-                percentiles, volume and upper and lower bounds.
-
-        As an example:
-
-        ```python
-        from financetoolkit import FixedIncome
-
-        fixedincome = FixedIncome(start_date='2023-12-01')
-
-        effr = fixedincome.get_federal_reserve_rates()
-
-        effr.loc[:, ['Rate', '1st Percentile', '25th Percentile', '75th Percentile', '99th Percentile']]
-        ```
-
-        Which returns:
-
-        | Effective Date   |   Rate |   1st Percentile |   25th Percentile |   75th Percentile |   99th Percentile |
-        |:-----------------|-------:|-----------------:|------------------:|------------------:|------------------:|
-        | 2023-12-01       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0544 |
-        | 2023-12-04       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-05       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-06       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-07       | 0.0533 |            0.053 |            0.0531 |            0.0534 |            0.0545 |
-        | 2023-12-08       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-11       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-12       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0544 |
-        | 2023-12-13       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0545 |
-        | 2023-12-14       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0535 |
-        """
-        rate = rate.upper()
-
-        if rate == "EFFR":
-            fed_data = fed_model.get_effective_federal_funds_rate()
-        elif rate == "OBFR":
-            fed_data = fed_model.get_overnight_banking_funding_rate()
-        elif rate == "TGCR":
-            fed_data = fed_model.get_tri_party_general_collateral_rate()
-        elif rate == "BGCR":
-            fed_data = fed_model.get_broad_general_collateral_rate()
-        elif rate == "SOFR":
-            fed_data = fed_model.get_secured_overnight_financing_rate()
-        else:
-            raise ValueError(
-                "Rate must be one of 'EFFR', 'OBFR', 'TGCR', 'BGCR' or 'SOFR'."
-            )
-
-        fed_data = fed_data.loc[self._start_date : self._end_date]
-
-        fed_data = fed_data.round(rounding if rounding else self._rounding)
-
-        return fed_data
-
-    @handle_errors
-    def get_euribor_rates(
-        self,
-        maturities: str | list | None = None,
-        nominal: bool = True,
-        rounding: int | None = None,
-    ):
-        """
-        Euribor rates, short for Euro Interbank Offered Rate, are the interest rates at which a panel
-        of European banks lend funds to one another in the interbank market. These rates are published
-        daily by the European Money Markets Institute (EMMI) and serve as a benchmark for various
-        financial products and contracts, including mortgages, loans, and derivatives, across the Eurozone.
-
-        The Euribor rates are determined for different maturities, typically ranging from overnight to 12 months
-        The most common maturities are 1 month, 3 months, 6 months, and 12 months. Each maturity represents
-        the time period for which the funds are borrowed, with longer maturities generally implying higher
-        interest rates due to increased uncertainty and risk over longer time horizons.
-
-        For more information, see for example: https://data.ecb.europa.eu/data/datasets/FM/FM.M.U2.EUR.RT.MM.EURIBOR6MD_.HSTA
-
-        Args:
-            maturities (str | list | None, optional): Maturities for which to retrieve rates. Defaults to None.
-                When set to None, it will retrieve rates for 1 month, 3 months, 6 months, and 12 months.
-            nominal (bool, optional): Flag indicating whether to retrieve nominal rates. Defaults to True.
-            rounding (int | None, optional): Rounding precision for the rates. Defaults to None.
-
-        Returns:
-            pandas.DataFrame: DataFrame containing the Euribor rates for the specified maturities.
-
-        As an example:
-
-        ```python
-        from financetoolkit import FixedIncome
-
-        fixedincome = FixedIncome(start_date='2023-12-01')
-
-        euribor_rates = fixedincome.get_euribor_rates()
-        ```
-
-        Which returns:
-
-        |         |   1-Month |   3-Month |   6-Month |   12-Month |
-        |:--------|----------:|----------:|----------:|-----------:|
-        | 2023-12 |    0.0386 |    0.0393 |    0.0392 |     0.0367 |
-        | 2024-01 |    0.0387 |    0.0393 |    0.0389 |     0.0361 |
-        | 2024-02 |    0.0387 |    0.0392 |    0.039  |     0.0367 |
-        | 2024-03 |    0.0385 |    0.0392 |    0.0389 |     0.0372 |
-        """
-        if isinstance(maturities, str):
-            maturities = [maturities]
-
-        maturity_names = {
-            "1M": "1-Month",
-            "3M": "3-Month",
-            "6M": "6-Month",
-            "1Y": "12-Month",
-        }
-
-        maturities = ["1M", "3M", "6M", "1Y"] if maturities is None else maturities
-        euribor_rates = pd.DataFrame(
-            columns=[maturity_names[maturity] for maturity in maturities]
-        )
-
-        for maturity in maturities:
-            if maturity not in ["1M", "3M", "6M", "1Y"]:
-                print(
-                    f"Invalid maturity: {maturity}, please choose from 1M, 3M, 6M, 1Y."
-                )
-
-            maturity_name = maturity_names[maturity]
-
-            if not nominal and maturity == "3M" and len(maturities) > 1:
-                print("Please note that only the 3-Month Euribor rate has a real rate.")
-
-            euribor_rates[maturity_name] = euribor_model.get_euribor_rate(
-                maturity=maturity,
-                nominal=nominal if not nominal and maturity == "3M" else True,
-            )
-
-        euribor_rates = euribor_rates.loc[self._start_date : self._end_date]
-
-        euribor_rates = euribor_rates.round(rounding if rounding else self._rounding)
-
-        return euribor_rates
-
     @handle_errors
     def get_ice_bofa_option_adjusted_spread(
         self,
         maturity: bool = True,
         rounding: int | None = None,
     ):
         """
@@ -1378,7 +1144,278 @@
         )
 
         yield_to_worst = yield_to_worst.loc[self._start_date : self._end_date]
 
         yield_to_worst = yield_to_worst.round(rounding if rounding else self._rounding)
 
         return yield_to_worst
+
+    @handle_errors
+    def get_euribor_rates(
+        self,
+        maturities: str | list | None = None,
+        nominal: bool = True,
+        rounding: int | None = None,
+    ):
+        """
+        Euribor rates, short for Euro Interbank Offered Rate, are the interest rates at which a panel
+        of European banks lend funds to one another in the interbank market. These rates are published
+        daily by the European Money Markets Institute (EMMI) and serve as a benchmark for various
+        financial products and contracts, including mortgages, loans, and derivatives, across the Eurozone.
+
+        The Euribor rates are determined for different maturities, typically ranging from overnight to 12 months
+        The most common maturities are 1 month, 3 months, 6 months, and 12 months. Each maturity represents
+        the time period for which the funds are borrowed, with longer maturities generally implying higher
+        interest rates due to increased uncertainty and risk over longer time horizons.
+
+        For more information, see for example: https://data.ecb.europa.eu/data/datasets/FM/FM.M.U2.EUR.RT.MM.EURIBOR6MD_.HSTA
+
+        Args:
+            maturities (str | list | None, optional): Maturities for which to retrieve rates. Defaults to None.
+                When set to None, it will retrieve rates for 1 month, 3 months, 6 months, and 12 months.
+            nominal (bool, optional): Flag indicating whether to retrieve nominal rates. Defaults to True.
+            rounding (int | None, optional): Rounding precision for the rates. Defaults to None.
+
+        Returns:
+            pandas.DataFrame: DataFrame containing the Euribor rates for the specified maturities.
+
+        As an example:
+
+        ```python
+        from financetoolkit import FixedIncome
+
+        fixedincome = FixedIncome(start_date='2023-12-01')
+
+        euribor_rates = fixedincome.get_euribor_rates()
+        ```
+
+        Which returns:
+
+        |         |   1-Month |   3-Month |   6-Month |   12-Month |
+        |:--------|----------:|----------:|----------:|-----------:|
+        | 2023-12 |    0.0386 |    0.0393 |    0.0392 |     0.0367 |
+        | 2024-01 |    0.0387 |    0.0393 |    0.0389 |     0.0361 |
+        | 2024-02 |    0.0387 |    0.0392 |    0.039  |     0.0367 |
+        | 2024-03 |    0.0385 |    0.0392 |    0.0389 |     0.0372 |
+        """
+        if isinstance(maturities, str):
+            maturities = [maturities]
+
+        maturity_names = {
+            "1M": "1-Month",
+            "3M": "3-Month",
+            "6M": "6-Month",
+            "1Y": "12-Month",
+        }
+
+        maturities = ["1M", "3M", "6M", "1Y"] if maturities is None else maturities
+        euribor_rates = pd.DataFrame(
+            columns=[maturity_names[maturity] for maturity in maturities]
+        )
+
+        for maturity in maturities:
+            if maturity not in ["1M", "3M", "6M", "1Y"]:
+                print(
+                    f"Invalid maturity: {maturity}, please choose from 1M, 3M, 6M, 1Y."
+                )
+
+            maturity_name = maturity_names[maturity]
+
+            if not nominal and maturity == "3M" and len(maturities) > 1:
+                print("Please note that only the 3-Month Euribor rate has a real rate.")
+
+            euribor_rates[maturity_name] = euribor_model.get_euribor_rate(
+                maturity=maturity,
+                nominal=nominal if not nominal and maturity == "3M" else True,
+            )
+
+        euribor_rates = euribor_rates.loc[self._start_date : self._end_date]
+
+        euribor_rates = euribor_rates.round(rounding if rounding else self._rounding)
+
+        return euribor_rates
+
+    def get_european_central_bank_rates(
+        self, rate: str | None = None, rounding: int | None = None
+    ):
+        """
+        The Governing Council of the ECB sets the key interest rates for the
+        euro area. The available rates are:
+
+        - Main refinancing operations (refinancing)
+        - Marginal lending facility (lending)
+        - Deposit facility (deposit)
+
+        The main refinancing operations (MRO) rate is the interest rate banks
+        pay when they borrow money from the ECB for one week. When they do this,
+        they have to provide collateral to guarantee that the money will be paid back.
+
+        The marginal lending facility rate is the interest rate banks pay when they
+        borrow from the ECB overnight. When they do this, they have to provide collateral,
+        for example securities, to guarantee that the money will be paid back.
+
+        The deposit facility rate is one of the three interest rates the ECB sets every
+        six weeks as part of its monetary policy. The rate defines the interest banks
+        receive for depositing money with the central bank overnight.
+
+        See source: https://data.ecb.europa.eu/main-figures/
+
+        Args:
+            rate (str, optional): The rate to return. Defaults to None, which returns all rates.
+                Choose between 'refinancing', 'lending' or 'deposit'.
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the ECB rates.
+
+        As an example:
+
+        ```python
+        from financetoolkit import FixedIncome
+
+        fixedincome = FixedIncome(start_date='2023-12-01')
+
+        fixedincome.get_european_central_bank_rates()
+        ```
+
+        Which returns:
+
+        |            |   Refinancing |   Lending |   Deposit |
+        |:-----------|--------------:|----------:|----------:|
+        | 2023-12-01 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-02 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-03 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-04 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-05 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-06 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-07 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-08 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-09 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-10 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-11 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-12 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-13 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-14 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-15 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-16 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-17 |         0.045 |    0.0475 |      0.04 |
+        | 2023-12-18 |         0.045 |    0.0475 |      0.04 |
+        """
+        ecb_rates = pd.DataFrame()
+
+        if rate and rate not in ["refinancing", "lending", "deposit"]:
+            raise ValueError(
+                "Rate must be one of 'refinancing', 'lending' or 'deposit' or left empty for all."
+            )
+
+        if not rate or rate == "refinancing":
+            ecb_rates["Refinancing"] = ecb_model.get_main_refinancing_operations()
+        if not rate or rate == "lending":
+            ecb_rates["Lending"] = ecb_model.get_marginal_lending_facility()
+        if not rate or rate == "deposit":
+            ecb_rates["Deposit"] = ecb_model.get_deposit_facility()
+
+        ecb_rates = ecb_rates.loc[self._start_date : self._end_date]
+
+        ecb_rates = ecb_rates.round(rounding if rounding else self._rounding)
+
+        return ecb_rates
+
+    def get_federal_reserve_rates(
+        self, rate: str = "EFFR", rounding: int | None = None
+    ):
+        """
+        Get the Federal Reserve rates as published by the Federal Reserve Bank of New York.
+        The federal funds market consists of domestic unsecured borrowings in U.S. dollars
+        by depository institutions from other depository institutions and certain other
+        entities, primarily government-sponsored enterprises.
+
+        The following rates are available:
+
+        - Effective Federal Funds Rate (EFFR)
+        - Overnight Bank Funding Rate (OBFR)
+        - Tri-Party General Collateral Rate (TGCR)
+        - Broad General Collateral Rate (BGCR)
+        - Secured Overnight Financing Rate (SOFR)
+
+        The effective federal funds rate (EFFR) is calculated as a volume-weighted median
+        of overnight federal funds transactions reported in the FR 2420 Report of Selected
+        Money Market Rates.
+
+        The overnight bank funding rate (OBFR) is calculated as a volume-weighted median
+        of overnight federal funds transactions, Eurodollar transactions, and the
+        domestic deposits reported as “Selected Deposits” in the FR 2420 Report.
+
+        The TGCR is calculated as a volume-weighted median of transaction-level
+        tri-party repo data collected from the Bank of New York Mellon.
+
+        The BGCR is calculated as a volume-weighted median of transaction-level
+        tri-party repo data collected from the Bank of New York Mellon as well
+        as GCF Repo transaction data obtained from the U.S. Department of the
+        Treasury’s Office of Financial Research (OFR).
+
+        The SOFR is calculated as a volume-weighted median of transaction-level
+        tri-party repo data collected from the Bank of New York Mellon as well as
+        GCF Repo transaction data and data on bilateral Treasury repo transactions
+        cleared through FICC's DVP service, which are obtained from the U.S.
+        Department of the Treasury’s Office of Financial Research (OFR).
+
+        The New York Fed publishes the rates for the prior business day on the New
+        York Fed’s website between 8:00 and 9:00 a.m.
+
+        See source: https://www.newyorkfed.org/markets/reference-rates/
+
+        Args:
+            rate (str): The rate to return. Defaults to 'EFFR' (Effective Federal Funds Rate).
+
+        Returns:
+            pd.DataFrame: A DataFrame containing the Federal Reserve rates including the rate,
+                percentiles, volume and upper and lower bounds.
+
+        As an example:
+
+        ```python
+        from financetoolkit import FixedIncome
+
+        fixedincome = FixedIncome(start_date='2023-12-01')
+
+        effr = fixedincome.get_federal_reserve_rates()
+
+        effr.loc[:, ['Rate', '1st Percentile', '25th Percentile', '75th Percentile', '99th Percentile']]
+        ```
+
+        Which returns:
+
+        | Effective Date   |   Rate |   1st Percentile |   25th Percentile |   75th Percentile |   99th Percentile |
+        |:-----------------|-------:|-----------------:|------------------:|------------------:|------------------:|
+        | 2023-12-01       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0544 |
+        | 2023-12-04       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
+        | 2023-12-05       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
+        | 2023-12-06       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
+        | 2023-12-07       | 0.0533 |            0.053 |            0.0531 |            0.0534 |            0.0545 |
+        | 2023-12-08       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
+        | 2023-12-11       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
+        | 2023-12-12       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0544 |
+        | 2023-12-13       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0545 |
+        | 2023-12-14       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0535 |
+        """
+        rate = rate.upper()
+
+        if rate == "EFFR":
+            fed_data = fed_model.get_effective_federal_funds_rate()
+        elif rate == "OBFR":
+            fed_data = fed_model.get_overnight_banking_funding_rate()
+        elif rate == "TGCR":
+            fed_data = fed_model.get_tri_party_general_collateral_rate()
+        elif rate == "BGCR":
+            fed_data = fed_model.get_broad_general_collateral_rate()
+        elif rate == "SOFR":
+            fed_data = fed_model.get_secured_overnight_financing_rate()
+        else:
+            raise ValueError(
+                "Rate must be one of 'EFFR', 'OBFR', 'TGCR', 'BGCR' or 'SOFR'."
+            )
+
+        fed_data = fed_data.loc[self._start_date : self._end_date]
+
+        fed_data = fed_data.round(rounding if rounding else self._rounding)
+
+        return fed_data
```

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/fred_model.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fixedincome/helpers.py` & `financetoolkit-1.9.1/financetoolkit/fixedincome/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/fundamentals_model.py` & `financetoolkit-1.9.1/financetoolkit/fundamentals_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,14 +477,24 @@
             f"{ticker}?period={period}&apikey={api_key}"
         )
         analyst_estimates = helpers.get_financial_data(url=url, sleep_timer=sleep_timer)
 
         try:
             analyst_estimates = analyst_estimates.drop("symbol", axis=1)
 
+            # One day is deducted from the date because it could be that
+            # the date is reported as 2023-07-01 while the data is about the
+            # second quarter of 2023. This usually happens when companies
+            # have a different financial year than the calendar year. It doesn't
+            # matter for others that are correctly reporting since 2023-06-31
+            # minus one day is still 2023
+            analyst_estimates["date"] = pd.to_datetime(
+                analyst_estimates["date"]
+            ) - pd.offsets.Day(1)
+
             if quarter:
                 analyst_estimates["date"] = pd.to_datetime(
                     analyst_estimates["date"]
                 ).dt.to_period("Q")
             else:
                 analyst_estimates["date"] = pd.to_datetime(
                     analyst_estimates["date"].astype(str)
@@ -589,15 +599,14 @@
             )
         except ValueError as error:
             print(
                 f"Not able to convert DataFrame to float64 and int due to {error}. This could result in"
                 "issues when values are zero and is predominantly relevant for "
                 "ratio calculations."
             )
-
         analyst_estimates_total.columns = pd.PeriodIndex(
             analyst_estimates_total.columns, freq="Q" if quarter else "Y"
         )
 
         analyst_estimates_total = analyst_estimates_total.sort_index(axis=1).truncate(
             before=start_date, axis=1
         )
```

### Comparing `financetoolkit-1.9.0/financetoolkit/helpers.py` & `financetoolkit-1.9.1/financetoolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/historical_model.py` & `financetoolkit-1.9.1/financetoolkit/historical_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/altman_model.py` & `financetoolkit-1.9.1/financetoolkit/models/altman_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/dupont_model.py` & `financetoolkit-1.9.1/financetoolkit/models/dupont_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/enterprise_model.py` & `financetoolkit-1.9.1/financetoolkit/models/enterprise_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/growth_model.py` & `financetoolkit-1.9.1/financetoolkit/models/growth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/helpers.py` & `financetoolkit-1.9.1/financetoolkit/models/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/intrinsic_model.py` & `financetoolkit-1.9.1/financetoolkit/models/intrinsic_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/models_controller.py` & `financetoolkit-1.9.1/financetoolkit/models/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/piotroski_model.py` & `financetoolkit-1.9.1/financetoolkit/models/piotroski_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/models/wacc_model.py` & `financetoolkit-1.9.1/financetoolkit/models/wacc_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/normalization/balance.csv` & `financetoolkit-1.9.1/financetoolkit/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/normalization/cash.csv` & `financetoolkit-1.9.1/financetoolkit/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/normalization/income.csv` & `financetoolkit-1.9.1/financetoolkit/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/normalization_model.py` & `financetoolkit-1.9.1/financetoolkit/normalization_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/binomial_trees_model.py` & `financetoolkit-1.9.1/financetoolkit/options/binomial_trees_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/black_scholes_model.py` & `financetoolkit-1.9.1/financetoolkit/options/black_scholes_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/greeks_model.py` & `financetoolkit-1.9.1/financetoolkit/options/greeks_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/helpers.py` & `financetoolkit-1.9.1/financetoolkit/options/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/options_controller.py` & `financetoolkit-1.9.1/financetoolkit/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/options/options_model.py` & `financetoolkit-1.9.1/financetoolkit/options/options_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/performance/helpers.py` & `financetoolkit-1.9.1/financetoolkit/performance/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/performance/performance_controller.py` & `financetoolkit-1.9.1/financetoolkit/performance/performance_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/performance/performance_model.py` & `financetoolkit-1.9.1/financetoolkit/performance/performance_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/efficiency_model.py` & `financetoolkit-1.9.1/financetoolkit/ratios/efficiency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/liquidity_model.py` & `financetoolkit-1.9.1/financetoolkit/ratios/liquidity_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/profitability_model.py` & `financetoolkit-1.9.1/financetoolkit/ratios/profitability_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/ratios_controller.py` & `financetoolkit-1.9.1/financetoolkit/ratios/ratios_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/solvency_model.py` & `financetoolkit-1.9.1/financetoolkit/ratios/solvency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/ratios/valuation_model.py` & `financetoolkit-1.9.1/financetoolkit/ratios/valuation_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/cvar_model.py` & `financetoolkit-1.9.1/financetoolkit/risk/cvar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/evar_model.py` & `financetoolkit-1.9.1/financetoolkit/risk/evar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/garch_model.py` & `financetoolkit-1.9.1/financetoolkit/risk/garch_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/helpers.py` & `financetoolkit-1.9.1/financetoolkit/risk/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/risk_controller.py` & `financetoolkit-1.9.1/financetoolkit/risk/risk_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/risk_model.py` & `financetoolkit-1.9.1/financetoolkit/risk/risk_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/risk/var_model.py` & `financetoolkit-1.9.1/financetoolkit/risk/var_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/breadth_model.py` & `financetoolkit-1.9.1/financetoolkit/technicals/breadth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/helpers.py` & `financetoolkit-1.9.1/financetoolkit/technicals/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/momentum_model.py` & `financetoolkit-1.9.1/financetoolkit/technicals/momentum_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/statistic_model.py` & `financetoolkit-1.9.1/financetoolkit/technicals/statistic_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/technicals_controller.py` & `financetoolkit-1.9.1/financetoolkit/technicals/technicals_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -3131,14 +3131,117 @@
                 lag=lag,
                 rounding=rounding if rounding else self._rounding,
                 axis="index",
             )
 
         return triangular_moving_average.round(rounding if rounding else self._rounding)
 
+    @handle_errors
+    def get_support_resistance_levels(
+        self,
+        sensitivity: float = 0.05,
+        period: str = "daily",
+        close_column: str = "Adj Close",
+        window: int = 14,
+        rounding: int | None = None,
+    ) -> pd.Series | pd.DataFrame:
+        """
+        Retrieves the support and resistance levels for the specified period and assets.
+
+        The Support and Resistance Levels are price levels where the price tends to stop and reverse.
+
+        - Support Levels: These are the valleys where the price tends to stop going down and may start to go up.
+        Think of support levels as "floors" that the price has trouble falling below.
+        - Resistance Levels: These are the peaks where the price tends to stop going up and may start to go down.
+        Think of resistance levels as "ceilings" that the price has trouble breaking through.
+
+        It does so by:
+
+        - Looking for Peaks and Valleys: The function looks at the stock prices and finds the high points
+        (peaks) and low points (valleys) over time.
+        - Grouping Similar Peaks and Valleys: Sometimes, prices will stop at similar points multiple times.
+        The function groups these similar peaks and valleys together to identify key resistance and
+        support levels.
+
+        Args:
+            sensitivity (float, optional): The sensitivity parameter to determine the significance of the peaks
+                and valleys. A higher sensitivity value will result in fewer support and resistance levels
+                being identified. Defaults to 0.05.
+            period (str, optional): The time period to consider for historical data.
+                Can be "daily", "weekly", "quarterly", or "yearly". Defaults to "daily".
+            close_column (str, optional): The column name for closing prices in the historical data.
+                Defaults to "Adj Close".
+            window (int, optional): Number of periods for calculating support and resistance levels.
+                The number of periods (time intervals) over which to calculate the support and resistance levels.
+                Defaults to 14.
+            rounding (int | None, optional): The number of decimals to round the results to.
+                If None, the rounding value specified during the initialization of the Toolkit instance will be used.
+                Defaults to None.
+
+        Returns:
+           pd.DataFrame: The support and resistance levels for each asset.
+
+        Raises:
+            ValueError: If the specified `period` is not one of the valid options.
+
+        Notes:
+        - The method retrieves historical data based on the specified `period` and calculates the
+          support and resistance levels for each asset in the Toolkit instance.
+
+        As an example:
+
+        ```python
+        from financetoolkit import Toolkit
+
+        toolkit = Toolkit(tickers=["AAPL", "MSFT"])
+
+        support_resistance_levels = toolkit.technicals.get_support_resistance_levels()
+        ```
+        """
+        if period not in [
+            "intraday",
+            "daily",
+            "weekly",
+            "monthly",
+            "quarterly",
+            "yearly",
+        ]:
+            raise ValueError(
+                "Period must be intraday, daily, weekly, monthly, quarterly, or yearly."
+            )
+        if period == "intraday":
+            if self._historical_data[period].empty:
+                raise ValueError(
+                    "Please define the 'intraday_period' parameter when initializing the Toolkit."
+                )
+            close_column = "Close"
+
+        historical_data = self._historical_data[period]
+
+        support_resistance_levels = {}
+
+        for ticker in historical_data[close_column].columns:
+            support_resistance_levels[
+                ticker
+            ] = overlap_model.get_support_resistance_levels(
+                prices=historical_data[close_column][ticker],
+                window=window,
+                sensitivity=sensitivity,
+            )
+
+        support_resistance_levels_df = (
+            pd.concat(support_resistance_levels, axis=1)
+            .swaplevel(1, 0, axis=1)
+            .sort_index(axis=1)
+        )
+
+        return support_resistance_levels_df.round(
+            rounding if rounding else self._rounding
+        )
+
     def collect_volatility_indicators(
         self,
         period: str = "daily",
         window: int = 14,
         close_column: str = "Adj Close",
         rounding: int | None = None,
         growth: bool = False,
```

### Comparing `financetoolkit-1.9.0/financetoolkit/technicals/volatility_model.py` & `financetoolkit-1.9.1/financetoolkit/technicals/volatility_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.9.0/financetoolkit/toolkit_controller.py` & `financetoolkit-1.9.1/financetoolkit/toolkit_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -3025,16 +3025,29 @@
                 for ticker in self._tickers
                 if ticker not in self._invalid_tickers
             ]
 
         income_statement = self._income_statement
 
         if trailing:
+            # This is a special case where the trailing period does not make sense
+            # for the Weighted Average Shares and Weighted Average Shares Diluted.
+            weighted_average_shares = income_statement.loc[
+                :, ["Weighted Average Shares", "Weighted Average Shares Diluted"], :
+            ]
+
+            # The rolling window is calculated for the rest of the income statement.
             income_statement = self._income_statement.T.rolling(trailing).sum().T
 
+            # The Weighted Average Shares and Weighted Average Shares Diluted should
+            # not be summed up but rather kept equal to the current value.
+            income_statement.loc[
+                weighted_average_shares.index
+            ] = weighted_average_shares
+
         if growth:
             self._income_statement_growth = _calculate_growth(
                 income_statement,
                 lag=lag,
                 rounding=rounding if rounding else self._rounding,
                 axis="columns",
             )
```

### Comparing `financetoolkit-1.9.0/pyproject.toml` & `financetoolkit-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.9.0"
+version = "1.9.1"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
```

### Comparing `financetoolkit-1.9.0/PKG-INFO` & `financetoolkit-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.9.0
+Version: 1.9.1
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/projects/financetoolkit
 License: MIT
 Keywords: Finance,Toolkit,Financial,Analysis,Fundamental,Technical,Quantitative,Database,Equities,Currencies,Economics,ETFs,Funds,Indices,Moneymarkets,Commodities,Options
 Author: Jeroen Bouma
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -134,14 +134,17 @@
 
 # a Technical example
 ichimoku_cloud = companies.technicals.get_ichimoku_cloud()
 
 # a Fixed Income example
 corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
 
+# a Fixed Income example
+corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
+
 # an Economics example
 unemployment_rates = companies.economics.get_unemployment_rate()
 ````
 
 Generally, the functions return a DataFrame with a multi-index in which all tickers, in this case Apple and Microsoft, are presented. To keep things manageable for this README, I select just Apple but in essence the list of tickers can be endless as I've seen DataFrames with thousands of tickers. The filtering is done through `.loc['AAPL']` and `.xs('AAPL', level=1, axis=1)` based on whether it's fundamental data or historical data respectively.
 
 ### Obtaining Historical Data
@@ -281,17 +284,17 @@
 |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
 | 2024-04-19 | 0.0518 | 0.0532 | 0.0561 | 0.0594 | 0.0678 | 0.0804 | 0.1385 |
 | 2024-04-22 | 0.0517 | 0.0532 | 0.056  | 0.0593 | 0.0671 | 0.0793 | 0.1377 |
 | 2024-04-23 | 0.0514 | 0.0528 | 0.0556 | 0.0589 | 0.066  | 0.0777 | 0.1364 |
 | 2024-04-24 | 0.0518 | 0.0531 | 0.0559 | 0.0592 | 0.0664 | 0.0778 | 0.1361 |
 | 2024-04-25 | 0.0524 | 0.0537 | 0.0564 | 0.0598 | 0.0673 | 0.079  | 0.1368 |
 
-And below Effective Yields, Option-Adjusted Spreads (OAS), Yield to Worst and Total Returns are plotted over time for the different maturity periods.
+And below a variety of Fixed Income metrics are shown all acquired from the Fixed Income module.
 
-![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/816cf251-4152-4341-a08e-a36268f5f721)
+![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/dfe2a819-87d8-46be-892c-f90663bc177d)
 
 ### Understanding Key Economic Indicators
 
 Get insights for 60+ countries into key economic indicators such as the Consumer Price Index (CPI), Gross Domestic Product (GDP), Unemployment Rates and 3-month and 10-year Government Interest Rates. This is done through the `economics` module and can be used as a standalone module as well by using `from financetoolkit import Economics`. For example see a selection of the countries below:
 
 |      |   Colombia |   United States |   Sweden |   Japan |   Germany |
 |:-----|-----------:|----------------:|---------:|--------:|----------:|
@@ -301,14 +304,15 @@
 | 2020 |     0.1586 |          0.0809 |   0.0848 |  0.0278 |    0.0362 |
 | 2021 |     0.1381 |          0.0537 |   0.0889 |  0.0282 |    0.0358 |
 | 2022 |     0.1122 |          0.0365 |   0.0748 |  0.026  |    0.0307 |
 
 And below these Unemployment Rates are plotted over time:
 
 ![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
+![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
 
 # Core Functionality and Metrics
 
 The Finance Toolkit has the ability to collect 30+ years of financial statements and calculate 150+ financial metrics. The following list shows all of the available functionality and metrics.
 
 Each ratio and indicator has a corresponding function that can be called directly for example `ratios.get_return_on_equity` or `technicals.get_relative_strength_index`. However, there are also functions that collect multiple ratios or indicators at once such as `ratios.collect_profitability_ratios`. These functions are useful when you want to collect a large amount of ratios or indicators at once.
 
@@ -2575,14 +2579,231 @@
 
 </details>
 
 ## Fixed Income
 
 The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
 
+<details>
+    <summary><b>Bond Valuations</b></summary>
+The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
+
+All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_present_value()
+```
+
+> **Bond Statistics**
+
+The bond statistics contains a variety of different metrics to evaluate a bond. These include:
+
+- **Par Value:** The face value of the bond.
+- **Coupon Rate:** The annual coupon rate (in decimal).
+- **Years to Maturity:** The number of years until the bond matures.
+- **Yield to Maturity:** The yield to maturity of the bond (in decimal).
+- **Frequency:** The number of coupon payments per year.
+- **Present Value:** The present value of the bond.
+- **Current Yield:** The annual coupon payment divided by the bond price.
+- **Effective Yield:** The return on a bond that has its interest payments (or coupons) reinvested at the same rate by the bondholder.
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+- **DV01:** The dollar value of a 0.01% change in yield to maturity.
+- **Convexity:** The second derivative of the bond price with respect to the yield to maturity.
+
+It gives a complete overview of the bond's performance. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_statistics) and an example below which shows the bond statistics for six different bonds using this functionality.
+
+|                     |   Bond 1 |   Bond 2 |   Bond 3 |    Bond 4 |   Bond 5 |   Bond 6 |
+|:--------------------|---------:|---------:|---------:|----------:|---------:|---------:|
+| Par Value           | 100      | 250      |  50      | 1000      |  85      | 320      |
+| Coupon Rate         |   0.05   |   0.02   |   0.075  |    0      |   0.15   |   0.015  |
+| Years to Maturity   |   5      |  10      |   2      |   10      |   3      |   1      |
+| Yield to Maturity   |   0.08   |   0.021  |   0.03   |    0      |   0.16   |   0.04   |
+| Frequency           |   1      |   1      |   4      |    1      |   2      |  12      |
+| Present Value       |  88.0219 | 247.766  |  54.3518 | 1000      |  83.0353 | 312.171  |
+| Current Yield       |   0.0568 |   0.0202 |   0.069  |    0      |   0.1535 |   0.0154 |
+| Effective Yield     |   0.05   |   0.02   |   0.0771 |    0      |   0.1556 |   0.0151 |
+| Macaulay's Duration |   4.5116 |   9.1576 |   1.8849 |   10      |   2.5667 |   0.9932 |
+| Modified Duration   |   4.1774 |   8.9693 |   1.8709 |   10      |   2.3766 |   0.9899 |
+| Effective Duration  |   4.0677 |   8.5181 |   1.8477 |    9.4713 |   2.2952 |   0.9844 |
+| Dollar Duration     |   3.677  |  22.2228 |   1.0168 |  100      |   1.9734 |   3.0902 |
+| DV01                |   0.0004 |   0.0022 |   0      |    0.01   |   0.0001 |   0      |
+| Convexity           |  22.4017 |  93.7509 |   4.0849 |  110      |   7.0923 |   1.0662 |
+
+> **Present Value**
+
+The bond price is the present value of the bond's future cash flows. It is calculated by discounting the bond's coupon payments and principal repayment to the present value using the bond's yield to maturity. The present value is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_price).
+
+> **Duration**
+
+The bond duration is a measure of the bond's sensitivity to changes in interest rates. It is the weighted average of the bond's cash flows, where the weights are the present value of each cash flow divided by the bond's price. It is possible to calculate the following durations:
+
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+
+The duration values are depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_duration).
+
+> **Yield to Maturity**
+
+The Yield to Maturity (YTM) is the total return anticipated on a bond if it is held until it matures. It is the internal rate of return of an investment in a bond if the investor holds the bond until maturity and receives all payments as scheduled. The yield to maturity is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_yield_to_maturity).
+
+</details>
+
+<details>
+    <summary><b>Derivative Valuations</b></summary>
+The Derivative Valuations section contains a variety of models that can be used to value derivative instruments such as Swaptions. These models include the Black Model and the Bachelier Model.
+
+All derivative valuations can be called by using `get_` to get a single valuation. E.g. `get_derivative_price`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_derivative_price(model_type="black")
+```
+
+> **Black Model**
+
+The Black Model is a mathematical model used to calculate the price of European-style options. It is based on the Black-Scholes model but is used for interest rate options. The Black Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+> **Bachelier Model**
+
+The Bachelier Model is a mathematical model used to calculate the price of European-style options. It is based on the normal distribution and is used for interest rate options as opposed to the Black model which uses a log-normal distribution. The Bachelier Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+</details>
+
+<details>
+    <summary><b>Central Banks</b></summary>
+
+The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
+
+All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_european_central_bank_rates()
+```
+
+> **Main Refinancing Operations**
+
+The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+
+> **Marginal Lending Facility**
+
+The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Deposit Facility**
+
+The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Euribor Rates**
+
+The Euro Interbank Offered Rate (Euribor) is a daily reference rate based on the averaged interest rates at which Eurozone banks offer to lend unsecured funds to other banks in the euro wholesale money market. It is widely used as the base rate for a variety of financial products, including mortgages, savings accounts, and derivatives. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_euribor_rates).
+
+> **Effective Federal Funds Rate**
+
+The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Overnight Bank Funding Rate**
+
+The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Tri-Party General Collateral Rate**
+
+The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Broad General Collateral Rate**
+
+The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Secured Overnight Financing Rate (SOFR)**
+
+The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+</details>
+
+<details>
+    <summary><b>Government Bonds</b></summary>
+
+It is possible to view both short-term (3-month) and long-term (10-year) interest rates for each of the available countries. These rates relate to the interest rates at which countries issue government bonds and are used as a benchmark for other interest rates in the economy. For example, the German government bond yield is an overall indicator of the European economy.
+
+These interest rates can be obtained with `get_government_bond_yield`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_government_bond_yield()
+```
+
+> **Long Term Interest Rates (10 year)**
+
+Long-term interest rates refer to government bonds maturing in ten years. Rates are mainly determined by the price charged by the lender, the risk from the borrower and the fall in the capital value. Long-term interest rates are generally averages of daily rates, measured as a percentage. These interest rates are implied by the prices at which the government bonds are traded on financial markets, not the interest rates at which the loans were issued.
+
+In all cases, they refer to bonds whose capital repayment is guaranteed by governments. Long-term interest rates are one of the determinants of business investment. Low long term interest rates encourage investment in new equipment and high interest rates discourage it. Investment is, in turn, a major source of economic growth. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+> **Short Term Interest Rates (3 month)**
+
+Short-term interest rates are the rates at which short-term borrowings are effected between financial institutions or the rate at which short-term government paper is issued or traded in the market. Short-term interest rates are generally averages of daily rates, measured as a percentage.
+
+Short-term interest rates are based on three-month money market rates where available. Typical standardised names are “money market rate” and “treasury bill rate”. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+</details>
+
+<details>
+    <summary><b>Corporate Bonds</b></summary>
+
+The Corporate Bonds section features the widely used ICE BofA benchmarks which include option-adjusted spreads, effective yields and the total returns. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All corporate bond metrics can be called by using `get_` to get a single metric. E.g. `get_ice_bofa_option_adjusted_spread` or `get_ice_bofa_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_ice_bofa_option_adjusted_spread()
+```
+
+> **Option-Adjusted Spread (OAS)**
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_option_adjusted_spread).
+
+> **Effective Yield**
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_effective_yield).
+
+> **Total Return**
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_total_return).
+
+> **Yield to Worst**
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_yield_to_worst).
+
+</details>
+
+## Fixed Income
+
+The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
+
 <details>
     <summary><b>Bond Valuations</b></summary>
 The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
 
 All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
 
 ```python
```

