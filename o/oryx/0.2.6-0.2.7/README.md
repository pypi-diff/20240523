# Comparing `tmp/oryx-0.2.6.tar.gz` & `tmp/oryx-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oryx-0.2.6.tar", max compression
+gzip compressed data, was "oryx-0.2.7.tar", max compression
```

## Comparing `oryx-0.2.6.tar` & `oryx-0.2.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11357 2023-12-20 15:58:36.518131 oryx-0.2.6/LICENSE
--rw-r--r--   0        0        0      760 2023-12-20 15:58:36.518369 oryx-0.2.6/oryx/__init__.py
--rw-r--r--   0        0        0      879 2023-12-20 15:58:36.518538 oryx-0.2.6/oryx/bijectors/__init__.py
--rw-r--r--   0        0        0     1859 2023-12-20 15:58:36.518729 oryx-0.2.6/oryx/core/__init__.py
--rw-r--r--   0        0        0      838 2023-12-20 15:58:36.518892 oryx-0.2.6/oryx/core/interpreters/__init__.py
--rw-r--r--   0        0        0    58079 2023-12-20 15:58:36.519104 oryx-0.2.6/oryx/core/interpreters/harvest.py
--rw-r--r--   0        0        0    25106 2023-12-20 15:58:36.519246 oryx-0.2.6/oryx/core/interpreters/harvest_test.py
--rw-r--r--   0        0        0      877 2023-12-20 15:58:36.519417 oryx-0.2.6/oryx/core/interpreters/inverse/__init__.py
--rw-r--r--   0        0        0     3779 2023-12-20 15:58:36.519531 oryx-0.2.6/oryx/core/interpreters/inverse/bijector_extensions.py
--rw-r--r--   0        0        0     2369 2023-12-20 15:58:36.519625 oryx-0.2.6/oryx/core/interpreters/inverse/bijector_extensions_test.py
--rw-r--r--   0        0        0    12936 2023-12-20 15:58:36.519772 oryx-0.2.6/oryx/core/interpreters/inverse/core.py
--rw-r--r--   0        0        0     9396 2023-12-20 15:58:36.519920 oryx-0.2.6/oryx/core/interpreters/inverse/custom_inverse.py
--rw-r--r--   0        0        0     5583 2023-12-20 15:58:36.520085 oryx-0.2.6/oryx/core/interpreters/inverse/custom_inverse_test.py
--rw-r--r--   0        0        0    12927 2023-12-20 15:58:36.520219 oryx-0.2.6/oryx/core/interpreters/inverse/inverse_test.py
--rw-r--r--   0        0        0     8756 2024-01-18 19:44:34.129713 oryx-0.2.6/oryx/core/interpreters/inverse/rules.py
--rw-r--r--   0        0        0     6300 2023-12-20 15:58:36.520472 oryx-0.2.6/oryx/core/interpreters/inverse/slice.py
--rw-r--r--   0        0        0     3587 2023-12-20 15:58:36.520565 oryx-0.2.6/oryx/core/interpreters/inverse/slice_test.py
--rw-r--r--   0        0        0     4619 2023-12-20 15:58:36.520684 oryx-0.2.6/oryx/core/interpreters/log_prob.py
--rw-r--r--   0        0        0     4414 2023-12-20 15:58:36.520796 oryx-0.2.6/oryx/core/interpreters/log_prob_test.py
--rw-r--r--   0        0        0    14002 2023-12-20 15:58:36.520920 oryx-0.2.6/oryx/core/interpreters/propagate.py
--rw-r--r--   0        0        0     8637 2023-12-20 15:58:36.521039 oryx-0.2.6/oryx/core/interpreters/propagate_test.py
--rw-r--r--   0        0        0     2635 2023-12-20 15:58:36.521170 oryx-0.2.6/oryx/core/kwargs_util.py
--rw-r--r--   0        0        0     3709 2023-12-20 15:58:36.521257 oryx-0.2.6/oryx/core/kwargs_util_test.py
--rw-r--r--   0        0        0     1538 2023-12-20 15:58:36.521379 oryx-0.2.6/oryx/core/ppl/__init__.py
--rw-r--r--   0        0        0    13084 2023-12-20 15:58:36.521505 oryx-0.2.6/oryx/core/ppl/effect_handler.py
--rw-r--r--   0        0        0     5572 2023-12-20 15:58:36.521628 oryx-0.2.6/oryx/core/ppl/effect_handler_test.py
--rw-r--r--   0        0        0     2421 2023-12-20 15:58:36.521720 oryx-0.2.6/oryx/core/ppl/plate_util.py
--rw-r--r--   0        0        0    19210 2023-12-20 15:58:36.521801 oryx-0.2.6/oryx/core/ppl/transformations.py
--rw-r--r--   0        0        0    15091 2023-12-20 15:58:36.521984 oryx-0.2.6/oryx/core/ppl/transformations_test.py
--rw-r--r--   0        0        0     8233 2023-12-20 15:58:36.522110 oryx-0.2.6/oryx/core/primitive.py
--rw-r--r--   0        0        0     1000 2023-12-20 15:58:36.522207 oryx-0.2.6/oryx/core/primitive_test.py
--rw-r--r--   0        0        0     1185 2023-12-20 15:58:36.522282 oryx-0.2.6/oryx/core/pytree.py
--rw-r--r--   0        0        0     1158 2023-12-20 15:58:36.522360 oryx-0.2.6/oryx/core/serialize.py
--rw-r--r--   0        0        0     1771 2023-12-20 15:58:36.522451 oryx-0.2.6/oryx/core/serialize_test.py
--rw-r--r--   0        0        0     1313 2023-12-20 15:58:36.522617 oryx-0.2.6/oryx/core/state/__init__.py
--rw-r--r--   0        0        0     5147 2023-12-20 15:58:36.522743 oryx-0.2.6/oryx/core/state/api.py
--rw-r--r--   0        0        0    10727 2023-12-20 15:58:36.522872 oryx-0.2.6/oryx/core/state/function.py
--rw-r--r--   0        0        0     7829 2023-12-20 15:58:36.522989 oryx-0.2.6/oryx/core/state/function_test.py
--rw-r--r--   0        0        0     5940 2023-12-20 15:58:36.523111 oryx-0.2.6/oryx/core/state/module.py
--rw-r--r--   0        0        0     5208 2023-12-20 15:58:36.523226 oryx-0.2.6/oryx/core/state/registrations.py
--rw-r--r--   0        0        0     2419 2023-12-20 15:58:36.523299 oryx-0.2.6/oryx/core/state/registrations_test.py
--rw-r--r--   0        0        0     3903 2023-12-20 15:58:36.523379 oryx-0.2.6/oryx/core/trace_util.py
--rw-r--r--   0        0        0      891 2023-12-20 15:58:36.523523 oryx-0.2.6/oryx/distributions/__init__.py
--rw-r--r--   0        0        0     4642 2023-12-20 15:58:36.523644 oryx-0.2.6/oryx/distributions/distribution_extensions.py
--rw-r--r--   0        0        0     9042 2023-12-20 15:58:36.523753 oryx-0.2.6/oryx/distributions/distribution_extensions_test.py
--rw-r--r--   0        0        0    25803 2023-12-20 15:58:36.523966 oryx-0.2.6/oryx/examples/notebooks/a_tour_of_oryx.ipynb
--rw-r--r--   0        0        0    35465 2023-12-20 15:58:36.524140 oryx-0.2.6/oryx/examples/notebooks/probabilistic_programming.ipynb
--rw-r--r--   0        0        0      776 2023-12-20 15:58:36.524292 oryx-0.2.6/oryx/experimental/__init__.py
--rw-r--r--   0        0        0     3551 2023-12-20 15:58:36.524419 oryx-0.2.6/oryx/experimental/autoconj/addn.py
--rw-r--r--   0        0        0     2513 2023-12-20 15:58:36.524512 oryx-0.2.6/oryx/experimental/autoconj/addn_test.py
--rw-r--r--   0        0        0     6447 2023-12-20 15:58:36.524640 oryx-0.2.6/oryx/experimental/autoconj/canonicalize.py
--rw-r--r--   0        0        0    10757 2023-12-20 15:58:36.524781 oryx-0.2.6/oryx/experimental/autoconj/canonicalize_test.py
--rw-r--r--   0        0        0     9416 2023-12-20 15:58:36.524912 oryx-0.2.6/oryx/experimental/autoconj/einsum.py
--rw-r--r--   0        0        0     3499 2023-12-20 15:58:36.525007 oryx-0.2.6/oryx/experimental/autoconj/einsum_test.py
--rw-r--r--   0        0        0      775 2023-12-20 15:58:36.525126 oryx-0.2.6/oryx/experimental/matching/__init__.py
--rw-r--r--   0        0        0    27479 2023-12-20 15:58:36.525241 oryx-0.2.6/oryx/experimental/matching/jax_rewrite.py
--rw-r--r--   0        0        0     7764 2023-12-20 15:58:36.525370 oryx-0.2.6/oryx/experimental/matching/jax_rewrite_test.py
--rw-r--r--   0        0        0    25942 2023-12-20 15:58:36.525488 oryx-0.2.6/oryx/experimental/matching/matcher.py
--rw-r--r--   0        0        0    10758 2023-12-20 15:58:36.525617 oryx-0.2.6/oryx/experimental/matching/matcher_test.py
--rw-r--r--   0        0        0    13413 2023-12-20 15:58:36.525738 oryx-0.2.6/oryx/experimental/matching/rules.py
--rw-r--r--   0        0        0     5064 2023-12-20 15:58:36.525879 oryx-0.2.6/oryx/experimental/matching/rules_test.py
--rw-r--r--   0        0        0      999 2023-12-20 15:58:36.526047 oryx-0.2.6/oryx/experimental/mcmc/__init__.py
--rw-r--r--   0        0        0     8073 2023-12-20 15:58:36.526165 oryx-0.2.6/oryx/experimental/mcmc/kernels.py
--rw-r--r--   0        0        0     4231 2023-12-20 15:58:36.526275 oryx-0.2.6/oryx/experimental/mcmc/kernels_test.py
--rw-r--r--   0        0        0     1308 2023-12-20 15:58:36.526356 oryx-0.2.6/oryx/experimental/mcmc/utils.py
--rw-r--r--   0        0        0     1633 2023-12-20 15:58:36.526473 oryx-0.2.6/oryx/experimental/nn/__init__.py
--rw-r--r--   0        0        0    20112 2023-12-20 15:58:36.526575 oryx-0.2.6/oryx/experimental/nn/base.py
--rw-r--r--   0        0        0     4633 2023-12-20 15:58:36.526696 oryx-0.2.6/oryx/experimental/nn/base_test.py
--rw-r--r--   0        0        0     3453 2023-12-20 15:58:36.526783 oryx-0.2.6/oryx/experimental/nn/combinator.py
--rw-r--r--   0        0        0     7708 2023-12-20 15:58:36.526897 oryx-0.2.6/oryx/experimental/nn/combinator_test.py
--rw-r--r--   0        0        0     6870 2023-12-20 15:58:36.527005 oryx-0.2.6/oryx/experimental/nn/convolution.py
--rw-r--r--   0        0        0     6387 2023-12-20 15:58:36.527113 oryx-0.2.6/oryx/experimental/nn/convolution_test.py
--rw-r--r--   0        0        0     4413 2023-12-20 15:58:36.527221 oryx-0.2.6/oryx/experimental/nn/core.py
--rw-r--r--   0        0        0     9196 2023-12-20 15:58:36.527339 oryx-0.2.6/oryx/experimental/nn/core_test.py
--rw-r--r--   0        0        0     1748 2023-12-20 15:58:36.527440 oryx-0.2.6/oryx/experimental/nn/function.py
--rw-r--r--   0        0        0    16874 2023-12-20 15:58:36.527508 oryx-0.2.6/oryx/experimental/nn/function_test.py
--rw-r--r--   0        0        0     5050 2023-12-20 15:58:36.527638 oryx-0.2.6/oryx/experimental/nn/normalization.py
--rw-r--r--   0        0        0     8423 2023-12-20 15:58:36.527766 oryx-0.2.6/oryx/experimental/nn/normalization_test.py
--rw-r--r--   0        0        0     4295 2023-12-20 15:58:36.527881 oryx-0.2.6/oryx/experimental/nn/pooling.py
--rw-r--r--   0        0        0     7503 2023-12-20 15:58:36.527986 oryx-0.2.6/oryx/experimental/nn/pooling_test.py
--rw-r--r--   0        0        0     2410 2023-12-20 15:58:36.528059 oryx-0.2.6/oryx/experimental/nn/reshape.py
--rw-r--r--   0        0        0     2531 2023-12-20 15:58:36.528138 oryx-0.2.6/oryx/experimental/nn/reshape_test.py
--rw-r--r--   0        0        0      954 2023-12-20 15:58:36.528282 oryx-0.2.6/oryx/experimental/optimizers/__init__.py
--rw-r--r--   0        0        0     9921 2023-12-20 15:58:36.528405 oryx-0.2.6/oryx/experimental/optimizers/optix.py
--rw-r--r--   0        0        0     6634 2023-12-20 15:58:36.528526 oryx-0.2.6/oryx/experimental/optimizers/optix_test.py
--rw-r--r--   0        0        0      668 2023-12-20 15:58:36.528658 oryx-0.2.6/oryx/internal/__init__.py
--rw-r--r--   0        0        0      739 2023-12-20 15:58:36.528753 oryx-0.2.6/oryx/internal/test_util.py
--rw-r--r--   0        0        0     1693 2023-12-20 15:58:36.528884 oryx-0.2.6/oryx/tools/build_oryx_docs.py
--rw-r--r--   0        0        0      703 2023-12-20 15:58:36.529007 oryx-0.2.6/oryx/util/__init__.py
--rw-r--r--   0        0        0     1416 2023-12-20 15:58:36.529083 oryx-0.2.6/oryx/util/summary.py
--rw-r--r--   0        0        0     1910 2023-12-20 15:58:36.529160 oryx-0.2.6/oryx/util/summary_test.py
--rw-r--r--   0        0        0     1304 2024-01-18 20:35:44.240986 oryx-0.2.6/oryx/version.py
--rw-r--r--   0        0        0      448 2024-01-18 20:35:44.241253 oryx-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 oryx-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-20 15:58:36.518131 oryx-0.2.7/LICENSE
+-rw-r--r--   0        0        0      760 2024-05-16 20:40:18.227830 oryx-0.2.7/oryx/__init__.py
+-rw-r--r--   0        0        0      879 2024-05-16 20:40:18.227922 oryx-0.2.7/oryx/bijectors/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-16 20:40:18.227994 oryx-0.2.7/oryx/core/__init__.py
+-rw-r--r--   0        0        0      838 2024-05-16 20:40:18.228073 oryx-0.2.7/oryx/core/interpreters/__init__.py
+-rw-r--r--   0        0        0    64096 2024-05-16 20:40:18.228266 oryx-0.2.7/oryx/core/interpreters/harvest.py
+-rw-r--r--   0        0        0    26477 2024-05-16 20:40:18.228403 oryx-0.2.7/oryx/core/interpreters/harvest_test.py
+-rw-r--r--   0        0        0      877 2024-05-16 20:40:18.228574 oryx-0.2.7/oryx/core/interpreters/inverse/__init__.py
+-rw-r--r--   0        0        0     3779 2024-05-16 20:40:18.228675 oryx-0.2.7/oryx/core/interpreters/inverse/bijector_extensions.py
+-rw-r--r--   0        0        0     2369 2024-05-16 20:40:18.228747 oryx-0.2.7/oryx/core/interpreters/inverse/bijector_extensions_test.py
+-rw-r--r--   0        0        0    12936 2024-05-16 20:40:18.228934 oryx-0.2.7/oryx/core/interpreters/inverse/core.py
+-rw-r--r--   0        0        0     9396 2024-05-16 20:40:18.229088 oryx-0.2.7/oryx/core/interpreters/inverse/custom_inverse.py
+-rw-r--r--   0        0        0     5583 2024-05-16 20:40:18.229174 oryx-0.2.7/oryx/core/interpreters/inverse/custom_inverse_test.py
+-rw-r--r--   0        0        0    12927 2024-05-16 20:40:18.229302 oryx-0.2.7/oryx/core/interpreters/inverse/inverse_test.py
+-rw-r--r--   0        0        0     8754 2024-05-16 20:40:18.229444 oryx-0.2.7/oryx/core/interpreters/inverse/rules.py
+-rw-r--r--   0        0        0     6300 2024-05-16 20:40:18.231172 oryx-0.2.7/oryx/core/interpreters/inverse/slice.py
+-rw-r--r--   0        0        0     3587 2024-05-16 20:40:18.231292 oryx-0.2.7/oryx/core/interpreters/inverse/slice_test.py
+-rw-r--r--   0        0        0     4619 2024-05-16 20:40:18.231367 oryx-0.2.7/oryx/core/interpreters/log_prob.py
+-rw-r--r--   0        0        0     4414 2024-05-16 20:40:18.231449 oryx-0.2.7/oryx/core/interpreters/log_prob_test.py
+-rw-r--r--   0        0        0    14159 2024-05-16 20:40:18.231602 oryx-0.2.7/oryx/core/interpreters/propagate.py
+-rw-r--r--   0        0        0     8637 2024-05-16 20:40:18.231973 oryx-0.2.7/oryx/core/interpreters/propagate_test.py
+-rw-r--r--   0        0        0     2635 2024-05-16 20:40:18.232076 oryx-0.2.7/oryx/core/kwargs_util.py
+-rw-r--r--   0        0        0     3709 2024-05-16 20:40:18.232161 oryx-0.2.7/oryx/core/kwargs_util_test.py
+-rw-r--r--   0        0        0     1538 2024-05-16 20:40:18.232233 oryx-0.2.7/oryx/core/ppl/__init__.py
+-rw-r--r--   0        0        0    13268 2024-05-16 20:40:18.232384 oryx-0.2.7/oryx/core/ppl/effect_handler.py
+-rw-r--r--   0        0        0     5572 2024-05-16 20:40:18.232520 oryx-0.2.7/oryx/core/ppl/effect_handler_test.py
+-rw-r--r--   0        0        0     2421 2024-05-16 20:40:18.232625 oryx-0.2.7/oryx/core/ppl/plate_util.py
+-rw-r--r--   0        0        0    19210 2024-05-16 20:40:18.232740 oryx-0.2.7/oryx/core/ppl/transformations.py
+-rw-r--r--   0        0        0    15091 2024-05-16 20:40:18.232950 oryx-0.2.7/oryx/core/ppl/transformations_test.py
+-rw-r--r--   0        0        0     8233 2024-05-16 20:40:18.233136 oryx-0.2.7/oryx/core/primitive.py
+-rw-r--r--   0        0        0     1000 2024-05-16 20:40:18.233478 oryx-0.2.7/oryx/core/primitive_test.py
+-rw-r--r--   0        0        0     1185 2024-05-16 20:40:18.233544 oryx-0.2.7/oryx/core/pytree.py
+-rw-r--r--   0        0        0     1158 2024-05-16 20:40:18.233607 oryx-0.2.7/oryx/core/serialize.py
+-rw-r--r--   0        0        0     1771 2024-05-16 20:40:18.233678 oryx-0.2.7/oryx/core/serialize_test.py
+-rw-r--r--   0        0        0     1313 2024-05-16 20:40:18.233758 oryx-0.2.7/oryx/core/state/__init__.py
+-rw-r--r--   0        0        0     5147 2024-05-16 20:40:18.233833 oryx-0.2.7/oryx/core/state/api.py
+-rw-r--r--   0        0        0    10727 2024-05-16 20:40:18.233957 oryx-0.2.7/oryx/core/state/function.py
+-rw-r--r--   0        0        0     7829 2024-05-16 20:40:18.234038 oryx-0.2.7/oryx/core/state/function_test.py
+-rw-r--r--   0        0        0     5940 2024-05-16 20:40:18.234124 oryx-0.2.7/oryx/core/state/module.py
+-rw-r--r--   0        0        0     5208 2024-05-16 20:40:18.234203 oryx-0.2.7/oryx/core/state/registrations.py
+-rw-r--r--   0        0        0     2419 2024-05-16 20:40:18.234269 oryx-0.2.7/oryx/core/state/registrations_test.py
+-rw-r--r--   0        0        0     3903 2024-05-16 20:40:18.234340 oryx-0.2.7/oryx/core/trace_util.py
+-rw-r--r--   0        0        0      891 2024-05-16 20:40:18.234406 oryx-0.2.7/oryx/distributions/__init__.py
+-rw-r--r--   0        0        0     4642 2024-05-16 20:40:18.234489 oryx-0.2.7/oryx/distributions/distribution_extensions.py
+-rw-r--r--   0        0        0     9042 2024-05-16 20:40:18.234678 oryx-0.2.7/oryx/distributions/distribution_extensions_test.py
+-rw-r--r--   0        0        0    25768 2024-05-16 20:40:18.234809 oryx-0.2.7/oryx/examples/notebooks/a_tour_of_oryx.ipynb
+-rw-r--r--   0        0        0    35465 2024-05-23 18:21:11.181498 oryx-0.2.7/oryx/examples/notebooks/probabilistic_programming.ipynb
+-rw-r--r--   0        0        0      776 2024-05-16 20:40:18.234934 oryx-0.2.7/oryx/experimental/__init__.py
+-rw-r--r--   0        0        0     3551 2024-05-16 20:40:18.235017 oryx-0.2.7/oryx/experimental/autoconj/addn.py
+-rw-r--r--   0        0        0     2513 2024-05-16 20:40:18.235092 oryx-0.2.7/oryx/experimental/autoconj/addn_test.py
+-rw-r--r--   0        0        0     6447 2024-05-16 20:40:18.235175 oryx-0.2.7/oryx/experimental/autoconj/canonicalize.py
+-rw-r--r--   0        0        0    10757 2024-05-16 20:40:18.235303 oryx-0.2.7/oryx/experimental/autoconj/canonicalize_test.py
+-rw-r--r--   0        0        0     9416 2024-05-16 20:40:18.235438 oryx-0.2.7/oryx/experimental/autoconj/einsum.py
+-rw-r--r--   0        0        0     3499 2024-05-16 20:40:18.235512 oryx-0.2.7/oryx/experimental/autoconj/einsum_test.py
+-rw-r--r--   0        0        0      775 2024-05-16 20:40:18.235588 oryx-0.2.7/oryx/experimental/matching/__init__.py
+-rw-r--r--   0        0        0    27479 2024-05-16 20:40:18.235695 oryx-0.2.7/oryx/experimental/matching/jax_rewrite.py
+-rw-r--r--   0        0        0     7764 2024-05-16 20:40:18.235792 oryx-0.2.7/oryx/experimental/matching/jax_rewrite_test.py
+-rw-r--r--   0        0        0    25942 2024-05-16 20:40:18.235908 oryx-0.2.7/oryx/experimental/matching/matcher.py
+-rw-r--r--   0        0        0    10758 2024-05-16 20:40:18.236043 oryx-0.2.7/oryx/experimental/matching/matcher_test.py
+-rw-r--r--   0        0        0    13413 2024-05-16 20:40:18.236171 oryx-0.2.7/oryx/experimental/matching/rules.py
+-rw-r--r--   0        0        0     5064 2024-05-16 20:40:18.236253 oryx-0.2.7/oryx/experimental/matching/rules_test.py
+-rw-r--r--   0        0        0      999 2024-05-16 20:40:18.236329 oryx-0.2.7/oryx/experimental/mcmc/__init__.py
+-rw-r--r--   0        0        0     8073 2024-05-16 20:40:18.236408 oryx-0.2.7/oryx/experimental/mcmc/kernels.py
+-rw-r--r--   0        0        0     4231 2024-05-16 20:40:18.236489 oryx-0.2.7/oryx/experimental/mcmc/kernels_test.py
+-rw-r--r--   0        0        0     1308 2024-05-16 20:40:18.236561 oryx-0.2.7/oryx/experimental/mcmc/utils.py
+-rw-r--r--   0        0        0     1633 2024-05-16 20:40:18.236633 oryx-0.2.7/oryx/experimental/nn/__init__.py
+-rw-r--r--   0        0        0    20112 2024-05-23 18:21:11.181786 oryx-0.2.7/oryx/experimental/nn/base.py
+-rw-r--r--   0        0        0     4633 2024-05-16 20:40:18.236825 oryx-0.2.7/oryx/experimental/nn/base_test.py
+-rw-r--r--   0        0        0     3453 2024-05-16 20:40:18.236913 oryx-0.2.7/oryx/experimental/nn/combinator.py
+-rw-r--r--   0        0        0     7708 2024-05-16 20:40:18.236996 oryx-0.2.7/oryx/experimental/nn/combinator_test.py
+-rw-r--r--   0        0        0     6870 2024-05-16 20:40:18.237075 oryx-0.2.7/oryx/experimental/nn/convolution.py
+-rw-r--r--   0        0        0     6387 2024-05-16 20:40:18.237149 oryx-0.2.7/oryx/experimental/nn/convolution_test.py
+-rw-r--r--   0        0        0     4413 2024-05-16 20:40:18.237237 oryx-0.2.7/oryx/experimental/nn/core.py
+-rw-r--r--   0        0        0     9196 2024-05-16 20:40:18.237352 oryx-0.2.7/oryx/experimental/nn/core_test.py
+-rw-r--r--   0        0        0     1748 2024-05-16 20:40:18.237429 oryx-0.2.7/oryx/experimental/nn/function.py
+-rw-r--r--   0        0        0    16874 2024-05-16 20:40:18.237513 oryx-0.2.7/oryx/experimental/nn/function_test.py
+-rw-r--r--   0        0        0     5050 2024-05-16 20:40:18.237602 oryx-0.2.7/oryx/experimental/nn/normalization.py
+-rw-r--r--   0        0        0     8423 2024-05-16 20:40:18.237737 oryx-0.2.7/oryx/experimental/nn/normalization_test.py
+-rw-r--r--   0        0        0     4295 2024-05-16 20:40:18.237812 oryx-0.2.7/oryx/experimental/nn/pooling.py
+-rw-r--r--   0        0        0     7503 2024-05-16 20:40:18.237880 oryx-0.2.7/oryx/experimental/nn/pooling_test.py
+-rw-r--r--   0        0        0     2410 2024-05-16 20:40:18.237947 oryx-0.2.7/oryx/experimental/nn/reshape.py
+-rw-r--r--   0        0        0     2531 2024-05-16 20:40:18.238007 oryx-0.2.7/oryx/experimental/nn/reshape_test.py
+-rw-r--r--   0        0        0      954 2024-05-16 20:40:18.238077 oryx-0.2.7/oryx/experimental/optimizers/__init__.py
+-rw-r--r--   0        0        0     9921 2024-05-16 20:40:18.238192 oryx-0.2.7/oryx/experimental/optimizers/optix.py
+-rw-r--r--   0        0        0     6634 2024-05-16 20:40:18.238263 oryx-0.2.7/oryx/experimental/optimizers/optix_test.py
+-rw-r--r--   0        0        0      668 2024-05-16 20:40:18.238324 oryx-0.2.7/oryx/internal/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-16 20:40:18.238402 oryx-0.2.7/oryx/internal/test_util.py
+-rw-r--r--   0        0        0     1693 2024-05-16 20:40:18.238476 oryx-0.2.7/oryx/tools/build_oryx_docs.py
+-rw-r--r--   0        0        0      703 2024-05-16 20:40:18.238541 oryx-0.2.7/oryx/util/__init__.py
+-rw-r--r--   0        0        0     1416 2024-05-16 20:40:18.238602 oryx-0.2.7/oryx/util/summary.py
+-rw-r--r--   0        0        0     1910 2024-05-16 20:40:18.238663 oryx-0.2.7/oryx/util/summary_test.py
+-rw-r--r--   0        0        0     1304 2024-05-23 18:21:11.181961 oryx-0.2.7/oryx/version.py
+-rw-r--r--   0        0        0      448 2024-05-23 18:21:11.182105 oryx-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 oryx-0.2.7/PKG-INFO
```

### Comparing `oryx-0.2.6/LICENSE` & `oryx-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oryx-0.2.6/oryx/__init__.py` & `oryx-0.2.7/oryx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/bijectors/__init__.py` & `oryx-0.2.7/oryx/bijectors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/__init__.py` & `oryx-0.2.7/oryx/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/__init__.py` & `oryx-0.2.7/oryx/core/interpreters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/harvest.py` & `oryx-0.2.7/oryx/core/interpreters/harvest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -53,14 +53,21 @@
 same `(tag, name)` appears more than once. Another option is `'append'`, in
 which all sows of the same name will be appended into a growing array. Finally,
 there is `'clobber'`, where only the final sown value for a given `(tag, name)`
 will be returned. The final optional argument for `sow` is `key`, which will
 automatically be tied-in to the output of `sow` to introduce a fake
 data-dependence. By default, it is `None`.
 
