# Comparing `tmp/adelie-1.1.31.tar.gz` & `tmp/adelie-1.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelie-1.1.31.tar", last modified: Tue May  7 00:12:44 2024, max compression
+gzip compressed data, was "adelie-1.1.32.tar", last modified: Thu May 23 01:54:22 2024, max compression
```

## Comparing `adelie-1.1.31.tar` & `adelie-1.1.32.tar`

### file list

```diff
@@ -1,736 +1,739 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.025352 adelie-1.1.31/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 00:12:32.000000 adelie-1.1.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 00:12:32.000000 adelie-1.1.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-07 00:12:44.025352 adelie-1.1.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-07 00:12:32.000000 adelie-1.1.31/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 00:12:32.000000 adelie-1.1.31/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.913352 adelie-1.1.31/adelie/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/bcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16287 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39442 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    30930 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    38400 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/adelie_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/bcd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/configs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/glm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.897352 adelie-1.1.31/adelie/src/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/include/adelie_core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/include/adelie_core/bcd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/admm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/bcd/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/configs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.917352 adelie-1.1.31/adelie/src/include/adelie_core/glm/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_binomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_cox.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multibase.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_poisson.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.921352 adelie-1.1.31/adelie/src/include/adelie_core/io/
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17372 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/io/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.921352 adelie-1.1.31/adelie/src/include/adelie_core/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23510 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_interaction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_subset.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/matrix/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.921352 adelie-1.1.31/adelie/src/include/adelie_core/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/optimization/bisect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/optimization/newton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/optimization/nnls.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/optimization/search_pivot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.925352 adelie-1.1.31/adelie/src/include/adelie_core/solver/
--rw-r--r--   0 runner    (1001) docker     (127)    17965 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22175 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/solver/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.925352 adelie-1.1.31/adelie/src/include/adelie_core/state/
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.929352 adelie-1.1.31/adelie/src/include/adelie_core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/algorithm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/counting_iterator.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.929352 adelie-1.1.31/adelie/src/include/adelie_core/util/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/format.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/functional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/stopwatch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/tqdm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/include/adelie_core/util/types.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    27065 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/optimization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    69524 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/state.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.901352 adelie-1.1.31/adelie/src/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.929352 adelie-1.1.31/adelie/src/third_party/eigen3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.933352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/KLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.905352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.933352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.933352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.949352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.901352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.949352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.949352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.949352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.949352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.953352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.953352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.901352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.953352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.953352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.953352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.957352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.957352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.957352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.957352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.957352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.961352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.965352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.969352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.969352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.973352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.977352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.985352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.985352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.985352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.989352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.989352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.989352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.989352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.993352 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.905352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.993352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.997352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.905352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.009352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.009352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.009352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
--rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.909352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.013352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.017352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:43.909352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.021352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.025352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.025352 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
--rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)   112154 2024-05-07 00:12:32.000000 adelie-1.1.31/adelie/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:12:44.025352 adelie-1.1.31/adelie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42418 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 00:12:43.000000 adelie-1.1.31/adelie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-07 00:12:33.000000 adelie-1.1.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:12:44.025352 adelie-1.1.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-07 00:12:33.000000 adelie-1.1.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.137778 adelie-1.1.32/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 01:54:14.000000 adelie-1.1.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-23 01:54:14.000000 adelie-1.1.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-23 01:54:22.133778 adelie-1.1.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-23 01:54:14.000000 adelie-1.1.32/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 01:54:14.000000 adelie-1.1.32/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.005777 adelie-1.1.32/adelie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39466 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40387 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38423 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.009777 adelie-1.1.32/adelie/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/adelie_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/bcd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/configs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/glm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.989777 adelie-1.1.32/adelie/src/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.009777 adelie-1.1.32/adelie/src/include/adelie_core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.009777 adelie-1.1.32/adelie/src/include/adelie_core/bcd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.009777 adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/admm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.009777 adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/bcd/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/configs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.013778 adelie-1.1.32/adelie/src/include/adelie_core/glm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_binomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_cox.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multibase.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_poisson.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.013778 adelie-1.1.32/adelie/src/include/adelie_core/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/io/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.017778 adelie-1.1.32/adelie/src/include/adelie_core/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25559 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_interaction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18403 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_one_hot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13179 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_standardize.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_subset.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25500 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/matrix/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.017778 adelie-1.1.32/adelie/src/include/adelie_core/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/optimization/bisect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/optimization/newton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/optimization/nnls.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/optimization/search_pivot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.017778 adelie-1.1.32/adelie/src/include/adelie_core/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)    17965 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/solver/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.021777 adelie-1.1.32/adelie/src/include/adelie_core/state/
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.021777 adelie-1.1.32/adelie/src/include/adelie_core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/algorithm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/counting_iterator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.021777 adelie-1.1.32/adelie/src/include/adelie_core/util/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/format.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/functional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/stopwatch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/tqdm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/include/adelie_core/util/types.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/matrix_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/optimization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69517 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/state.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.993777 adelie-1.1.32/adelie/src/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.021777 adelie-1.1.32/adelie/src/third_party/eigen3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.029778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.997777 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.029778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.029778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.045778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.993777 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.045778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.045778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.993777 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.049778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.053778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.053778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.053778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.053778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.057778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.057778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.061778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.065778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.069778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.069778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.069778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.073778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.077778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.085778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.089778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.089778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.089778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.089778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.089778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.093778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.093778 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.997777 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.097778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.101778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:21.997777 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.113778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.001778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.117778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.121778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.125778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.125778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.125778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.125778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.129778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.129778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.129778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.001778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)   112640 2024-05-23 01:54:14.000000 adelie-1.1.32/adelie/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:54:22.133778 adelie-1.1.32/adelie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    42576 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 01:54:21.000000 adelie-1.1.32/adelie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-23 01:54:14.000000 adelie-1.1.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:54:22.137778 adelie-1.1.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-23 01:54:14.000000 adelie-1.1.32/setup.py
```

### Comparing `adelie-1.1.31/LICENSE` & `adelie-1.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/PKG-INFO` & `adelie-1.1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.31
+Version: 1.1.32
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.31/README.md` & `adelie-1.1.32/README.md`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/bcd.py` & `adelie-1.1.32/adelie/bcd.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/cv.py` & `adelie-1.1.32/adelie/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,31 @@
 import scipy.sparse
 
 
 @dataclass
 class CVGrpnetResult:
     """Result of K-fold CV group elastic net.
     """
+
     lmdas: np.ndarray
+    """
+    The common regularization path used for all folds.
+    """
     losses: np.ndarray
+    """
+    ``losses[k,i]`` is the CV loss when validating on fold ``k`` at ``lmdas[i]``.
+    """
     avg_losses: np.ndarray
+    """
+    ``avg_losses[i]`` is the average CV loss at ``lmdas[i]``.
+    """
     best_idx: int
+    """
+    Argmin of ``avg_losses``.
+    """
     
     def plot_loss(self):
         """Plots the average K-fold CV loss.
 
         For each fitted :math:`\\lambda`, the average K-fold CV loss
         as well as an error bar of one standard deviation (above and below) is plotted.
         """
@@ -53,15 +66,15 @@
 
     def fit(
         self, 
         *, 
         lmda_path_size: int =100,
         **grpnet_params,
     ):
-        """Fit group elastic net until the best CV :math:`\\lambda`.
+        """Fits group elastic net until the best CV :math:`\\lambda`.
 
         Parameters
         ----------
         lmda_path_size : int, optional
             Number of regularizations in the path.
             Default is ``100``.
         **grpnet_params
@@ -105,15 +118,15 @@
     early_exit: bool =False,
     min_ratio: float =1e-1,
     lmda_path_size: int =100,
     n_folds: int =5,
     seed: int =None,
     **grpnet_params,
 ):
-    """Cross-validation group elastic net solver.
+    """Solves cross-validated group elastic net via naive method.
 
     This function was written with the intent that ``glm``
     is to be one of the GLMs defined in ``adelie.glm``.
     In particular, we assume the observation weights ``w`` associated with ``glm``
     has the property that if ``w[i] == 0``,
     then the ``i`` th prediction :math:`\\eta_i` is ignored in the computation of the loss.
```

### Comparing `adelie-1.1.31/adelie/data.py` & `adelie-1.1.32/adelie/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     elif glm == "cox":
         signal_scale = np.sqrt(rho * np.sum(beta) ** 2 + (1-rho) * np.sum(beta ** 2))
         noise_scale = signal_scale / np.sqrt(snr)
         eta = eta.ravel()
         s = np.round(np.random.exponential(1, n))
         t = 1 + s + np.round(np.exp(eta / noise_scale + np.random.normal(0, 1, n)))
         C = 1 + s + np.round(np.exp(np.random.normal(0, 1, n)))
-        d = t < C
+        d = (t < C).astype(eta.dtype)
         t = np.minimum(t, C)
         return cox(
             start=s,
             stop=t,
             status=d,
         )
     else:
```

### Comparing `adelie-1.1.31/adelie/diagnostic.py` & `adelie-1.1.32/adelie/diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     Returns
     -------
     linear_preds : (L, n) or (L, n, K) np.ndarray
         Linear predictions.
 
     See Also
     --------
-    adelie.glm.GlmBase64
-    adelie.glm.GlmMultiBase64
+    adelie.adelie_core.glm.GlmBase64
+    adelie.adelie_core.glm.GlmMultiBase64
     """
     is_multi = len(intercepts.shape) == 2
     if is_multi:
         K = intercepts.shape[1]
         X = matrix.kronecker_eye(X, K, n_threads=n_threads)
         n = X.rows() // K
         y_shape = (n, K)
```

### Comparing `adelie-1.1.31/adelie/glm.py` & `adelie-1.1.32/adelie/glm.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,72 +6,93 @@
     GlmMultiBase32,
 )
 from typing import Union
 import numpy as np
 import warnings
 
 
+def _coerce_dtype(y, dtype):
+    dtype_map = {
+        np.dtype("float32"): np.float32,
+        np.dtype("float64"): np.float64,
+    }
+    valid_dtypes = list(dtype_map.keys())
+    y = np.array(y, order="C")
+    if dtype is None:
+        if not (y.dtype in valid_dtypes):
+            raise RuntimeError(
+                "y must have an underlying type of np.float32 or np.float64, "
+                "or dtype must be explicitly specified."
+            )
+        dtype = dtype_map[y.dtype]
+    else:
+        if not (dtype in valid_dtypes):
+            raise RuntimeError("dtype must be either np.float32 or np.float64.")
+    y = y.astype(dtype)
+    return y, dtype
+
+
 class glm_base:
     """Base wrapper GLM class.
 
     All Python wrapper classes for core GLM classes must inherit from this class.
     The purpose of this class is to expose extra member interface
     that are more easily written in Python (and not speed-critical).
     """
     def __init__(self, y, weights, core_base, dtype):
         self.core_base = core_base
+        self.y = np.array(y, copy=True, dtype=dtype)
         self.dtype = dtype
-        self.y = np.array(y, order="C", dtype=dtype)
         if len(y.shape) != 1:
             raise RuntimeError("y must be 1-dimensional.")
         n = y.shape[0]
         if not (weights is None):
             if weights.shape != (n,):
                 raise RuntimeError("y and weights must have same length.")
             weights_sum = np.sum(weights)
             if not np.allclose(weights_sum, 1):
                 warnings.warn("Normalizing weights to sum to 1.")
                 weights = weights / weights_sum
         else:
             weights = np.full(n, 1/n, dtype=dtype)
-        self.weights = np.array(weights, order="C", dtype=dtype)
+        self.weights = np.array(weights, copy=True, dtype=dtype)
 
 
 class multiglm_base:
-    """Base wrapper Multi-response GLM class.
+    """Base wrapper multi-response GLM class.
 
     All Python wrapper classes for core multi-response GLM classes must inherit from this class.
     The purpose of this class is to expose extra member interface
     that are more easily written in Python (and not speed-critical).
     """
     def __init__(self, y, weights, core_base, dtype):
         self.core_base = core_base
+        self.y = np.array(y, copy=True, dtype=dtype)
         self.dtype = dtype
-        self.y = np.array(y, order="C", dtype=dtype)
         if len(y.shape) != 2:
             raise RuntimeError("y must be 2-dimensional.")
         n = y.shape[0]
         if not (weights is None):
             if weights.shape != (n,):
                 raise RuntimeError("y rows and weights must have same length.")
             weights_sum = np.sum(weights)
             if not np.allclose(weights_sum, 1):
                 warnings.warn("Normalizing weights to sum to 1.")
                 weights = weights / np.sum(weights)
         else:
             weights = np.full(n, 1/n, dtype=dtype)
-        self.weights = np.array(weights, order="C", dtype=dtype)
+        self.weights = np.array(weights, copy=True, dtype=dtype)
 
 
 def binomial(
     y: np.ndarray,
     *,
     weights: np.ndarray =None,
     link: str ="logit",
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
 ):
     """Creates a Binomial GLM family object.
 
     The Binomial GLM family with the logit link function 
     specifies the loss function as:
 
     .. math::
@@ -113,36 +134,42 @@
 
             - ``"logit"``: the logit link function.
             - ``"probit"``: the probit link function.
 
         Default is ``"logit"``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``y``,
+        in which case ``y`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
 
     Returns
     -------
     glm
         Binomial GLM object.
 
     See Also
     --------
-    adelie.glm.GlmBase64
+    adelie.adelie_core.glm.GlmBinomialLogit64
+    adelie.adelie_core.glm.GlmBinomialProbit64
     """
     dispatcher = {
         "logit": {
             np.float64: core.glm.GlmBinomialLogit64,
             np.float32: core.glm.GlmBinomialLogit32,
         },
         "probit": {
             np.float64: core.glm.GlmBinomialProbit64,
             np.float32: core.glm.GlmBinomialProbit32,
         },
     }
 
+    y, dtype = _coerce_dtype(y, dtype)
+
     core_base = dispatcher[link][dtype]
 
     class _binomial(glm_base, core_base):
         def __init__(self):
             glm_base.__init__(self, y, weights, core_base, dtype)
             core_base.__init__(self, self.y, self.weights)
 
@@ -156,15 +183,15 @@
 def cox(
     start: np.ndarray,
     stop: np.ndarray,
     status: np.ndarray,
     *,
     weights: np.ndarray =None,
     tie_method: str ="efron",
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
 ):
     """Creates a Cox GLM family object.
 
     The Cox GLM family specifies the loss function as:
 
     .. math::
         \\begin{align*}
@@ -230,36 +257,41 @@
 
             - ``"efron"``
             - ``"breslow"``
 
         Default is ``"efron"``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``status``,
+        in which case ``status`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
 
     Returns
     -------
     glm
         Cox GLM object.
 
     See Also
     --------
-    adelie.glm.GlmBase64
+    adelie.adelie_core.glm.GlmCox64
     """
     dispatcher = {
         np.float64: core.glm.GlmCox64,
         np.float32: core.glm.GlmCox32,
     }
 
+    status, dtype = _coerce_dtype(status, dtype)
+
     core_base = dispatcher[dtype]
 
     class _cox(glm_base, core_base):
         def __init__(self):