+## `sow_cond`
+
+`sow_cond` is a variant of `sow`, that takes an additional positional argument,
+`pred`. It supports a single `mode` `'cond_clobber'`, which is like `clobber`,
+but sows values conditionally on `pred`, falling back on zeros if no sow took
+place. This allows reaping values from loop iterations besides the final one.
+
 ## `harvest`
 
 `harvest` is a function transformation that augments the behaviors of `sow`s
 in the function body. Recall, that by default, `sow`s act as identity functions
 and do not affect the semantics of a function. Harvesting `f` produces a
 function that can take advantage of `sow`s present in its execution. `harvest`
 is a function that takes in a function `f` and a string `tag`. `harvest` will
@@ -235,16 +242,62 @@
       value is sown with the same name and tag, it will replace this value 3.
       `'append'` - sown values of the same name and tag are appended to a
       growing list. Append mode assumes some ordering on the values being sown
       defined by data-dependence.
     key: an optional JAX value that will be tied into the sown value.
 
   Returns:
-    The original `value` that was passed in.
+    The original `value` that was passed in, or a planted value.
   """
+  if mode == 'cond_clobber':
+    raise ValueError("For 'cond_clobber' mode, use `sow_cond`.'")
+  return _sow(value, tag=tag, name=name, mode=mode, key=key)
+
+
+def sow_cond(
+    value,
+    pred,
+    *,
+    tag: Hashable,
+    name: str,
+    mode: str = 'cond_clobber',
+    key=None,
+):
+  """Marks a value, alongside a predicate, with a name and a tag.
+
+  The predicate determines whether the value is to be clobbered in this loop
+  iteration -- if it's reaped but never clobbered, the value will be full of
+  zeros.
+
+  Args:
+    value: A JAX value to be tagged and named.
+    pred: Whether to sow the value.
+    tag: a string representing the tag of the sown value.
+    name: a string representing the name to sow the value with.
+    mode: The mode by which to sow the value. There are three options: 1.
+      `'strict'` - if another value is sown with the same name and tag in the
+      same context, harvest will throw an error. 2. `'clobber'` - if another is
+      value is sown with the same name and tag, it will replace this value 3.
+      `'append'` - sown values of the same name and tag are appended to a
+      growing list. Append mode assumes some ordering on the values being sown
+      defined by data-dependence.
+    key: an optional JAX value that will be tied into the sown value.
+
+  Returns:
+    The original `value` that was passed in, or a planted value.
+  """
+  if mode != 'cond_clobber':
+    raise ValueError("`sow_cond` only supports 'cond_clobber' mode.")
+  return _sow(value, tag=tag, name=name, mode=mode, key=key, pred=pred)[0]
+
+
+def _sow(value, *, tag, name, mode, key=None, pred=None):
+  assert (pred is not None) == (mode == 'cond_clobber')
+  if pred is not None:
+    value = value, pred
   value = tree_util.tree_map(jax_core.raise_as_much_as_possible, value)
   if key is not None:
     value = prim.tie_in(key, value)
   flat_args, in_tree = tree_util.tree_flatten(value)
   out_flat = sow_p.bind(*flat_args, name=name, tag=tag, mode=mode, tree=in_tree)
   return tree_util.tree_unflatten(in_tree, out_flat)
 
@@ -437,15 +490,15 @@
 @dataclasses.dataclass
 class HarvestContext:
   """A context that handles `sow`s and `nest`s in a `HarvestTrace`."""
   settings: HarvestSettings
 
   def process_sow(self, *values, name, tag, mode, tree):
     """Handles a `sow` primitive in a `HarvestTrace`."""
-    if mode not in {'strict', 'append', 'clobber'}:
+    if mode not in {'strict', 'append', 'clobber', 'cond_clobber'}:
       raise ValueError(f'Invalid mode: {mode}')
     if tag != self.settings.tag:
       if self.settings.exclusive:
         return values
       return sow_p.bind(*values, name=name, tag=tag, tree=tree, mode=mode)
     if (self.settings.allowlist is not None and
         name not in self.settings.allowlist):
@@ -489,14 +542,15 @@
 
 reap_custom_rules = {}
 
 
 @dataclasses.dataclass
 class Reap:
   value: Any
+  pred: Any
   metadata: Dict[str, Any]
 
 
 @dataclasses.dataclass
 class ReapContext(HarvestContext):
   """Contains the settings and storage for the current trace in the stack."""
   settings: HarvestSettings
@@ -504,21 +558,33 @@
 
   def get_custom_rule(self, primitive):
     return reap_custom_rules.get(primitive)
 
   def handle_sow(self, *values, name, tag, tree, mode):
     """Stores a sow in the reaps dictionary."""
     del tag
-    if name in self.reaps:
-      raise ValueError(f'Variable has already been reaped: {name}')
+    if prev_reap := self.reaps.get(name):
+      if {mode, prev_reap.metadata['mode']} - {'clobber', 'cond_clobber'}:
+        raise ValueError(f'Variable has already been reaped: {name}')
     avals = tree_util.tree_unflatten(
         tree,
         [jax_core.raise_to_shaped(jax_core.get_aval(v)) for v in values])
-    self.reaps[name] = Reap(
-        tree_util.tree_unflatten(tree, values), dict(mode=mode, aval=avals))
+    vals = tree_util.tree_unflatten(tree, values)
+    pred = None
+    if mode == 'cond_clobber':
+      avals, _ = avals
+      vals, pred = vals
+      if prev_reap:
+        if prev_reap.metadata['mode'] == 'clobber':
+          vals = lax.cond(pred, lambda: vals, lambda: prev_reap.value)
+        elif prev_reap.metadata['mode'] == 'cond_clobber':
+          vals = lax.cond(pred, lambda: vals, lambda: prev_reap.value)
+          pred = pred | prev_reap.pred
+    metadata = dict(mode=mode, aval=avals)
+    self.reaps[name] = Reap(vals, pred, metadata)
     return values
 
   def reap_higher_order_primitive(self, trace, call_primitive, f, tracers,
                                   params, is_map):
     """Wraps the inner function with a reap trace."""
     name = jax_util.wrap_name(params.pop('name', f.__name__), 'reap')
     vals = [t.val for t in tracers]
@@ -533,36 +599,42 @@
         assert all(out_axis == 0 for out_axis in out_axes)
         out_tree, _ = aux()
         return (0,) * out_tree.num_leaves
 
       params = dict(params, out_axes_thunk=new_out_axes_thunk)
     out_flat = call_primitive.bind(f, *vals, name=name, **params)
     out_tree, metadata = aux()
-    out_vals, reaps = tree_util.tree_unflatten(out_tree, out_flat)
+    out_vals, reaps, preds = tree_util.tree_unflatten(out_tree, out_flat)
     out_tracers = jax_util.safe_map(trace.pure, out_vals)
     reap_tracers = tree_util.tree_map(trace.pure, reaps)
-    return out_tracers, reap_tracers, metadata
+    pred_tracers = tree_util.tree_map(trace.pure, preds)
+    return out_tracers, reap_tracers, pred_tracers, metadata
 
   def process_nest(self, trace, f, *tracers, scope, name, **params):
-    out_tracers, reap_tracers, _ = self.reap_higher_order_primitive(
+    out_tracers, reap_tracers, _, _ = self.reap_higher_order_primitive(
         trace, nest_p, f, tracers, dict(params, name=name, scope=scope), False)
     tag = self.settings.tag
     if reap_tracers:
       flat_reap_tracers, reap_tree = tree_util.tree_flatten(reap_tracers)
       trace.process_primitive(
           sow_p, flat_reap_tracers,
           dict(name=scope, tag=tag, tree=reap_tree, mode='strict'))
     return out_tracers
 
   def process_higher_order_primitive(self, trace, call_primitive, f, tracers,
                                      params, is_map):
-    out_tracers, reap_tracers, metadata = self.reap_higher_order_primitive(
-        trace, call_primitive, f, tracers, params, is_map)
+    out_tracers, reap_tracers, pred_tracers, metadata = (
+        self.reap_higher_order_primitive(
+            trace, call_primitive, f, tracers, params, is_map
+        )
+    )
     tag = self.settings.tag
     for k, v in reap_tracers.items():
+      if metadata[k]['mode'] == 'cond_clobber':
+        v = (v, pred_tracers[k])
       flat_reap_tracers, reap_tree = tree_util.tree_flatten(v)
       trace.process_primitive(
           sow_p, flat_reap_tracers,
           dict(name=k, tag=tag, tree=reap_tree, mode=metadata[k]['mode']))
     return out_tracers
 
   def process_custom_jvp_call(self, trace, primitive, fun, jvp, tracers, *,
@@ -579,18 +651,22 @@
       out_tracers = jax_util.safe_map(trace.full_raise, outs)
       yield out_tracers, (None, None)
 
     jvp, aux2 = _jvp_subtrace(jvp, trace.main)
     out_flat = primitive.bind(fun, jvp, *vals_in, symbolic_zeros=symbolic_zeros)
     fst, (out_tree, metadata) = lu.merge_linear_aux(aux1, aux2)
     if fst:
-      out, reaps = tree_util.tree_unflatten(out_tree, out_flat)
-      out_tracers, reap_tracers = tree_util.tree_map(trace.pure, (out, reaps))
+      out, reaps, preds = tree_util.tree_unflatten(out_tree, out_flat)
+      out_tracers, reap_tracers, pred_tracers = tree_util.tree_map(
+          trace.pure, (out, reaps, preds)
+      )
       tag = context.settings.tag
       for k, v in reap_tracers.items():
+        if metadata[k]['mode'] == 'cond_clobber':
+          v = (v, pred_tracers[k])
         flat_reap_tracers, reap_tree = tree_util.tree_flatten(v)
         trace.process_primitive(
             sow_p, flat_reap_tracers,
             dict(name=k, tag=tag, tree=reap_tree, mode=metadata[k]['mode']))
     else:
       out_tracers = jax_util.safe_map(trace.pure, out_flat)
     return out_tracers
@@ -617,18 +693,22 @@
     fwd, aux2 = _fwd_subtrace(fwd, trace.main)
     bwd_ = reap_function(lu.wrap_init(bwd), trace.main, context.settings, True)
     bwd = reap_wrapper_drop_aux(bwd_, trace).call_wrapped
     out_flat = primitive.bind(fun, fwd, bwd, *vals_in, out_trees=out_trees,
                               symbolic_zeros=symbolic_zeros)
     fst, (out_tree, metadata) = lu.merge_linear_aux(aux1, aux2)
     if fst:
-      out, reaps = tree_util.tree_unflatten(out_tree, out_flat)
-      out_tracers, reap_tracers = tree_util.tree_map(trace.pure, (out, reaps))
+      out, reaps, preds = tree_util.tree_unflatten(out_tree, out_flat)
+      out_tracers, reap_tracers, pred_tracers = tree_util.tree_map(
+          trace.pure, (out, reaps, preds)
+      )
       tag = context.settings.tag
       for k, v in reap_tracers.items():
+        if metadata[k]['mode'] == 'cond_clobber':
+          v = (v, pred_tracers[k])
         flat_reap_tracers, reap_tree = tree_util.tree_flatten(v)
         trace.process_primitive(
             sow_p, flat_reap_tracers,
             dict(name=k, tag=tag, tree=reap_tree, mode=metadata[k]['mode']))
     else:
       out_tracers = jax_util.safe_map(trace.pure, out_flat)
     return out_tracers
@@ -644,54 +724,57 @@
     bwd_transform = lambda bwd: bwd
     return vals, todo, bwd_transform
 
 
 @lu.transformation
 def reap_function(main: jax_core.MainTrace, settings: HarvestSettings,
                   return_metadata: bool, args: Iterable[Any]):
-  """A function transformation that returns reap values."""
+  """A function transformation that returns reap values and predicates."""
   trace = HarvestTrace(main, jax_core.cur_sublevel())
   in_tracers = jax_util.safe_map(trace.pure, args)
   context = ReapContext(settings, {})
   with trace_util.new_dynamic_context(main, context):
     ans = yield in_tracers, {}
     out_tracers = jax_util.safe_map(trace.full_raise, ans)
     reap_tracers = tree_util.tree_map(
         lambda x: tree_util.tree_map(trace.full_raise, x.value), context.reaps)
+    pred_tracers = tree_util.tree_map(
+        lambda x: trace.full_raise(x.pred), context.reaps)
     reap_metadata = tree_util.tree_map(lambda x: x.metadata, context.reaps)
     del main
-  out_values, reap_values = tree_util.tree_map(lambda x: x.val,
-                                               (out_tracers, reap_tracers))
+  out_values, reap_values, pred_values = tree_util.tree_map(
+      lambda x: x.val, (out_tracers, reap_tracers, pred_tracers)
+  )
   if return_metadata:
-    out = (out_values, reap_values, reap_metadata)
+    out = (out_values, reap_values, pred_values, reap_metadata)
   else:
-    out = (out_values, reap_values)
+    out = (out_values, reap_values, pred_values)
   yield out
 
 
 def reap_eval(
     f: lu.WrappedFun, trace: HarvestTrace,
     settings: HarvestSettings) -> Tuple[lu.WrappedFun, Callable[[], Any]]:
   f = reap_function(f, trace.main, settings, True)
   return reap_wrapper(f, trace)
 
 
 @lu.transformation_with_aux
 def reap_wrapper(trace: HarvestTrace, *args):
   del trace
-  out, reaps, metadata = yield (args,), {}
-  out_flat, out_tree = tree_util.tree_flatten((out, reaps))
+  out, reaps, preds, metadata = yield (args,), {}
+  out_flat, out_tree = tree_util.tree_flatten((out, reaps, preds))
   yield out_flat, (out_tree, metadata)
 
 
 @lu.transformation
 def reap_wrapper_drop_aux(trace: HarvestTrace, *args):
   del trace
-  out, reaps, _ = yield (args,), {}
-  out_flat, _ = tree_util.tree_flatten((out, reaps))
+  out, reaps, preds, _ = yield (args,), {}
+  out_flat, _ = tree_util.tree_flatten((out, reaps, preds))
   yield out_flat
 
 
 def call_and_reap(f,
                   *,
                   tag: Hashable,
                   allowlist: Optional[Iterable[str]] = None,
@@ -709,28 +792,56 @@
     exclusive: determines whether or not to execute in "exclusive" mode where
       other tags are removed during execution.
 
   Returns:
     A new function that executes the original and returns its sown values as
     an additional return value.
   """
+
+  def wrapped(*args, **kwargs):
+    out, reaps, preds = _call_and_reap(
+        f,
+        tag=tag,
+        allowlist=allowlist,
+        blocklist=blocklist,
+        exclusive=exclusive,
+    )(*args, **kwargs)
+
+    def select_from_pred(pred, value):
+      if pred is None:
+        return value
+      else:
+        return tree_util.tree_map(
+            lambda leaf: lax.select(pred, leaf, lax.zeros_like_array(leaf)),
+            value,
+        )
+
+    return out, tree_util.tree_map(
+        select_from_pred, preds, reaps, is_leaf=lambda x: x is None
+    )
+
+  return wrapped
+
+
+def _call_and_reap(f, *, tag, allowlist, blocklist, exclusive):
+  """Like call_and_reap but including predicates."""
   blocklist = frozenset(blocklist)
   if allowlist is not None:
     allowlist = frozenset(allowlist)
   settings = HarvestSettings(tag, blocklist, allowlist, exclusive)
 
   def wrapped(*args, **kwargs):
     fun = lu.wrap_init(f, kwargs)
     flat_args, in_tree = tree_util.tree_flatten(args)
     flat_fun, out_tree = api_util.flatten_fun_nokwargs(fun, in_tree)
     with jax_core.new_main(HarvestTrace) as main:
       flat_fun = reap_function(flat_fun, main, settings, False)