-            self.start = start.astype(dtype)
-            self.stop = stop.astype(dtype)
+            self.start = np.array(start, copy=True, dtype=dtype)
+            self.stop = np.array(stop, copy=True, dtype=dtype)
             glm_base.__init__(self, status, weights, core_base, dtype)
             self.status = self.y
             self.tie_method = tie_method
             core_base.__init__(
                 self, 
                 self.start, 
                 self.stop, 
@@ -282,15 +314,15 @@
     return _cox()
 
 
 def gaussian(
     y: np.ndarray,
     *,
     weights: np.ndarray =None,
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
     opt: bool =True,
 ):
     """Creates a Gaussian GLM family object.
 
     The Gaussian GLM family specifies the loss function as:
 
     .. math::
@@ -308,36 +340,41 @@
         Response vector :math:`y`.
     weights : (n,) np.ndarray, optional
         Observation weights :math:`W`.
         Weights are normalized such that they sum to ``1``.
         Default is ``None``, in which case, it is set to ``np.full(n, 1/n)``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``y``,
+        in which case ``y`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
     opt : bool, optional
         If ``True``, an optimized routine is used when passed into ``adelie.grpnet``.
         Otherwise, a general routine with IRLS is used.
         This flag is mainly for developers for testing purposes.
         We advise users to use the default value.
         Default is ``True``.
 
     Returns
     -------
     glm
         Gaussian GLM object.
 
     See Also
     --------
-    adelie.glm.GlmBase64
+    adelie.adelie_core.glm.GlmGaussian64
     """
     dispatcher = {
         np.float64: core.glm.GlmGaussian64,
         np.float32: core.glm.GlmGaussian32,
     }
 
+    y, dtype = _coerce_dtype(y, dtype)
+
     core_base = dispatcher[dtype]
 
     class _gaussian(glm_base, core_base):
         def __init__(self):
             self.opt = opt
             glm_base.__init__(self, y, weights, core_base, dtype)
             core_base.__init__(self, self.y, self.weights)
@@ -349,20 +386,20 @@
     return _gaussian()
 
 
 def multigaussian(
     y: np.ndarray,
     *,
     weights: np.ndarray =None,
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
     opt: bool =True,
 ):
-    """Creates a Multi-response Gaussian GLM family object.
+    """Creates a MultiGaussian GLM family object.
 
-    The Multi-Response Gaussian GLM family specifies the loss function as:
+    The MultiGaussian GLM family specifies the loss function as:
 
     .. math::
         \\begin{align*}
             \\ell(\\eta)
             =
             \\frac{1}{K}
             \\sum\\limits_{i=1}^n 
@@ -378,36 +415,41 @@
         Response matrix :math:`y`.
     weights : (n,) np.ndarray, optional
         Observation weights :math:`W`.
         Weights are normalized such that they sum to ``1``.
         Default is ``None``, in which case, it is set to ``np.full(n, 1/n)``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``y``,
+        in which case ``y`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
     opt : bool, optional
         If ``True``, an optimized routine is used when passed into ``adelie.grpnet``.
         Otherwise, a general routine with IRLS is used.
         This flag is mainly for developers for testing purposes.
         We advise users to use the default value.
         Default is ``True``.
 
     Returns
     -------
     glm
-        Multi-response Gaussian GLM object.
+        MultiGaussian GLM object.
 
     See Also
     --------
-    adelie.glm.GlmBase64
+    adelie.adelie_core.glm.GlmMultiGaussian64
     """
     dispatcher = {
         np.float64: core.glm.GlmMultiGaussian64,
         np.float32: core.glm.GlmMultiGaussian32,
     }
 
+    y, dtype = _coerce_dtype(y, dtype)
+
     core_base = dispatcher[dtype]
 
     class _multigaussian(multiglm_base, core_base):
         def __init__(self):
             self.opt = opt
             multiglm_base.__init__(self, y, weights, core_base, dtype)
             core_base.__init__(self, self.y, self.weights)
@@ -419,15 +461,15 @@
     return _multigaussian()
 
 
 def multinomial(
     y: np.ndarray,
     *,
     weights: np.ndarray =None,
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
 ):
     """Creates a Multinomial GLM family object.
 
     The Multinomial GLM family specifies the loss function as:
 
     .. math::
         \\begin{align*}
@@ -457,30 +499,35 @@
         Response matrix :math:`y`.
     weights : (n,) np.ndarray, optional
         Observation weights :math:`W`.
         Weights are normalized such that they sum to ``1``.
         Default is ``None``, in which case, it is set to ``np.full(n, 1/n)``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``y``,
+        in which case ``y`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
 
     Returns
     -------
     glm
         Multinomial GLM object.
 
     See Also
     --------
-    adelie.glm.GlmMultiBase64
+    adelie.adelie_core.glm.GlmMultinomial64
     """
     dispatcher = {
         np.float64: core.glm.GlmMultinomial64,
         np.float32: core.glm.GlmMultinomial32,
     }
 
+    y, dtype = _coerce_dtype(y, dtype)
+
     core_base = dispatcher[dtype]
 
     class _multinomial(multiglm_base, core_base):
         def __init__(self):
             multiglm_base.__init__(self, y, weights, core_base, dtype)
             core_base.__init__(self, self.y, self.weights)
 
@@ -491,15 +538,15 @@
     return _multinomial()
 
 
 def poisson(
     y: np.ndarray,
     *,
     weights: np.ndarray =None,
-    dtype: Union[np.float32, np.float64] =np.float64,
+    dtype: Union[np.float32, np.float64] =None,
 ):
     """Creates a Poisson GLM family object.
 
     The Poisson GLM family specifies the loss function as:
 
     .. math::
         \\begin{align*}
@@ -518,30 +565,35 @@
         Response vector :math:`y`.
     weights : (n,) np.ndarray, optional
         Observation weights :math:`W`.
         Weights are normalized such that they sum to ``1``.
         Default is ``None``, in which case, it is set to ``np.full(n, 1/n)``.
     dtype : Union[np.float32, np.float64], optional
         The underlying data type.
-        Default is ``np.float64``.
+        If ``None``, it is inferred from ``y``,
+        in which case ``y`` must have an underlying data type of
+        ``np.float32`` or ``np.float64``.
+        Default is ``None``.
 
     Returns
     -------
     glm
         Poisson GLM object.
 
     See Also
     --------
-    adelie.glm.GlmBase64
+    adelie.adelie_core.glm.GlmPoisson64
     """
     dispatcher = {
         np.float64: core.glm.GlmPoisson64,
         np.float32: core.glm.GlmPoisson32,
     }
 
+    y, dtype = _coerce_dtype(y, dtype)
+
     core_base = dispatcher[dtype]
 
     class _poisson(glm_base, core_base):
         def __init__(self):
             glm_base.__init__(self, y, weights, core_base, dtype)
             core_base.__init__(self, self.y, self.weights)
```

### Comparing `adelie-1.1.31/adelie/io.py` & `adelie-1.1.32/adelie/io.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/logger.py` & `adelie-1.1.32/adelie/logger.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/matrix.py` & `adelie-1.1.32/adelie/matrix.py`

 * *Files 18% similar despite different names*

```diff
@@ -86,32 +86,35 @@
             if (
                 (len(key) == 2) and
                 (not isinstance(key[0], valid_one_type)) and 
                 (not isinstance(key[1], valid_one_type))
             ):
                 raise ValueError(
                     "If row and column subsets are provided, "
-                    "at least one must be an integer or a slice. "
+                    "at least one must not be a list-like object. "
                 )
         elif isinstance(key, valid_some_type):
             key = (key,)
         else:
             raise ValueError(
                 "Subsets must be integer, slice, list, or np.ndarray objects."
             )
 
         def _convert_subset(s, size):
             if isinstance(s, (int, np.integer)):
                 return np.array([s])
             elif isinstance(s, (list, np.ndarray)):
-                s = np.array(s, dtype=int)
-                if np.unique(s).shape[0] != s.shape[0]:
-                    raise ValueError(
-                        "Subset does not contain unique elements."
-                    )
+                if s.dtype == np.dtype("bool"):
+                    s = np.where(s)[0]
+                else:
+                    s = np.array(s, dtype=int)
+                    if np.unique(s).shape[0] != s.shape[0]:
+                        raise ValueError(
+                            "Subset does not contain unique elements."
+                        )
                 return s
             elif isinstance(s, slice):
                 start = 0 if s.start is None else s.start
                 stop = size if s.stop is None else s.stop
                 step = 1 if s.step is None else s.step
                 if (
                     (start != 0) or 
@@ -216,15 +219,15 @@
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixCovBase64
+    adelie.adelie_core.matrix.MatrixCovBlockDiag64
     """
     mats = [
         dense(mat, method="cov", n_threads=1)
         if isinstance(mat, np.ndarray) else
         mat
         for mat in mats
     ]
@@ -303,15 +306,16 @@
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveCConcatenate64
+    adelie.adelie_core.matrix.MatrixNaiveRConcatenate64
     """
     mats = [
         dense(mat, method="naive", n_threads=n_threads)
         if isinstance(mat, np.ndarray) else
         mat
         for mat in mats
     ]
@@ -336,24 +340,25 @@
 
     core_base = dispatcher[axis][dtype]
     py_base = PyMatrixNaiveBase
 
     class _concatenate(core_base, py_base):
         def __init__(self):
             self.mats = mats
-            core_base.__init__(self, self.mats, n_threads)
+            core_base.__init__(self, self.mats)
             py_base.__init__(self, n_threads=n_threads)
 
     return _concatenate()
 
 
 def dense(
     mat: np.ndarray,
     *,
     method: str ="naive",
+    copy: bool =False,
     n_threads: int =1,
 ):
     """Creates a viewer of a dense matrix.
     
     Parameters
     ----------
     mat : np.ndarray
@@ -361,27 +366,31 @@
     method : str, optional
         Method type. It must be one of the following:
 
             - ``"naive"``: naive method.
             - ``"cov"``: covariance method.
 
         Default is ``"naive"``.
+    copy : bool, optional
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixCovBase64
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixCovDense64F
+    adelie.adelie_core.matrix.MatrixNaiveDense64F
     """
     naive_dispatcher = {
         np.dtype("float64"): {
             "C": core.matrix.MatrixNaiveDense64C,
             "F": core.matrix.MatrixNaiveDense64F,
         },
         np.dtype("float32"): {
@@ -423,57 +432,54 @@
     py_base = {
         "naive" : PyMatrixNaiveBase,
         "cov" : PyMatrixCovBase,
     }[method]
 
     class _dense(core_base, py_base):
         def __init__(self):
-            self.mat = mat
+            self.mat = np.array(mat, copy=copy)
             core_base.__init__(self, self.mat, n_threads)
             py_base.__init__(self, n_threads=n_threads)
 
     return _dense()
 
 
 def interaction(
     mat: np.ndarray,
     intr_map: dict,
-    *,
     levels: np.ndarray =None,
+    *,
+    copy: bool =False,
     n_threads: int =1,
 ):
-    """Creates a viewer of a matrix with pairwise interactions.
+    """Creates a matrix with pairwise interactions.
 
     This matrix :math:`X \\in \\mathbb{R}^{n\\times p}` represents pairwise interaction terms
     within a given base matrix :math:`Z \\in \\mathbb{R}^{n\\times d}` 
     where the interaction structure is defined as follows.
     We assume :math:`Z` contains, in general, a combination of
     continuous and discrete features (as columns).
     Denote :math:`L : \\{1,\\ldots, d\\} \\to \\mathbb{N}` as
-    the mapping that maps each feature index of :math:`Z` to the number of levels of that feature,
+    the mapping that maps each feature index of :math:`Z` to the number of levels of that feature
     where a value of :math:`0` means the feature is continuous
     and otherwise means it is discrete with that many levels (or categories).
     Let :math:`S \\subseteq \\{1,\\ldots, d\\}^2` denote the set of
     valid and unique pairs of feature indices of :math:`Z`.
     A pair is *valid* if the two values are not equal.
     We define uniqueness up to ordering so that :math:`(x,y)` and :math:`(y,x)` are considered the same pairs.
     Finally, for each pair :math:`(i, j) \\in S`,
-    define the interaction term :math:`X_{i:j}` as
+    define the interaction term :math:`Z_{i:j}` as
 
     .. math::
         \\begin{align*}
-            X_{i:j}
+            Z_{i:j}
             &:=
             \\begin{cases}
                 \\begin{bmatrix}
-                    \\mathbf{1} & Z_{i}
-                \\end{bmatrix}
-                \\star
-                \\begin{bmatrix}
-                    \\mathbf{1} & Z_{j}
+                    Z_{i} & Z_{j} & Z_i \\odot Z_j
                 \\end{bmatrix}
                 ,& L(i) = 0, L(j) = 0 \\\\
                 \\begin{bmatrix}
                     \\mathbf{1} & Z_{i}
                 \\end{bmatrix}
                 \\star
                 I_{Z_{j}}
@@ -506,55 +512,62 @@
                 A_{1} \\odot B_{2} &
                 \\cdots &
                 A_{d_A} \\odot B_{2} &
                 \\cdots
             \\end{bmatrix}
         \\end{align*}
 
-    Then, :math:`X` is defined as the column-wise concatenation of :math:`X_{i:j}`.
+    Then, :math:`X` is defined as the column-wise concatenation of :math:`Z_{i:j}`
+    in lexicographical order of :math:`(i,j) \\in S`.
 
     .. note::
-        Every discrete feature of `Z` *must* take on values in the range :math:`[0, \\ell)`
+        Every discrete feature of `Z` *must* take on values in the set 
+        :math:`\\{0, \\ldots, \\ell-1\\}`
         where :math:`\\ell` is the number of levels for that feature.
 
     .. note::
         This matrix only works for naive method!
 
     Parameters
     ----------
     mat : (n, d) np.ndarray
         The dense matrix :math:`Z` from which to construct interaction terms.
     intr_map : dict
         Dictionary mapping a column index of ``mat``
         to a list of (column) indices to pair with.
         If the value of a key-value pair is ``None``,
         then every column is paired with the key.
-        Internally, only valid and unique (as defined above) pairs are registered.
+        Internally, only valid and unique (as defined above) pairs are registered
+        to construct :math:`S`.
         Moreover, the pairs are stored in lexicographical order of ``(key, val)``
         for each ``val`` in ``intr_map[key]`` and for each ``key``.
     levels : (d,) np.ndarray, optional
         Number of levels for each column in ``mat``.
         A non-positive value indicates that the column is a continuous variable
         whereas a positive value indicates that it is a discrete variable with
         that many levels (or categories).
         If ``None``, it is initialized to be ``np.zeros(d)``
         so that every column is a continuous variable.
         Default is ``None``.
+    copy : bool, optional
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveInteractionDense64F
     """
     dispatcher = {
         np.dtype("float64"): {
             "C": core.matrix.MatrixNaiveInteractionDense64C,
             "F": core.matrix.MatrixNaiveInteractionDense64F,
         },
         np.dtype("float32"): {
@@ -610,30 +623,31 @@
             pairs_seen.add((key, val))
     if len(pairs) <= 0:
         raise ValueError("No valid pairs exist. There must be at least one valid pair.")
     pairs = np.array(pairs, dtype=np.int32)
 
     class _interaction(core_base, py_base):
         def __init__(self):
-            self.mat = mat
+            self.mat = np.array(mat, copy=copy)
             self.pairs = pairs
-            self.levels = np.array(levels, copy=False, dtype=np.int32)
+            self.levels = np.array(levels, copy=True, dtype=np.int32)
             core_base.__init__(self, self.mat, self.pairs, self.levels, n_threads)
             py_base.__init__(self, n_threads=n_threads)
         
     return _interaction()
 
 
 def kronecker_eye(
     mat: Union[np.ndarray, MatrixNaiveBase32, MatrixNaiveBase64],
     K: int,
     *,
+    copy: bool =False,
     n_threads: int =1,
 ):
-    """Creates a viewer of a matrix Kronecker product identity matrix.
+    """Creates a Kronecker product with identity matrix.
 
     The matrix is represented as :math:`X \\otimes I_K`
     where :math:`X` is the underlying dense matrix and 
     :math:`I_K` is the identity matrix of dimension :math:`K`.
 
     .. note::
         This matrix only works for naive method!
@@ -641,26 +655,32 @@
     Parameters
     ----------
     mat : Union[np.ndarray, MatrixNaiveBase32, MatrixNaiveBase64]
         The matrix to view as a Kronecker product with identity matrix.
         If ``np.ndarray``, a specialized class is created with more optimized routines.
     K : int
         Dimension of the identity matrix.
+    copy : bool, optional
+        This argument is only used if ``mat`` is a ``np.ndarray``.
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveKroneckerEye64
+    adelie.adelie_core.matrix.MatrixNaiveKroneckerEyeDense64F
     """
     if isinstance(mat, np.ndarray):
         dispatcher = {
             np.dtype("float64"): {
                 "C": core.matrix.MatrixNaiveKroneckerEyeDense64C,
                 "F": core.matrix.MatrixNaiveKroneckerEyeDense64F,
             },
@@ -672,14 +692,15 @@
         dtype = mat.dtype
         order = (
             "C"
             if mat.flags.c_contiguous else
             "F"
         )
         core_base = dispatcher[dtype][order]
+        mat = np.array(mat, copy=copy)
     else:
         dispatcher = {
             np.float64: core.matrix.MatrixNaiveKroneckerEye64,
             np.float32: core.matrix.MatrixNaiveKroneckerEye32,
         }
         dtype = _to_dtype(mat)
         core_base = dispatcher[dtype]
@@ -690,20 +711,134 @@
             self.mat = mat
             core_base.__init__(self, self.mat, K, n_threads)
             py_base.__init__(self, n_threads=n_threads)
 
     return _kronecker_eye()
 
 
+def one_hot(
+    mat: np.ndarray,
+    levels: np.ndarray =None,
+    *,
+    copy: bool =False,
+    n_threads: int =1,
+):
+    """Creates a one-hot encoded matrix.
+
+    This matrix :math:`X \\in \\mathbb{R}^{n \\times p}`
+    represents a one-hot encoding of a given base matrix
+    :math:`Z \\in \\mathbb{R}^{n \\times d}`.
+    We assume :math:`Z` contains, in general, a combination of
+    continuous and discrete features (as columns).
+    Denote :math:`L : \\{1, \\ldots, d\\} \\to \\mathbb{N}` as
+    the mapping that maps each feature index of :math:`Z` to the number of levels of that feature
+    where a value of :math:`0` means the feature is continuous
+    and otherwise means it is discrete with that many levels (or categories).
+    For every :math:`j` th column of :math:`Z`,
+    define the possibly one-hot encoded version :math:`\\tilde{Z}_j` as
+
+    .. math::
+        \\begin{align*}
+            \\tilde{Z}_j
+            &:=
+            \\begin{cases}
+                Z_j ,& L(j) = 0 \\\\
+                I_{Z_j} ,& L(j) > 0
+            \\end{cases}
+        \\end{align*}
+
+    Here, :math:`I_{v}` is the indicator matrix, or one-hot encoding, of :math:`v`.
+
+    Then, :math:`X` is defined as the column-wise concatenation of :math:`\\tilde{Z}_j`
+    in order of :math:`j`.
+
+    .. note::
+        Every discrete feature of `Z` *must* take on values in the set 
+        :math:`\\{0, \\ldots, \\ell-1\\}`
+        where :math:`\\ell` is the number of levels for that feature.
+
+    .. note::
+        This matrix only works for naive method!
+    
+    Parameters
+    ----------
+    mat : (n, d) np.ndarray
+        The dense matrix :math:`Z` from which to construct one-hot encodings.
+    levels : (d,) np.ndarray, optional
+        Number of levels for each column in ``mat``.
+        A non-positive value indicates that the column is a continuous variable
+        whereas a positive value indicates that it is a discrete variable with
+        that many levels (or categories).
+        If ``None``, it is initialized to be ``np.zeros(d)``
+        so that every column is a continuous variable.
+        Default is ``None``.
+    copy : bool, optional
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
+    n_threads : int, optional
+        Number of threads.
+        Default is ``1``.
+
+    Returns
+    -------
+    wrap
+        Wrapper matrix object.
+
+    See Also
+    --------
+    adelie.adelie_core.matrix.MatrixNaiveOneHotDense64F
+    """
+    dispatcher = {
+        np.dtype("float64"): {
+            "C": core.matrix.MatrixNaiveOneHotDense64C,
+            "F": core.matrix.MatrixNaiveOneHotDense64F,
+        },
+        np.dtype("float32"): {
+            "C": core.matrix.MatrixNaiveOneHotDense32C,
+            "F": core.matrix.MatrixNaiveOneHotDense32F,
+        },
+    }
+    dtype = mat.dtype
+    order = (
+        "F"
+        # prioritize choosing Fortran contiguity
+        if mat.flags.f_contiguous else
+        "C"
+    )
+    if order == "C":
+        warnings.warn(
+            "Detected matrix to be C-contiguous. "
+            "Performance may improve with F-contiguous matrix."
+        )
+    core_base = dispatcher[dtype][order]
+    py_base = PyMatrixNaiveBase
+
+    _, d = mat.shape
+
+    if levels is None:
+        levels = np.zeros(d, dtype=int)
+
+    class _one_hot(core_base, py_base):
+        def __init__(self):
+            self.mat = np.array(mat, copy=copy)
+            self.levels = np.array(levels, copy=True, dtype=np.int32)
+            core_base.__init__(self, self.mat, self.levels, n_threads)
+            py_base.__init__(self, n_threads=n_threads)
+        
+    return _one_hot()
+
+
 def lazy_cov(
     mat: np.ndarray,
     *,
+    copy: bool =False,
     n_threads: int =1,
 ):
-    """Creates a viewer of a lazy covariance matrix.
+    """Creates a lazy covariance matrix.
 
     The lazy covariance matrix :math:`A` uses 
     the underlying matrix :math:`X` given by ``mat``
     to compute the values of :math:`A` dynamically.
     It only computes rows of :math:`A`
     on-the-fly that are needed when calling its member functions.
     This is useful in ``adelie.solver.gaussian_cov`` where
@@ -713,26 +848,30 @@
     .. note::
         This matrix only works for covariance method!
 
     Parameters
     ----------
     mat : (n, p) np.ndarray
         The data matrix from which to lazily compute the covariance.
+    copy : bool, optional
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixCovBase64
+    adelie.adelie_core.matrix.MatrixCovLazyCov64F
     """
     dispatcher = {
         np.dtype("float64"): {
             "C": core.matrix.MatrixCovLazyCov64C,
             "F": core.matrix.MatrixCovLazyCov64F,
         },
         np.dtype("float32"): {
@@ -748,15 +887,15 @@
         "F"
     )
     core_base = dispatcher[dtype][order]
     py_base = PyMatrixCovBase
 
     class _lazy_cov(core_base, py_base):
         def __init__(self):
-            self.mat = mat
+            self.mat = np.array(mat, copy=copy)
             core_base.__init__(self, self.mat, n_threads)
             py_base.__init__(self, n_threads=n_threads)
 
     return _lazy_cov()
 
 
 def snp_phased_ancestry(
@@ -794,15 +933,15 @@
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
     adelie.io.snp_phased_ancestry
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveSNPPhasedAncestry64
     """
     dispatcher = {
         np.float64: core.matrix.MatrixNaiveSNPPhasedAncestry64,
         np.float32: core.matrix.MatrixNaiveSNPPhasedAncestry32,
     }
     core_base = dispatcher[dtype]
     py_base = PyMatrixNaiveBase
@@ -850,15 +989,15 @@
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
     adelie.io.snp_unphased
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveSNPUnphased64
     """
     dispatcher = {
         np.float64: core.matrix.MatrixNaiveSNPUnphased64,
         np.float32: core.matrix.MatrixNaiveSNPUnphased32,
     }
     core_base = dispatcher[dtype]
     py_base = PyMatrixNaiveBase
@@ -871,14 +1010,15 @@
     return _snp_unphased()
 
 
 def sparse(
     mat: Union[csc_matrix, csr_matrix],
     *,
     method: str ="naive",
+    copy: bool =False,
     n_threads: int =1,
 ):
     """Creates a viewer of a sparse matrix.
 
     .. note::
         Regardless of the storage order of the input matrix,
         we internally convert the matrix to CSC order for performance reasons.
@@ -890,37 +1030,43 @@
     method : str, optional
         Method type. It must be one of the following:
 
             - ``"naive"``: naive method.
             - ``"cov"``: covariance method.
 
         Default is ``"naive"``.
+    copy : bool, optional
+        If ``True``, a copy of ``mat`` is stored internally.
+        Otherwise, a reference is stored instead.
+        Default is ``False``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
         Wrapper matrix object.
 
     See Also
     --------
-    adelie.matrix.MatrixCovBase64
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixCovSparse64F
+    adelie.adelie_core.matrix.MatrixNaiveSparse64F
     """
     if not (isinstance(mat, csr_matrix) or isinstance(mat, csc_matrix)):
         raise TypeError("mat must be scipy.sparse.csr_matrix or scipy.sparse.csc_matrix.")
 
-    mat.prune()
-    mat.sort_indices()
-
     if isinstance(mat, csr_matrix):
         warnings.warn("Converting to CSC format.")
         mat = mat.tocsc(copy=True)
+    elif copy:
+        mat = mat.copy()
+
+    mat.prune()
+    mat.sort_indices()
 
     naive_dispatcher = {
         np.dtype("float64"): core.matrix.MatrixNaiveSparse64F,
         np.dtype("float32"): core.matrix.MatrixNaiveSparse32F,
     }
     
     cov_dispatcher = {
@@ -954,14 +1100,141 @@
                 n_threads,
             )
             py_base.__init__(self, n_threads=n_threads)
 
     return _sparse()
 
 
+def standardize(
+    mat: Union[np.ndarray, MatrixNaiveBase32, MatrixNaiveBase64],
+    centers: np.ndarray =None,
+    scales: np.ndarray =None,
+    ddof: int =0,
+    *,
+    n_threads: int =1,
+):
+    """Creates a standardized matrix.
+
+    Given a matrix :math:`Z \\in \\mathbb{R}^{n \\times p}`,
+    the standardized matrix :math:`X \\in \\mathbb{R}^{n \\times p}`
+    of :math:`Z` centered by :math:`c \\in \\mathbb{R}^{p}` and scaled by :math:`s \\in \\mathbb{R}^p`
+    is defined by 
+    
+    .. math::
+        \\begin{align*}
+            X = (Z - \\mathbf{1} c^\\top) \\mathrm{diag}(s)^{-1}
+        \\end{align*}
+
+    We define the column means :math:`\\overline{Z} \\in \\mathbb{R}^p` to be
+
+    .. math::
+        \\begin{align*}
+            \\overline{Z}
+            =
+            \\frac{1}{n} Z^\\top \\mathbf{1}
+        \\end{align*}
+
+    Lastly, we define the column standard deviations :math:`\\hat{\\sigma} \\in \\mathbb{R}^p` to be
+
+    .. math::
+        \\begin{align*}
+            \\hat{\\sigma}_j
+            =
+            \\frac{1}{\\sqrt{n - \\mathrm{df}}} \\|Z_{\\cdot j} - c_j \\mathbf{1} \\|_2
+        \\end{align*}
+
+    where :math:`\\mathrm{df}` is the degrees of freedom given by ``ddof``.
+
+    .. note::
+        This matrix only works for naive method!
+    
+    Parameters
+    ----------
+    mat : Union[np.ndarray, MatrixNaiveBase32, MatrixNaiveBase64]
+        The underlying matrix :math:`Z` to standardize.
+    centers : np.ndarray, optional
+        The center values :math:`c` for each column of ``mat``.
+        If ``None``, the column means :math:`\\overline{Z}` are used as centers.
+        Default is ``None``.
+    scales : np.ndarray, optional
+        The scale values :math:`s` for each column of ``mat``.
+        If ``None``, the column standard deviations :math:`\\hat{\\sigma}` are used as scales.
+        Default is ``None``.
+    ddof : int, optional
+        The degrees of freedom used to compute ``scales``.
+        This is only used if ``scales`` is ``None``.
+        Default is ``0``.
+    n_threads : int, optional
+        Number of threads.
+        Default is ``1``.
+
+    Returns
+    -------
+    wrap
+        Wrapper matrix object.
+
+    See Also
+    --------
+    adelie.adelie_core.matrix.MatrixNaiveStandardize64
+    """
+    if isinstance(mat, (list, np.ndarray)):
+        mat = np.ndarray(mat, order="F", copy=True)
+        if centers is None:
+            centers = np.mean(mat, axis=0)
+        mat -= centers[None]
+        if scales is None:
+            n = mat.shape[0]
+            scales = np.sqrt(
+                np.sum(mat ** 2, axis=0) / (n - ddof)
+            )
+        mat /= scales[None]
+        return mat
+
+    dtype = _to_dtype(mat)
+    dispatcher = {
+        np.float32: core.matrix.MatrixNaiveStandardize32,
+        np.float64: core.matrix.MatrixNaiveStandardize64,
+    }
+    core_base = dispatcher[dtype]
+    py_base = PyMatrixNaiveBase
+
+    n, p = mat.shape
+    sqrt_weights = np.full(n, 1/np.sqrt(n), dtype=dtype) 
+    is_centers_none = centers is None
+
+    if is_centers_none:
+        centers = np.empty(p, dtype=dtype) 
+        mat.mul(sqrt_weights, sqrt_weights, centers)
+
+    if scales is None:
+        if is_centers_none:
+            means = centers
+        else:
+            means = np.empty(p, dtype=dtype) 
+            mat.mul(sqrt_weights, sqrt_weights, means)
+
+        vars = np.empty((p, 1, 1), dtype=dtype, order="F")
+        buffer = np.empty((n, 1), dtype=dtype, order="F")
+        for j in range(p):
+            mat.cov(j, 1, sqrt_weights, vars[j], buffer) 
+        vars = vars.reshape(p)
+        vars += centers * (centers - 2 * means)
+        scales = np.sqrt((n / (n - ddof)) * vars)
+
+    class _standardize(core_base, py_base):
+        def __init__(self):
+            self.mat = mat
+            self.centers = np.array(centers, copy=True, dtype=dtype)
+            self.scales = np.array(scales, copy=True, dtype=dtype)
+            core_base.__init__(self, mat, self.centers, self.scales, n_threads)
+            py_base.__init__(self, n_threads=n_threads)
+        
+    return _standardize()
+
+
 def subset(
     mat: Union[np.ndarray, MatrixNaiveBase32, MatrixNaiveBase64],
     indices: np.ndarray,
     *,
     axis: int=0,
     n_threads: int =1,
 ):
@@ -1012,15 +1285,16 @@
     -------
     wrap
         Wrapper matrix object.
         If ``mat`` is ``np.ndarray`` then the usual numpy subsetted matrix is returned.
 
     See Also
     --------
-    adelie.matrix.MatrixNaiveBase64
+    adelie.adelie_core.matrix.MatrixNaiveCSubset64
+    adelie.adelie_core.matrix.MatrixNaiveRSubset64
     """
     if isinstance(mat, np.ndarray):
         if axis == 0:
             return mat[indices]
         else:
             return mat[:, indices]
 
@@ -1041,11 +1315,12 @@
 
     core_base = dispatcher[axis][dtype]
     py_base = PyMatrixNaiveBase
 
     class _subset(core_base, py_base):
         def __init__(self):
             self.mat = mat
-            core_base.__init__(self, mat, indices, n_threads)
+            self.indices = np.array(indices, copy=True, dtype=np.int32)
+            core_base.__init__(self, mat, self.indices, n_threads)
             py_base.__init__(self, n_threads=n_threads)
         
     return _subset()
```

### Comparing `adelie-1.1.31/adelie/solver.py` & `adelie-1.1.32/adelie/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
     check_state: bool =False,
     progress_bar: bool =True,
     warm_start =None,
     exit_cond: Callable =None,
 ):
-    """Gaussian elastic net solver via covariance method.
+    """Solves Gaussian group elastic net via covariance method.
 
     The Gaussian elastic net problem via covariance method minimizes the following:
 
     .. math::
         \\begin{align*}
             \\mathrm{minimize}_{\\beta} \\quad&
             \\frac{1}{2} \\beta^\\top A \\beta - v^\\top \\beta
@@ -420,15 +420,15 @@
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
     check_state: bool =False,
     progress_bar: bool =True,
     warm_start =None,
     exit_cond: Callable =None,
 ):
-    """Group elastic net solver.
+    """Solves group elastic net via naive method.
 
     The group elastic net problem minimizes the following:
 
     .. math::
         \\begin{align*}
             \\mathrm{minimize}_{\\beta, \\beta_0} \\quad&
             \\ell(\\eta)
```

### Comparing `adelie-1.1.31/adelie/src/adelie_core.cpp` & `adelie-1.1.32/adelie/src/adelie_core.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 
     py::bind_vector<std::vector<ad::util::rowmat_type<double>>>(m, "VectorMatrix64");
     py::bind_vector<std::vector<ad::util::rowmat_type<float>>>(m, "VectorMatrix32");
 
     auto m_bcd = m.def_submodule("bcd", "BCD submodule.");
     register_bcd(m_bcd);
 
-    register_configs(m);
+    auto m_configs = m.def_submodule("configs", "Configurations submodule.");
+    register_configs(m_configs);
 
     auto m_glm = m.def_submodule("glm", "GLM submodule.");
     register_glm(m_glm);
 
     auto m_io = m.def_submodule("io", "IO submodule.");
     register_io(m_io);
 
     auto m_matrix = m.def_submodule("matrix", "Matrix submodule.");
     register_matrix(m_matrix);
 
+    auto m_matrix_utils = m_matrix.def_submodule("utils", "Matrix utility submodule.");
+    register_matrix_utils(m_matrix_utils);
+
     auto m_optimization = m.def_submodule("optimization", "Optimization submodule.");
     register_optimization(m_optimization);
 
     auto m_solver = m.def_submodule("solver", "Grpnet submodule.");
     register_solver(m_solver);
 
     auto m_state = m.def_submodule("state", "State submodule.");
```

### Comparing `adelie-1.1.31/adelie/src/bcd.cpp` & `adelie-1.1.32/adelie/src/bcd.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/decl.hpp` & `adelie-1.1.32/adelie/src/decl.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 PYBIND11_MAKE_OPAQUE(std::vector<adelie_core::util::rowmat_type<float>>);
 
 namespace py = pybind11;
 
 void register_bcd(py::module_&);
 void register_configs(py::module_&);
 void register_matrix(py::module_&);
+void register_matrix_utils(py::module_&);
 void register_optimization(py::module_&);
 void register_state(py::module_&);
 void register_solver(py::module_&);
 void register_io(py::module_&);
 void register_glm(py::module_&);
```

### Comparing `adelie-1.1.31/adelie/src/glm.cpp` & `adelie-1.1.32/adelie/src/glm.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -115,42 +115,42 @@
         )delimiter")
         .def(py::init<
             const string_t&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >(),
             py::arg("name"),
-            py::arg("y"),
-            py::arg("weights")
+            py::arg("y").noconvert(),
+            py::arg("weights").noconvert()
         )
         .def_readonly("name", &internal_t::name, R"delimiter(
-            Name of the GLM family.
+        Name of the GLM family.
         )delimiter")
         .def_readonly("is_multi", &internal_t::is_multi, R"delimiter(
-            See ``adelie.glm.GlmMultiBase64``.
-            It is always ``False`` for this base class.
+        See ``adelie.adelie_core.glm.GlmMultiBase64``.
+        It is always ``False`` for this base class.
         )delimiter")
         .def_readonly("is_symmetric", &internal_t::is_symmetric, R"delimiter(
-            See ``adelie.glm.GlmMultiBase64``.
-            It is always ``False`` for this base class.
+        See ``adelie.adelie_core.glm.GlmMultiBase64``.
+        It is always ``False`` for this base class.
         )delimiter")
         .def("gradient", &internal_t::gradient, R"delimiter(
-        Gradient of the negative loss function.
+        Computes the gradient of the negative loss function.
 
-        Computes :math:`-\nabla \ell(\eta)`.
+        Computes the (negative) gradient :math:`-\nabla \ell(\eta)`.
 
         Parameters
         ----------
         eta : (n,) np.ndarray
             Natural parameter.
         grad : (n,) np.ndarray
             The gradient to store.
         )delimiter")
         .def("hessian", &internal_t::hessian, R"delimiter(
-        Diagonal hessian majorization of the loss function.
+        Computes a diagonal hessian majorization of the loss function.
 
         Computes a diagonal majorization of the hessian :math:`\nabla^2 \ell(\eta)`.
 
         .. note::
             Although the hessian is in general a fully dense matrix,
             we only require the user to output a diagonal matrix.
             It is recommended that the diagonal matrix dominates the full hessian.
@@ -164,15 +164,15 @@
             Natural parameter.
         grad : (n,) np.ndarray
             Gradient as in ``gradient`` method.
         hess : (n,) np.ndarray
             The hessian to store.
         )delimiter")
         .def("inv_hessian_gradient", &internal_t::inv_hessian_gradient, R"delimiter(
-        Inverse hessian of the (negative) gradient of the loss function.
+        Computes the inverse hessian of the (negative) gradient of the loss function.
 
         Computes :math:`-(\nabla^2 \ell(\eta))^{-1} \nabla \ell(\eta)`.
 
         .. note::
             Unlike the ``hessian`` method, this function may use the full hessian matrix.
             The diagonal hessian majorization is provided in case it speeds-up computations,
             but it can be ignored.
@@ -187,30 +187,30 @@
             Gradient as in ``gradient`` method.
         hess : (n,) np.ndarray
             Hessian as in ``hessian`` method.
         inv_hess_grad : (n,) np.ndarray
             The inverse hessian gradient to store.
         )delimiter")
         .def("loss", &internal_t::loss, R"delimiter(
-        Loss function.
+        Computes the loss function.
 
         Computes :math:`\ell(\eta)`.
 
         Parameters
         ----------
         eta : (n,) np.ndarray
             Natural parameter.
 
         Returns
         -------
         loss : float
             Loss.
         )delimiter")
         .def("loss_full", &internal_t::loss_full, R"delimiter(
-        Loss function at the saturated model.
+        Computes the loss function at the saturated model.
 
         Computes :math:`\ell(\eta^\star)` where :math:`\eta^\star` is the minimizer.
 
         Returns
         -------
         loss : float
             Loss at the saturated model.
@@ -220,54 +220,60 @@
 
 template <class T>
 void glm_binomial_logit(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmBinomialLogit<T>;
     using base_t = typename internal_t::base_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name, 
+        "Core GLM class for Binomial logit family."
+        )
         .def(py::init<
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >())
         ;
 }
 
 template <class T>
 void glm_binomial_probit(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmBinomialProbit<T>;
     using base_t = typename internal_t::base_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name, 
+        "Core GLM class for Binomial probit family."
+        )
         .def(py::init<
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >())
         ;
 }
 
 template <class T>
 void glm_cox(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmCox<T>;
     using base_t = typename internal_t::base_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core GLM class for Cox family."
+        )
         .def(py::init<
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>& ,
             const std::string&
         >(),
-            py::arg("start"),
-            py::arg("stop"),
-            py::arg("status"),
-            py::arg("weights"),
+            py::arg("start").noconvert(),
+            py::arg("stop").noconvert(),
+            py::arg("status").noconvert(),
+            py::arg("weights").noconvert(),
             py::arg("tie_method")
         )
         .def_readonly("start_order", &internal_t::start_order)
         .def_readonly("start_so", &internal_t::start_so)
         .def_readonly("stop_order", &internal_t::stop_order)
         .def_readonly("stop_to", &internal_t::stop_to)
         .def_readonly("status_to", &internal_t::status_to)
@@ -318,29 +324,33 @@
 
 template <class T>
 void glm_gaussian(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmGaussian<T>;
     using base_t = typename internal_t::base_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core GLM class for Gaussian family."
+        )
         .def(py::init<
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >())
         ;
 }
 
 template <class T>
 void glm_poisson(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmPoisson<T>;
     using base_t = typename internal_t::base_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core GLM class for Poisson family."
+        )
         .def(py::init<
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >())
         ;
 }
 
@@ -423,15 +433,15 @@
 {
     using trampoline_t = PyGlmMultiBase<T>;
     using internal_t = ad::glm::GlmMultiBase<T>;
     using string_t = typename internal_t::string_t;
     using rowarr_value_t = typename internal_t::rowarr_value_t;
     using vec_value_t = typename internal_t::vec_value_t;
     py::class_<internal_t, trampoline_t>(m, name, R"delimiter(
-        Base Multi-response GLM class.
+        Base multi-response GLM class.
 
         The generalized multi-response linear model is given by the (weighted) negative likelihood
         
         .. math::
             \begin{align*}
                 \ell(\eta) = \frac{1}{K} \sum\limits_{i=1}^n w_{i} \left(
                     -\sum\limits_{k=1}^K y_{ik} \eta_{ik} + A_i(\eta)
@@ -451,43 +461,43 @@
         .def(py::init<
             const string_t&,
             const Eigen::Ref<const rowarr_value_t>&,
             const Eigen::Ref<const vec_value_t>& ,
             bool
         >(),
             py::arg("name"),
-            py::arg("y"),
-            py::arg("weights"),
+            py::arg("y").noconvert(),
+            py::arg("weights").noconvert(),
             py::arg("is_symmetric")
         )
         .def_readonly("name", &internal_t::name, R"delimiter(
-            Name of the GLM family.
+        Name of the GLM family.
         )delimiter")
         .def_readonly("is_multi", &internal_t::is_multi, R"delimiter(
         ``True`` if it defines a multi-response GLM family.
         It is always ``True`` for this base class.
         )delimiter")
         .def_readonly("is_symmetric", &internal_t::is_symmetric, R"delimiter(
         ``True`` if the GLM is symmetric in :math:`\eta_{i\cdot}` (along the classes)
         for each :math:`i`.
         )delimiter")
         .def("gradient", &internal_t::gradient, R"delimiter(
-        Gradient of the negative loss function.
+        Computes the gradient of the negative loss function.
 
-        Computes :math:`-\nabla \ell(\eta)`.
+        Computes the (negative) gradient :math:`-\nabla \ell(\eta)`.
 
         Parameters
         ----------
         eta : (n, K) np.ndarray
             Natural parameter.
         grad : (n, K) np.ndarray
             The gradient to store.
         )delimiter")
         .def("hessian", &internal_t::hessian, R"delimiter(
-        Diagonal hessian majorization of the loss function.
+        Computes a diagonal hessian majorization of the loss function.
 
         Computes a diagonal majorization of the hessian :math:`\nabla^2 \ell(\eta)`.
 
         .. note::
             Although the hessian is in general a fully dense matrix,
             we only require the user to output a diagonal matrix.
             It is recommended that the diagonal matrix dominates the full hessian.
@@ -501,15 +511,15 @@
             Natural parameter.
         grad : (n, K) np.ndarray
             Gradient as in ``gradient`` method.
         hess : (n, K) np.ndarray
             The hessian to store.
         )delimiter")
         .def("inv_hessian_gradient", &internal_t::inv_hessian_gradient, R"delimiter(
-        Inverse hessian of the (negative) gradient of the loss function.
+        Computes the inverse hessian of the (negative) gradient of the loss function.
 
         Computes :math:`-(\nabla^2 \ell(\eta))^{-1} \nabla \ell(\eta)`.
 
         .. note::
             Unlike the ``hessian`` method, this function may use the full hessian matrix.
             The diagonal hessian majorization is provided in case it speeds-up computations,
             but it can be ignored.
@@ -524,30 +534,30 @@
             Gradient as in ``gradient`` method.
         hess : (n, K) np.ndarray
             Hessian as in ``hessian`` method.
         inv_hess_grad : (n, K) np.ndarray
             The inverse hessian gradient to store.
         )delimiter")
         .def("loss", &internal_t::loss, R"delimiter(
-        Loss function.
+        Computes the loss function.
 
         Computes :math:`\ell(\eta)`.
 
         Parameters
         ----------
         eta : (n, K) np.ndarray
             Natural parameter.
 
         Returns
         -------
         loss : float
             Loss.
         )delimiter")
         .def("loss_full", &internal_t::loss_full, R"delimiter(
-        Loss function at the saturated model.
+        Computes the loss function at the saturated model.
 
         Computes :math:`\ell(\eta^\star)` where :math:`\eta^\star` is the minimizer.
 
         Returns
         -------
         loss : float
             Loss at the saturated model.
@@ -558,30 +568,34 @@
 template <class T>
 void glm_multigaussian(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmMultiGaussian<T>;
     using base_t = typename internal_t::base_t;
     using rowarr_value_t = typename internal_t::rowarr_value_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core GLM class for MultiGaussian family."
+        )
         .def(py::init<
             const Eigen::Ref<const rowarr_value_t>&,
             const Eigen::Ref<const vec_value_t>& 
         >())
         ;
 }
 
 template <class T>
 void glm_multinomial(py::module_& m, const char* name)
 {
     using internal_t = ad::glm::GlmMultinomial<T>;
     using base_t = typename internal_t::base_t;
     using rowarr_value_t = typename internal_t::rowarr_value_t;
     using vec_value_t = typename internal_t::vec_value_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core GLM class for Multinomial family."
+        )
         .def(py::init<
             const Eigen::Ref<const rowarr_value_t>&,
             const Eigen::Ref<const vec_value_t>&
         >())
         ;
 }
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/admm.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/admm.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -43,51 +43,51 @@
         // x-update
         Eigen::Map<vec_value_t> zmu(buff.data(), m);
         Eigen::Map<vec_value_t> linear_curr(buff.data() + m, d);
         Eigen::Map<vec_value_t> QTx(buff.data() + m+d, d);
         Eigen::Map<vec_value_t> x_buffer1(buff.data() + m+2*d, d);
         Eigen::Map<vec_value_t> x_buffer2(buff.data() + m+3*d, d);
         zmu = z - u;
-        linear_curr.matrix().noalias() = zmu.matrix() * AQ_c;
+        linear_curr.matrix() = zmu.matrix() * AQ_c;
         linear_curr = QTv_c + rho * linear_curr;
         size_t x_iters;
         unconstrained::newton_abs_solver(
             quad_c,
             linear_curr,
             l1,
             l2,
             1e-12,
             1000,
             QTx,
             x_iters,
             x_buffer1,
             x_buffer2
         );
-        x.matrix().noalias() = QTx.matrix() * Q_c.transpose();
+        x.matrix() = QTx.matrix() * Q_c.transpose();
 
         // z-update
         Eigen::Map<vec_value_t> Ax(buff.data(), m);
         Eigen::Map<vec_value_t> z_prev(buff.data()+m, m);
-        Ax.matrix().noalias() = x.matrix() * A.transpose();
+        Ax.matrix() = x.matrix() * A.transpose();
         z_prev = z;
         z = (u + Ax).min(b);
 
         // u-update
         Eigen::Map<vec_value_t> r(buff.data()+2*m, m);
         r = Ax - z;
         u += r;
 
         // check convergence
         Eigen::Map<vec_value_t> s(buff.data()+3*m, d);
-        s.matrix().noalias() = (z - z_prev).matrix() * A;
+        s.matrix() = (z - z_prev).matrix() * A;
         const auto eps_pri = std::sqrt(m) * tol_abs + tol_rel * std::max<value_t>(
             Ax.matrix().norm(), z.matrix().norm()
         );
         Eigen::Map<vec_value_t> ATu(buff.data()+3*m+d, d);
-        ATu.matrix().noalias() = u.matrix() * A;
+        ATu.matrix() = u.matrix() * A;
         const auto eps_dual = std::sqrt(d) * tol_abs + tol_rel * rho * ATu.matrix().norm();
         if (
             (r.square().sum() <= eps_pri * eps_pri) &&
             (rho * rho * s.square().sum() <= eps_dual * eps_dual)
         ) break;
     }
 }
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     {
         Eigen::Map<vec_value_t> x_uncnstr(buff.data()+2*d, d);
         size_t x_iters;
         unconstrained::newton_abs_solver(
             quad, linear, l1, l2, newton_tol, newton_max_iters, 
             x_uncnstr, x_iters, x_buffer1, x_buffer2
         );
-        x_buffer1.matrix().noalias() = x_uncnstr.matrix() * A.transpose();
+        x_buffer1.matrix() = x_uncnstr.matrix() * A.transpose();
         // if unconstrained solution is feasible
         if ((x_buffer1 <= b).all()) {
             x = x_uncnstr;
             mu.setZero();
             mu_resid = v;
             mu_rsq = v.square().sum();
             return;
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/constrained/proximal_newton.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     }
 
     while (iters < max_iters) {
         ++iters;
 
         // compute v - A^T mu
         if (recompute_mu_resid) {
-            mu_resid.matrix().noalias() = mu.matrix() * A;
+            mu_resid.matrix() = mu.matrix() * A;
             mu_resid = v - mu_resid;
         }
 
         // compute x^star(mu)
         {
             size_t x_iters;
             unconstrained::newton_abs_solver(
@@ -128,15 +128,15 @@
             // then check passed and 0 is a valid primal solution.
             // TODO: generalize this constant.
             if (mu_loss <= l1 * (0.5+5e-5)) return;
             continue;
         }
 
         // compute (negative) gradient
-        grad.matrix().noalias() = x.matrix() * A.transpose();
+        grad.matrix() = x.matrix() * A.transpose();
         grad -= b;
 
         // check convergence
         if (is_prev_valid) {
             const auto convg_meas = std::abs(
                 ((mu-mu_prev) * (grad_prev-grad)).sum()
             ) / m;
@@ -158,15 +158,15 @@
         // Method 2: poor approximation
         //hess = (x_norm * x_buffer2.maxCoeff()) * AAT;
 
         // Method 3: cache ASA^T
         hess = (1 - l1 * x_buffer2).maxCoeff() * hess_buff;
 
         alpha_tmp = (x * x_buffer2) / x_norm;
-        alpha.matrix().noalias() = alpha_tmp.matrix() * A.transpose();
+        alpha.matrix() = alpha_tmp.matrix() * A.transpose();
         const auto l1_kappa_norm = l1 * x_norm / (x * x_buffer1 * alpha_tmp).sum();
         hess.noalias() += l1_kappa_norm * alpha.matrix().transpose() * alpha.matrix();
 
         // save old values
         mu_prev = mu;
         grad_prev = grad;
         is_prev_valid = true;
@@ -179,15 +179,15 @@
             nnls_iters, mu, grad, loss, [](){return false;}
         ); 
         recompute_mu_resid = true;
     }
 
     // compute v - A^T mu
     if (recompute_mu_resid) {
-        mu_resid.matrix().noalias() = mu.matrix() * A;
+        mu_resid.matrix() = mu.matrix() * A;
         mu_resid = v - mu_resid;
     }
     size_t x_iters;
     unconstrained::newton_abs_solver(
         quad, mu_resid, l1, l2, newton_tol, newton_max_iters, 
         x, x_iters, x_buffer1, x_buffer2
     );
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/brent.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/ista.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/unconstrained/newton.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/bcd/utils.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/bcd/utils.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_binomial.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_binomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_cox.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_cox.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_gaussian.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_gaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multibase.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multibase.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_multinomial.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_multinomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/glm/glm_poisson.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/glm/glm_poisson.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -68,28 +68,38 @@
     }
 
     outer_t cols() const
     {
         return snps() * ancestries();
     }
 
-    Eigen::Ref<const vec_outer_t> nnz() const 
+    Eigen::Ref<const vec_outer_t> nnz0() const 
     {
         if (!_is_read) throw_no_read();
         constexpr size_t slice = sizeof(bool_t) + 2 * sizeof(outer_t) + sizeof(chunk_inner_t);
         return Eigen::Map<const vec_outer_t>(
             reinterpret_cast<const outer_t*>(&_buffer[slice]),
-            n_haps * snps()
+            cols()
+        );
+    }
+
+    Eigen::Ref<const vec_outer_t> nnz1() const 
+    {
+        if (!_is_read) throw_no_read();
+        const size_t slice = sizeof(bool_t) + (2 + cols()) * sizeof(outer_t) + sizeof(chunk_inner_t);
+        return Eigen::Map<const vec_outer_t>(
+            reinterpret_cast<const outer_t*>(&_buffer[slice]),
+            cols()
         );
     }
 
     Eigen::Ref<const vec_outer_t> outer() const
     {
         if (!_is_read) throw_no_read();
-        const size_t slice = sizeof(bool_t) + (2 + n_haps * snps()) * sizeof(outer_t) + sizeof(chunk_inner_t);
+        const size_t slice = sizeof(bool_t) + 2 * (1 + cols()) * sizeof(outer_t) + sizeof(chunk_inner_t);
         return Eigen::Map<const vec_outer_t>(
             reinterpret_cast<const outer_t*>(&_buffer[slice]),
             snps() + 1
         );
     }
 
     Eigen::Ref<const buffer_t> col(int j) const
@@ -110,24 +120,33 @@
         );
         return (
             _col_anc + 
             reinterpret_cast<const outer_t*>(_col_anc)[hap]
         );
     }
 
+    inner_t n_chunks(int j, int anc, int hap) const
+    {
+        const auto* _col_anc_hap = col_anc_hap(j, anc, hap);
+        return *reinterpret_cast<const inner_t*>(_col_anc_hap);
+    }
+
+    iterator begin(int j, int anc, int hap, int chunk) const
+    {
+        return iterator(chunk, col_anc_hap(j, anc, hap));
+    }
+
     iterator begin(int j, int anc, int hap) const
     {
-        return iterator(0, col_anc_hap(j, anc, hap));
+        return begin(j, anc, hap, 0);
     }
 
     iterator end(int j, int anc, int hap) const
     {
-        const auto* _col_anc_hap = col_anc_hap(j, anc, hap);
-        const auto n_chunks = *reinterpret_cast<const inner_t*>(_col_anc_hap);
-        return iterator(n_chunks, _col_anc_hap);
+        return begin(j, anc, hap, n_chunks(j, anc, hap));
     }
 
     rowarr_value_t to_dense(
         size_t n_threads
     ) const
     {
         const size_t n = rows();
@@ -147,15 +166,15 @@
                     }
                 }
             }
         };
         if (n_threads <= 1) {
             for (outer_t j = 0; j < s; ++j) routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < s; ++j) routine(j);
         }
 
         return dense;
     }
 
     std::tuple<size_t, std::unordered_map<std::string, double>> write(
@@ -196,25 +215,45 @@
         if (max_chunks >= _max_inner) {
             throw util::adelie_core_error(
                 "calldata dimensions are too large! "
             );
         } 
 
         // compute number of non-zero values
-        vec_outer_t nnz(calldata.cols());
+        vec_outer_t nnz0(s * A);
+        vec_outer_t nnz1(s * A);
         sw.start();
-        compute_nnz(calldata, nnz, n_threads);
+        compute_nnz(
+            colarr_value_t::NullaryExpr(n, s * A, [&](auto i, auto j) {
+                const auto snp = j / A;
+                const auto anc = j % A;
+                const auto k = 2 * snp;
+                return calldata(i, k) && (ancestries(i, k) == anc);
+            }),
+            nnz0, 
+            n_threads
+        );
+        compute_nnz(
+            colarr_value_t::NullaryExpr(n, s * A, [&](auto i, auto j) {
+                const auto snp = j / A;
+                const auto anc = j % A;
+                const auto k = 2 * snp + 1;
+                return calldata(i, k) && (ancestries(i, k) == anc);
+            }),
+            nnz1, 
+            n_threads
+        );
         benchmark["nnz"] = sw.elapsed();
 
         // allocate sufficient memory (upper bound on size)
         const size_t preamble_size = (
             sizeof(bool_t) +                    // endian
             2 * sizeof(outer_t) +               // n, s
             sizeof(chunk_inner_t) +             // A
-            nnz.size() * sizeof(outer_t) +      // nnz
+            (nnz0.size() + nnz1.size()) * sizeof(outer_t) + // nnz0, nnz1
             (s + 1) * sizeof(outer_t)           // outer (snps)
         );
         buffer_t buffer(
             preamble_size +
             s * A * (               // for each snp, ancestry
                 sizeof(outer_t) +       // outer (ancestry)
                 n_haps * (              // for each hap
@@ -222,27 +261,31 @@
                     sizeof(inner_t) +       // n_chunks
                     max_chunks * (          // for each chunk
                         sizeof(inner_t) +       // chunk index
                         sizeof(chunk_inner_t)   // chunk nnz - 1
                     )
                 )
             ) +
-            nnz.sum() * sizeof(chunk_inner_t)   // nnz * char
+            (nnz0.sum() + nnz1.sum()) * sizeof(chunk_inner_t)   // nnz * char
         );
 
         // populate buffer
         size_t idx = 0;
         reinterpret_cast<bool_t&>(buffer[idx]) = endian; idx += sizeof(bool_t);
         reinterpret_cast<outer_t&>(buffer[idx]) = n; idx += sizeof(outer_t);
         reinterpret_cast<outer_t&>(buffer[idx]) = s; idx += sizeof(outer_t);
         reinterpret_cast<chunk_inner_t&>(buffer[idx]) = A; idx += sizeof(chunk_inner_t);
         Eigen::Map<vec_outer_t>(
             reinterpret_cast<outer_t*>(&buffer[idx]),
-            nnz.size()
-        ) = nnz; idx += sizeof(outer_t) * nnz.size();
+            nnz0.size()
+        ) = nnz0; idx += sizeof(outer_t) * nnz0.size();
+        Eigen::Map<vec_outer_t>(
+            reinterpret_cast<outer_t*>(&buffer[idx]),
+            nnz1.size()
+        ) = nnz1; idx += sizeof(outer_t) * nnz1.size();
 
         // outer[i] = number of bytes to jump from beginning of file 
         // to start reading snp i.
         // outer[i+1] - outer[i] = total number of bytes for snp i. 
         Eigen::Map<vec_outer_t> outer(
             reinterpret_cast<outer_t*>(&buffer[idx]),
             s + 1
@@ -299,15 +342,15 @@
             }
             outer[j+1] = snp_bytes;
         };
         sw.start();
         if (n_threads <= 1) {
             for (outer_t j = 0; j < s; ++j) outer_routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < s; ++j) outer_routine(j);
         }
         benchmark["outer_time"] = sw.elapsed();
 
         // cumsum outer
         for (outer_t j = 0; j < s; ++j) outer[j+1] += outer[j];
 
@@ -391,15 +434,15 @@
                 );
             }
         };
         sw.start();
         if (n_threads <= 1) {
             for (outer_t j = 0; j < s; ++j) inner_routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < s; ++j) inner_routine(j);
         }
         benchmark["inner"] = sw.elapsed();
 
         sw.start();
         auto file_ptr = fopen_safe(_filename.c_str(), "wb");
         auto fp = file_ptr.get();
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/io/io_snp_unphased.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/io/io_snp_unphased.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,28 @@
         inner_t chunk_it,
         const char* ctg_buffer
     ):
         chunk_it(chunk_it),
         ctg_buffer(ctg_buffer),
         n_chunks(*reinterpret_cast<const inner_t*>(ctg_buffer))
     {
-        buffer_idx += sizeof(inner_t);
+        if (chunk_it >= n_chunks) return;
+
+        // increment past n_chunks and chunk_it number of chunks
+        buffer_idx = sizeof(inner_t);
+        for (int i = 0; i < chunk_it; ++i) {
+            buffer_idx += sizeof(inner_t);
+            const size_t nnz = (
+                static_cast<inner_t>(*reinterpret_cast<const chunk_inner_t*>(ctg_buffer + buffer_idx))
+                + 1
+            );
+            buffer_idx += (
+                sizeof(chunk_inner_t) + nnz * sizeof(char)
+            );
+        }
         if (n_chunks) update();
     }
 
     ADELIE_CORE_STRONG_INLINE
     IOSNPChunkIterator& operator++() { 
         buffer_idx += sizeof(char);
         ++inner;
@@ -211,24 +224,33 @@
         const auto _col = col(j);
         return (
             _col.data() +
             reinterpret_cast<const outer_t*>(_col.data())[ctg]
         );
     }
 
+    inner_t n_chunks(int j, size_t ctg) const
+    {
+        const auto* _col_ctg = col_ctg(j, ctg);
+        return *reinterpret_cast<const inner_t*>(_col_ctg);
+    }
+
+    iterator begin(int j, size_t ctg, size_t chnk) const
+    {
+        return iterator(chnk, col_ctg(j, ctg));
+    }
+
     iterator begin(int j, size_t ctg) const
     {
-        return iterator(0, col_ctg(j, ctg));
+        return begin(j, ctg, 0);
     }
 
     iterator end(int j, size_t ctg) const
     {
-        const auto* _col_ctg = col_ctg(j, ctg);
-        const auto n_chunks = *reinterpret_cast<const inner_t*>(_col_ctg);
-        return iterator(n_chunks, _col_ctg);
+        return begin(j, ctg, n_chunks(j, ctg));
     }
 
     rowarr_value_t to_dense(
         size_t n_threads
     ) const
     {
         const auto n = rows();
@@ -246,15 +268,15 @@
                     dense_j[*it] = val;
                 }
             }
         };
         if (n_threads <= 1) {
             for (outer_t j = 0; j < p; ++j) routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < p; ++j) routine(j);
         }
 
         return dense;
     }
 
     std::tuple<size_t, std::unordered_map<std::string, double>> write(
@@ -387,15 +409,15 @@
             }
             outer[j+1] = col_bytes;
         };
         sw.start();
         if (n_threads <= 1) {
             for (outer_t j = 0; j < p; ++j) outer_routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < p; ++j) outer_routine(j);
         }
         benchmark["outer_time"] = sw.elapsed();
 
         // cumsum outer
         for (outer_t j = 0; j < p; ++j) outer[j+1] += outer[j];
 
@@ -465,15 +487,15 @@
                 );
             }
         };
         sw.start();
         if (n_threads <= 1) {
             for (outer_t j = 0; j < p; ++j) inner_routine(j);
         } else {
-            #pragma omp parallel for schedule(auto) num_threads(n_threads)
+            #pragma omp parallel for schedule(static) num_threads(n_threads)
             for (outer_t j = 0; j < p; ++j) inner_routine(j);
         }
         benchmark["inner"] = sw.elapsed();
         
         sw.start();
         auto file_ptr = fopen_safe(_filename.c_str(), "wb");
         auto fp = file_ptr.get();
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/io/utils.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/io/utils.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -56,17 +56,18 @@
         for (size_t j = 0; j < p; ++j) routine(j);
     } else {
         #pragma omp parallel for schedule(static) num_threads(n_threads)
         for (size_t j = 0; j < p; ++j) routine(j);
     }
 }
 
+template <class MType>
 ADELIE_CORE_STRONG_INLINE
 void compute_nnz(
-    const Eigen::Ref<const util::colarr_type<int8_t>>& m,
+    const MType& m,
     Eigen::Ref<util::rowvec_type<uint64_t>> out,
     size_t n_threads
 )
 {
     const auto n = m.rows();
     const auto p = m.cols();
     const auto routine = [&](auto j) {
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     
 private:
     const std::vector<base_t*> _mat_list;   // (L,) list of naive matrices
     const size_t _rows;                     // number of rows
     const size_t _cols;                     // number of columns
     const vec_index_t _slice_map;           // (p,) array mapping to matrix slice
     const vec_index_t _index_map;           // (p,) array mapping to (relative) index of the slice
-    const size_t _n_threads;                // number of threads
     vec_value_t _buff;                      // (n,) buffer
 
     static inline auto init_rows(
         const std::vector<base_t*>& mat_list
     )
     {
         if (mat_list.size() == 0) {
@@ -87,31 +86,26 @@
             begin += pi;
         } 
         return index_map;
     }
 
 public:
     explicit MatrixNaiveCConcatenate(
-        const std::vector<base_t*>& mat_list,
-        size_t n_threads
+        const std::vector<base_t*>& mat_list
     ): 
         _mat_list(mat_list),
         _rows(init_rows(mat_list)),
         _cols(init_cols(mat_list)),
         _slice_map(init_slice_map(mat_list, _cols)),
         _index_map(init_index_map(mat_list, _cols)),
-        _n_threads(n_threads),
         _buff(_rows)
     {
         if (mat_list.size() <= 0) {
             throw util::adelie_core_error("mat_list must be non-empty.");
         }
-        if (n_threads < 1) {
-            throw util::adelie_core_error("n_threads must be >= 1.");
-        }
     }
 
     value_t cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
         const Eigen::Ref<const vec_value_t>& weights
     ) override
@@ -260,15 +254,14 @@
     using typename base_t::rowmat_value_t;
     using typename base_t::sp_mat_value_t;
     
 private:
     const std::vector<base_t*> _mat_list;   // (L,) list of naive matrices
     const size_t _rows;                     // number of rows
     const size_t _cols;                     // number of columns
-    const size_t _n_threads;                // number of threads (currently not used)
     vec_value_t _buff;                      // (p,) buffer
 
     static inline auto init_rows(
         const std::vector<base_t*>& mat_list
     )
     {
         size_t n = 0;
@@ -292,29 +285,24 @@
         }
 
         return p;
     }
 
 public:
     explicit MatrixNaiveRConcatenate(
-        const std::vector<base_t*>& mat_list,
-        size_t n_threads
+        const std::vector<base_t*>& mat_list
     ): 
         _mat_list(mat_list),
         _rows(init_rows(mat_list)),
         _cols(init_cols(mat_list)),
-        _n_threads(n_threads),
         _buff(_cols)
     {
         if (mat_list.size() <= 0) {
             throw util::adelie_core_error("mat_list must be non-empty.");
         }
-        if (n_threads < 1) {
-            throw util::adelie_core_error("n_threads must be >= 1.");
-        }
     }
 
     value_t cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
         const Eigen::Ref<const vec_value_t>& weights
     ) override
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -133,39 +133,68 @@
         base_t::check_cov(
             j, q, sqrt_weights.size(), 
             out.rows(), out.cols(), buffer.rows(), buffer.cols(), 
             rows(), cols()
         );
         
         if (q == 1) {
-            out(0, 0) = (_mat.col(j).transpose().array() * sqrt_weights).square().sum();
+            const auto sqrt_w_mj = (_mat.col(j).transpose().array() * sqrt_weights).matrix();
+            Eigen::Map<vec_value_t> vbuff(_buff.data(), _n_threads);
+            out(0, 0) = ddot(sqrt_w_mj, sqrt_w_mj, _n_threads, vbuff);
             return;
         }
 
         auto& Xj = buffer;
         
         auto Xj_array = Xj.array();
         dmmeq(
-            Xj_array,
+            Xj_array, 
             _mat.middleCols(j, q).array().colwise() * sqrt_weights.matrix().transpose().array(),
             _n_threads
         );
 
-        Eigen::setNbThreads(_n_threads);
-        out.noalias() = Xj.transpose() * Xj;
-        Eigen::setNbThreads(1);
+        out.setZero();
+        auto out_lower = out.template selfadjointView<Eigen::Lower>();
+        out_lower.rankUpdate(Xj.transpose());
+        out.template triangularView<Eigen::Upper>() = out.transpose();
     }
 
     void sp_btmul(
         const sp_mat_value_t& v, 
         Eigen::Ref<rowmat_value_t> out
     ) override
     {
         base_t::check_sp_btmul(
             v.rows(), v.cols(), out.rows(), out.cols(), rows(), cols()
         );
-        out.noalias() = v * _mat.transpose();
+        if (_n_threads <= 1) {
+            out.noalias() = v * _mat.transpose();
+            return;
+        }
+        sp_mat_value_t vc;
+        if (!v.isCompressed()) {
+            vc = v;
+            if (!vc.isCompressed()) vc.makeCompressed();
+        }
+        const sp_mat_value_t& v_ref = (vc.size() != 0) ? vc : v;
+
+        const auto outer = v_ref.outerIndexPtr();
+        const auto inner = v_ref.innerIndexPtr();
+        const auto value = v_ref.valuePtr();
+        #pragma omp parallel for schedule(static) num_threads(_n_threads)
+        for (int k = 0; k < v_ref.outerSize(); ++k) {
+            const Eigen::Map<const sp_mat_value_t> vk(
+                1,
+                v_ref.cols(),
+                outer[k+1] - outer[k],
+                outer + k,
+                inner,
+                value
+            );
+            auto out_k = out.row(k);
+            out_k = vk * _mat.transpose();
+        };
     }
 };
 
 } // namespace matrix
 } // namespace adelie_core
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         base_t::check_cmul(j, v.size(), weights.size(), rows(), cols());
         Eigen::Map<const rowmat_value_t> V(v.data(), rows() / _K, _K);
         Eigen::Map<const rowmat_value_t> W(weights.data(), V.rows(), V.cols());
         int i = j / _K;
         int l = j - _K * i;
         Eigen::Map<vec_value_t> _v(_buff.data(), V.rows());
         Eigen::Map<vec_value_t> _w(_buff.data() + V.rows(), V.rows());
-        _v = V.col(l);
-        _w = W.col(l);
+        dvveq(_v, V.col(l), _n_threads);
+        dvveq(_w, W.col(l), _n_threads);
         return _mat->cmul(i, _v, _w);
     }
 
     void ctmul(
         int j, 
         value_t v, 
         Eigen::Ref<vec_value_t> out
@@ -70,15 +70,16 @@
         base_t::check_ctmul(j, out.size(), rows(), cols());
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
         int i = j / _K;
         int l = j - _K * i;
         Eigen::Map<vec_value_t> _out(_buff.data(), Out.rows());
         dvzero(_out, _n_threads);
         _mat->ctmul(i, v, _out);
-        Out.col(l).array() += _out;
+        auto Out_l = Out.col(l).array();
+        dvaddi(Out_l, _out, _n_threads);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
@@ -92,24 +93,21 @@
         for (int l = 0; l < _K; ++l) {
             const auto j_l = std::max(j-l, 0);
             const auto i_begin = j_l / static_cast<int>(_K) + ((j_l % _K) != 0);
             if (j-l+q <= 0) continue;
             const auto i_end = (j-l+q-1) / static_cast<int>(_K) + 1;
             const auto i_q = i_end - i_begin;
             if (i_q <= 0) continue;
-            _v = V.col(l);
-            _w = W.col(l);
-            Eigen::Map<vec_value_t> _out(
-                _buff.data() + 2 * V.rows(),
-                i_q
-            );
+            dvveq(_v, V.col(l), _n_threads);
+            dvveq(_w, W.col(l), _n_threads);
+            Eigen::Map<vec_value_t> _out(_buff.data() + 2 * V.rows(), i_q);
             _mat->bmul(i_begin, i_q, _v, _w, _out);
-            for (int i = i_begin; i < i_end; ++i){
-                out[i*_K+l-j] = _out[i-i_begin];
-            }
+            Eigen::Map<rowmat_value_t> Out(out.data(), out.size() / _K, _K);
+            auto Out_curr = Out.col(l-j).segment(i_begin, i_q);
+            dvveq(Out_curr, _out, _n_threads);
         }
     }
 
     void btmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
@@ -121,35 +119,44 @@
             const auto j_l = std::max(j-l, 0);
             const auto i_begin = j_l / static_cast<int>(_K) + ((j_l % _K) != 0);
             if (j-l+q <= 0) continue;
             const auto i_end = (j-l+q-1) / static_cast<int>(_K) + 1;
             const auto i_q = i_end - i_begin;
             if (i_q <= 0) continue;
             Eigen::Map<vec_value_t> _v(_buff.data(), i_q);
-            for (int i = i_begin; i < i_end; ++i) {
-                _v[i-i_begin] = v[i*_K+l-j];
-            }
-            Eigen::Map<vec_value_t> _out(
-                _buff.data() + i_q,
-                Out.rows()
-            );
-            _out.setZero();
+            Eigen::Map<const rowmat_value_t> V(v.data(), v.size() / _K, _K);
+            dvveq(_v, V.col(l-j).segment(i_begin, i_q), _n_threads);
+            Eigen::Map<vec_value_t> _out(_buff.data() + i_q, Out.rows());
+            dvzero(_out, _n_threads);
             _mat->btmul(i_begin, i_q, _v, _out);
-            Out.col(l).array() += _out;
+            auto Out_l = Out.col(l).array();
+            dvaddi(Out_l, _out, _n_threads);
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
-        // TODO: this can maybe be parallelized?
-        bmul(0, cols(), v, weights, out);
+        Eigen::Map<const rowmat_value_t> V(v.data(), rows() / _K, _K);
+        Eigen::Map<const rowmat_value_t> W(weights.data(), V.rows(), V.cols());
+        Eigen::Map<vec_value_t> _v(_buff.data(), V.rows());
+        Eigen::Map<vec_value_t> _w(_buff.data() + V.rows(), V.rows());
+        const auto p = _mat->cols();
+        for (int l = 0; l < _K; ++l) {
+            dvveq(_v, V.col(l), _n_threads);
+            dvveq(_w, W.col(l), _n_threads);
+            Eigen::Map<vec_value_t> _out(_buff.data() + 2 * V.rows(), p);
+            _mat->mul(_v, _w, _out);
+            Eigen::Map<rowmat_value_t> Out(out.data(), out.size() / _K, _K);
+            auto Out_l = Out.col(l).array();
+            dvveq(Out_l, _out, _n_threads);
+        }
     }
 
     void cov(
         int j, int q,
         const Eigen::Ref<const vec_value_t>& sqrt_weights,
         Eigen::Ref<colmat_value_t> out,
         Eigen::Ref<colmat_value_t> buffer
@@ -157,27 +164,27 @@
     {
         base_t::check_cov(
             j, q, sqrt_weights.size(), 
             out.rows(), out.cols(), buffer.rows(), buffer.cols(), 
             rows(), cols()
         );
         Eigen::Map<const rowmat_value_t> sqrt_W(sqrt_weights.data(), rows() / _K, _K);
-        out.setZero(); // do NOT parallelize!
+        out.setZero();
         for (int l = 0; l < _K; ++l) {
             const auto j_l = std::max(j-l, 0);
             const auto i_begin = j_l / static_cast<int>(_K) + ((j_l % _K) != 0);
             if (j-l+q <= 0) continue;
             const auto i_end = (j-l+q-1) / static_cast<int>(_K) + 1;
             const auto i_q = i_end - i_begin;
             if (i_q <= 0) continue;
             if (_buff.size() < sqrt_W.rows() + i_q * i_q) {
                 _buff.resize(_buff.size() + i_q * i_q);
             }
             Eigen::Map<vec_value_t> _sqrt_weights(_buff.data(), sqrt_W.rows());
-            _sqrt_weights = sqrt_W.col(l);
+            dvveq(_sqrt_weights, sqrt_W.col(l), _n_threads);
             Eigen::Map<colmat_value_t> _out(
                 _buff.data() + _sqrt_weights.size(),
                 i_q, i_q
             );
             Eigen::Map<colmat_value_t> _buffer(
                 buffer.data(),
                 _mat->rows(),
@@ -364,17 +371,17 @@
         Eigen::Map<rowmat_value_t> Out(out.data(), rows() / _K, _K);
         int n_processed = 0;
         while (n_processed < q) {
             const int i = (j + n_processed) / _K;
             const int l = (j + n_processed) - _K * i;
             const int size = std::min<int>(_K-l, q-n_processed);
             Eigen::Map<const vec_value_t> _v(v.data() + n_processed, size);
-            for (int k = 0; k < size; ++k) {
-                auto _out = Out.col(l+k);
-                dvaddi(_out, _v[k] * _mat.col(i), _n_threads);
+            for (int j = 0; j < _v.size(); ++j) {
+                auto Out_curr = Out.col(l+j);
+                dvaddi(Out_curr, _v[j] * _mat.col(i), _n_threads);
             }
             n_processed += size;
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
@@ -384,15 +391,14 @@
     {
         base_t::check_bmul(0, cols(), v.size(), weights.size(), out.size(), rows(), cols());
         dvveq(_vbuff, v * weights, _n_threads);
         Eigen::Map<const rowmat_value_t> VW(_vbuff.data(), rows() / _K, _K);
         Eigen::Map<rowmat_value_t> Out(out.data(), cols() / _K, _K);
         Eigen::setNbThreads(_n_threads);
         Out.noalias() = _mat.transpose() * VW;
-        Eigen::setNbThreads(1);
     }
 
     void cov(
         int j, int q,
         const Eigen::Ref<const vec_value_t>& sqrt_weights,
         Eigen::Ref<colmat_value_t> out,
         Eigen::Ref<colmat_value_t> buffer
@@ -409,33 +415,33 @@
             const auto j_l = std::max(j-l, 0);
             const auto i_begin = j_l / static_cast<int>(_K) + ((j_l % _K) != 0);
             if (j-l+q <= 0) continue;
             const auto i_end = (j-l+q-1) / static_cast<int>(_K) + 1;
             const auto i_q = i_end - i_begin;
             if (i_q <= 0) continue;
 
-            auto buff = buffer.topLeftCorner(_mat.rows(), i_q);
-            auto buff_array = buff.array();
+            Eigen::Map<colmat_value_t> sqrt_WX(buffer.data(), _mat.rows(), i_q);
+            auto sqrt_WX_array = sqrt_WX.array();
             dmmeq(
-                buff_array,
+                sqrt_WX_array,
                 _mat.middleCols(i_begin, i_q).array().colwise() * sqrt_W.col(l).array(),
                 _n_threads
             );
+
+            if (_vbuff.size() < i_q * i_q) _vbuff.resize(i_q * i_q);
+            Eigen::Map<colmat_value_t> XTWX(_vbuff.data(), i_q, i_q);
+            XTWX.setZero(); // do NOT parallelize!
+            XTWX.template selfadjointView<Eigen::Lower>().rankUpdate(sqrt_WX.transpose());
             for (int i1 = 0; i1 < i_q; ++i1) {
                 for (int i2 = 0; i2 <= i1; ++i2) {
-                    out((i1+i_begin)*_K+l-j, (i2+i_begin)*_K+l-j) = (
-                        buff.col(i1).dot(buff.col(i2))
-                    );
-                }
-            }
-            for (int i1 = 0; i1 < i_q; ++i1) {
-                for (int i2 = i1 + 1; i2 < i_q; ++i2) {
                     const auto fi1 = (i1+i_begin)*_K+l-j;
                     const auto fi2 = (i2+i_begin)*_K+l-j;
-                    out(fi1, fi2) = out(fi2, fi1);
+                    const auto val = XTWX(i1, i2);
+                    out(fi1, fi2) = val;
+                    out(fi2, fi1) = val;
                 }
             }
         }
     }
 
     int rows() const override { return _K * _mat.rows(); }
     int cols() const override { return _K * _mat.cols(); }
@@ -479,27 +485,43 @@
                 v.cols() / _K,
                 inners.size(),
                 outers.data(),
                 inners.data(),
                 values.data()
             );
 
-            _out.noalias() = _v * _mat.transpose();
-
             const auto routine = [&](int k) {
                 Eigen::Map<rowmat_value_t> out_k(
                     out.row(k).data(), _out.cols(), _K                
                 );
                 out_k.col(l) = _out.row(k);
             };
+
             if (_n_threads <= 1) {
-                for (int k = 0; k < out.rows(); ++k) routine(k);
-            } else {
-                #pragma omp parallel for schedule(static) num_threads(_n_threads)
-                for (int k = 0; k < out.rows(); ++k) routine(k);
-            }
+                _out.noalias() = _v * _mat.transpose();
+                for (int k = 0; k < _v.outerSize(); ++k) routine(k);
+                continue;
+            }
+
+            const auto outer = _v.outerIndexPtr();
+            const auto inner = _v.innerIndexPtr();
+            const auto value = _v.valuePtr();
+            #pragma omp parallel for schedule(static) num_threads(_n_threads)
+            for (int k = 0; k < _v.outerSize(); ++k) {
+                const Eigen::Map<const sp_mat_value_t> vk(
+                    1,
+                    _v.cols(),
+                    outer[k+1] - outer[k],
+                    outer + k,
+                    inner,
+                    value
+                );
+                auto out_k = _out.row(k);
+                out_k = vk * _mat.transpose();
+                routine(k);
+            };
         }
     }
 };
 
 } // namespace matrix
 } // namespace adelie_core
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,163 +1,150 @@
 #pragma once
-#include <cstdio>
 #include <string>
 #include <vector>
+#include <adelie_core/matrix/matrix_naive_base.hpp>
 #include <adelie_core/matrix/utils.hpp>
-#include <adelie_core/io/io_snp_unphased.hpp>
-#include <omp.h>
+#include <adelie_core/io/io_snp_phased_ancestry.hpp>
 
 namespace adelie_core {
 namespace matrix {
 
 template <class ValueType,
           class MmapPtrType=std::unique_ptr<char, std::function<void(char*)>>>
-class MatrixNaiveSNPUnphased: public MatrixNaiveBase<ValueType>
+class MatrixNaiveSNPPhasedAncestry: public MatrixNaiveBase<ValueType>
 {
 public:
     using base_t = MatrixNaiveBase<ValueType>;
     using typename base_t::value_t;
-    using typename base_t::index_t;
     using typename base_t::vec_value_t;
     using typename base_t::vec_index_t;
     using typename base_t::colmat_value_t;
     using typename base_t::rowmat_value_t;
     using typename base_t::sp_mat_value_t;
     using string_t = std::string;
-    using io_t = io::IOSNPUnphased<MmapPtrType>;
+    using io_t = io::IOSNPPhasedAncestry<MmapPtrType>;
     
 protected:
-    static constexpr value_t _inf = std::numeric_limits<value_t>::infinity();
     const io_t _io;             // IO handler
     const size_t _n_threads;    // number of threads
-    util::rowarr_type<index_t> _ibuff;
-    util::rowarr_type<value_t> _vbuff;
+    util::rowvec_type<char> _bbuff;
+    vec_index_t _ibuff;
+    vec_value_t _buff;
 
     static auto init_io(
         const string_t& filename,
         const string_t& read_mode
     )
     {
         io_t io(filename, read_mode);
         io.read();
         return io;
     }
 
     ADELIE_CORE_STRONG_INLINE
     value_t _cmul(
-        int j, 
+        int j,
         const Eigen::Ref<const vec_value_t>& v,
-        const Eigen::Ref<const vec_value_t>& weights
-    ) const
+        const Eigen::Ref<const vec_value_t>& weights,
+        size_t n_threads
+    ) 
     {
-        const value_t imp = _io.impute()[j];
-        value_t sum = 0;
-        for (int c = 0; c < io_t::n_categories; ++c) {
-            auto it = _io.begin(j, c);
-            const auto end = _io.end(j, c);
-            const value_t val = (c == 0) ? imp : c;
-            value_t curr_sum = 0;
-            for (; it != end; ++it) {
-                const auto idx = *it;
-                curr_sum += v[idx] * weights[idx]; 
-            }
-            sum += curr_sum * val;
-        }
-        return sum;
+        return snp_phased_ancestry_dot(
+            _io, j, v * weights, n_threads, _buff
+        );
     }
 
     ADELIE_CORE_STRONG_INLINE
     void _ctmul(
-        int j, 
-        value_t v, 
-        Eigen::Ref<vec_value_t> out
-    ) const
+        int j,
+        value_t v,
+        Eigen::Ref<vec_value_t> out,
+        size_t n_threads
+    )
     {
-        const value_t imp = _io.impute()[j];
-        for (int c = 0; c < io_t::n_categories; ++c) {
-            auto it = _io.begin(j, c);
-            const auto end = _io.end(j, c);
-            const value_t curr_val = v * ((c == 0) ? imp : c);
-            for (; it != end; ++it) {
-                const auto idx = *it;
-                out[idx] += curr_val; 
-            }
-        }
+        return snp_phased_ancestry_axi(
+            _io, j, v, out, n_threads
+        );
     }
 
+    auto ancestries() const { return _io.ancestries(); }
+
 public:
-    explicit MatrixNaiveSNPUnphased(
+    explicit MatrixNaiveSNPPhasedAncestry(
         const string_t& filename,
         const string_t& read_mode,
         size_t n_threads
     ): 
         _io(init_io(filename, read_mode)),
         _n_threads(n_threads),
-        _ibuff(n_threads, _io.rows()),
-        _vbuff(n_threads, _io.rows())
+        _bbuff(_io.rows()),
+        _ibuff(_io.rows()),
+        _buff(n_threads * std::max<size_t>(1, _io.ancestries()))
     {
         if (n_threads < 1) {
             throw util::adelie_core_error("n_threads must be >= 1.");
         }
-        _vbuff.setConstant(_inf);
+        _bbuff.setZero();
     }
 
     value_t cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
         const Eigen::Ref<const vec_value_t>& weights
     ) override
     {
         base_t::check_cmul(j, v.size(), weights.size(), rows(), cols());
-        return _cmul(j, v, weights);
+        return _cmul(j, v, weights, _n_threads);
     }
 
     void ctmul(
         int j, 
         value_t v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
-        _ctmul(j, v, out);
+        _ctmul(j, v, out, _n_threads);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_bmul(j, q, v.size(), weights.size(), out.size(), rows(), cols());
-        for (int t = 0; t < q; ++t) {
-            out[t] = _cmul(j + t, v, weights);
-        }
+        if (_buff.size() < q * _n_threads) _buff.resize(q * _n_threads);
+        snp_phased_ancestry_block_dot(
+            _io, j, q, v * weights, out, _n_threads, _buff
+        );
     }
 
     void btmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
-        for (int t = 0; t < q; ++t) {
-            _ctmul(j + t, v[t], out);
-        }
+        if (_buff.size() < q * _n_threads) _buff.resize(q * _n_threads);
+        snp_phased_ancestry_block_axi(
+            _io, j, q, v, out, _n_threads
+        );
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
         const auto routine = [&](int t) {
-            out[t] = _cmul(t, v, weights);
+            out[t] = _cmul(t, v, weights, 1);
         };
         if (_n_threads <= 1) {
             for (int t = 0; t < cols(); ++t) routine(t);
         } else {
             #pragma omp parallel for schedule(static) num_threads(_n_threads)
             for (int t = 0; t < cols(); ++t) routine(t);
         }
@@ -171,112 +158,202 @@
     ) override
     {
         base_t::check_cov(
             j, q, sqrt_weights.size(), 
             out.rows(), out.cols(), buffer.rows(), buffer.cols(), 
             rows(), cols()
         );
+        
+        const auto A = ancestries();
 
-        const auto routine = [&](int i1) {
-            const auto thr_id = omp_get_thread_num();
-            const auto index_1 = j+i1;
-            const value_t imp_1 = _io.impute()[index_1];
-
-            // if covariance must be computed,
-            // cache index_1 information. 
-            size_t nnz = 0;
-            if (i1) {
-                for (int c = 0; c < io_t::n_categories; ++c) {
-                    auto it = _io.begin(index_1, c);
-                    const auto end = _io.end(index_1, c);
-                    const value_t val = (c == 0) ? imp_1 : c;
-                    for (; it != end; ++it) {
-                        const auto idx = *it;
-                        _vbuff(thr_id, idx) = val;
-                        _ibuff(thr_id, nnz) = idx;
-                        ++nnz;
+        out.setZero(); // don't parallelize! q is usually small
+
+        int n_solved0 = 0;
+        while (n_solved0 < q) {
+            const auto begin0 = j + n_solved0;
+            const auto snp0 = begin0 / A;
+            const auto ancestry_lower0 = begin0 % A;
+            const auto ancestry_upper0 = std::min<int>(ancestry_lower0 + q - n_solved0, A);
+
+            int n_solved1 = 0;
+            while (n_solved1 <= n_solved0) {
+                const auto begin1 = j + n_solved1;
+                const auto snp1 = begin1 / A;
+                const auto ancestry_lower1 = begin1 % A;
+                const auto ancestry_upper1 = std::min<int>(ancestry_lower1 + q - n_solved1, A);
+
+                if (n_solved0 == n_solved1) {
+                    const auto begin = begin0;
+                    const auto snp = snp0;
+                    const auto a_low = ancestry_lower0;
+                    const auto a_high = ancestry_upper0;
+                    const auto a_size = a_high - a_low;
+
+                    // increase buffer including cross-term computation part as well
+                    if (_buff.size() < a_size * a_size * _n_threads) {
+                        _buff.resize(a_size * a_size * _n_threads);
+                    }
+
+                    // compute quadratic diagonal part
+                    auto out_diag = out.diagonal().segment(n_solved0, a_size);
+                    snp_phased_ancestry_block_dot(
+                        _io, begin0, a_size, sqrt_weights.square(), out_diag, _n_threads, _buff
+                    );
+
+                    // compute cross-terms
+                    //for (int k0 = 0; k0 < a_size; ++k0) {
+                    //    // cache hap0 information
+                    //    size_t nnz = 0;
+                    //    auto it0 = _io.begin(snp, a_low + k0, 0);
+                    //    const auto end0 = _io.end(snp, a_low + k0, 0);
+                    //    for (; it0 != end0; ++it0) {
+                    //        const auto idx = *it0;
+                    //        _bbuff[idx] = true;
+                    //        _ibuff[nnz] = idx;
+                    //        ++nnz;
+                    //    }
+
+                    //    // loop through hap1's ancestries
+                    //    for (int k1 = 0; k1 < a_size; ++k1) {
+                    //        auto it1 = _io.begin(snp, a_low + k1, 1);
+                    //        const auto end1 = _io.end(snp, a_low + k1, 1);
+                    //        value_t sum = 0;
+                    //        for (; it1 != end1; ++it1) {
+                    //            const auto idx = *it1;
+                    //            const auto sqrt_w = sqrt_weights[idx];
+                    //            sum += sqrt_w * sqrt_w * _bbuff[idx];
+                    //        }
+
+                    //        const auto kk0 = n_solved0 + k0;
+                    //        const auto kk1 = n_solved0 + k1;
+                    //        out(kk0, kk1) += sum;
+                    //        out(kk1, kk0) += sum;
+                    //    }
+
+                    //    // keep invariance by populating with false
+                    //    for (size_t i = 0; i < nnz; ++i) {
+                    //        _bbuff[_ibuff[i]] = false;
+                    //    }
+                    //}
+
+                    #pragma omp parallel for schedule(static) num_threads(_n_threads) collapse(2) if(_n_threads > 1)
+                    for (int k0 = 0; k0 < a_size; ++k0) {
+                        for (int k1 = 0; k1 < a_size; ++k1) {
+                            auto it0 = _io.begin(snp, a_low + k0, 0);
+                            const auto end0 = _io.end(snp, a_low + k0, 0);
+                            auto it1 = _io.begin(snp, a_low + k1, 1);
+                            const auto end1 = _io.end(snp, a_low + k1, 1);
+
+                            value_t sum = 0;
+                            while (
+                                (it0 != end0) &&
+                                (it1 != end1)
+                            ) {
+                                const auto idx0 = *it0;
+                                const auto idx1 = *it1;
+                                if (idx0 < idx1) {
+                                    ++it0; 
+                                    continue;
+                                }
+                                else if (idx0 > idx1) {
+                                    ++it1;
+                                    continue;
+                                } 
+                                else {
+                                    const auto sqrt_w = sqrt_weights[idx0];
+                                    sum += sqrt_w * sqrt_w;
+                                    ++it0;
+                                    ++it1;
+                                }
+                            }
+
+                            const auto kk0 = n_solved0 + k0;
+                            const auto kk1 = n_solved0 + k1;
+                            out(kk0, kk1) += sum * (1 + (kk0 == kk1));
+                        }
+                    }
+
+                    for (int k0 = 0; k0 < a_size; ++k0) {
+                        for (int k1 = 0; k1 < k0; ++k1) {
+                            const auto kk0 = n_solved0 + k0;
+                            const auto kk1 = n_solved0 + k1;
+                            const auto tmp = out(kk0, kk1);
+                            out(kk0, kk1) += out(kk1, kk0);
+                            out(kk1, kk0) += tmp;
+                        }
                     }
+
+                    n_solved1 += ancestry_upper1 - ancestry_lower1;
+                    continue;
                 }
-            } 
 
-            for (int i2 = 0; i2 <= i1; ++i2) {
-                const auto index_2 = j+i2;
+                /* general routine */
 
-                if (i1 == i2) {
-                    value_t sum = 0;
-                    for (int c = 0; c < io_t::n_categories; ++c) {
-                        auto it = _io.begin(index_1, c);
-                        const auto end = _io.end(index_1, c);
-                        const value_t val = (c == 0) ? imp_1 : c;
-                        value_t curr_sum = 0;
+                const auto ancestry_size0 = ancestry_upper0-ancestry_lower0;
+                const auto ancestry_size1 = ancestry_upper1-ancestry_lower1;
+                for (int a0 = 0; a0 < ancestry_size0; ++a0) {
+                    size_t nnz = 0;
+                    for (int hap0 = 0; hap0 < io_t::n_haps; ++hap0) {
+                        auto it = _io.begin(snp0, ancestry_lower0+a0, hap0);
+                        const auto end = _io.end(snp0, ancestry_lower0+a0, hap0);
                         for (; it != end; ++it) {
                             const auto idx = *it;
-                            const auto val = sqrt_weights[idx];
-                            curr_sum += val * val;
+                            if (!_bbuff[idx]) {
+                                _ibuff[nnz] = idx;
+                                ++nnz;
+                            }
+                            _bbuff[idx] += 1;
                         }
-                        sum += curr_sum * val *val; 
                     }
-                    out(i1, i2) = sum;
-                    continue;
-                }
 
-                value_t sum = 0;
-                const value_t imp_2 = _io.impute()[index_2];
-                for (int c = 0; c < io_t::n_categories; ++c) {
-                    auto it = _io.begin(index_2, c);
-                    const auto end = _io.end(index_2, c);
-                    const value_t val = (c == 0) ? imp_2 : c;
-                    value_t curr_sum = 0;
-                    for (; it != end; ++it) {
-                        const auto idx = *it;
-                        const auto v1 = _vbuff(thr_id, idx);
-                        if (std::isinf(v1)) continue;
-                        const auto sqrt_w = sqrt_weights[idx];
-                        curr_sum += sqrt_w * sqrt_w * v1;
+                    for (int a1 = 0; a1 < ancestry_size1; ++a1) {
+                        const auto sum = snp_phased_ancestry_dot(
+                            _io, begin1 + a1, 
+                            vec_value_t::NullaryExpr(sqrt_weights.size(), [&](auto i) {
+                                const auto sqrt_wi = sqrt_weights[i];
+                                return sqrt_wi * sqrt_wi * _bbuff[i];
+                            }),
+                            _n_threads,
+                            _buff
+                        );
+                        const auto kk0 = n_solved0 + a0;
+                        const auto kk1 = n_solved1 + a1;
+                        out(kk0, kk1) = sum;
+                        out(kk1, kk0) = sum;
+                    }
+
+                    for (size_t i = 0; i < nnz; ++i) {
+                        _bbuff[_ibuff[i]] = 0;
                     }
-                    sum += curr_sum * val;
                 }
-                out(i1, i2) = sum;
-            }
 
-            // keep invariance by populating with inf
-            for (size_t i = 0; i < nnz; ++i) {
-                _vbuff(thr_id, _ibuff(thr_id, i)) = _inf;
-            }
-        };
-        if ((_n_threads <= 1) || (q == 1)) {
-            for (int i1 = 0; i1 < q; ++i1) routine(i1);
-        } else {
-            #pragma omp parallel for schedule(static) num_threads(_n_threads)
-            for (int i1 = 0; i1 < q; ++i1) routine(i1);
-        }
-        for (int i1 = 0; i1 < q; ++i1) {
-            for (int i2 = i1+1; i2 < q; ++i2) {
-                out(i1, i2) = out(i2, i1);
+                n_solved1 += ancestry_upper1 - ancestry_lower1;
             }
-        }
+            n_solved0 += ancestry_upper0 - ancestry_lower0;
+        }     
     }
 
     int rows() const override { return _io.rows(); }
-    int cols() const override { return _io.cols(); }
+    int cols() const override { return _io.snps() * ancestries(); }
 
     void sp_btmul(
         const sp_mat_value_t& v,
         Eigen::Ref<rowmat_value_t> out
     ) override
     {
         base_t::check_sp_btmul(
             v.rows(), v.cols(), out.rows(), out.cols(), rows(), cols()
         );
+        const auto A = ancestries();
         const auto routine = [&](int k) {
             typename sp_mat_value_t::InnerIterator it(v, k);
             auto out_k = out.row(k);
             out_k.setZero();
             for (; it; ++it) {
-                _ctmul(it.index(), it.value(), out_k);
+                _ctmul(it.index(), it.value(), out_k, 1);
             }
         };
         if (_n_threads <= 1) {
             for (int k = 0; k < v.outerSize(); ++k) routine(k);
         } else {
             #pragma omp parallel for schedule(static) num_threads(_n_threads)
             for (int k = 0; k < v.outerSize(); ++k) routine(k);
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -21,122 +21,126 @@
     using vec_sp_index_t = util::rowvec_type<typename sparse_t::StorageIndex>;
 
     static_assert(!sparse_t::IsRowMajor, "MatrixNaiveSparse: only column-major allowed!");
     
 private:
     const Eigen::Map<const sparse_t> _mat;  // underlying sparse matrix
     const size_t _n_threads;                // number of threads
+    vec_value_t _buff;
 
     ADELIE_CORE_STRONG_INLINE
     value_t _cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
-        const Eigen::Ref<const vec_value_t>& weights
-    ) const
+        const Eigen::Ref<const vec_value_t>& weights,
+        size_t n_threads
+    ) 
     {
         const auto outer = _mat.outerIndexPtr()[j];
         const auto size = _mat.outerIndexPtr()[j+1] - outer;
         const Eigen::Map<const vec_sp_index_t> inner(
             _mat.innerIndexPtr() + outer, size
         );
         const Eigen::Map<const vec_sp_value_t> value(
             _mat.valuePtr() + outer, size
         );
-        return spddot(inner, value, v * weights);
+        return spddot(inner, value, v * weights, n_threads, _buff);
     }
 
     ADELIE_CORE_STRONG_INLINE
     void _ctmul(
         int j, 
         value_t v, 
-        Eigen::Ref<vec_value_t> out
+        Eigen::Ref<vec_value_t> out,
+        size_t n_threads
     ) const
     {
         const auto outer = _mat.outerIndexPtr()[j];
         const auto size = _mat.outerIndexPtr()[j+1] - outer;
         const Eigen::Map<const vec_sp_index_t> inner(
             _mat.innerIndexPtr() + outer, size
         );
         const Eigen::Map<const vec_sp_value_t> value(
             _mat.valuePtr() + outer, size
         );
-        spaxi(inner, value, v, out);
+        spaxi(inner, value, v, out, n_threads);
     }
     
 public:
     explicit MatrixNaiveSparse(
         size_t rows,
         size_t cols,
         size_t nnz,
         const Eigen::Ref<const vec_sp_index_t>& outer,
         const Eigen::Ref<const vec_sp_index_t>& inner,
         const Eigen::Ref<const vec_sp_value_t>& value,
         size_t n_threads
     ): 
         _mat(rows, cols, nnz, outer.data(), inner.data(), value.data()),
-        _n_threads(n_threads)
+        _n_threads(n_threads),
+        _buff(n_threads)
     {
         if (n_threads < 1) {
             throw util::adelie_core_error("n_threads must be >= 1.");
         }
     }
 
     value_t cmul(
         int j, 
         const Eigen::Ref<const vec_value_t>& v,
         const Eigen::Ref<const vec_value_t>& weights
     ) override
     {
         base_t::check_cmul(j, v.size(), weights.size(), rows(), cols());
-        return _cmul(j, v, weights);
+        return _cmul(j, v, weights, _n_threads);
     }
 
     void ctmul(
         int j, 
         value_t v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_ctmul(j, out.size(), rows(), cols());
-        _ctmul(j, v, out);
+        _ctmul(j, v, out, _n_threads);
     }
 
     void bmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_bmul(j, q, v.size(), weights.size(), out.size(), rows(), cols());
         for (int k = 0; k < q; ++k) {
-            out[k] = _cmul(j+k, v, weights);
+            out[k] = _cmul(j+k, v, weights, _n_threads);
         }
     }
 
     void btmul(
         int j, int q, 
         const Eigen::Ref<const vec_value_t>& v, 
         Eigen::Ref<vec_value_t> out
     ) override
     {
         base_t::check_btmul(j, q, v.size(), out.size(), rows(), cols());
         for (int k = 0; k < q; ++k) {
-            _ctmul(j+k, v[k], out);
+            _ctmul(j+k, v[k], out, _n_threads);
         }
     }
 
     void mul(
         const Eigen::Ref<const vec_value_t>& v, 
         const Eigen::Ref<const vec_value_t>& weights,
         Eigen::Ref<vec_value_t> out
     ) override
     {
         const auto routine = [&](int k) {
-            out[k] = _cmul(k, v, weights);
+            out[k] = _cmul(k, v, weights, 1);
         };
         if (_n_threads <= 1) {
             for (int k = 0; k < out.size(); ++k) routine(k);
         } else {
             #pragma omp parallel for schedule(static) num_threads(_n_threads)
             for (int k = 0; k < out.size(); ++k) routine(k);
         }
@@ -209,13 +213,34 @@
         const sp_mat_value_t& v, 
         Eigen::Ref<rowmat_value_t> out
     ) override
     {
         base_t::check_sp_btmul(
             v.rows(), v.cols(), out.rows(), out.cols(), rows(), cols()
         );
-        out = v * _mat.transpose();
+        const auto outer = v.outerIndexPtr();
+        const auto inner = v.innerIndexPtr();
+        const auto value = v.valuePtr();
+
+        const auto routine = [&](auto k) {
+            const Eigen::Map<const sp_mat_value_t> vk(
+                1,
+                v.cols(),
+                outer[k+1] - outer[k],
+                outer + k,
+                inner,
+                value
+            );
+            auto out_k = out.row(k);
+            out_k = vk * _mat.transpose();
+        };
+        if (_n_threads <= 1) {
+            for (int k = 0; k < v.outerSize(); ++k) routine(k);
+        } else {
+            #pragma omp parallel for schedule(static) num_threads(_n_threads)
+            for (int k = 0; k < v.outerSize(); ++k) routine(k);
+        }
     }
 };
 
 } // namespace matrix
 } // namespace adelie_core
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/matrix/matrix_naive_subset.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/matrix/matrix_naive_subset.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     using typename base_t::index_t;
     using typename base_t::vec_value_t;
     using typename base_t::vec_index_t;
     using typename base_t::colmat_value_t;
     using typename base_t::rowmat_value_t;
     using typename base_t::sp_mat_value_t;
     using dyn_vec_index_t = std::vector<index_t>;
+    using map_cvec_index_t = Eigen::Map<const vec_index_t>;
     
 private:
     base_t* _mat;               // underlying matrix
-    const vec_index_t _subset;  // column subset
+    const map_cvec_index_t _subset;  // column subset
     const std::tuple<
         vec_index_t,
         dyn_vec_index_t
     > _subset_cinfo;            // 1) number of elements left
                                 // in the contiguous sub-chunk
                                 // starting at _subset[i]
                                 // 2) beginning index to each
@@ -71,15 +72,15 @@
 public:
     explicit MatrixNaiveCSubset(
         base_t* mat,
         const Eigen::Ref<const vec_index_t>& subset,
         size_t n_threads
     ): 
         _mat(mat),
-        _subset(subset),
+        _subset(subset.data(), subset.size()),
         _subset_cinfo(init_subset_cinfo(subset)),
         _n_threads(n_threads)
     {
         if ((subset.minCoeff() < 0) || (subset.maxCoeff() >= mat->cols())) {
             throw util::adelie_core_error(
                 "subset must contain unique values in the range [0, p) "
                 "where p is the number of columns."
@@ -245,18 +246,19 @@
     using typename base_t::value_t;
     using typename base_t::vec_value_t;
     using typename base_t::vec_index_t;
     using typename base_t::colmat_value_t;
     using typename base_t::rowmat_value_t;
     using typename base_t::sp_mat_value_t;
     using vec_bool_t = util::rowvec_type<bool>;
+    using map_cvec_index_t = Eigen::Map<const vec_index_t>;
     
 private:
     base_t* _mat;               // underlying matrix
-    const vec_index_t _subset;
+    const map_cvec_index_t _subset;
     const vec_value_t _mask;  
     const size_t _n_threads;
     vec_value_t _buffer;
     vec_value_t _cov_buffer;
 
     static auto init_mask(
         size_t n,
@@ -280,15 +282,15 @@
 public:
     explicit MatrixNaiveRSubset(
         base_t* mat,
         const Eigen::Ref<const vec_index_t>& subset,
         size_t n_threads
     ): 
         _mat(mat),
-        _subset(subset),
+        _subset(subset.data(), subset.size()),
         _mask(init_mask(mat->rows(), subset)),
         _n_threads(n_threads),
         _buffer(mat->rows())
     {
         if ((subset.minCoeff() < 0) || (subset.maxCoeff() >= mat->rows())) {
             throw util::adelie_core_error(
                 "subset must contain unique values in the range [0, n) "
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/optimization/bisect.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/optimization/bisect.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/optimization/newton.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/optimization/newton.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/optimization/nnls.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/optimization/nnls.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/optimization/search_pivot.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/optimization/search_pivot.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -259,23 +259,23 @@
             auto ak = screen_beta.segment(ss_value_begin, gsize); // corresponding beta
             auto gk = screen_grad.segment(ss_value_begin, gsize); // corresponding gradient
             const auto& Vk = screen_transforms[ss_idx]; // corresponding V in SVD of X_c
             const auto A_kk = screen_vars.segment(ss_value_begin, gsize);  // corresponding A diagonal 
             const auto pk = penalty[k];
 
             auto gk_transformed = buffer3.head(ak.size());
-            gk_transformed.matrix().noalias() = (
+            gk_transformed.matrix() = (
                 gk.matrix() * Vk
             );
 
             // save old beta in buffer with transformation
             auto ak_old = buffer4.head(ak.size());
             ak_old = ak;
             auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
-            ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
+            ak_old_transformed.matrix() = ak_old.matrix() * Vk; 
             auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
 
             // update group coefficients
             size_t iters;
             gk_transformed += A_kk * ak_old_transformed; 
             update_coefficients_f(
                 A_kk, gk_transformed, l1 * pk, l2 * pk, 
@@ -291,15 +291,15 @@
             del_transformed = ak_transformed - ak_old_transformed;
 
             update_convergence_measure(convg_measure, del_transformed, A_kk);
 
             update_rsq(rsq, del_transformed, A_kk, gk_transformed);
 
             // update new coefficient
-            ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
+            ak.matrix() = ak_transformed.matrix() * Vk.transpose();
 
             // update gradient
             auto del = buffer2.head(ak.size());
             del = ak - ak_old;
             auto indices = buffer_index.head(ak.size());
             indices = util::rowvec_type<index_t>::LinSpaced(
                 ak.size(),
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -107,23 +107,23 @@
             // compute current gradient
             X.bmul(groups[k], gsize, resid, weights, gk);
             if (intercept) {
                 gk -= resid_sum * Xk_mean;
             }
 
             auto gk_transformed = buffer3.head(ak.size());
-            gk_transformed.matrix().noalias() = (
+            gk_transformed.matrix() = (
                 gk.matrix() * Vk
             );
 
             // save old beta in buffer with transformation
             auto ak_old = buffer4.head(ak.size());
             ak_old = ak;
             auto ak_old_transformed = buffer4.segment(ak.size(), ak.size());
-            ak_old_transformed.matrix().noalias() = ak_old.matrix() * Vk; 
+            ak_old_transformed.matrix() = ak_old.matrix() * Vk; 
             auto ak_transformed = buffer4.segment(2 * ak.size(), ak.size());
 
             // update group coefficients
             size_t iters;
             gk_transformed += A_kk * ak_old_transformed; 
             update_coefficients_f(
                 A_kk, gk_transformed, l1 * pk, l2 * pk, 
@@ -139,15 +139,15 @@
             del_transformed = ak_transformed - ak_old_transformed;
 
             update_convergence_measure(convg_measure, del_transformed, A_kk);
 
             update_rsq(rsq, del_transformed, A_kk, gk_transformed);
 
             // update new coefficient
-            ak.matrix().noalias() = ak_transformed.matrix() * Vk.transpose();
+            ak.matrix() = ak_transformed.matrix() * Vk.transpose();
 
             // update residual
             auto del = buffer1.head(ak.size());
             del = ak_old - ak;
             X.btmul(groups[k], gsize, del, resid);
             resid_sum += (Xk_mean * del).sum();
         }
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/solver/utils.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/solver/utils.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,28 @@
         // compute column-means
         Eigen::Map<vec_value_t> Xi_means(
             screen_X_means.data() + sb, gs
         );
         Xi_means = X_means.segment(g, gs);
 
         // resize output and buffer 
-        auto Xi = buffer1.leftCols(gs);
+        Eigen::Map<util::colmat_type<value_t>> Xi(
+            buffer1.data(), n, gs
+        );
         Eigen::Map<util::colmat_type<value_t>> XiTXi(
             buffer2.data(), gs, gs
         );
 
         // compute weighted covariance matrix
         X.cov(g, gs, weights_sqrt, XiTXi, Xi);
 
         if (intercept) {
-            XiTXi.noalias() -= Xi_means.matrix().transpose() * Xi_means.matrix();
+            auto XiTXi_lower = XiTXi.template selfadjointView<Eigen::Lower>();
+            XiTXi_lower.rankUpdate(Xi_means.matrix().transpose(), -1);
+            XiTXi.template triangularView<Eigen::Upper>() = XiTXi.transpose();
         }
 
         if (gs == 1) {
             util::colmat_type<value_t, 1, 1> Q;
             Q(0, 0) = 1;
             screen_transforms[i] = Q;
             screen_vars[sb] = XiTXi(0, 0);
```

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_glm_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_glm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/algorithm.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/counting_iterator.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/counting_iterator.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/exceptions.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/format.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/format.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/macros.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/macros.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/stopwatch.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/stopwatch.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/tqdm.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/tqdm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/include/adelie_core/util/types.hpp` & `adelie-1.1.32/adelie/src/include/adelie_core/util/types.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/io.cpp` & `adelie-1.1.32/adelie/src/io.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,16 @@
             py::arg("filename"),
             py::arg("read_mode")
         )
         .def_property_readonly("rows", &io_t::rows, "Number of rows.")
         .def_property_readonly("snps", &io_t::snps, "Number of SNPs.")
         .def_property_readonly("cols", &io_t::cols, "Number of columns.")
         .def_property_readonly("ancestries", &io_t::ancestries, "Number of ancestries.")
-        .def_property_readonly("nnz", &io_t::nnz, "Number of non-zero entries for each column.")
+        .def_property_readonly("nnz0", &io_t::nnz0, "Number of non-zero entries for each column for haplotype 0.")
+        .def_property_readonly("nnz1", &io_t::nnz1, "Number of non-zero entries for each column for haplotype 1.")
         .def("to_dense", &io_t::to_dense, 
             py::arg("n_threads")=1,
         R"delimiter(
         Creates a dense SNP phased, ancestry matrix from the file.
 
         Parameters
         ----------
```

### Comparing `adelie-1.1.31/adelie/src/matrix.cpp` & `adelie-1.1.32/adelie/src/matrix.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,24 @@
 #include <adelie_core/matrix/matrix_cov_lazy_cov.hpp>
 #include <adelie_core/matrix/matrix_cov_sparse.hpp>
 #include <adelie_core/matrix/matrix_naive_base.hpp>
 #include <adelie_core/matrix/matrix_naive_concatenate.hpp>
 #include <adelie_core/matrix/matrix_naive_dense.hpp>
 #include <adelie_core/matrix/matrix_naive_interaction.hpp>
 #include <adelie_core/matrix/matrix_naive_kronecker_eye.hpp>
+#include <adelie_core/matrix/matrix_naive_one_hot.hpp>
 #include <adelie_core/matrix/matrix_naive_snp_unphased.hpp>
 #include <adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp>
 #include <adelie_core/matrix/matrix_naive_sparse.hpp>
+#include <adelie_core/matrix/matrix_naive_standardize.hpp>
 #include <adelie_core/matrix/matrix_naive_subset.hpp>
 
 namespace py = pybind11;
 namespace ad = adelie_core;
 
-template <class ValueType = double>
-void utils(py::module_& m)
-{
-    using value_t = ValueType;
-    using ref_rowarr_value_t = Eigen::Ref<ad::util::rowarr_type<value_t>>;
-    using ref_rowmat_value_t = Eigen::Ref<ad::util::rowmat_type<value_t>>;
-    using ref_vec_value_t = Eigen::Ref<ad::util::rowvec_type<value_t>>;
-    using ref_mvec_value_t = Eigen::Ref<Eigen::Matrix<value_t, 1, Eigen::Dynamic, Eigen::RowMajor>>;
-    using cref_vec_value_t = Eigen::Ref<const ad::util::rowvec_type<value_t>>;
-    using cref_rowarr_value_t = Eigen::Ref<const ad::util::rowarr_type<value_t>>;
-    using cref_colmat_value_t = Eigen::Ref<const ad::util::colmat_type<value_t>>;
-    using cref_mvec_value_t = Eigen::Ref<const Eigen::Matrix<value_t, 1, Eigen::Dynamic, Eigen::RowMajor>>;
-
-    m.def("dvaddi", ad::matrix::dvaddi<ref_vec_value_t, cref_vec_value_t>);
-    m.def("dmmeq", ad::matrix::dmmeq<ref_rowarr_value_t, cref_rowarr_value_t>);
-    m.def("dvzero", ad::matrix::dvzero<ref_vec_value_t>);
-    m.def("ddot", ad::matrix::ddot<cref_mvec_value_t, cref_mvec_value_t, ref_vec_value_t>);
-    m.def("dax", ad::matrix::dax<value_t, cref_vec_value_t, ref_vec_value_t>);
-    m.def("dgemv", ad::matrix::dgemv<ad::util::operator_type::_eq, cref_colmat_value_t, cref_mvec_value_t, ref_rowmat_value_t, ref_mvec_value_t>);
-}
-
 template <class T>
 class PyMatrixCovBase: public ad::matrix::MatrixCovBase<T>
 {
     using base_t = ad::matrix::MatrixCovBase<T>;
 public:
     /* Inherit the constructors */
     using base_t::base_t;
@@ -362,14 +343,17 @@
         .def("rows", &internal_t::rows, R"delimiter(
         Number of rows.
         )delimiter")
         .def("cols", &internal_t::cols, R"delimiter(
         Number of columns.
         )delimiter")
         /* Augmented API for Python */
+        .def_property_readonly("ndim", [](const internal_t&) { return 2; }, R"delimiter(
+        Number of dimensions. It is always ``2``.
+        )delimiter")
         .def_property_readonly("shape", [](const internal_t& m) {
             return std::make_tuple(m.rows(), m.cols());
         }, R"delimiter(
         Shape of the matrix.
         )delimiter")
         ;
 }
@@ -434,28 +418,34 @@
         )delimiter")
         .def("rows", &internal_t::rows, R"delimiter(
         Number of rows.
         )delimiter")
         .def("cols", &internal_t::cols, R"delimiter(
         Number of columns.
         )delimiter")
+        /* Augmented API for Python */
+        .def_property_readonly("ndim", [](const internal_t&) { return 2; }, R"delimiter(
+        Number of dimensions. It is always ``2``.
+        )delimiter")
         .def_property_readonly("shape", [](const internal_t& m) {
             return std::make_tuple(m.rows(), m.cols());
         }, R"delimiter(
         Shape of the matrix.
         )delimiter")
         ;
 }
 
 template <class ValueType>
 void matrix_cov_block_diag(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixCovBlockDiag<ValueType>;
     using base_t = typename internal_t::base_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name, 
+        "Core matrix class for covariance block-diagonal matrix."
+        )
         .def(
             py::init([](py::list mat_list_py, size_t n_threads) {
                 std::vector<base_t*> mat_list;
                 mat_list.reserve(mat_list_py.size());
                 for (auto obj : mat_list_py) {
                     mat_list.push_back(py::cast<base_t*>(obj));
                 }
@@ -469,30 +459,33 @@
 
 template <class DenseType>
 void matrix_cov_dense(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixCovDense<DenseType>;
     using base_t = typename internal_t::base_t;
     using dense_t = typename internal_t::dense_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for covariance dense matrix."
+        )
         .def(
             py::init<const Eigen::Ref<const dense_t>&, size_t>(), 
             py::arg("mat").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class DenseType>
 void matrix_cov_lazy_cov(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixCovLazyCov<DenseType>;
     using base_t = typename internal_t::base_t;
     using dense_t = typename internal_t::dense_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for covariance lazy-covariance matrix.")
         .def(
             py::init<const Eigen::Ref<const dense_t>&, size_t>(), 
             py::arg("mat").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
@@ -501,85 +494,91 @@
 void matrix_cov_sparse(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixCovSparse<SparseType>;
     using base_t = typename internal_t::base_t;
     using sparse_t = typename internal_t::sparse_t; 
     using vec_sp_value_t = typename internal_t::vec_sp_value_t;
     using vec_sp_index_t = typename internal_t::vec_sp_index_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for covariance sparse matrix."
+        )
         .def(
             py::init<
                 size_t,
                 size_t,
                 size_t,
                 const Eigen::Ref<const vec_sp_index_t>&,
                 const Eigen::Ref<const vec_sp_index_t>&,
                 const Eigen::Ref<const vec_sp_value_t>&,
                 size_t
             >(), 
             py::arg("rows"),
             py::arg("cols"),
             py::arg("nnz"),
-            py::arg("outer"),
-            py::arg("inner"),
-            py::arg("value"),
+            py::arg("outer").noconvert(),
+            py::arg("inner").noconvert(),
+            py::arg("value").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class ValueType>
 void matrix_naive_cconcatenate(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveCConcatenate<ValueType>;
     using base_t = typename internal_t::base_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive column-wise concatenated matrix."
+        )
         .def(
-            py::init([](py::list mat_list_py, size_t n_threads) {
+            py::init([](py::list mat_list_py) {
                 std::vector<base_t*> mat_list;
                 mat_list.reserve(mat_list_py.size());
                 for (auto obj : mat_list_py) {
                     mat_list.push_back(py::cast<base_t*>(obj));
                 }
-                return new internal_t(mat_list, n_threads);
+                return new internal_t(mat_list);
             }), 
-            py::arg("mat_list").noconvert(),
-            py::arg("n_threads")
+            py::arg("mat_list").noconvert()
         )
         ;
 }
 
 template <class ValueType>
 void matrix_naive_rconcatenate(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveRConcatenate<ValueType>;
     using base_t = typename internal_t::base_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive row-wise concatenated matrix."
+        )
         .def(
-            py::init([](py::list mat_list_py, size_t n_threads) {
+            py::init([](py::list mat_list_py) {
                 std::vector<base_t*> mat_list;
                 mat_list.reserve(mat_list_py.size());
                 for (auto obj : mat_list_py) {
                     mat_list.push_back(py::cast<base_t*>(obj));
                 }
-                return new internal_t(mat_list, n_threads);
+                return new internal_t(mat_list);
             }), 
-            py::arg("mat_list").noconvert(),
-            py::arg("n_threads")
+            py::arg("mat_list").noconvert()
         )
         ;
 }
 
 template <class DenseType>
 void matrix_naive_dense(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveDense<DenseType>;
     using base_t = typename internal_t::base_t;
     using dense_t = typename internal_t::dense_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive dense matrix."
+        )
         .def(
             py::init<const Eigen::Ref<const dense_t>&, size_t>(), 
             py::arg("mat").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
@@ -588,38 +587,52 @@
 void matrix_naive_interaction_dense(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveInteractionDense<DenseType>;
     using base_t = typename internal_t::base_t;
     using dense_t = typename internal_t::dense_t;
     using rowarr_index_t = typename internal_t::rowarr_index_t;
     using vec_index_t = typename internal_t::vec_index_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive interaction matrix."
+        )
         .def(
             py::init<
                 const Eigen::Ref<const dense_t>&,
                 const Eigen::Ref<const rowarr_index_t>&,
                 const Eigen::Ref<const vec_index_t>&,
                 size_t 
             >(), 
             py::arg("mat").noconvert(),
             py::arg("pairs").noconvert(),
             py::arg("levels").noconvert(),
             py::arg("n_threads")
         )
-        .def_property_readonly("groups", &internal_t::groups)
-        .def_property_readonly("group_sizes", &internal_t::group_sizes)
+        .def_property_readonly("groups", &internal_t::groups, R"delimiter(
+        List of starting indices to each group where `G` is the number of groups.
+        ``groups[i]`` is the starting index of the ``i`` th group. 
+        The groups are naturally defined by ``pairs``.
+        In the order of the rows of ``pairs``,
+        we group all columns of the current matrix
+        corresponding to each row of ``pairs``.
+        )delimiter")
+        .def_property_readonly("group_sizes", &internal_t::group_sizes, R"delimiter(
+        List of group sizes corresponding to each element in ``groups``.
+        ``group_sizes[i]`` is the group size of the ``i`` th group. 
+        )delimiter")
         ;
 }
 
 template <class ValueType>
 void matrix_naive_kronecker_eye(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveKroneckerEye<ValueType>;
     using base_t = typename internal_t::base_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive Kronecker product with identity matrix."
+        )
         .def(
             py::init<base_t&, size_t, size_t>(), 
             py::arg("mat"),
             py::arg("K"),
             py::arg("n_threads")
         )
         ;
@@ -627,31 +640,72 @@
 
 template <class DenseType>
 void matrix_naive_kronecker_eye_dense(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveKroneckerEyeDense<DenseType>;
     using base_t = typename internal_t::base_t;
     using dense_t = typename internal_t::dense_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive Kronecker product (dense) with identity matrix."
+        )
         .def(
             py::init<const Eigen::Ref<const dense_t>&, size_t, size_t>(), 
-            py::arg("mat"),
+            py::arg("mat").noconvert(),
             py::arg("K"),
             py::arg("n_threads")
         )
         ;
 }
 
+template <class DenseType>
+void matrix_naive_one_hot_dense(py::module_& m, const char* name)
+{
+    using internal_t = ad::matrix::MatrixNaiveOneHotDense<DenseType>;
+    using base_t = typename internal_t::base_t;
+    using dense_t = typename internal_t::dense_t;
+    using vec_index_t = typename internal_t::vec_index_t;
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive (dense) one-hot encoded matrix."
+        )
+        .def(
+            py::init<
+                const Eigen::Ref<const dense_t>&,
+                const Eigen::Ref<const vec_index_t>&,
+                size_t 
+            >(), 
+            py::arg("mat").noconvert(),
+            py::arg("levels").noconvert(),
+            py::arg("n_threads")
+        )
+        .def_property_readonly("groups", &internal_t::groups, R"delimiter(
+        List of starting indices to each group where `G` is the number of groups.
+        ``groups[i]`` is the starting index of the ``i`` th group. 
+        The groups are naturally defined by the columns of ``mat``.
+        In the order of the columns of ``mat``,
+        we group all columns of the current matrix 
+        corresponding to each column of ``mat``.
+        This way, the continuous features each form a group of size one
+        and the discrete features form a group across their one-hot encodings.
+        )delimiter")
+        .def_property_readonly("group_sizes", &internal_t::group_sizes, R"delimiter(
+        List of group sizes corresponding to each element in ``groups``.
+        ``group_sizes[i]`` is the group size of the ``i`` th group. 
+        )delimiter")
+        ;
+}
+
 template <class ValueType>
 void matrix_naive_snp_unphased(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveSNPUnphased<ValueType>;
     using base_t = typename internal_t::base_t;
     using string_t = typename internal_t::string_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive SNP unphased matrix."
+        )
         .def(
             py::init<
                 const string_t&,
                 const string_t&,
                 size_t
             >(), 
             py::arg("filename"),
@@ -663,15 +717,17 @@
 
 template <class ValueType>
 void matrix_naive_snp_phased_ancestry(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveSNPPhasedAncestry<ValueType>;
     using base_t = typename internal_t::base_t;
     using string_t = typename internal_t::string_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive SNP phased, ancestry matrix."
+        )
         .def(
             py::init<
                 const string_t&,
                 const string_t&,
                 size_t
             >(), 
             py::arg("filename"),
@@ -685,86 +741,112 @@
 void matrix_naive_sparse(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveSparse<SparseType>;
     using base_t = typename internal_t::base_t;
     using sparse_t = typename internal_t::sparse_t; 
     using vec_sp_value_t = typename internal_t::vec_sp_value_t;
     using vec_sp_index_t = typename internal_t::vec_sp_index_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive sparse matrix."
+        )
         .def(
             py::init<
                 size_t,
                 size_t,
                 size_t,
                 const Eigen::Ref<const vec_sp_index_t>&,
                 const Eigen::Ref<const vec_sp_index_t>&,
                 const Eigen::Ref<const vec_sp_value_t>&,
                 size_t
             >(), 
             py::arg("rows"),
             py::arg("cols"),
             py::arg("nnz"),
-            py::arg("outer"),
-            py::arg("inner"),
-            py::arg("value"),
+            py::arg("outer").noconvert(),
+            py::arg("inner").noconvert(),
+            py::arg("value").noconvert(),
+            py::arg("n_threads")
+        )
+        ;
+}
+
+template <class ValueType>
+void matrix_naive_standardize(py::module_& m, const char* name)
+{
+    using internal_t = ad::matrix::MatrixNaiveStandardize<ValueType>;
+    using base_t = typename internal_t::base_t;
+    using vec_value_t = typename internal_t::vec_value_t;
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive standardized matrix."
+        )
+        .def(py::init<
+            base_t&,
+            const Eigen::Ref<const vec_value_t>&,
+            const Eigen::Ref<const vec_value_t>&,
+            size_t
+        >(),
+            py::arg("mat"),
+            py::arg("centers").noconvert(),
+            py::arg("scales").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class ValueType>
 void matrix_naive_csubset(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveCSubset<ValueType>;
     using base_t = typename internal_t::base_t;
     using vec_index_t = typename internal_t::vec_index_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive column-subsetted matrix."
+        )
         .def(
             py::init<
                 base_t*,
                 const Eigen::Ref<const vec_index_t>&,
                 size_t
             >(),
             py::arg("mat"),
-            py::arg("subset"),
+            py::arg("subset").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class ValueType>
 void matrix_naive_rsubset(py::module_& m, const char* name)
 {
     using internal_t = ad::matrix::MatrixNaiveRSubset<ValueType>;
     using base_t = typename internal_t::base_t;
     using vec_index_t = typename internal_t::vec_index_t;
-    py::class_<internal_t, base_t>(m, name)
+    py::class_<internal_t, base_t>(m, name,
+        "Core matrix class for naive row-subsetted matrix."
+        )
         .def(
             py::init<
                 base_t*,
                 const Eigen::Ref<const vec_index_t>&,
                 size_t
             >(),
             py::arg("mat"),
-            py::arg("subset"),
+            py::arg("subset").noconvert(),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class T, int Storage>
 using dense_type = Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Storage>;
 template <class T, int Storage>
 using sparse_type = Eigen::SparseMatrix<T, Storage>;
 
 void register_matrix(py::module_& m)
 {
-    /* utils */
-    utils(m);
-
     /* base matrices */
     matrix_naive_base<double>(m, "MatrixNaiveBase64");
     matrix_naive_base<float>(m, "MatrixNaiveBase32");
     matrix_cov_base<double>(m, "MatrixCovBase64");
     matrix_cov_base<float>(m, "MatrixCovBase32");
 
     /* cov matrices */
@@ -803,20 +885,28 @@
     matrix_naive_kronecker_eye<double>(m, "MatrixNaiveKroneckerEye64");
     matrix_naive_kronecker_eye<float>(m, "MatrixNaiveKroneckerEye32");
     matrix_naive_kronecker_eye_dense<dense_type<double, Eigen::RowMajor>>(m, "MatrixNaiveKroneckerEyeDense64C");
     matrix_naive_kronecker_eye_dense<dense_type<double, Eigen::ColMajor>>(m, "MatrixNaiveKroneckerEyeDense64F");
     matrix_naive_kronecker_eye_dense<dense_type<float, Eigen::RowMajor>>(m, "MatrixNaiveKroneckerEyeDense32C");
     matrix_naive_kronecker_eye_dense<dense_type<float, Eigen::ColMajor>>(m, "MatrixNaiveKroneckerEyeDense32F");
 
+    matrix_naive_one_hot_dense<dense_type<double, Eigen::RowMajor>>(m, "MatrixNaiveOneHotDense64C");
+    matrix_naive_one_hot_dense<dense_type<double, Eigen::ColMajor>>(m, "MatrixNaiveOneHotDense64F");
+    matrix_naive_one_hot_dense<dense_type<float, Eigen::RowMajor>>(m, "MatrixNaiveOneHotDense32C");
+    matrix_naive_one_hot_dense<dense_type<float, Eigen::ColMajor>>(m, "MatrixNaiveOneHotDense32F");
+
     matrix_naive_snp_unphased<double>(m, "MatrixNaiveSNPUnphased64");
     matrix_naive_snp_unphased<float>(m, "MatrixNaiveSNPUnphased32");
     matrix_naive_snp_phased_ancestry<double>(m, "MatrixNaiveSNPPhasedAncestry64");
     matrix_naive_snp_phased_ancestry<float>(m, "MatrixNaiveSNPPhasedAncestry32");
 
     matrix_naive_sparse<sparse_type<double, Eigen::ColMajor>>(m, "MatrixNaiveSparse64F");
     matrix_naive_sparse<sparse_type<float, Eigen::ColMajor>>(m, "MatrixNaiveSparse32F");
 
+    matrix_naive_standardize<double>(m, "MatrixNaiveStandardize64");
+    matrix_naive_standardize<float>(m, "MatrixNaiveStandardize32");
+
     matrix_naive_csubset<double>(m, "MatrixNaiveCSubset64");
     matrix_naive_csubset<float>(m, "MatrixNaiveCSubset32");
     matrix_naive_rsubset<double>(m, "MatrixNaiveRSubset64");
     matrix_naive_rsubset<float>(m, "MatrixNaiveRSubset32");
 }
```

### Comparing `adelie-1.1.31/adelie/src/optimization.cpp` & `adelie-1.1.32/adelie/src/optimization.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/solver.cpp` & `adelie-1.1.32/adelie/src/solver.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/state.cpp` & `adelie-1.1.32/adelie/src/state.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     using value_t = typename state_t::value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     using dyn_vec_mat_value_t = typename state_t::dyn_vec_mat_value_t;
 
     py::class_<state_t>(m, name, R"delimiter(
-        Base core state class for all gaussian pin methods.
+        Base state class for Gaussian, pin classes.
         )delimiter")
         .def(py::init<
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&, 
@@ -300,15 +300,15 @@
     using value_t = typename state_t::value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     using dyn_vec_mat_value_t = typename state_t::dyn_vec_mat_value_t;
 
     py::class_<state_t, base_t, PyStateGaussianPinNaive<matrix_t>>(m, name, R"delimiter(
-        Core state class for gaussian, pin, naive method.
+        Core state class for Gaussian, pin, naive method.
         )delimiter")
         .def(py::init<
             matrix_t&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
@@ -448,15 +448,15 @@
     using value_t = typename state_t::value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     using dyn_vec_mat_value_t = typename state_t::dyn_vec_mat_value_t;
 
     py::class_<state_t, base_t, PyStateGaussianPinCov<matrix_t>>(m, name, R"delimiter(
-        Core state class for gaussian, pin, covariance method.
+        Core state class for Gaussian, pin, covariance method.
         )delimiter")
         .def(py::init<
             matrix_t&,
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
@@ -577,15 +577,15 @@
     using value_t = typename state_t::value_t;
     using index_t = typename state_t::index_t;
     using safe_bool_t = typename state_t::safe_bool_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t>(m, name, R"delimiter(
-        Base core state class for all non-pin methods.
+        Base state class for non-pin classes.
         )delimiter") 
         .def(py::init<
             const Eigen::Ref<const vec_index_t>&, 
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
@@ -920,15 +920,15 @@
     using state_t = ad::state::StateGaussianNaive<matrix_t>;
     using base_t = typename state_t::base_t;
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t, base_t, PyStateGaussianNaive<matrix_t>>(m, name, R"delimiter(
-        Core state class for gaussian, naive method.
+        Core state class for Gaussian, naive method.
         )delimiter")
         .def(py::init<
             matrix_t&,
             const Eigen::Ref<const vec_value_t>&,
             value_t,
             value_t,
             const Eigen::Ref<const vec_value_t>&,
@@ -1091,15 +1091,15 @@
     using state_t = ad::state::StateMultiGaussianNaive<matrix_t>;
     using base_t = typename state_t::base_t;
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t, base_t, PyStateMultiGaussianNaive<matrix_t>>(m, name, R"delimiter(
-        Core state class for multigaussian, naive method.
+        Core state class for MultiGaussian, naive method.
         )delimiter")
         .def(py::init<
             const std::string&,
             size_t,
             bool,
             matrix_t&,
             const Eigen::Ref<const vec_value_t>&,
@@ -1242,15 +1242,15 @@
     using state_t = ad::state::StateGaussianCov<matrix_t>;
     using base_t = typename state_t::base_t;
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t, base_t, PyStateGaussianCov<matrix_t>>(m, name, R"delimiter(
-        Core state class for gaussian, covariance method.
+        Core state class for Gaussian, covariance method.
         )delimiter")
         .def(py::init<
             matrix_t&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_index_t>&,
             value_t, 
@@ -1391,15 +1391,15 @@
     using state_t = ad::state::StateGlmNaive<matrix_t>;
     using base_t = typename state_t::base_t;
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t, base_t, PyStateGlmNaive<matrix_t>>(m, name, R"delimiter(
-        Core state class for glm, naive method.
+        Core state class for GLM, naive method.
         )delimiter")
         .def(py::init<
             matrix_t&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_value_t>&,
             const Eigen::Ref<const vec_index_t>&,
             const Eigen::Ref<const vec_index_t>&,
@@ -1549,15 +1549,15 @@
     using state_t = ad::state::StateMultiGlmNaive<matrix_t>;
     using base_t = typename state_t::base_t;
     using value_t = typename state_t::value_t;
     using vec_value_t = typename state_t::vec_value_t;
     using vec_index_t = typename state_t::vec_index_t;
     using vec_bool_t = typename state_t::vec_bool_t;
     py::class_<state_t, base_t, PyStateMultiGlmNaive<matrix_t>>(m, name, R"delimiter(
-        Core state class for multiglm, naive method.
+        Core state class for multi-response GLM, naive method.
         )delimiter")
         .def(py::init<
             const std::string&,
             size_t,
             bool,
             matrix_t&,
             const Eigen::Ref<const vec_value_t>&,
```

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Cholesky` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/CholmodSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Core` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Core`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Eigenvalues` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Geometry` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Householder` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Jacobi` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/KLUSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/LU` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/LU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/MetisSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/OrderingMethods` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/PaStiXSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/PardisoSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/QR` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/QR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SPQRSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SVD` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/Sparse` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseCholesky` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseCore` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseLU` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SparseQR` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdDeque` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdList` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/StdVector` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/SuperLUSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/UmfPackSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/BVH` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/FFT` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/Splines` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h` & `adelie-1.1.32/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/adelie/state.py` & `adelie-1.1.32/adelie/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -366,15 +366,15 @@
     tol: float =1e-7,
     adev_tol: float =0.9,
     ddev_tol: float =1e-4,
     newton_tol: float =1e-12,
     newton_max_iters: int =1000,
     n_threads: int =1,
 ):
-    """Creates a gaussian, pin, naive method state object.
+    """Creates a Gaussian, pin, naive method state object.
 
     Define the following quantities:
 
         - :math:`X_c` as :math:`X` if ``intercept`` is ``False`` and otherwise 
           the column-centered version.
         - :math:`y_c` as :math:`y` if ``intercept`` is ``False`` and otherwise
           the centered version.
@@ -517,25 +517,25 @@
     class _gaussian_pin_naive(gaussian_pin_naive_base, core_base):
         def __init__(self):
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._X = X
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
-            self._weights = np.array(weights, copy=False, dtype=dtype)
-            self._screen_set = np.array(screen_set, copy=False, dtype=int)
-            self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
+            self._weights = np.array(weights, copy=True, dtype=dtype)
+            self._screen_set = np.array(screen_set, copy=True, dtype=int)
+            self._lmda_path = np.array(lmda_path, copy=True, dtype=dtype)
             # dynamic inputs require a copy to not modify user's inputs
-            self._resid = np.copy(resid).astype(dtype)
-            self._screen_beta = np.copy(screen_beta).astype(dtype)
-            self._screen_is_active = np.copy(screen_is_active).astype(bool)
-            self._active_set = np.copy(active_set).astype(int)
+            self._resid = np.array(resid, copy=True, dtype=dtype)
+            self._screen_beta = np.array(screen_beta, copy=True, dtype=dtype)
+            self._screen_is_active = np.array(screen_is_active, copy=True, dtype=bool)
+            self._active_set = np.array(active_set, copy=True, dtype=int)
 
             (
                 self._screen_begins,
             ) = deduce_states(
                 group_sizes=group_sizes,
                 screen_set=screen_set,
             )
@@ -659,15 +659,15 @@
     max_iters: int =int(1e5),
     tol: float =1e-7,
     rdev_tol: float =1e-4,
     newton_tol: float =1e-12,
     newton_max_iters: int =1000,
     n_threads: int =1,
 ):
-    """Creates a gaussian pin covariance method state object.
+    """Creates a Gaussian, pin, covariance method state object.
 
     Define the following quantities:
 
         - :math:`X_c` as :math:`X` if ``intercept`` is ``False`` and otherwise 
           the column-centered version.
         - :math:`y_c` as :math:`y - \\eta^0` if ``intercept`` is ``False`` and otherwise
           the centered version.
@@ -796,24 +796,24 @@
     class _gaussian_pin_cov(gaussian_pin_cov_base, core_base):
         def __init__(self):
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._A = A
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
-            self._screen_set = np.array(screen_set, copy=False, dtype=int)
-            self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
+            self._screen_set = np.array(screen_set, copy=True, dtype=int)
+            self._lmda_path = np.array(lmda_path, copy=True, dtype=dtype)
             # dynamic inputs require a copy to not modify user's inputs
-            self._screen_beta = np.copy(screen_beta).astype(dtype)
-            self._screen_grad = np.copy(screen_grad).astype(dtype)
-            self._screen_is_active = np.copy(screen_is_active).astype(bool)
-            self._active_set = np.copy(active_set).astype(int)
+            self._screen_beta = np.array(screen_beta, copy=True, dtype=dtype)
+            self._screen_grad = np.array(screen_grad, copy=True, dtype=dtype)
+            self._screen_is_active = np.array(screen_is_active, copy=True, dtype=bool)
+            self._active_set = np.array(active_set, copy=True, dtype=int)
 
             (
                 self._screen_begins,
             ) = deduce_states(
                 group_sizes=group_sizes,
                 screen_set=screen_set,
             )
@@ -1048,15 +1048,15 @@
     lmda_path_size: int =100,
     max_screen_size: int =None,
     max_active_size: int =None,
     pivot_subset_ratio: float =0.1,
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
 ):
-    """Creates a gaussian, covariance method state object.
+    """Creates a Gaussian, covariance method state object.
 
     Parameters
     ----------
     A : (p, p) Union[adelie.matrix.MatrixCovBase64, adelie.matrix.MatrixCovBase32]
         Positive semi-definite matrix.
         It is typically one of the matrices defined in ``adelie.matrix`` submodule.
     v : (p,) np.ndarray
@@ -1233,18 +1233,18 @@
     class _gaussian_cov(base, core_base):
         def __init__(self):
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._A = A
-            self._v = np.array(v, copy=False, dtype=dtype)
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
+            self._v = np.array(v, copy=True, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._grad = np.array(grad, copy=False, dtype=dtype)
             self._active_set = np.array(active_set, copy=False, dtype=int)
 
@@ -1582,15 +1582,15 @@
     lmda_path_size: int =100,
     max_screen_size: int =None,
     max_active_size: int =None,
     pivot_subset_ratio: float =0.1,
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
 ):
-    """Creates a gaussian, naive method state object.
+    """Creates a Gaussian, naive method state object.
 
     Define the following quantities:
 
         - :math:`X_c` as :math:`X` if ``intercept`` is ``False`` and otherwise 
           the column-centered version.
         - :math:`y_c` as :math:`y - \\eta^0` if ``intercept`` is ``False`` and otherwise
           the centered version.
@@ -1805,35 +1805,36 @@
         def __init__(self):
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._glm = glm.gaussian(y=y, weights=weights, dtype=dtype)
             self._X = X
-            self._X_means = np.array(X_means, copy=False, dtype=dtype)
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
-            self._offsets = np.array(offsets, copy=False, dtype=dtype)
+            self._X_means = np.array(X_means, copy=True, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
+            self._offsets = np.array(offsets, copy=True, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
+            self._resid = np.array(resid, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 X=self._X,
                 X_means=self._X_means,
                 y_mean=y_mean,
                 y_var=y_var,
-                resid=resid,
+                resid=self._resid,
                 resid_sum=resid_sum,
                 groups=self._groups,
                 group_sizes=self._group_sizes,
                 alpha=alpha,
                 penalty=self._penalty,
                 weights=self._glm.weights,
                 lmda_path=self._lmda_path,
@@ -1916,15 +1917,15 @@
     lmda_path_size: int =100,
     max_screen_size: int =None,
     max_active_size: int =None,
     pivot_subset_ratio: float =0.1,
     pivot_subset_min: int =1,
     pivot_slack_ratio: float =1.25,
 ):
-    """Creates a multi-gaussian, naive method state object.
+    """Creates a MultiGaussian, naive method state object.
 
     Define the following quantities: 
 
         - :math:`\\tilde{X} = X\\otimes I_K` if ``intercept`` is ``False``, 
           and otherwise :math:`[1 \\otimes I_K, X \\otimes I_K]`.
         - :math:`\\tilde{y}` as the flattened version of :math:`y-\\eta^0` as row-major.
         - :math:`\\tilde{W} = K^{-1} (W \\otimes I_K)`. 
@@ -2152,26 +2153,27 @@
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._glm = glm.multigaussian(y=y, weights=weights, dtype=dtype)
             self._X = X_raw
             self._X_expanded = X
-            self._X_means = np.array(X_means, copy=False, dtype=dtype)
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
+            self._X_means = np.array(X_means, copy=True, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
             self._weights_expanded = np.repeat(self._glm.weights, repeats=n_classes) / n_classes
-            self._offsets = np.array(offsets, copy=False, dtype=dtype)
+            self._offsets = np.array(offsets, copy=True, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
+            self._resid = np.array(resid, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 group_type=group_type,
                 n_classes=n_classes,
@@ -2180,15 +2182,15 @@
                 X_means=self._X_means,
                 # y_mean is not used in the solver since global intercept is turned off,
                 # but it is used to compute loss_null and loss_full.
                 # This is not the actual y_mean, but it is a value that will result in correct
                 # calculation of loss_null and loss_full.
                 y_mean=np.linalg.norm(np.sum(weights[:, None] * (y - offsets), axis=-1) / n_classes),
                 y_var=y_var,
-                resid=resid,
+                resid=self._resid,
                 resid_sum=resid_sum,
                 groups=self._groups,
                 group_sizes=self._group_sizes,
                 alpha=alpha,
                 penalty=self._penalty,
                 weights=self._weights_expanded,
                 lmda_path=self._lmda_path,
@@ -2506,24 +2508,26 @@
         def __init__(self):
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._glm = glm
             self._X = X
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
-            self._offsets = np.array(offsets, copy=False, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
+            self._offsets = np.array(offsets, copy=True, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
+            self._eta = np.array(eta, copy=False, dtype=dtype)
+            self._resid = np.array(resid, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 X=self._X,
                 groups=self._groups,
@@ -2561,16 +2565,16 @@
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
                 active_set_size=active_set_size,
                 active_set=self._active_set,
                 beta0=beta0,
                 lmda=lmda,
                 grad=self._grad,
-                eta=eta,
-                resid=resid,
+                eta=self._eta,
+                resid=self._resid,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
             obj = base.create_from_core(
                 cls, state, core_state, _glm_naive, core_base,
             )
@@ -2858,24 +2862,26 @@
             self._core_type = core_base
             ## save inputs due to lifetime issues
             # static inputs require a reference to input
             # or copy if it must be made
             self._glm = glm
             self._X = X_raw
             self._X_expanded = X
-            self._groups = np.array(groups, copy=False, dtype=int)
-            self._group_sizes = np.array(group_sizes, copy=False, dtype=int)
-            self._penalty = np.array(penalty, copy=False, dtype=dtype)
-            self._offsets = np.array(offsets, copy=False, dtype=dtype)
+            self._groups = np.array(groups, copy=True, dtype=int)
+            self._group_sizes = np.array(group_sizes, copy=True, dtype=int)
+            self._penalty = np.array(penalty, copy=True, dtype=dtype)
+            self._offsets = np.array(offsets, copy=True, dtype=dtype)
             self._lmda_path = np.array(lmda_path, copy=False, dtype=dtype)
             self._screen_set = np.array(screen_set, copy=False, dtype=int)
             self._screen_beta = np.array(screen_beta, copy=False, dtype=dtype)
             self._screen_is_active = np.array(screen_is_active, copy=False, dtype=bool)
             self._active_set = np.array(active_set, copy=False, dtype=int)
             self._grad = np.array(grad, copy=False, dtype=dtype)
+            self._eta = np.array(eta, copy=False, dtype=dtype)
+            self._resid = np.array(resid, copy=False, dtype=dtype)
 
             # MUST call constructor directly and not use super()!
             # https://pybind11.readthedocs.io/en/stable/advanced/classes.html#forced-trampoline-class-initialisation
             core_base.__init__(
                 self,
                 group_type=group_type,
                 n_classes=n_classes,
@@ -2916,16 +2922,16 @@
                 screen_beta=self._screen_beta,
                 screen_is_active=self._screen_is_active,
                 active_set_size=active_set_size,
                 active_set=self._active_set,
                 beta0=0,
                 lmda=lmda,
                 grad=self._grad,
-                eta=eta,
-                resid=resid,
+                eta=self._eta,
+                resid=self._resid,
             )
 
         @classmethod
         def create_from_core(cls, state, core_state):
             obj = base.create_from_core(
                 cls, state, core_state, _multiglm_naive, core_base,
             )
```

### Comparing `adelie-1.1.31/adelie.egg-info/PKG-INFO` & `adelie-1.1.32/adelie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.31
+Version: 1.1.32
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.31/adelie.egg-info/SOURCES.txt` & `adelie-1.1.32/adelie.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 adelie/src/adelie_core.cpp
 adelie/src/bcd.cpp
 adelie/src/configs.cpp
 adelie/src/decl.hpp
 adelie/src/glm.cpp
 adelie/src/io.cpp
 adelie/src/matrix.cpp
+adelie/src/matrix_utils.cpp
 adelie/src/optimization.cpp
 adelie/src/solver.cpp
 adelie/src/state.cpp
 adelie/src/include/adelie_core/configs.hpp
 adelie/src/include/adelie_core/bcd/utils.hpp
 adelie/src/include/adelie_core/bcd/constrained/admm.hpp
 adelie/src/include/adelie_core/bcd/constrained/coordinate_descent.hpp
@@ -59,17 +60,19 @@
 adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
 adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_interaction.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
+adelie/src/include/adelie_core/matrix/matrix_naive_one_hot.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
+adelie/src/include/adelie_core/matrix/matrix_naive_standardize.hpp
 adelie/src/include/adelie_core/matrix/matrix_naive_subset.hpp
 adelie/src/include/adelie_core/matrix/utils.hpp
 adelie/src/include/adelie_core/optimization/bisect.hpp
 adelie/src/include/adelie_core/optimization/newton.hpp
 adelie/src/include/adelie_core/optimization/nnls.hpp
 adelie/src/include/adelie_core/optimization/search_pivot.hpp
 adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
```

### Comparing `adelie-1.1.31/pyproject.toml` & `adelie-1.1.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adelie-1.1.31/setup.py` & `adelie-1.1.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Optional multithreaded build
 ParallelCompile("NPY_NUM_BUILD_JOBS").install()
 
 __version__ = open("VERSION", "r").read().strip()
 
 extra_compile_args = sysconfig.get_config_var('CFLAGS').split()
 extra_compile_args += [
+    "-g0",
     "-Wall", 
     "-Wextra", 
     "-DNDEBUG", 
     "-O3",
 ]
 libraries = []
 extra_link_args = []
```