-      out_flat, reaps = flat_fun.call_wrapped(flat_args)
+      out_flat, reaps, preds = flat_fun.call_wrapped(flat_args)
       del main
-    return tree_util.tree_unflatten(out_tree(), out_flat), reaps
+    return tree_util.tree_unflatten(out_tree(), out_flat), reaps, preds
 
   return wrapped
 
 
 def reap(f,
          *,
          tag: Hashable,
@@ -762,16 +873,16 @@
         exclusive=exclusive)(*args, **kwargs)[1]
 
   return wrapped
 
 
 @lu.transformation_with_aux
 def _reap_metadata_wrapper(*args):
-  out, reaps, metadata = yield (args,), {}
-  yield (out, reaps), metadata
+  out, reaps, preds, metadata = yield (args,), {}
+  yield (out, reaps, preds), metadata
 
 
 def _get_harvest_metadata(closed_jaxpr, settings, *args):
   """Probes a jaxpr for metadata like its sown values."""
   fun = lu.wrap_init(jax_core.jaxpr_as_fun(closed_jaxpr))
   with jax_core.new_main(HarvestTrace) as main:
     settings = HarvestSettings(settings.tag, settings.blocklist,
@@ -785,16 +896,27 @@
         flat_args)
     pe.trace_to_jaxpr_final(flat_fun, in_avals)
     metadata = aux()
     out_tree()
   return metadata
 
 
+def _update_clobber_carry(carry_reaps, carry_preds, name, val, preds, mode):
+  if mode == 'cond_clobber':
+    carry_reaps[name], carry_preds[name] = lax.cond(
+        preds[name],
+        lambda val=val: (val, True),
+        lambda name=name: (carry_reaps[name], carry_preds[name]),
+    )
+  else:
+    carry_reaps[name] = val
+
+
 def _reap_scan_rule(trace: HarvestTrace, *tracers, length, reverse, jaxpr,
-                    num_consts, num_carry, linear, unroll):
+                    num_consts, num_carry, linear, unroll, _split_transpose):
   """Reaps the body of a scan to pull out `clobber` and `append` sows."""
 
   const_tracers, carry_tracers, xs_tracers = jax_util.split_list(
       tracers, [num_consts, num_carry])
   _, carry_avals, xs_avals = tree_util.tree_map(
       lambda x: x.aval, (const_tracers, carry_tracers, xs_tracers))
   const_vals, carry_vals, xs_vals = tree_util.tree_map(
@@ -805,130 +927,158 @@
   x_avals = [t.aval for t in x_tracers]
   x_vals = [t.val for t in x_tracers]
   metadata = _get_harvest_metadata(jaxpr, settings,
                                    *(const_vals + carry_vals + x_vals))
 
   reap_modes = collections.defaultdict(set)
   reap_carry_avals = {}
+  cond_carry_avals = {}
   for name, meta in metadata.items():
     mode = meta['mode']
     aval = meta['aval']
     if mode == 'strict':
       raise ValueError(f'Cannot use strict mode for \'{name}\' inside `scan`.')
     reap_modes[mode].add(name)
     if mode == 'clobber':
       reap_carry_avals[name] = aval
+      cond_carry_avals[name] = None
+    if mode == 'cond_clobber':
+      reap_carry_avals[name] = aval
+      cond_carry_avals[name] = jax_core.raise_to_shaped(jax_core.get_aval(True))
+
   body_fun = jax_core.jaxpr_as_fun(jaxpr)
 
-  reap_carry_flat_avals, _ = tree_util.tree_flatten(reap_carry_avals)
+  reap_carry_flat_avals = tree_util.tree_leaves(
+      (reap_carry_avals, cond_carry_avals)
+  )
 
   reap_carry_in_tree = tree_util.tree_structure(
-      ((carry_avals, reap_carry_avals), xs_avals))
+      ((carry_avals, reap_carry_avals, cond_carry_avals), xs_avals))
 
   def new_body(carry, x):
-    carry, _ = carry
+    carry, carry_reaps, carry_preds = carry
     all_values = const_vals + tree_util.tree_leaves((carry, x))
-    out, reaps = call_and_reap(
+    out, reaps, preds = _call_and_reap(
         body_fun,
         tag=settings.tag,
         allowlist=settings.allowlist,
         blocklist=settings.blocklist,
         exclusive=settings.exclusive)(*all_values)
     carry_out, y = jax_util.split_list(out, [num_carry])
-    carry_reaps = {
-        name: val
-        for name, val in reaps.items()
-        if name in reap_modes['clobber']
-    }
+    clobber_reap_modes = reap_modes['clobber'] | reap_modes['cond_clobber']
+    for name, val in reaps.items():
+      if name in clobber_reap_modes:
+        _update_clobber_carry(carry_reaps, carry_preds, name, val, preds, mode)
     xs_reaps = {
         name: val for name, val in reaps.items() if name in reap_modes['append']
     }
-    return (carry_out, carry_reaps), (y, xs_reaps)
+    return (carry_out, carry_reaps, carry_preds), (y, xs_reaps)
 
   new_body_jaxpr, consts, out_tree = lcf._initial_style_jaxpr(  # pylint: disable=protected-access
       new_body, reap_carry_in_tree,
       tuple(carry_avals + reap_carry_flat_avals + x_avals))
   dummy_reap_carry_vals = tree_util.tree_map(
-      lambda x: jnp.zeros(x.shape, x.dtype), reap_carry_flat_avals)
+      lambda x: jnp.zeros(x.shape, x.dtype),
+      reap_carry_flat_avals,
+  )
   out = lax.scan_p.bind(
       *(consts + carry_vals + dummy_reap_carry_vals + xs_vals),
       reverse=reverse,
       length=length,
       jaxpr=new_body_jaxpr,
       num_consts=len(consts),
       num_carry=len(carry_vals + dummy_reap_carry_vals),
       linear=(linear[:len(consts)] + (False,) * len(dummy_reap_carry_vals) +
               linear[len(consts):]),
-      unroll=unroll)
-  (carry_out,
-   carry_reaps), (ys, ys_reaps) = tree_util.tree_unflatten(out_tree, out)
-  (carry_out, carry_reaps), (ys, ys_reaps) = tree_util.tree_map(
-      trace.pure, ((carry_out, carry_reaps), (ys, ys_reaps)))
-  for k, v in {**carry_reaps, **ys_reaps}.items():
+      unroll=unroll,
+      _split_transpose=_split_transpose)
+  (carry_out, carry_reaps, carry_preds), (ys, ys_reaps) = (
+      tree_util.tree_unflatten(out_tree, out)
+  )
+  (carry_out, carry_reaps, carry_preds), (ys, ys_reaps) = tree_util.tree_map(
+      trace.pure, ((carry_out, carry_reaps, carry_preds), (ys, ys_reaps))
+  )
+  for k, v in carry_reaps.items():
+    mode = metadata[k]['mode']
+    _sow(v, tag=settings.tag, mode=mode, name=k, pred=carry_preds[k])
+  for k, v in ys_reaps.items():
     sow(v, tag=settings.tag, mode=metadata[k]['mode'], name=k)
   return carry_out + ys
 
 
 reap_custom_rules[lcf.scan_p] = _reap_scan_rule
 
 
 def _reap_while_rule(trace: HarvestTrace, *tracers, cond_jaxpr, body_jaxpr,
                      cond_nconsts, body_nconsts):
-  """Reaps the body of a while loop to get the reaps of the final iteration."""
+  """Reaps the body of a while loop to get the reaps of `clobber` sows."""
   cond_const_tracers, body_const_tracers, init_tracers = jax_util.split_list(
       tracers, [cond_nconsts, body_nconsts])
   _, init_avals = tree_util.tree_map(lambda x: x.aval,
                                      (body_const_tracers, init_tracers))
   cond_const_vals, body_const_vals, init_vals = tree_util.tree_map(
       lambda x: x.val, (cond_const_tracers, body_const_tracers, init_tracers))
   context = trace_util.get_dynamic_context(trace)
   settings = context.settings
   body_metadata = _get_harvest_metadata(body_jaxpr, settings,
                                         *(body_const_tracers + init_tracers))
+  reap_avals = {}
+  cond_avals = collections.defaultdict(lambda: None)
   for k, meta in body_metadata.items():
     mode = meta['mode']
-    if mode != 'clobber':
+    if mode not in ['clobber', 'cond_clobber']:
       raise ValueError(
-          f'Must use clobber mode for \'{k}\' inside of a `while_loop`.')
-  reap_avals = {k: v['aval'] for k, v in body_metadata.items()}
+          f"Must use clobber or cond_clobber mode for '{k}' inside of a"
+          ' `while_loop`.'
+      )
+    reap_avals[k] = meta['aval']
+    if mode == 'cond_clobber':
+      cond_avals[k] = jax_core.raise_to_shaped(jax_core.get_aval(True))
 
   cond_fun = jax_core.jaxpr_as_fun(cond_jaxpr)
   body_fun = jax_core.jaxpr_as_fun(body_jaxpr)
   reap_settings = dict(
       tag=settings.tag,
       allowlist=settings.allowlist,
       blocklist=settings.blocklist,
       exclusive=settings.exclusive)
 
-  def new_cond(carry, _):
+  def new_cond(carry, *_):
     return cond_fun(*(cond_const_vals + carry))
 
-  def new_body(carry, _):
-    carry, reaps = call_and_reap(body_fun,
-                                 **reap_settings)(*(body_const_vals + carry))
-    return (carry, reaps)
-
-  new_in_avals, new_in_tree = tree_util.tree_flatten((init_avals, reap_avals))
+  def new_body(carry, carry_reaps, carry_preds):
+    carry, reaps, preds = _call_and_reap(body_fun, **reap_settings)(
+        *(body_const_vals + carry)
+    )
+    for name, val in reaps.items():
+      mode = body_metadata[name]['mode']
+      _update_clobber_carry(carry_reaps, carry_preds, name, val, preds, mode)
+    return (carry, carry_reaps, carry_preds)
+
+  new_in_avals, new_in_tree = tree_util.tree_flatten(
+      (init_avals, reap_avals, cond_avals)
+  )
   new_cond_jaxpr, cond_consts, _ = lcf._initial_style_jaxpr(  # pylint: disable=protected-access
       new_cond, new_in_tree, tuple(new_in_avals))
   new_body_jaxpr, body_consts, out_tree = lcf._initial_style_jaxpr(  # pylint: disable=protected-access
       new_body, new_in_tree, tuple(new_in_avals))
   dummy_reap_vals = tree_util.tree_map(lambda x: jnp.zeros(x.shape, x.dtype),
-                                       reap_avals)
+                                       (reap_avals, cond_avals))
   new_in_vals = tree_util.tree_leaves((init_vals, dummy_reap_vals))
   out = lax.while_p.bind(
       *(cond_consts + body_consts + new_in_vals),
       cond_nconsts=len(cond_consts),
       body_nconsts=len(body_consts),
       cond_jaxpr=new_cond_jaxpr,
       body_jaxpr=new_body_jaxpr)
   out = jax_util.safe_map(trace.pure, out)
-  out, reaps = tree_util.tree_unflatten(out_tree, out)
+  out, reaps, preds = tree_util.tree_unflatten(out_tree, out)
   for k, v in reaps.items():
-    sow(v, name=k, tag=settings.tag, mode=body_metadata[k]['mode'])
+    mode = body_metadata[k]['mode']
+    _sow(v, name=k, tag=settings.tag, mode=mode, pred=preds[k])
   return out
 
 
 reap_custom_rules[lcf.while_p] = _reap_while_rule
 
 
 def _check_branch_metadata(branch_metadatas):
@@ -963,28 +1113,29 @@
       exclusive=settings.exclusive)
   branch_metadatas = tuple(
       _get_harvest_metadata(branch, settings, *ops_tracers)
       for branch in branches)
   _check_branch_metadata(branch_metadatas)
   branch_funs = tuple(map(jax_core.jaxpr_as_fun, branches))
   reaped_branches = tuple(
-      call_and_reap(f, **reap_settings) for f in branch_funs)
+      _call_and_reap(f, **reap_settings) for f in branch_funs)
   in_tree = tree_util.tree_structure(ops_avals)
   new_branch_jaxprs, consts, out_trees = (
       lcf._initial_style_jaxprs_with_common_consts(  # pylint: disable=protected-access
           reaped_branches, in_tree, ops_avals, lax.cond_p.name))
   out = lax.cond_p.bind(
       index_val,
       *(tuple(consts) + ops_vals),
       branches=tuple(new_branch_jaxprs),
       linear=(False,) * len(tuple(consts) + linear))
   out = jax_util.safe_map(trace.pure, out)
-  out, reaps = tree_util.tree_unflatten(out_trees[0], out)
+  out, reaps, preds = tree_util.tree_unflatten(out_trees[0], out)
   for k, v in reaps.items():
-    sow(v, name=k, tag=settings.tag, mode=branch_metadatas[0][k]['mode'])
+    mode = branch_metadatas[0][k]['mode']
+    _sow(v, name=k, tag=settings.tag, mode=mode, pred=preds[k])
   return out
 
 
 reap_custom_rules[lcf.cond_p] = _reap_cond_rule
 
 
 def _reap_checkpoint_rule(trace, *tracers, jaxpr, policy, prevent_cse,
@@ -997,29 +1148,30 @@
       tag=settings.tag,
       allowlist=settings.allowlist,
       blocklist=settings.blocklist,
       exclusive=settings.exclusive)
   closed_jaxpr = jax_core.ClosedJaxpr(jaxpr, ())
   reap_metadata = _get_harvest_metadata(closed_jaxpr, settings, *tracers)
   remat_fun = jax_core.jaxpr_as_fun(closed_jaxpr)
-  reaped_remat_fun = call_and_reap(remat_fun, **reap_settings)
+  reaped_remat_fun = _call_and_reap(remat_fun, **reap_settings)
   reap_jaxpr, consts, out_tree = lcf._initial_style_jaxpr(  # pylint: disable=protected-access
       reaped_remat_fun, tree_util.tree_structure(invals),
       tuple(t.aval for t in tracers))
   outvals = ad_checkpoint.remat_p.bind(
       *consts,
       *invals,
       jaxpr=reap_jaxpr.jaxpr,
       policy=policy,
       prevent_cse=prevent_cse,
       differentiated=differentiated)
   outvals = jax_util.safe_map(trace.pure, outvals)
-  out, reaps = tree_util.tree_unflatten(out_tree, outvals)
+  out, reaps, preds = tree_util.tree_unflatten(out_tree, outvals)
   for k, v in reaps.items():
-    sow(v, name=k, tag=settings.tag, mode=reap_metadata[k]['mode'])
+    mode = reap_metadata[k]['mode']
+    _sow(v, name=k, tag=settings.tag, mode=mode, pred=preds[k])
   return out
 
 
 reap_custom_rules[ad_checkpoint.remat_p] = _reap_checkpoint_rule
 
 
 @lu.cache
@@ -1036,15 +1188,16 @@
   return jaxpr, final_consts, out_avals
 
 
 def _calc_extra_inps(num_consts, params):
   in_shardings = (
       sharding_impls.UNSPECIFIED,) * num_consts + params['in_shardings']
   donated_invars = (False,) * num_consts + params['donated_invars']
-  return in_shardings, donated_invars
+  in_layouts = (None,) * num_consts + params['in_layouts']
+  return in_shardings, donated_invars, in_layouts
 
 
 def _reap_pjit_rule(trace, *tracers, **params):
   """Reap pjit rule."""
   if params['in_shardings'] and not any(
       sharding_impls.is_unspecified(i) for i in params['in_shardings']
   ):
@@ -1067,34 +1220,39 @@
       tag=settings.tag,
       allowlist=settings.allowlist,
       blocklist=settings.blocklist,
       exclusive=settings.exclusive)
   closed_jaxpr = params['jaxpr']
   reap_metadata = _get_harvest_metadata(closed_jaxpr, settings, *tracers)
   pjit_fun = jax_core.jaxpr_as_fun(closed_jaxpr)
-  reaped_pjit_fun = lu.wrap_init(call_and_reap(pjit_fun, **reap_settings))
+  reaped_pjit_fun = lu.wrap_init(_call_and_reap(pjit_fun, **reap_settings))
   in_tree = tree_util.tree_structure(invals)
   flat_fun, out_tree = api_util.flatten_fun_nokwargs(reaped_pjit_fun, in_tree)
 
   reap_jaxpr, final_consts, out_avals = _oryx_pjit_jaxpr(
       flat_fun, tuple(t.aval for t in tracers))
-  in_shardings, donated_invars = _calc_extra_inps(
+  in_shardings, donated_invars, in_layouts = _calc_extra_inps(
       len(final_consts), params)
 
-  new_params = {**params,
-                'jaxpr': reap_jaxpr,
-                'out_shardings': (sharding_impls.UNSPECIFIED,) * len(out_avals),
-                'in_shardings': in_shardings,
-                'donated_invars': donated_invars}
+  new_params = {
+      **params,
+      'jaxpr': reap_jaxpr,
+      'out_shardings': (sharding_impls.UNSPECIFIED,) * len(out_avals),
+      'in_shardings': in_shardings,
+      'donated_invars': donated_invars,
+      'in_layouts': in_layouts,
+      'out_layouts': (None,) * len(out_avals)
+  }
   outvals = pjit.pjit_p.bind(*final_consts, *invals, **new_params)
 
   outvals = jax_util.safe_map(trace.pure, outvals)
-  out, reaps = tree_util.tree_unflatten(out_tree(), outvals)
+  out, reaps, preds = tree_util.tree_unflatten(out_tree(), outvals)
   for k, v in reaps.items():
-    sow(v, name=k, tag=settings.tag, mode=reap_metadata[k]['mode'])
+    mode = reap_metadata[k]['mode']
+    _sow(v, name=k, tag=settings.tag, mode=mode, pred=preds[k])
   return out
 
 
 reap_custom_rules[pjit.pjit_p] = _reap_pjit_rule
 
 
 plant_custom_rules = {}
@@ -1113,16 +1271,20 @@
     return plant_custom_rules.get(primitive)
 
   def handle_sow(self, *values, name, tag, tree, mode):
     """Returns the value stored in the plants dictionary."""
     if name in self._already_planted:
       raise ValueError(f'Variable has already been planted: {name}')
     if name in self.plants:
-      self._already_planted.add(name)
-      return tree_util.tree_leaves(self.plants[name])
+      if not mode.endswith('clobber'):
+        self._already_planted.add(name)
+      if mode == 'cond_clobber':
+        return tree_util.tree_leaves((self.plants[name], True))
+      else:
+        return tree_util.tree_leaves(self.plants[name])
     return sow_p.bind(*values, name=name, tag=tag, mode=mode, tree=tree)
 
   def process_nest(self, trace, f, *tracers, scope, name, **params):
     return self.process_higher_order_primitive(
         trace, nest_p, f, tracers, dict(params, name=name, scope=scope), False)
 
   def process_higher_order_primitive(self, trace, call_primitive, f, tracers,
@@ -1267,15 +1429,15 @@
       del main
     return tree_util.tree_unflatten(out_tree(), out_flat)
 
   return wrapped
 
 
 def _plant_scan_rule(trace: HarvestTrace, *tracers, length, reverse, jaxpr,
-                     num_consts, num_carry, linear, unroll):
+                     num_consts, num_carry, linear, unroll, _split_transpose):
   """Injects values into a scan according to their sow mode."""
 
   const_tracers, carry_tracers, xs_tracers = jax_util.split_list(
       tracers, [num_consts, num_carry])
   carry_avals, xs_avals = tree_util.tree_map(lambda x: x.aval,
                                              (carry_tracers, xs_tracers))
   const_vals, carry_vals, xs_vals = tree_util.tree_map(
@@ -1295,33 +1457,33 @@
     aval = meta['aval']
     if mode == 'strict':
       raise ValueError(f'Cannot use strict mode for \'{name}\' inside `scan`.')
     plant_modes[mode].add(name)
     if mode == 'append' and name in plants:
       plant_xs_avals[name] = aval
   body_fun = jax_core.jaxpr_as_fun(jaxpr)
-  clobber_plants = {
+  all_clobber_plants = {
       name: value
       for name, value in plants.items()
-      if name in plant_modes['clobber']
+      if name in plant_modes['clobber'] | plant_modes['cond_clobber']
   }
   append_plants = {
       name: value
       for name, value in plants.items()
       if name in plant_modes['append']
   }
 
   plant_xs_flat_avals, _ = tree_util.tree_flatten(plant_xs_avals)
 
   plant_xs_in_tree = tree_util.tree_structure(
       (carry_avals, (xs_avals, plant_xs_avals)))
 
   def new_body(carry, x):
     x, plants = x
-    all_plants = {**plants, **clobber_plants}
+    all_plants = {**plants, **all_clobber_plants}
     all_values = const_vals + tree_util.tree_leaves((carry, x))
     out = plant(
         body_fun,
         tag=settings.tag,
         allowlist=settings.allowlist,
         blocklist=settings.blocklist,
         exclusive=settings.exclusive)(all_plants, *all_values)
@@ -1336,15 +1498,16 @@
       *(consts + carry_vals + xs_vals + plant_vals),
       reverse=reverse,
       length=length,
       jaxpr=new_body_jaxpr,
       num_consts=len(consts),
       num_carry=num_carry,
       linear=linear + (False,) * len(plant_vals),
-      unroll=unroll)
+      unroll=unroll,
+      _split_transpose=_split_transpose)
   return out
 
 
 plant_custom_rules[lcf.scan_p] = _plant_scan_rule
 
 
 def _plant_while_rule(trace: HarvestTrace, *tracers, cond_jaxpr, body_jaxpr,
@@ -1357,17 +1520,19 @@
       lambda x: x.val, (cond_const_tracers, body_const_tracers, init_tracers))
   context = trace_util.get_dynamic_context(trace)
   settings = context.settings
   body_metadata = _get_harvest_metadata(body_jaxpr, settings,
                                         *(body_const_tracers + init_tracers))
   for k, meta in body_metadata.items():
     mode = meta['mode']
-    if mode != 'clobber':
+    if mode not in ['clobber', 'cond_clobber']:
       raise ValueError(
-          f'Must use clobber mode for \'{k}\' inside of a `while_loop`.')
+          f"Must use clobber or cond_clobber mode for '{k}' inside of a"
+          ' `while_loop`.'
+      )
 
   body_fun = jax_core.jaxpr_as_fun(body_jaxpr)
   plant_settings = dict(
       tag=settings.tag,
       allowlist=settings.allowlist,
       blocklist=settings.blocklist,
       exclusive=settings.exclusive)
@@ -1494,22 +1659,26 @@
   planted_pjit_fun = lu.wrap_init(functools.partial(
       plant(pjit_fun, **plant_settings), plants))
   in_tree = tree_util.tree_structure(invals)
   flat_fun, _ = api_util.flatten_fun_nokwargs(planted_pjit_fun, in_tree)
 
   planted_jaxpr, final_consts, out_avals = _oryx_pjit_jaxpr(
       flat_fun, tuple(t.aval for t in tracers))
-  in_shardings, donated_invars = _calc_extra_inps(
+  in_shardings, donated_invars, in_layouts = _calc_extra_inps(
       len(final_consts), params)
 
-  new_params = {**params,
-                'jaxpr': planted_jaxpr,
-                'out_shardings': (sharding_impls.UNSPECIFIED,) * len(out_avals),
-                'in_shardings': in_shardings,
-                'donated_invars': donated_invars}
+  new_params = {
+      **params,
+      'jaxpr': planted_jaxpr,
+      'out_shardings': (sharding_impls.UNSPECIFIED,) * len(out_avals),
+      'in_shardings': in_shardings,
+      'donated_invars': donated_invars,
+      'in_layouts': in_layouts,
+      'out_layouts': (None,) * len(out_avals),
+  }
   outvals = pjit.pjit_p.bind(*final_consts, *invals, **new_params)
 
   return jax_util.safe_map(trace.pure, outvals)
 
 
 plant_custom_rules[pjit.pjit_p] = _plant_pjit_rule
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/harvest_test.py` & `oryx-0.2.7/oryx/core/interpreters/harvest_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,14 +44,15 @@
 from oryx.core import trace_util
 from oryx.core.interpreters import harvest
 from oryx.internal import test_util
 
 config.update('jax_traceback_filtering', 'off')
 
 sow = harvest.sow
+sow_cond = harvest.sow_cond
 reap = harvest.reap
 call_and_reap = harvest.call_and_reap
 plant = harvest.plant
 nest = harvest.nest
 
 variable = functools.partial(sow, tag='variable')
 harvest_variables = functools.partial(harvest.harvest, tag='variable')
@@ -678,15 +679,15 @@
     def body(carry, x):
       x = variable(x + carry, name='x', mode='append')
       return x, x
 
     def f(init):
       return lax.scan(body, init, jnp.arange(5.))
 
-    (carry, out), variables = harvest_variables(f)({}, 1.)
+    (carry, out), variables = (harvest_variables(f))({}, 1.)
     true_out = jnp.array([1., 2., 4., 7., 11.])
     np.testing.assert_allclose(carry, 11.)
     np.testing.assert_allclose(out, true_out)
     self.assertListEqual(['x'], list(variables.keys()))
     np.testing.assert_allclose(variables['x'], true_out)
 
   def test_harvest_append_mode_in_nested_scan_and_cond_should_accumulate(self):
@@ -708,30 +709,65 @@
     (carry, out), variables = harvest_variables(f)({}, 1.)
     true_out = jnp.array([1., 2., 4., 7., 11.])
     np.testing.assert_allclose(carry, 11.)
     np.testing.assert_allclose(out, true_out)
     self.assertListEqual(['x'], list(variables.keys()))
     np.testing.assert_allclose(variables['x'], true_out)
 
-  def test_harvest_clobber_mode_in_scan_should_return_final_value(self):
+  @parameterized.parameters(False, True)
+  def test_harvest_clobber_mode_in_scan_should_return_final_value(
+      self, disable_jit
+  ):
 
     def body(carry, x):
       x = variable(x + carry, name='x', mode='clobber')
       return x, x
 
     def f(init):
       return lax.scan(body, init, jnp.arange(5.))
 
-    (carry, out), variables = harvest_variables(f)({}, 1.)
-    true_out = jnp.array([1., 2., 4., 7., 11.])
-    np.testing.assert_allclose(carry, 11.)
+    (carry, out), variables = jax.disable_jit(disable_jit)(
+        harvest_variables(f)
+    )({}, 1.0)
+    true_out = jnp.array([1.0, 2.0, 4.0, 7.0, 11.0])
+    np.testing.assert_allclose(carry, 11.0)
     np.testing.assert_allclose(out, true_out)
     self.assertListEqual(['x'], list(variables.keys()))
     np.testing.assert_allclose(variables['x'], true_out[-1])
 
+  @parameterized.named_parameters(
+      ('scan', True),
+      ('while_loop', False),
+      ('scan_disable_jit', True, True),
+      ('while_loop_disable_jit', False, True),
+  )
+  def test_can_reap_and_plant_looped_values_in_cond_clobber_mode(
+      self, static_length, disable_jit=False
+  ):
+    length = 5
+
+    def body(index, x):
+      x = x + index
+      values = []
+      for i, pred in enumerate(index == np.arange(length + 1)):
+        values.append(sow_cond(x, pred, name=f'x{i}', tag='variable'))
+      return jax.lax.select_n(index, *values)
+
+    def f(upper, init):
+      return lax.fori_loop(0, length if static_length else upper, body, init)
+
+    out, variables = jax.disable_jit(disable_jit)(harvest_variables(f))(
+        dict(x3=0.5), length, 1.
+    )
+    np.testing.assert_allclose(out, 0.5 + 4)
+    default = 0.
+    self.assertDictEqual(
+        dict(x0=1., x1=2., x2=4., x4=out, x5=default), variables
+    )
+
   def test_non_clobber_mode_in_while_loop_should_error_with_reap_and_plant(
       self):
 
     def cond(carry):
       i, _ = carry
       return i < 5
 
@@ -741,75 +777,87 @@
       return (i + 1, val + 1.)
 
     def f(init):
       return lax.while_loop(cond, body, init)
 
     with self.assertRaisesRegex(
         ValueError,
-        'Must use clobber mode for \'x\' inside of a `while_loop`.'):
-      reap_variables(f)((0, 0.))
+        "Must use clobber or cond_clobber mode for 'x' inside of a"
+        ' `while_loop`.',
+    ):
+      reap_variables(f)((0, 0.0))
 
     with self.assertRaisesRegex(
         ValueError,
-        'Must use clobber mode for \'x\' inside of a `while_loop`.'):
+        "Must use clobber or cond_clobber mode for 'x' inside of a"
+        ' `while_loop`.',
+    ):
       plant_variables(f)(dict(x=4.), (0, 0.))
 
-  def test_can_reap_final_values_from_while_loop(self):
+  @parameterized.parameters(False, True)
+  def test_can_reap_final_values_from_while_loop(self, disable_jit):
 
     def cond(carry):
       i, _ = carry
       return i < 5
 
     def body(carry):
       i, val = carry
       val = variable(val, name='x', mode='clobber')
       return (i + 1, val + 1.)
 
     def f(init):
       return lax.while_loop(cond, body, init)
 
-    reaps = reap_variables(f)((0, 0.))
+    reaps = jax.disable_jit(disable_jit)(reap_variables(f))((0, 0.))
 
     self.assertDictEqual(reaps, dict(x=4.))
 
-  def test_can_plant_values_into_each_iteration_of_while_loop(self):
+  @parameterized.parameters(False, True)
+  def test_can_plant_values_into_each_iteration_of_while_loop(
+      self, disable_jit
+  ):
 
     def cond(carry):
       i, _, _ = carry
       return i < 5
 
     def body(carry):
       i, val, val2 = carry
       val = variable(val, name='x', mode='clobber')
       return (i + 1, val + 1., val + val2)
 
     def f(init):
       return lax.while_loop(cond, body, init)
 
-    out = plant_variables(f)(dict(x=5.), (0, 0., 0.))
+    out = jax.disable_jit(disable_jit)(plant_variables(f))(
+        dict(x=5.0), (0, 0.0, 0.0)
+    )
 
     self.assertTupleEqual(out, (5, 6., 25.))
 
-  def test_can_reap_and_plant_values_into_while_loop(self):
+  @parameterized.parameters(False, True)
+  def test_can_reap_and_plant_values_into_while_loop(self, disable_jit):
 
     def cond(carry):
       i, _, _ = carry
       return i < 5
 
     def body(carry):
       i, val, val2 = carry
       val = variable(val, name='x', mode='clobber')
       val2 = variable(val2, name='y', mode='clobber')
       return (i + 1, val + 1., val + val2)
 
     def f(init):
       return lax.while_loop(cond, body, init)
 
-    out, reaps = call_and_reap_variables(plant_variables(f))(dict(x=5.),
-                                                             (0, 0., 0.))
+    out, reaps = jax.disable_jit(disable_jit)(
+        call_and_reap_variables(plant_variables(f))
+    )(dict(x=5.0), (0, 0.0, 0.0))
 
     self.assertTupleEqual(out, (5, 6., 25.))
     self.assertDictEqual(reaps, dict(y=20.))
 
   def test_must_have_identical_sow_in_both_branches_of_cond(self):
 
     def f(pred, x):
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/__init__.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/bijector_extensions.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/bijector_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/bijector_extensions_test.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/bijector_extensions_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/core.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/custom_inverse.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/custom_inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/custom_inverse_test.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/custom_inverse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/inverse_test.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/inverse_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/rules.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -254,14 +254,14 @@
 
 
 # Monkey patching JAX so we can define custom, more numerically stable inverses.
 jax.scipy.special.expit = custom_inverse(jax.scipy.special.expit)
 jax.scipy.special.logit = custom_inverse(jax.scipy.special.logit)
 jax.nn.sigmoid = jax.scipy.special.expit
 jax.nn.softplus = custom_inverse(jax.nn.softplus)
-jax.scipy.special.expit.def_inverse_unary(f_inv=jax.scipy.special.logit,
-                                          f_ildj=expit_ildj)
-jax.scipy.special.logit.def_inverse_unary(f_inv=jax.scipy.special.expit,
-                                          f_ildj=logit_ildj)
-jax.nn.softplus.def_inverse_unary(f_inv=softplus_inv,
-                                  f_ildj=softplus_ildj)
-
+jax.scipy.special.expit.def_inverse_unary(
+    f_inv=jax.scipy.special.logit, f_ildj=expit_ildj
+)  # pytype: disable=attribute-error
+jax.scipy.special.logit.def_inverse_unary(
+    f_inv=jax.scipy.special.expit, f_ildj=logit_ildj
+)  # pytype: disable=attribute-error
+jax.nn.softplus.def_inverse_unary(f_inv=softplus_inv, f_ildj=softplus_ildj)  # pytype: disable=attribute-error
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/slice.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/inverse/slice_test.py` & `oryx-0.2.7/oryx/core/interpreters/inverse/slice_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/log_prob.py` & `oryx-0.2.7/oryx/core/interpreters/log_prob.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/log_prob_test.py` & `oryx-0.2.7/oryx/core/interpreters/log_prob_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/propagate.py` & `oryx-0.2.7/oryx/core/interpreters/propagate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -380,17 +380,21 @@
 
   new_jaxpr = _to_jaxpr(
       f, tuple(api_util.shaped_abstractify(i) for i in flat_vals))
 
   in_shardings = (sharding_impls.UNSPECIFIED,) * len(flat_vals)
   donated_invars = (False,) * len(flat_vals)
   out_shardings = (sharding_impls.UNSPECIFIED,) * len(new_jaxpr.out_avals)
+  in_layouts = (None,) * len(flat_vals)
+  out_layouts = (None,) * len(new_jaxpr.out_avals)
 
   new_params = {
       **params,
       'jaxpr': new_jaxpr,
       'in_shardings': in_shardings,
       'out_shardings': out_shardings,
       'donated_invars': donated_invars,
+      'in_layouts': in_layouts,
+      'out_layouts': out_layouts,
   }
   flat_out = pjit.pjit_p.bind(*flat_vals, **new_params)
   return tree_util.tree_unflatten(out_tree(), flat_out)
```

### Comparing `oryx-0.2.6/oryx/core/interpreters/propagate_test.py` & `oryx-0.2.7/oryx/core/interpreters/propagate_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/kwargs_util.py` & `oryx-0.2.7/oryx/core/kwargs_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/kwargs_util_test.py` & `oryx-0.2.7/oryx/core/kwargs_util_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/ppl/__init__.py` & `oryx-0.2.7/oryx/core/ppl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/ppl/effect_handler.py` & `oryx-0.2.7/oryx/core/ppl/effect_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -272,21 +272,25 @@
   in_shardings = (sharding_impls.UNSPECIFIED,) * num_state + params[
       'in_shardings'
   ]
   donated_invars = (False,) * num_state + params['donated_invars']
   out_shardings = (sharding_impls.UNSPECIFIED,) * num_state + params[
       'out_shardings'
   ]
+  in_layouts = (None,) * num_state + params['in_layouts']
+  out_layouts = (None,) * num_state + params['out_layouts']
 
   new_params = {
       **params,
       'jaxpr': new_jaxpr,
       'in_shardings': in_shardings,
       'out_shardings': out_shardings,
       'donated_invars': donated_invars,
+      'in_layouts': in_layouts,
+      'out_layouts': out_layouts,
   }
 
   ans_state = pjit.pjit_p.bind(*state_invals, **new_params)
   return tree_util.tree_unflatten(out_tree(), ans_state)
 
 
 custom_effect_handler_rules[pjit.pjit_p] = _pjit_effect_handler_rule
```

### Comparing `oryx-0.2.6/oryx/core/ppl/effect_handler_test.py` & `oryx-0.2.7/oryx/core/ppl/effect_handler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/ppl/plate_util.py` & `oryx-0.2.7/oryx/core/ppl/plate_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/ppl/transformations.py` & `oryx-0.2.7/oryx/core/ppl/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/ppl/transformations_test.py` & `oryx-0.2.7/oryx/core/ppl/transformations_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/primitive.py` & `oryx-0.2.7/oryx/core/primitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/primitive_test.py` & `oryx-0.2.7/oryx/core/primitive_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/pytree.py` & `oryx-0.2.7/oryx/core/pytree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/serialize.py` & `oryx-0.2.7/oryx/core/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/serialize_test.py` & `oryx-0.2.7/oryx/core/serialize_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/__init__.py` & `oryx-0.2.7/oryx/core/state/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/api.py` & `oryx-0.2.7/oryx/core/state/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/function.py` & `oryx-0.2.7/oryx/core/state/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/function_test.py` & `oryx-0.2.7/oryx/core/state/function_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/module.py` & `oryx-0.2.7/oryx/core/state/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/registrations.py` & `oryx-0.2.7/oryx/core/state/registrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/state/registrations_test.py` & `oryx-0.2.7/oryx/core/state/registrations_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/core/trace_util.py` & `oryx-0.2.7/oryx/core/trace_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/distributions/__init__.py` & `oryx-0.2.7/oryx/distributions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/distributions/distribution_extensions.py` & `oryx-0.2.7/oryx/distributions/distribution_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/distributions/distribution_extensions_test.py` & `oryx-0.2.7/oryx/distributions/distribution_extensions_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/examples/notebooks/a_tour_of_oryx.ipynb` & `oryx-0.2.7/oryx/examples/notebooks/a_tour_of_oryx.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999069940476191%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(6, 'The source code for Oryx can be found [on "*

 * *            "GitHub](https://github.com/jax-ml/oryx).')], delete: [6]}}}"}*

```diff
@@ -79,15 +79,15 @@
             "source": [
                 "Oryx is an experimental library that extends [JAX](https://github.com/google/jax) to applications ranging from building and training complex neural networks to approximate Bayesian inference in deep generative models. Like JAX provides `jit`, `vmap`, and `grad`, Oryx provides a set of **composable function transformations** that enable writing simple code and transforming it to build complexity while staying completely interoperable with JAX.\n",
                 "\n",
                 "JAX can only safely transform pure, functional code (i.e. code without side-effects). While pure code can be easier to write and reason about, \"impure\" code can often be more concise and more easily expressive.\n",
                 "\n",
                 "At its core, Oryx is a library that enables \"augmenting\" pure functional code to accomplish tasks like defining state or pulling out intermediate values. Its goal is to be as thin of a layer on top of JAX as possible, leveraging JAX's minimalist approach to numerical computing. Oryx is conceptually divided into several \"layers\", each building on the one below it.\n",
                 "\n",
-                "The source code for Oryx can be found [on GitHub](https://github.com/tensorflow/probability/tree/main/spinoffs/oryx)."
+                "The source code for Oryx can be found [on GitHub](https://github.com/jax-ml/oryx)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "colab_type": "text",
                 "id": "8cloSFmOiJqn"
```

### Comparing `oryx-0.2.6/oryx/examples/notebooks/probabilistic_programming.ipynb` & `oryx-0.2.7/oryx/examples/notebooks/probabilistic_programming.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999620253164557%*

 * *Differences: {"'cells'": "{73: {'source': {insert: [(2, '  flat_state, sample_tree = "*

 * *            "jax.tree.flatten(weights)\\n'), (5, '    return "*

 * *            "target_log_prob(jax.tree.unflatten(sample_tree, states))\\n'), (19, '  samples = "*

 * *            "jax.tree.unflatten(sample_tree, flat_states)\\n')], delete: [19, 5, 2]}}}"}*

```diff
@@ -901,32 +901,32 @@
             "metadata": {
                 "id": "nmjmxzGhN855"
             },
             "outputs": [],
             "source": [
                 "@jit\n",
                 "def run_chain(key, weights):\n",
-                "  flat_state, sample_tree = jax.tree_flatten(weights)\n",
+                "  flat_state, sample_tree = jax.tree.flatten(weights)\n",
                 "\n",
                 "  def flat_log_prob(*states):\n",
-                "    return target_log_prob(jax.tree_unflatten(sample_tree, states))\n",
+                "    return target_log_prob(jax.tree.unflatten(sample_tree, states))\n",
                 "\n",
                 "  def trace_fn(_, results):\n",
                 "    return results.inner_results.accepted_results.target_log_prob\n",
                 "\n",
                 "  flat_states, log_probs = tfp.mcmc.sample_chain(\n",
                 "    1000,\n",
                 "    num_burnin_steps=9000,\n",
                 "    kernel=tfp.mcmc.DualAveragingStepSizeAdaptation(\n",
                 "        tfp.mcmc.HamiltonianMonteCarlo(flat_log_prob, 1e-3, 100),\n",
                 "        9000, target_accept_prob=0.7),\n",
                 "    trace_fn=trace_fn,\n",
                 "    current_state=flat_state,\n",
                 "    seed=key)\n",
-                "  samples = jax.tree_unflatten(sample_tree, flat_states)\n",
+                "  samples = jax.tree.unflatten(sample_tree, flat_states)\n",
                 "  return samples, log_probs\n",
                 "posterior_weights, log_probs = run_chain(random.PRNGKey(0), weights)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 0,
```

### Comparing `oryx-0.2.6/oryx/experimental/__init__.py` & `oryx-0.2.7/oryx/experimental/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/addn.py` & `oryx-0.2.7/oryx/experimental/autoconj/addn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/addn_test.py` & `oryx-0.2.7/oryx/experimental/autoconj/addn_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/canonicalize.py` & `oryx-0.2.7/oryx/experimental/autoconj/canonicalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/canonicalize_test.py` & `oryx-0.2.7/oryx/experimental/autoconj/canonicalize_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/einsum.py` & `oryx-0.2.7/oryx/experimental/autoconj/einsum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/autoconj/einsum_test.py` & `oryx-0.2.7/oryx/experimental/autoconj/einsum_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/__init__.py` & `oryx-0.2.7/oryx/experimental/matching/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/jax_rewrite.py` & `oryx-0.2.7/oryx/experimental/matching/jax_rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/jax_rewrite_test.py` & `oryx-0.2.7/oryx/experimental/matching/jax_rewrite_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/matcher.py` & `oryx-0.2.7/oryx/experimental/matching/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/matcher_test.py` & `oryx-0.2.7/oryx/experimental/matching/matcher_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/rules.py` & `oryx-0.2.7/oryx/experimental/matching/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/matching/rules_test.py` & `oryx-0.2.7/oryx/experimental/matching/rules_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/mcmc/__init__.py` & `oryx-0.2.7/oryx/experimental/mcmc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/mcmc/kernels.py` & `oryx-0.2.7/oryx/experimental/mcmc/kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/mcmc/kernels_test.py` & `oryx-0.2.7/oryx/experimental/mcmc/kernels_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/mcmc/utils.py` & `oryx-0.2.7/oryx/experimental/mcmc/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/__init__.py` & `oryx-0.2.7/oryx/experimental/nn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/base.py` & `oryx-0.2.7/oryx/experimental/nn/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -332,15 +332,15 @@
   def _call(self, *args, **kwargs):
     init_key = kwargs.pop('init_key', None)
     layer = self.init(init_key, *args, **kwargs)
     return layer(*args, **kwargs)
 
   def init(self, init_key, *args, name=None, **kwargs):
     """Initializes a Template into a Layer."""
-    specs = jax.tree_map(state.make_array_spec, args)
+    specs = jax.tree.map(state.make_array_spec, args)
     kwargs = dict(
         cls=self.cls,
         specs=specs,
         init_args=self.init_args,
         init_kwargs=self.init_kwargs,
     )
     layer = primitive.initial_style_bind(template_init_p)(
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/base_test.py` & `oryx-0.2.7/oryx/experimental/nn/base_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/combinator.py` & `oryx-0.2.7/oryx/experimental/nn/combinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/combinator_test.py` & `oryx-0.2.7/oryx/experimental/nn/combinator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/convolution.py` & `oryx-0.2.7/oryx/experimental/nn/convolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/convolution_test.py` & `oryx-0.2.7/oryx/experimental/nn/convolution_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/core.py` & `oryx-0.2.7/oryx/experimental/nn/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/core_test.py` & `oryx-0.2.7/oryx/experimental/nn/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/function.py` & `oryx-0.2.7/oryx/experimental/nn/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/function_test.py` & `oryx-0.2.7/oryx/experimental/nn/function_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/normalization.py` & `oryx-0.2.7/oryx/experimental/nn/normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/normalization_test.py` & `oryx-0.2.7/oryx/experimental/nn/normalization_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/pooling.py` & `oryx-0.2.7/oryx/experimental/nn/pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/pooling_test.py` & `oryx-0.2.7/oryx/experimental/nn/pooling_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/reshape.py` & `oryx-0.2.7/oryx/experimental/nn/reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/nn/reshape_test.py` & `oryx-0.2.7/oryx/experimental/nn/reshape_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/optimizers/__init__.py` & `oryx-0.2.7/oryx/experimental/optimizers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/optimizers/optix.py` & `oryx-0.2.7/oryx/experimental/optimizers/optix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/experimental/optimizers/optix_test.py` & `oryx-0.2.7/oryx/experimental/optimizers/optix_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/internal/__init__.py` & `oryx-0.2.7/oryx/internal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/internal/test_util.py` & `oryx-0.2.7/oryx/internal/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/tools/build_oryx_docs.py` & `oryx-0.2.7/oryx/tools/build_oryx_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/util/__init__.py` & `oryx-0.2.7/oryx/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/util/summary.py` & `oryx-0.2.7/oryx/util/summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/util/summary_test.py` & `oryx-0.2.7/oryx/util/summary_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `oryx-0.2.6/oryx/version.py` & `oryx-0.2.7/oryx/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The oryx Authors.
+# Copyright 2024 The oryx Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Define Oryx version information."""
 
 # We follow Semantic Versioning (https://semver.org/)
 _MAJOR_VERSION = '0'
 _MINOR_VERSION = '2'
-_PATCH_VERSION = '6'
+_PATCH_VERSION = '7'
 
 # When building releases, we can update this value on the release branch to
 # reflect the current release candidate ('rc0', 'rc1') or, finally, the official
 # stable release (indicated by `_VERSION_SUFFIX = ''`). Outside the context of a
 # release branch, the current version is by default assumed to be a
 # 'development' version, labeled 'dev'.
 _VERSION_SUFFIX = 'dev'
```

### Comparing `oryx-0.2.6/PKG-INFO` & `oryx-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oryx
-Version: 0.2.6
+Version: 0.2.7
 Summary: Probabilistic programming and deep learning in JAX
 License: Apache 2.0
 Author: Google LLC
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

