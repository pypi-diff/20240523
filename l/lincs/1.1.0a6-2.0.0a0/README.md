# Comparing `tmp/lincs-1.1.0a6.tar.gz` & `tmp/lincs-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-1.1.0a6.tar", last modified: Tue Feb  6 05:49:35 2024, max compression
+gzip compressed data, was "lincs-2.0.0a0.tar", last modified: Thu May 23 13:06:28 2024, max compression
```

## Comparing `lincs-1.1.0a6.tar` & `lincs-2.0.0a0.tar`

### file list

```diff
@@ -1,414 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.262635 lincs-1.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-06 05:49:30.000000 lincs-1.1.0a6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-06 05:49:30.000000 lincs-1.1.0a6/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-06 05:49:30.000000 lincs-1.1.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-02-06 05:49:35.262635 lincs-1.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-02-06 05:49:30.000000 lincs-1.1.0a6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.194636 lincs-1.1.0a6/lincs/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    45688 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/command_line_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    17945 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.198636 lincs-1.1.0a6/lincs/liblincs/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/chrones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/classification.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/classification.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    32773 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/generation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/generation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/internal.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.198636 lincs-1.1.0a6/lincs/liblincs/io/
--rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/alternatives.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/alternatives.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/model.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/model.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/problem.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/validation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io/validation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/io.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/exception.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.190636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15253 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.202636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.206636 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations-without-progress.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds-without-progress.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/pre-processing.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/pre-processing.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-separation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/learning.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.206636 lincs-1.1.0a6/lincs/liblincs/liblincs-module/
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/liblincs-module/converters.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/liblincs-module/generation-functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30489 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/liblincs-module/io-classes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/liblincs-module/learning-classes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/liblincs-module/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.206636 lincs-1.1.0a6/lincs/liblincs/linear-programming/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/linear-programming/alglib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/linear-programming/alglib.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/linear-programming/glop.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/linear-programming/glop.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/linear-programming/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/randomness-utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/randomness-utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.206636 lincs-1.1.0a6/lincs/liblincs/sat/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/sat/eval-max-sat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/sat/eval-max-sat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/sat/minisat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/sat/minisat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/sat/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/unreachable.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/variant-dispatch.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.206636 lincs-1.1.0a6/lincs/liblincs/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.222636 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/
--rwxr-xr-x   0 runner    (1001) docker     (127)   615853 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibinternal.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    65139 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibinternal.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   322558 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibmisc.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    88614 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibmisc.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   493278 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/ap.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   179632 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/ap.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  1927587 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/dataanalysis.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   438786 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/dataanalysis.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    46242 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/diffequations.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    10465 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/diffequations.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   126902 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/fasttransforms.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    27863 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/fasttransforms.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   149125 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/integration.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    33746 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/integration.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  2674150 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/interpolation.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   500164 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/interpolation.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    76185 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7372 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_avx2.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    39356 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_fma.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     4704 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_fma.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    23798 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     4058 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_sse2.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  2288262 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/linalg.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   403192 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/linalg.h
--rwxr-xr-x   0 runner    (1001) docker     (127)  3545102 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/optimization.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   608685 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/optimization.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   752491 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/solvers.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   198547 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/solvers.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   339371 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/specialfunctions.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    77195 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/specialfunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (127)   612951 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/statistics.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    56614 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/statistics.h
--rwxr-xr-x   0 runner    (1001) docker     (127)        4 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/alglib/stdafx.h
--rw-r--r--   0 runner    (1001) docker     (127)   321644 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/doctest.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.226636 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/
--rw-r--r--   0 runner    (1001) docker     (127)    59653 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.226636 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.242636 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/
--rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/analyze.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/arena.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/assume.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/averages.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/averages.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/backtrack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/backward.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/bins.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/bins.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22171 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/block.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/block.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    36535 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/checker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/checker.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/clause.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/clause.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/collect.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13886 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/compact.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/condition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/config.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/constrain.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/contract.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/contract.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cover.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cover.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/decide.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/decompose.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/deduplicate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31395 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/elim.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/elim.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ema.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ema.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/extend.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/external.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/external.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/flags.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/flags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/format.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/format.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/gates.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/heap.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23229 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/internal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    47282 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/internal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/inttypes.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.h
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/level.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/limit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/limit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/lookahead.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/lucky.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/message.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/message.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/minimize.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/observer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/occs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/occs.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/options.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18179 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/options.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/parse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/phases.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/phases.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22375 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/probe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/profile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/profile.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/propagate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/queue.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/radix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/random.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/random.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/range.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/reduce.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/reluctant.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/rephase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/report.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/resources.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/resources.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/restart.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/restore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/score.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/score.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/shrink.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/signal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/solution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    39275 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    24693 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/stats.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/stats.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21969 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ternary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/transred.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/util.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/util.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/var.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/var.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/version.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/version.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    36971 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/walk.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/watch.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/watch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadicalinterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/card_oe.h
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/mcqd.h
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
--rw-r--r--   0 runner    (1001) docker     (127)    39841 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/lov-e.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    62179 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/magic_enum.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.194636 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.242636 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/
--rw-r--r--   0 runner    (1001) docker     (127)    35190 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/Solver.cc
--rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/Solver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/SolverTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.242636 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Alg.h
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/IntMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Sort.h
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Vec.h
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.242636 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/simp/
--rw-r--r--   0 runner    (1001) docker     (127)    22553 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    57901 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/rapidcsv.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/compat/
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/compat/optional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraint_builder.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34401 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/exceptions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/
--rw-r--r--   0 runner    (1001) docker     (127)    16614 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25566 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/optional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/uri.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/schema.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   102841 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/schema_parser.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/subschema.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.246636 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validation_results.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    68300 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validation_visitor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validator.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.258635 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/anchor.h
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/binary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/binary.h
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/collectionstack.h
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/convert.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/depthguard.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/depthguard.h
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/directives.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/directives.h
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/dll.h
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emit.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitfromevents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitfromevents.h
--rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitter.h
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterdef.h
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emittermanip.h
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterstate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterstate.h
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterstyle.h
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterutils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterutils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/eventhandler.h
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/indentation.h
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/mark.h
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/memory.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.258635 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/convert.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.262635 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator.h
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator_fwd.h
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node.h
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_data.h
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_iterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_ref.h
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/emit.h
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/impl.h
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/iterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/node.h
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/parse.h
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/ptr.h
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/type.h
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node_data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodebuilder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodebuilder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodeevents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodeevents.h
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/noexcept.h
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/null.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/null.h
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parse.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ptr_vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regex_yaml.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regex_yaml.h
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regeximpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanner.h
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanscalar.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanscalar.h
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantag.h
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantoken.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/setting.h
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/simplekey.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/singledocparser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/singledocparser.h
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stlemitter.h
--rw-r--r--   0 runner    (1001) docker     (127)    11907 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stream.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/streamcharsource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stringsource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/tag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/tag.h
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/token.h
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/traits.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/yaml.h
--rw-r--r--   0 runner    (1001) docker     (127)    70475 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/liblincs_module_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-02-06 05:49:30.000000 lincs-1.1.0a6/lincs/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 05:49:35.262635 lincs-1.1.0a6/lincs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 05:49:35.000000 lincs-1.1.0a6/lincs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 05:49:30.000000 lincs-1.1.0a6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 05:49:35.262635 lincs-1.1.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-02-06 05:49:30.000000 lincs-1.1.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.082069 lincs-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 13:06:23.000000 lincs-2.0.0a0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-23 13:06:23.000000 lincs-2.0.0a0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 13:06:23.000000 lincs-2.0.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-23 13:06:28.082069 lincs-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-23 13:06:23.000000 lincs-2.0.0a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.014068 lincs-2.0.0a0/lincs/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45688 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/command_line_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17945 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.018068 lincs-2.0.0a0/lincs/liblincs/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/chrones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15883 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/classification.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/classification.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33258 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/generation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/generation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/internal.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.018068 lincs-2.0.0a0/lincs/liblincs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/alternatives.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/alternatives.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    32476 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/model.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/problem.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/validation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io/validation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/io.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.010068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.022068 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations-without-progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds-without-progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/pre-processing.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/pre-processing.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-separation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60097 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/learning.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.026068 lincs-2.0.0a0/lincs/liblincs/liblincs-module/
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/liblincs-module/converters.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/liblincs-module/generation-functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30534 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/liblincs-module/io-classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22817 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/liblincs-module/learning-classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/liblincs-module/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.026068 lincs-2.0.0a0/lincs/liblincs/linear-programming/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/linear-programming/alglib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/linear-programming/alglib.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/linear-programming/glop.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/linear-programming/glop.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/linear-programming/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/randomness-utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/randomness-utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.026068 lincs-2.0.0a0/lincs/liblincs/sat/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/sat/eval-max-sat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/sat/eval-max-sat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/sat/minisat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/sat/minisat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/sat/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/unreachable.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/variant-dispatch.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.026068 lincs-2.0.0a0/lincs/liblincs/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.046069 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   615853 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibinternal.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65139 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibinternal.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   322558 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibmisc.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    88614 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibmisc.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   493278 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/ap.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179632 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/ap.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1927587 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/dataanalysis.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   438786 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/dataanalysis.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46242 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/diffequations.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10465 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/diffequations.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   126902 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/fasttransforms.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27863 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/fasttransforms.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   149125 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/integration.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33746 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/integration.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2674150 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/interpolation.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   500164 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/interpolation.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    76185 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7372 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_avx2.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39356 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_fma.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4704 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_fma.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23798 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4058 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_sse2.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2288262 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/linalg.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   403192 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/linalg.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  3545102 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/optimization.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   608685 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/optimization.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   752491 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/solvers.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   198547 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/solvers.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   339371 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/specialfunctions.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77195 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/specialfunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   612951 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/statistics.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56614 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/statistics.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)        4 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/alglib/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (127)   321644 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/doctest.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.046069 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/
+-rw-r--r--   0 runner    (1001) docker     (127)    59653 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.050068 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.066069 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/
+-rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/analyze.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/assume.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/backtrack.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/backward.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/bins.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/bins.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22171 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/block.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/block.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36535 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/collect.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13886 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/compact.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/condition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/constrain.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/decide.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/decompose.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/deduplicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31395 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/extend.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18647 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/external.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/external.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/format.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/format.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/gates.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/heap.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23229 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47282 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/inttypes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.h
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/level.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/lookahead.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/lucky.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/message.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/message.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/minimize.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18179 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/phases.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22375 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/probe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/propagate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/radix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/random.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/range.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/reduce.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/reluctant.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/rephase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/report.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/resources.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/resources.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/restart.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/restore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/score.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/score.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/shrink.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/signal.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39275 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24693 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21969 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ternary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/transred.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/var.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/var.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/version.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/version.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36971 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/walk.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadicalinterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/card_oe.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/mcqd.h
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39841 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/lov-e.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    62179 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/magic_enum.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.014068 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.066069 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    35190 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/Solver.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/Solver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17280 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/SolverTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.066069 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Alg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/IntMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Sort.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.066069 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/simp/
+-rw-r--r--   0 runner    (1001) docker     (127)    22553 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57901 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/rapidcsv.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.066069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.070069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.070069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/compat/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraint_builder.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.070069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34401 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/exceptions.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.070069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)    16614 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25566 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/optional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/uri.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/schema.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   102841 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/schema_parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/subschema.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.070069 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validation_results.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    68300 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validation_visitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.078069 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/anchor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/binary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/binary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/collectionstack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/depthguard.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/depthguard.h
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/directives.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/directives.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/dll.h
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emit.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitfromevents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitfromevents.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterdef.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emittermanip.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterstate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterstate.h
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterstyle.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterutils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterutils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/eventhandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/indentation.h
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/mark.h
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/memory.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.082069 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/convert.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.082069 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_iterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/emit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/iterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/node.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/parse.h
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/type.h
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodebuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodebuilder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodeevents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodeevents.h
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/noexcept.h
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/null.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/null.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ptr_vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regex_yaml.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regex_yaml.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regeximpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanscalar.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanscalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantag.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantoken.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/setting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/simplekey.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/singledocparser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/singledocparser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stlemitter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11907 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/streamcharsource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stringsource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/tag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/tag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/token.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/traits.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/yaml.h
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/liblincs_module_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-23 13:06:23.000000 lincs-2.0.0a0/lincs/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:06:28.082069 lincs-2.0.0a0/lincs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-23 13:06:27.000000 lincs-2.0.0a0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-05-23 13:06:28.000000 lincs-2.0.0a0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:06:27.000000 lincs-2.0.0a0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 13:06:27.000000 lincs-2.0.0a0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 13:06:27.000000 lincs-2.0.0a0/lincs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 13:06:27.000000 lincs-2.0.0a0/lincs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 13:06:23.000000 lincs-2.0.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:06:28.082069 lincs-2.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-05-23 13:06:23.000000 lincs-2.0.0a0/setup.py
```

### Comparing `lincs-1.1.0a6/COPYING` & `lincs-2.0.0a0/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/COPYING.LESSER` & `lincs-2.0.0a0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/PKG-INFO` & `lincs-2.0.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 1.1.0a6
+Version: 2.0.0a0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -15,30 +15,31 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: click~=8.1
-Requires-Dist: matplotlib~=3.5
+Requires-Dist: matplotlib~=3.7
+Requires-Dist: six~=1.16
 
 .. Copyright 2023-2024 Vincent Jacques
 
 .. This README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of `MCDA <https://en.wikipedia.org/wiki/Multiple-criteria_decision_analysis>`_ algorithms, usable as a command-line utility and through a Python (3.8+) API.
 
 *lincs* supports Linux, macOS and Windows, with the exception that GPU-based algorithms are not available on macOS, because CUDA itself is not available there.
 On these 3 OSes, *lincs* only support x86_64 CPUs.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v1.1.0a6/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v1.1.0a6/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v2.0.0a0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v2.0.0a0/COPYING.LESSER>`_.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
 
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 You should probably take a look at `our roadmap <https://mics-lab.github.io/lincs/roadmap.html>`_ first.
@@ -88,15 +89,15 @@
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Versioning
 ==========
 
-Starting with version 1.0.0, *lincs* uses `semantic versioning <https://semver.org/>`_.
+*lincs* uses `semantic versioning <https://semver.org/>`_.
 
 *lincs*' public API (that "must be declared" according to SemVer) is constituted exclusively by its `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_,
 **at a code level**: we consider a change as backward compatible if the client code doesn't need to be modified to keep working,
 even if that change requires recompiling the client code in some cases.
 
 Future backward compatible changes might change *lincs*' behavior, especially with regards to pseudo-random behavior.
 
@@ -109,22 +110,22 @@
 
 Default values
 ^^^^^^^^^^^^^^
 
 Default values of optional arguments are not considered part of the public API.
 They might change in future releases if we find values that perform better for most use-cases.
 
-We advice you write your scripts in an explicit way where it matters to you,
+We advice you write your code in an explicit way where it matters to you,
 and rely on implicit default values only where you want the potential future improvements.
 
 File formats
 ^^^^^^^^^^^^
 
 The same specification applies to files read and produced by *lincs*.
-This leads to an issue about backward compatibility:
+This leads to an issue with regard to backward compatibility:
 if we allow more flexibility in input files, new versions of *lincs* will be able to read both the old and the new format, in a backward-compatible way.
 But if *lincs* produces a file in the new format, existing client scripts might not be able to read it, making this change backward-incompatible.
 
 To solve this issue, we impose an additional constraint to *lincs*' public API:
 *lincs* will produce files in a new format only when the client uses the new feature that motivated the new format.
 
 That way, we know that the client already needs to modify their scripts, so they can adapt to the new format.
```

### Comparing `lincs-1.1.0a6/README.rst` & `lincs-2.0.0a0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Versioning
 ==========
 
-Starting with version 1.0.0, *lincs* uses `semantic versioning <https://semver.org/>`_.
+*lincs* uses `semantic versioning <https://semver.org/>`_.
 
 *lincs*' public API (that "must be declared" according to SemVer) is constituted exclusively by its `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_,
 **at a code level**: we consider a change as backward compatible if the client code doesn't need to be modified to keep working,
 even if that change requires recompiling the client code in some cases.
 
 Future backward compatible changes might change *lincs*' behavior, especially with regards to pseudo-random behavior.
 
@@ -86,22 +86,22 @@
 
 Default values
 ^^^^^^^^^^^^^^
 
 Default values of optional arguments are not considered part of the public API.
 They might change in future releases if we find values that perform better for most use-cases.
 
-We advice you write your scripts in an explicit way where it matters to you,
+We advice you write your code in an explicit way where it matters to you,
 and rely on implicit default values only where you want the potential future improvements.
 
 File formats
 ^^^^^^^^^^^^
 
 The same specification applies to files read and produced by *lincs*.
-This leads to an issue about backward compatibility:
+This leads to an issue with regard to backward compatibility:
 if we allow more flexibility in input files, new versions of *lincs* will be able to read both the old and the new format, in a backward-compatible way.
 But if *lincs* produces a file in the new format, existing client scripts might not be able to read it, making this change backward-incompatible.
 
 To solve this issue, we impose an additional constraint to *lincs*' public API:
 *lincs* will produce files in a new format only when the client uses the new feature that motivated the new format.
 
 That way, we know that the client already needs to modify their scripts, so they can adapt to the new format.
```

### Comparing `lincs-1.1.0a6/lincs/__init__.py` & `lincs-2.0.0a0/lincs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # General utilities
 from liblincs import UniformRandomBitsGenerator
 
 # Classification
 from . import classification
 
 # General information
-__version__ = "1.1.0a6"
+__version__ = "2.0.0a0"
 has_gpu = hasattr(classification, "ImproveProfilesWithAccuracyHeuristicOnGpu")
 
 try:
     del visualization
 except NameError:
     pass
```

### Comparing `lincs-1.1.0a6/lincs/classification.py` & `lincs-2.0.0a0/lincs/classification.py`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/command_line_interface.py` & `lincs-2.0.0a0/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/description.py` & `lincs-2.0.0a0/lincs/description.py`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/classification.cpp` & `lincs-2.0.0a0/lincs/liblincs/classification.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -17,28 +17,56 @@
   const Model& model,
   const Alternatives& alternatives,
   const unsigned boundary_index,
   const unsigned alternative_index,
   const unsigned criterion_index
 ) {
   const auto& performance = alternatives.get_alternatives()[alternative_index].get_profile()[criterion_index];
-  const auto& accepted_values = model.get_accepted_values()[criterion_index];
+  const auto& criterion = problem.get_criteria()[criterion_index];
   return dispatch(
-    problem.get_criteria()[criterion_index].get_values(),
-    [&model, &performance, &accepted_values, boundary_index](const Criterion::RealValues& values) {
-      const float threshold = accepted_values.get_real_thresholds().get_thresholds()[boundary_index];
-      return better_or_equal(values.get_preference_direction(), performance.get_real().get_value(), threshold);
-    },
-    [&model, &performance, &accepted_values, boundary_index](const Criterion::IntegerValues& values) {
-      const int threshold = accepted_values.get_integer_thresholds().get_thresholds()[boundary_index];
-      return better_or_equal(values.get_preference_direction(), performance.get_integer().get_value(), threshold);;
-    },
-    [&model, &performance, &accepted_values, boundary_index](const Criterion::EnumeratedValues& values) {
-      const std::string threshold_enum = accepted_values.get_enumerated_thresholds().get_thresholds()[boundary_index];
-      return values.get_value_ranks().at(performance.get_enumerated().get_value()) >= values.get_value_ranks().at(threshold_enum);
+    model.get_accepted_values()[criterion_index].get(),
+    [&model, &performance, &criterion, boundary_index](const AcceptedValues::RealThresholds& accepted_values) {
+      const float value = performance.get_real().get_value();
+      const std::optional<float> threshold = accepted_values.get_thresholds()[boundary_index];
+      if (threshold) {
+        switch (criterion.get_real_values().get_preference_direction()) {
+          case Criterion::PreferenceDirection::increasing:
+            return value >= *threshold;
+          case Criterion::PreferenceDirection::decreasing:
+            return value <= *threshold;
+        }
+        unreachable();
+      } else {
+        return false;
+      }
+    },
+    [&model, &performance, &criterion, boundary_index](const AcceptedValues::IntegerThresholds& accepted_values) {
+      const int value = performance.get_integer().get_value();
+      const std::optional<int> threshold = accepted_values.get_thresholds()[boundary_index];
+      if (threshold) {
+        switch (criterion.get_integer_values().get_preference_direction()) {
+          case Criterion::PreferenceDirection::increasing:
+            return value >= *threshold;
+          case Criterion::PreferenceDirection::decreasing:
+            return value <= *threshold;
+        }
+        unreachable();
+      } else {
+        return false;
+      }
+    },
+    [&model, &performance, &criterion, boundary_index](const AcceptedValues::EnumeratedThresholds& accepted_values) {
+      const auto& ranks = criterion.get_enumerated_values().get_value_ranks();
+      const std::string& value = performance.get_enumerated().get_value();
+      const std::optional<std::string>& threshold = accepted_values.get_thresholds()[boundary_index];
+      if (threshold) {
+        return ranks.at(value) >= ranks.at(*threshold);
+      } else {
+        return false;
+      }
     }
   );
 }
 
 bool is_good_enough(
   const Problem& problem,
   const Model& model,
@@ -91,14 +119,38 @@
       ++result.changed;
     }
   }
 
   return result;
 }
 
+unsigned count_correctly_classified_alternatives(const Problem& problem, const Model& model, const Alternatives& alternatives) {
+  CHRONE();
+
+  const unsigned categories_count = problem.get_ordered_categories().size();
+  const unsigned alternatives_count = alternatives.get_alternatives().size();
+
+  unsigned result = 0;
+
+  for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
+    unsigned category_index;
+    for (category_index = categories_count - 1; category_index != 0; --category_index) {
+      if (is_good_enough(problem, model, alternatives, category_index - 1, alternative_index)) {
+        break;
+      }
+    }
+
+    if (alternatives.get_alternatives()[alternative_index].get_category_index() == category_index) {
+      ++result;
+    }
+  }
+
+  return result;
+}
+
 TEST_CASE("Basic classification using weights") {
   Problem problem{
     {
       Criterion("Criterion 1", Criterion::RealValues(Criterion::PreferenceDirection::increasing, 0, 1)),
       Criterion("Criterion 2", Criterion::RealValues(Criterion::PreferenceDirection::increasing, 0, 1)),
       Criterion("Criterion 3", Criterion::RealValues(Criterion::PreferenceDirection::increasing, 0, 1)),
     },
@@ -226,8 +278,70 @@
   CHECK(alternatives.get_alternatives()[5].get_category_index() == 0);
   CHECK(alternatives.get_alternatives()[6].get_category_index() == 0);
   CHECK(alternatives.get_alternatives()[7].get_category_index() == 0);
   CHECK(result.unchanged == 0);
   CHECK(result.changed == 8);
 }
 
+TEST_CASE("Classification with unreachable thresholds") {
+  Problem problem{
+    {
+      Criterion("Criterion 1", Criterion::RealValues(Criterion::PreferenceDirection::increasing, 0, 1)),
+    },
+    {{"Cat 1"}, {"Cat 2"}, {"Cat 3"}, {"Cat 4"}},
+  };
+
+  Alternatives alternatives{problem, {
+    {"A", {Performance(Performance::Real(0.24))}, std::nullopt},
+    {"A", {Performance(Performance::Real(0.25))}, std::nullopt},
+    {"A", {Performance(Performance::Real(0.49))}, std::nullopt},
+    {"A", {Performance(Performance::Real(0.50))}, std::nullopt},
+    {"A", {Performance(Performance::Real(0.74))}, std::nullopt},
+    {"A", {Performance(Performance::Real(0.75))}, std::nullopt},
+  }};
+
+  classify_alternatives(
+    problem,
+    Model{
+      problem,
+      {
+        AcceptedValues(AcceptedValues::RealThresholds({0.25, 0.5, 0.75})),
+      },
+      {
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+      },
+    },
+    &alternatives);
+
+  CHECK(*alternatives.get_alternatives()[0].get_category_index() == 0);
+  CHECK(*alternatives.get_alternatives()[1].get_category_index() == 1);
+  CHECK(*alternatives.get_alternatives()[2].get_category_index() == 1);
+  CHECK(*alternatives.get_alternatives()[3].get_category_index() == 2);
+  CHECK(*alternatives.get_alternatives()[4].get_category_index() == 2);
+  CHECK(*alternatives.get_alternatives()[5].get_category_index() == 3);
+
+  classify_alternatives(
+    problem,
+    Model{
+      problem,
+      {
+        AcceptedValues(AcceptedValues::RealThresholds({0.25, 0.5, std::nullopt})),
+      },
+      {
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+        SufficientCoalitions(SufficientCoalitions::Weights({1})),
+      },
+    },
+    &alternatives);
+
+  CHECK(*alternatives.get_alternatives()[0].get_category_index() == 0);
+  CHECK(*alternatives.get_alternatives()[1].get_category_index() == 1);
+  CHECK(*alternatives.get_alternatives()[2].get_category_index() == 1);
+  CHECK(*alternatives.get_alternatives()[3].get_category_index() == 2);
+  CHECK(*alternatives.get_alternatives()[4].get_category_index() == 2);
+  CHECK(*alternatives.get_alternatives()[5].get_category_index() == 2);
+}
+
 }  // namespace lincs
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/generation.cpp` & `lincs-2.0.0a0/lincs/liblincs/generation.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -128,27 +128,43 @@
         // (Values clamped strictly inside ']min, max[' to make it easier to generate balanced learning sets)
         // Profiles must be ordered on each criterion, so we generate a random column...
         std::vector<float> column(boundaries_count);
         std::generate(
           column.begin(), column.end(),
           [&values_distribution, &gen]() { return values_distribution(gen); });
         // ... sort it according to the criterion's preference direction...
-        std::sort(column.begin(), column.end(), [&values](float left, float right) { return better_or_equal(values.get_preference_direction(), right, left); });
+        std::sort(column.begin(), column.end(), [&values](float left, float right) {
+          switch (values.get_preference_direction()) {
+            case Criterion::PreferenceDirection::increasing:
+              return left < right;
+            case Criterion::PreferenceDirection::decreasing:
+              return left > right;
+          }
+          unreachable();
+        });
         // ... and assign that column across all profiles.
         for (unsigned profile_index = 0; profile_index != boundaries_count; ++profile_index) {
           profiles[profile_index][criterion_index] = column[profile_index];
         }
       },
       [&gen, boundaries_count, &profiles, criterion_index](const Criterion::IntegerValues& values) {
         std::uniform_int_distribution<int> values_distribution(values.get_min_value(), values.get_max_value());
         std::vector<int> column(boundaries_count);
         std::generate(
           column.begin(), column.end(),
           [&values_distribution, &gen]() { return values_distribution(gen); });
-        std::sort(column.begin(), column.end(), [&values](float left, float right) { return better_or_equal(values.get_preference_direction(), right, left); });
+        std::sort(column.begin(), column.end(), [&values](int left, int right) {
+          switch (values.get_preference_direction()) {
+            case Criterion::PreferenceDirection::increasing:
+              return left < right;
+            case Criterion::PreferenceDirection::decreasing:
+              return left > right;
+          }
+          unreachable();
+        });
         for (unsigned profile_index = 0; profile_index != boundaries_count; ++profile_index) {
           profiles[profile_index][criterion_index] = column[profile_index];
         }
       },
       [&gen, boundaries_count, &profiles, criterion_index](const Criterion::EnumeratedValues& values) {
         std::uniform_int_distribution<unsigned> values_distribution(0, values.get_ordered_values().size() - 1);
         std::vector<unsigned> ranks(boundaries_count);
@@ -191,31 +207,31 @@
     [weights_sum](float w) { return w * weights_sum; });
 
   std::vector<AcceptedValues> accepted_values;
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     accepted_values.push_back(dispatch(
       problem.get_criteria()[criterion_index].get_values(),
       [boundaries_count, &profiles, criterion_index](const Criterion::RealValues&) {
-          std::vector<float> thresholds;
+          std::vector<std::optional<float>> thresholds;
           thresholds.reserve(boundaries_count);
           for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
             thresholds.push_back(std::get<float>(profiles[boundary_index][criterion_index]));
           }
           return AcceptedValues(AcceptedValues::RealThresholds(thresholds));
       },
       [boundaries_count, &profiles, criterion_index](const Criterion::IntegerValues&) {
-          std::vector<int> thresholds;
+          std::vector<std::optional<int>> thresholds;
           thresholds.reserve(boundaries_count);
           for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
             thresholds.push_back(std::get<int>(profiles[boundary_index][criterion_index]));
           }
           return AcceptedValues(AcceptedValues::IntegerThresholds(thresholds));
       },
       [boundaries_count, &profiles, criterion_index](const Criterion::EnumeratedValues&) {
-          std::vector<std::string> thresholds;
+          std::vector<std::optional<std::string>> thresholds;
           thresholds.reserve(boundaries_count);
           for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
             thresholds.push_back(std::get<std::string>(profiles[boundary_index][criterion_index]));
           }
           return AcceptedValues(AcceptedValues::EnumeratedThresholds(thresholds));
       }
     ));
@@ -651,20 +667,20 @@
 TEST_CASE("Random min/max") {
   Problem problem = generate_classification_problem(2, 2, 42, false);
   Model model = generate_mrsort_classification_model(problem, 42);
   Alternatives alternatives = generate_classified_alternatives(problem, model, 1, 44);
 
   CHECK(problem.get_criteria()[0].get_real_values().get_min_value() == doctest::Approx(-25.092));
   CHECK(problem.get_criteria()[0].get_real_values().get_max_value() == doctest::Approx(59.3086));
-  CHECK(model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[0] == doctest::Approx(6.52194));
+  CHECK(*model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[0] == doctest::Approx(6.52194));
   CHECK(alternatives.get_alternatives()[0].get_profile()[0].get_real().get_value() == doctest::Approx(45.3692));
 
   CHECK(problem.get_criteria()[1].get_real_values().get_min_value() == doctest::Approx(-63.313));
   CHECK(problem.get_criteria()[1].get_real_values().get_max_value() == doctest::Approx(46.3988));
-  CHECK(model.get_accepted_values()[1].get_real_thresholds().get_thresholds()[0] == doctest::Approx(24.0712));
+  CHECK(*model.get_accepted_values()[1].get_real_thresholds().get_thresholds()[0] == doctest::Approx(24.0712));
   CHECK(alternatives.get_alternatives()[0].get_profile()[1].get_real().get_value() == doctest::Approx(-15.8581));
 }
 
 TEST_CASE("Decreasing criterion") {
   Problem problem = generate_classification_problem(
     1, 3,
     44,
@@ -672,16 +688,16 @@
     {Criterion::PreferenceDirection::increasing, Criterion::PreferenceDirection::decreasing}
   );
   Model model = generate_mrsort_classification_model(problem, 42);
   Alternatives alternatives = generate_classified_alternatives(problem, model, 10, 44);
 
   CHECK(problem.get_criteria()[0].get_real_values().get_preference_direction() == Criterion::PreferenceDirection::decreasing);
   // Profiles are in decreasing order
-  CHECK(model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[0] == doctest::Approx(0.790612));
-  CHECK(model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[1] == doctest::Approx(0.377049));
+  CHECK(*model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[0] == doctest::Approx(0.790612));
+  CHECK(*model.get_accepted_values()[0].get_real_thresholds().get_thresholds()[1] == doctest::Approx(0.377049));
 
   CHECK(alternatives.get_alternatives()[0].get_profile()[0].get_real().get_value() == doctest::Approx(0.834842));
   CHECK(*alternatives.get_alternatives()[0].get_category_index() == 0);
 
   CHECK(alternatives.get_alternatives()[1].get_profile()[0].get_real().get_value() == doctest::Approx(0.432542));
   CHECK(*alternatives.get_alternatives()[1].get_category_index() == 1);
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/generation.hpp` & `lincs-2.0.0a0/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/alternatives.cpp` & `lincs-2.0.0a0/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/alternatives.hpp` & `lincs-2.0.0a0/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/model.cpp` & `lincs-2.0.0a0/lincs/liblincs/io/model.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,40 @@
   out << f;
 
   CHECK(ss.str() == "0.444866359");
 
   CHECK(YAML::Load(ss).as<float>() == 0x1.c78b0cp-2f);  // No approximation: no loss of precision
 }
 
+namespace YAML {
+
+template<typename T>
+Emitter& operator<<(Emitter& out, const std::optional<T>& o) {
+  if (o) {
+    out << *o;
+  } else {
+    out << Null;
+  }
+  return out;
+}
+
+template <typename T>
+struct convert<std::optional<T>> {
+  static bool decode(const Node& node, std::optional<T>& rhs) {
+    if (node.IsNull()) {
+      rhs.reset();
+    } else {
+      rhs = node.as<T>();
+    }
+    return true;
+  }
+};
+
+}
+
 namespace lincs {
 
 const std::string Model::json_schema(R"($schema: https://json-schema.org/draft/2020-12/schema
 title: NCS classification model
 type: object
 properties:
   kind:
@@ -140,55 +166,88 @@
     validate(accepted_values[criterion_index].get_value_type() == criterion.get_value_type(), "The value type of an accepted values descriptor must be the same as the value type of the corresponding criterion");
     dispatch(
       accepted_values[criterion_index].get(),
       [&criterion, criterion_index, boundaries_count](const AcceptedValues::RealThresholds& thresholds) {
         validate(thresholds.get_thresholds().size() == boundaries_count, "The number of real thresholds in an accepted values descriptor must be one less than the number of categories in the problem");
         const auto& criterion_values = criterion.get_real_values();
         for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
-          validate(criterion_values.is_acceptable(thresholds.get_thresholds()[boundary_index]), "Each threshold in an accepted values descriptor must be between the min and max values for the corresponding real criterion");
+          const std::optional<float> threshold = thresholds.get_thresholds()[boundary_index];
+          if (threshold) {
+            validate(criterion_values.is_acceptable(*threshold), "Each threshold in an accepted values descriptor must be between the min and max values for the corresponding real criterion");
+          }
         }
         for (unsigned boundary_index = 1; boundary_index != boundaries_count; ++boundary_index) {
-          validate(
-            better_or_equal(
-              criterion_values.get_preference_direction(),
-              thresholds.get_thresholds()[boundary_index],
-              thresholds.get_thresholds()[boundary_index - 1]
-            ),
-            "The real thresholds in an accepted values descriptor must be in preference order"
-          );
+          const std::optional<float> previous_threshold = thresholds.get_thresholds()[boundary_index - 1];
+          const std::optional<float> threshold = thresholds.get_thresholds()[boundary_index];
+          if (previous_threshold) {
+            if (threshold) {
+              switch (criterion_values.get_preference_direction()) {
+                case Criterion::PreferenceDirection::increasing:
+                  validate(*threshold >= *previous_threshold, "The real thresholds in an accepted values descriptor must be in preference order");
+                  break;
+                case Criterion::PreferenceDirection::decreasing:
+                  validate(*threshold <= *previous_threshold, "The real thresholds in an accepted values descriptor must be in preference order");
+                  break;
+              }
+            }
+          } else {
+            validate(!threshold, "After a null threshold, all subsequent thresholds must be null");
+          }
         }
       },
       [&criterion, criterion_index, boundaries_count](const AcceptedValues::IntegerThresholds& thresholds) {
         validate(thresholds.get_thresholds().size() == boundaries_count, "The number of integer thresholds in an accepted values descriptor must be one less than the number of categories in the problem");
         const auto& criterion_values = criterion.get_integer_values();
         for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
-          validate(criterion_values.is_acceptable(thresholds.get_thresholds()[boundary_index]), "Each threshold in an accepted values descriptor must be between the min and max values for the corresponding integer criterion");
+          const std::optional<int> threshold = thresholds.get_thresholds()[boundary_index];
+          if (threshold) {
+            validate(criterion_values.is_acceptable(*threshold), "Each threshold in an accepted values descriptor must be between the min and max values for the corresponding integer criterion");
+          }
         }
         for (unsigned boundary_index = 1; boundary_index != boundaries_count; ++boundary_index) {
-          validate(
-            better_or_equal(
-              criterion.get_integer_values().get_preference_direction(),
-              thresholds.get_thresholds()[boundary_index],
-              thresholds.get_thresholds()[boundary_index - 1]
-            ),
-            "The integer thresholds in an accepted values descriptor must be in preference order"
-          );
+          const std::optional<int> previous_threshold = thresholds.get_thresholds()[boundary_index - 1];
+          const std::optional<int> threshold = thresholds.get_thresholds()[boundary_index];
+          if (previous_threshold) {
+            if (threshold) {
+              switch (criterion_values.get_preference_direction()) {
+                case Criterion::PreferenceDirection::increasing:
+                  validate(*threshold >= *previous_threshold, "The integer thresholds in an accepted values descriptor must be in preference order");
+                  break;
+                case Criterion::PreferenceDirection::decreasing:
+                  validate(*threshold <= *previous_threshold, "The integer thresholds in an accepted values descriptor must be in preference order");
+                  break;
+              }
+            }
+          } else {
+            validate(!threshold, "After a null threshold, all subsequent thresholds must be null");
+          }
         }
       },
       [&criterion, criterion_index, boundaries_count](const AcceptedValues::EnumeratedThresholds& thresholds) {
         validate(thresholds.get_thresholds().size() == boundaries_count, "The number of enumerated thresholds in an accepted values descriptor must be one less than the number of categories in the problem");
         const auto& criterion_values = criterion.get_enumerated_values();
         for (unsigned boundary_index = 0; boundary_index != boundaries_count; ++boundary_index) {
-          validate(criterion_values.is_acceptable(thresholds.get_thresholds()[boundary_index]), "Each threshold in an accepted values descriptor must be in the enumerated values for the corresponding criterion");
+          const std::optional<std::string>& threshold = thresholds.get_thresholds()[boundary_index];
+          if (threshold) {
+            validate(criterion_values.is_acceptable(*threshold), "Each threshold in an accepted values descriptor must be in the enumerated values for the corresponding criterion");
+          }
         }
         for (unsigned boundary_index = 1; boundary_index != boundaries_count; ++boundary_index) {
-          validate(
-            criterion_values.get_value_rank(thresholds.get_thresholds()[boundary_index]) >= criterion_values.get_value_rank(thresholds.get_thresholds()[boundary_index - 1]),
-            "The enumerated thresholds in an accepted values descriptor must be in preference order"
-          );
+          const std::optional<std::string>& previous_threshold = thresholds.get_thresholds()[boundary_index - 1];
+          const std::optional<std::string>& threshold = thresholds.get_thresholds()[boundary_index];
+          if (previous_threshold) {
+            if (threshold) {
+              validate(
+                criterion_values.get_value_rank(*threshold) >= criterion_values.get_value_rank(*previous_threshold),
+                "The enumerated thresholds in an accepted values descriptor must be in preference order"
+              );
+            }
+          } else {
+            validate(!threshold, "After a null threshold, all subsequent thresholds must be null");
+          }
         }
       }
     );
   };
 
   validate(sufficient_coalitions.size() == boundaries_count, "The number of sufficient coalitions in the model must be one less than the number of categories in the problem");
   for (const auto& sufficient_coalitions_ : sufficient_coalitions) {
@@ -232,14 +291,16 @@
   #ifdef NDEBUG
   YAML::Emitter out(os);
   #else
   std::stringstream ss;
   YAML::Emitter out(ss);
   #endif
 
+  out.SetNullFormat(YAML::EMITTER_MANIP::LowerNull);
+
   bool use_coalitions_alias =
     sufficient_coalitions.size() > 1
     && std::all_of(std::next(sufficient_coalitions.begin()), sufficient_coalitions.end(), [&](const SufficientCoalitions& suff_coals) {
       return suff_coals == sufficient_coalitions.front();
     });
 
   out << YAML::BeginMap;
@@ -335,21 +396,21 @@
     const YAML::Node& yaml_acc_vals = yaml_accepted_values[criterion_index];
     assert(yaml_acc_vals["kind"].as<std::string>() == "thresholds");
     const YAML::Node& thresholds = yaml_acc_vals["thresholds"];
 
     accepted_values.push_back(dispatch(
       criterion.get_values(),
       [&thresholds, boundaries_count](const Criterion::RealValues&) {
-        return AcceptedValues(AcceptedValues::RealThresholds(thresholds.as<std::vector<float>>()));
+        return AcceptedValues(AcceptedValues::RealThresholds(thresholds.as<std::vector<std::optional<float>>>()));
       },
       [&thresholds, boundaries_count](const Criterion::IntegerValues&) {
-        return AcceptedValues(AcceptedValues::IntegerThresholds(thresholds.as<std::vector<int>>()));
+        return AcceptedValues(AcceptedValues::IntegerThresholds(thresholds.as<std::vector<std::optional<int>>>()));
       },
       [&thresholds, boundaries_count](const Criterion::EnumeratedValues&) {
-        return AcceptedValues(AcceptedValues::EnumeratedThresholds(thresholds.as<std::vector<std::string>>()));
+        return AcceptedValues(AcceptedValues::EnumeratedThresholds(thresholds.as<std::vector<std::optional<std::string>>>()));
       }
     ));
   }
 
   const YAML::Node& yaml_sufficient_coalitions = node["sufficient_coalitions"];
   std::vector<SufficientCoalitions> sufficient_coalitions;
   sufficient_coalitions.reserve(boundaries_count);
@@ -501,14 +562,59 @@
     criterion_weights: [0.75]
   - *coalitions
 )");
 
   CHECK(Model::load(problem, ss) == model);
 }
 
+TEST_CASE("dumping then loading model preserves data - null thresholds") {
+  Problem problem{
+    {
+      Criterion("Real", Criterion::RealValues(Criterion::PreferenceDirection::increasing, -1, 1)),
+      Criterion("Integer", Criterion::IntegerValues(Criterion::PreferenceDirection::increasing, 0, 100)),
+    },
+    {{"Cat 1"}, {"Cat 2"}, {"Cat 3"}, {"Cat 4"}, {"Cat 5"}},
+  };
+
+  Model model{
+    problem,
+    {
+      AcceptedValues(AcceptedValues::RealThresholds({-0.5, 0, std::nullopt, std::nullopt})),
+      AcceptedValues(AcceptedValues::IntegerThresholds({20, 40, 60, std::nullopt})),
+    },
+    {
+      SufficientCoalitions(SufficientCoalitions::Weights({0.5, 0.5})),
+      SufficientCoalitions(SufficientCoalitions::Weights({0.5, 0.5})),
+      SufficientCoalitions(SufficientCoalitions::Weights({0.5, 0.5})),
+      SufficientCoalitions(SufficientCoalitions::Weights({0.5, 0.5})),
+    },
+  };
+
+  std::stringstream ss;
+  model.dump(problem, ss);
+
+  CHECK(ss.str() == R"(kind: ncs-classification-model
+format_version: 1
+accepted_values:
+  - kind: thresholds
+    thresholds: [-0.5, 0, null, null]
+  - kind: thresholds
+    thresholds: [20, 40, 60, null]
+sufficient_coalitions:
+  - &coalitions
+    kind: weights
+    criterion_weights: [0.5, 0.5]
+  - *coalitions
+  - *coalitions
+  - *coalitions
+)");
+
+  CHECK(Model::load(problem, ss) == model);
+}
+
 TEST_CASE("dumping then loading model preserves data - enumerated criterion") {
   Problem problem{
     {Criterion("Criterion 1", Criterion::EnumeratedValues({"F", "E", "D", "C", "B", "A"}))},
     {{"Category 1"}, {"Category 2"}, {"Category 3"}},
   };
 
   Model model{
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/model.hpp` & `lincs-2.0.0a0/lincs/liblincs/io/model.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 // Copyright 2023-2024 Vincent Jacques
 
 #ifndef LINCS__IO__MODEL_HPP
 #define LINCS__IO__MODEL_HPP
 
+#include <optional>
+
 #include <boost/dynamic_bitset.hpp>
 
 #include "../internal.hpp"
 #include "problem.hpp"
 
 
 namespace lincs {
 
 class AcceptedValues {
  public:
   class RealThresholds {
    public:
-    RealThresholds(const std::vector<float>& thresholds_) : thresholds(thresholds_) {}
+    RealThresholds(const std::vector<std::optional<float>>& thresholds_) : thresholds(thresholds_) {}
 
    public:
     bool operator==(const RealThresholds& other) const {
       return thresholds == other.thresholds;
     }
 
    public:
-    const std::vector<float>& get_thresholds() const { return thresholds; }
+    const std::vector<std::optional<float>>& get_thresholds() const { return thresholds; }
 
    private:
-    std::vector<float> thresholds;
+    std::vector<std::optional<float>> thresholds;
   };
 
   class IntegerThresholds {
    public:
-    IntegerThresholds(const std::vector<int>& thresholds_) : thresholds(thresholds_) {}
+    IntegerThresholds(const std::vector<std::optional<int>>& thresholds_) : thresholds(thresholds_) {}
 
    public:
     bool operator==(const IntegerThresholds& other) const {
       return thresholds == other.thresholds;
     }
 
    public:
-    const std::vector<int>& get_thresholds() const { return thresholds; }
+    const std::vector<std::optional<int>>& get_thresholds() const { return thresholds; }
 
    private:
-    std::vector<int> thresholds;
+    std::vector<std::optional<int>> thresholds;
   };
 
   class EnumeratedThresholds {
    public:
-    EnumeratedThresholds(const std::vector<std::string>& thresholds_) : thresholds(thresholds_) {}
+    EnumeratedThresholds(const std::vector<std::optional<std::string>>& thresholds_) : thresholds(thresholds_) {}
 
    public:
     bool operator==(const EnumeratedThresholds& other) const {
       return thresholds == other.thresholds;
     }
 
    public:
-    const std::vector<std::string>& get_thresholds() const { return thresholds; }
+    const std::vector<std::optional<std::string>>& get_thresholds() const { return thresholds; }
 
    private:
-    std::vector<std::string> thresholds;
+    std::vector<std::optional<std::string>> thresholds;
   };
 
   // WARNING: keep the enum and the variant consistent with 'Criterion::ValueType'
   // WARNING: Adding a value to the enum will require fixing 'get_value_type' (and obviously 'get_kind' and 'is_thresholds')
   enum class Kind { thresholds };
   typedef std::variant<RealThresholds, IntegerThresholds, EnumeratedThresholds> Self;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/problem.cpp` & `lincs-2.0.0a0/lincs/liblincs/io/problem.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     items:
       type: object
       oneOf:
         - properties:
             name:
               type: string
             value_type:
-              description: May be extended in the future to handle criteria with integer values, or explicitly enumerated values.
               type: string
               enum: [real, integer]
             preference_direction:
               description: May be extended in the future to handle single-peaked criteria, or criteria with unknown preference direction.
               type: string
               enum: [increasing, isotone, decreasing, antitone]
             min_value:
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/problem.hpp` & `lincs-2.0.0a0/lincs/liblincs/io/problem.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include <cassert>
 #include <map>
 #include <string>
 #include <vector>
 
 #include "../variant-dispatch.hpp"
 #include "../unreachable.hpp"
-#include "validation.hpp"
+#include "exception.hpp"
 
 
 namespace lincs {
 
 class Criterion {
  public:
   enum class PreferenceDirection {
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/io/validation.cpp` & `lincs-2.0.0a0/lincs/liblincs/io/validation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 #include "../../../chrones.hpp"
 #include "../../../randomness-utils.hpp"
 
 
 namespace lincs {
 
-void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles() {
+void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles(
+  const unsigned model_indexes_begin,
+  const unsigned model_indexes_end
+) {
   CHRONE();
 
-  const int models_count = learning_data.models_count;
   #pragma omp parallel for
-  for (int model_index = 0; model_index < models_count; ++model_index) {
+  for (int model_indexes_index = model_indexes_begin; model_indexes_index < model_indexes_end; ++model_indexes_index) {
+    const unsigned model_index = learning_data.model_indexes[model_indexes_index];
     improve_model_profiles(model_index);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profiles(const unsigned model_index) {
   Array1D<Host, unsigned> criterion_indexes(learning_data.criteria_count, uninitialized);
   // Not worth parallelizing because criteria_count is typically small
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 namespace lincs {
 
 class ImproveProfilesWithAccuracyHeuristicOnCpu : public LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy {
  public:
   explicit ImproveProfilesWithAccuracyHeuristicOnCpu(LearningData& learning_data_) : learning_data(learning_data_) {}
 
  public:
-  void improve_profiles() override;
+  void improve_profiles(unsigned model_indexes_begin, unsigned model_indexes_end) override;
 
  private:
   void improve_model_profiles(const unsigned model_index);
 
   void improve_model_profile(
     const unsigned model_index,
     const unsigned profile_index,
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files 1% similar despite different names*

```diff
@@ -245,24 +245,28 @@
   assignments(host_learning_data.assignments.template clone_to<Device>()),
   weights(host_learning_data.models_count, host_learning_data.criteria_count, uninitialized),
   profile_ranks(host_learning_data.models_count, host_learning_data.boundaries_count, host_learning_data.criteria_count, uninitialized),
   desirabilities(host_learning_data.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::max_destinations_count, uninitialized),
   destination_ranks(host_learning_data.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::max_destinations_count, uninitialized)
 {}
 
-void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles() {
+void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles(
+  const unsigned model_indexes_begin,
+  const unsigned model_indexes_end
+) {
   CHRONE();
 
   // Get optimized weights
   copy(host_learning_data.weights, ref(gpu_learning_data.weights));
   // Get (re-)initialized profiles
   copy(host_learning_data.profile_ranks, ref(gpu_learning_data.profile_ranks));
 
   #pragma omp parallel for
-  for (int model_index = 0; model_index < host_learning_data.models_count; ++model_index) {
+  for (int model_indexes_index = model_indexes_begin; model_indexes_index < model_indexes_end; ++model_indexes_index) {
+    const unsigned model_index = host_learning_data.model_indexes[model_indexes_index];
     improve_model_profiles(model_index);
   }
 
   // Set improved profiles
   copy(gpu_learning_data.profile_ranks, ref(host_learning_data.profile_ranks));
 }
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Array2D<Device, unsigned> destination_ranks;  // [model_index][desination_index]
   };
 
  public:
   explicit ImproveProfilesWithAccuracyHeuristicOnGpu(LearningData& host_learning_data_) : host_learning_data(host_learning_data_), gpu_learning_data(host_learning_data) {}
 
  public:
-  void improve_profiles() override;
+  void improve_profiles(unsigned model_indexes_begin, unsigned model_indexes_end) override;
 
  private:
   void improve_model_profiles(const unsigned model_index);
 
   void improve_model_profile(
     const unsigned model_index,
     const unsigned profile_index,
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -84,22 +84,23 @@
 
     assert(!rank_probabilities.empty());
     return rank_probabilities;
   }
 }
 
 void InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::initialize_profiles(
-  unsigned model_indexes_begin,
+  const unsigned model_indexes_begin,
   const unsigned model_indexes_end
 ) {
   CHRONE();
 
+  // @todo(Performance, later) Parallelize these loops?
   // Embarrassingly parallel
-  for (; model_indexes_begin != model_indexes_end; ++model_indexes_begin) {
-    const unsigned model_index = learning_data.model_indexes[model_indexes_begin];
+  for (unsigned model_indexes_index = model_indexes_begin; model_indexes_index < model_indexes_end; ++model_indexes_index) {
+    const unsigned model_index = learning_data.model_indexes[model_indexes_index];
 
     // Embarrassingly parallel
     for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
       // Not parallel because of the profiles ordering constraint
       for (unsigned category_index = learning_data.categories_count - 1; category_index != 0; --category_index) {
         const unsigned profile_index = category_index - 1;
         unsigned rank = rank_generators[criterion_index][profile_index](learning_data.urbgs[model_index]);
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 #include "../../../linear-programming/alglib.hpp"
 #include "../../../linear-programming/glop.hpp"
 
 
 namespace lincs {
 
 template<typename LinearProgram>
-void OptimizeWeightsUsingLinearProgram<LinearProgram>::optimize_weights() {
+void OptimizeWeightsUsingLinearProgram<LinearProgram>::optimize_weights(
+  const unsigned model_indexes_begin,
+  const unsigned model_indexes_end
+) {
   CHRONE();
 
-  const int models_count = learning_data.models_count;
   #pragma omp parallel for
-  for (int model_index = 0; model_index < models_count; ++model_index) {
+  for (int model_indexes_index = model_indexes_begin; model_indexes_index < model_indexes_end; ++model_indexes_index) {
+    const unsigned model_index = learning_data.model_indexes[model_indexes_index];
     optimize_model_weights(model_index);
   }
 }
 
 template<typename LinearProgram>
 void OptimizeWeightsUsingLinearProgram<LinearProgram>::optimize_model_weights(unsigned model_index) {
   const float epsilon = 1e-6;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 template<typename LinearProgram>
 class OptimizeWeightsUsingLinearProgram : public LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy {
  public:
   OptimizeWeightsUsingLinearProgram(LearningData& learning_data_) : learning_data(learning_data_) {}
 
  public:
-  void optimize_weights() override;
+  void optimize_weights(unsigned model_indexes_begin, unsigned model_indexes_end) override;
 
  private:
   void optimize_model_weights(unsigned model_index);
 
  private:
   LearningData& learning_data;
 };
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations-without-progress.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations-without-progress.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds-without-progress.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds-without-progress.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,21 @@
 Model LearnMrsortByWeightsProfilesBreed::perform() {
   CHRONE();
 
   profiles_initialization_strategy.initialize_profiles(0, learning_data.models_count);
 
   while (true) {
     // Improve
-    weights_optimization_strategy.optimize_weights();
-    profiles_improvement_strategy.improve_profiles();
+    weights_optimization_strategy.optimize_weights(0, learning_data.models_count);
+    profiles_improvement_strategy.improve_profiles(0, learning_data.models_count);
+
+    // @todo(Feature, later) Rework this main loop. Its current problems:
+    //   - we return models that have gone through a last profiles improvement, but their weights have not been optimized
+    //   - we decide to stop the learning based on the accuracy of those models in this weird state
+    // Beware, if optimize_weights is run after improve_profiles, it must also be run during the breeding strategy.
 
     // Sort model_indexes by increasing model accuracy
     for (unsigned model_index = 0; model_index != learning_data.models_count; ++model_index) {
       learning_data.accuracies[model_index] = compute_accuracy(model_index);
     }
     std::sort(
       learning_data.model_indexes.begin(), learning_data.model_indexes.end(),
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
   ) :
     learning_data(learning_data_),
     profiles_initialization_strategy(profiles_initialization_strategy_),
     weights_optimization_strategy(weights_optimization_strategy_),
     profiles_improvement_strategy(profiles_improvement_strategy_),
     breeding_strategy(breeding_strategy_),
     termination_strategy(termination_strategy_),
-    observers(observers_) {}
+    observers(observers_)
+  {}
 
  public:
   Model perform();
 
  private:
   unsigned compute_accuracy(const unsigned model_index);
   bool is_correctly_assigned(const unsigned model_index, const unsigned alternative_index);
@@ -89,23 +90,23 @@
 };
 
 struct LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy {
   typedef LearnMrsortByWeightsProfilesBreed::LearningData LearningData;
 
   virtual ~WeightsOptimizationStrategy() {}
 
-  virtual void optimize_weights() = 0;
+  virtual void optimize_weights(unsigned model_indexes_begin, unsigned model_indexes_end) = 0;
 };
 
 struct LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy {
   typedef LearnMrsortByWeightsProfilesBreed::LearningData LearningData;
 
   virtual ~ProfilesImprovementStrategy() {}
 
-  virtual void improve_profiles() = 0;
+  virtual void improve_profiles(unsigned model_indexes_begin, unsigned model_indexes_end) = 0;
 };
 
 struct LearnMrsortByWeightsProfilesBreed::BreedingStrategy {
   typedef LearnMrsortByWeightsProfilesBreed::LearningData LearningData;
 
   virtual ~BreedingStrategy() {}
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/pre-processing.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/pre-processing.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   performance_ranks(criteria_count, alternatives_count, uninitialized),
   assignments(alternatives_count, uninitialized)
 {
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     dispatch(
       problem.get_criteria()[criterion_index].get_values(),
       [this, &learning_set, criterion_index](const Criterion::RealValues& values) {
-        const bool is_increasing = values.get_preference_direction() == Criterion::PreferenceDirection::increasing;
-        assert(is_increasing || values.get_preference_direction() == Criterion::PreferenceDirection::decreasing);
+        const bool is_increasing = values.is_increasing();
+        assert(is_increasing || values.is_decreasing());
 
         std::set<float> unique_values;
 
         unique_values.insert(values.get_min_value());
         unique_values.insert(values.get_max_value());
         for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
           unique_values.insert(learning_set.get_alternatives()[alternative_index].get_profile()[criterion_index].get_real().get_value());
@@ -52,16 +52,16 @@
         for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
           const float value = learning_set.get_alternatives()[alternative_index].get_profile()[criterion_index].get_real().get_value();
           const unsigned value_rank = value_ranks_for_criterion[value];
           performance_ranks[criterion_index][alternative_index] = value_rank;
         }
       },
       [this, &learning_set, criterion_index](const Criterion::IntegerValues& values) {
-        const bool is_increasing = values.get_preference_direction() == Criterion::PreferenceDirection::increasing;
-        assert(is_increasing || values.get_preference_direction() == Criterion::PreferenceDirection::decreasing);
+        const bool is_increasing = values.is_increasing();
+        assert(is_increasing || values.is_decreasing());
 
         std::set<int> unique_values;
 
         unique_values.insert(values.get_min_value());
         unique_values.insert(values.get_max_value());
         for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
           unique_values.insert(learning_set.get_alternatives()[alternative_index].get_profile()[criterion_index].get_integer().get_value());
@@ -113,57 +113,49 @@
 
   std::vector<AcceptedValues> accepted_values;
   accepted_values.reserve(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     accepted_values.push_back(dispatch(
       problem.get_criteria()[criterion_index].get_values(),
       [this, &boundaries, criterion_index](const Criterion::RealValues&) {
-        std::vector<float> thresholds;
+        std::vector<std::optional<float>> thresholds;
         thresholds.reserve(boundaries_count);
         for (const auto& boundary: boundaries) {
           const unsigned rank = boundary.profile_ranks[criterion_index];
-          if (rank == 0) {
+          if (rank < values_counts[criterion_index]) {
             thresholds.push_back(real_sorted_values.at(criterion_index)[rank]);
-          } else if (rank == values_counts[criterion_index]) {
-            // Past-the-end rank
-            thresholds.push_back(real_sorted_values.at(criterion_index)[values_counts[criterion_index] - 1]);
           } else {
-            thresholds.push_back(real_sorted_values.at(criterion_index)[rank]);
+            // Past-the-end rank => this criterion cannot help reach this category
+            thresholds.push_back(std::nullopt);
           }
         }
         return AcceptedValues(AcceptedValues::RealThresholds(thresholds));
       },
       [this, &boundaries, criterion_index](const Criterion::IntegerValues&) {
-        std::vector<int> thresholds;
+        std::vector<std::optional<int>> thresholds;
         thresholds.reserve(boundaries_count);
         for (const auto& boundary: boundaries) {
           const unsigned rank = boundary.profile_ranks[criterion_index];
-          if (rank == 0) {
+          if (rank < values_counts[criterion_index]) {
             thresholds.push_back(integer_sorted_values.at(criterion_index)[rank]);
-          } else if (rank == values_counts[criterion_index]) {
-            // Past-the-end rank
-            thresholds.push_back(integer_sorted_values.at(criterion_index)[values_counts[criterion_index] - 1]);
           } else {
-            thresholds.push_back(integer_sorted_values.at(criterion_index)[rank]);
+            thresholds.push_back(std::nullopt);
           }
         }
         return AcceptedValues(AcceptedValues::IntegerThresholds(thresholds));
       },
       [this, &boundaries, criterion_index](const Criterion::EnumeratedValues& values) {
-        std::vector<std::string> thresholds;
+        std::vector<std::optional<std::string>> thresholds;
         thresholds.reserve(boundaries_count);
         for (const auto& boundary: boundaries) {
           const unsigned rank = boundary.profile_ranks[criterion_index];
-          if (rank == 0) {
+          if (rank < values_counts[criterion_index]) {
             thresholds.push_back(values.get_ordered_values()[rank]);
-          } else if (rank == values_counts[criterion_index]) {
-            // Past-the-end rank
-            thresholds.push_back(values.get_ordered_values()[values_counts[criterion_index] - 1]);
           } else {
-            thresholds.push_back(values.get_ordered_values()[rank]);
+            thresholds.push_back(std::nullopt);
           }
         }
         return AcceptedValues(AcceptedValues::EnumeratedThresholds(thresholds));
       }));
   }
 
   std::vector<SufficientCoalitions> sufficient_coalitions;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/pre-processing.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/pre-processing.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #include "ucncs-by-max-sat-by-coalitions.hpp"
 
 #include <algorithm>
 #include <map>
 #include <type_traits>
 
 #include "../chrones.hpp"
+#include "../classification.hpp"
 #include "../sat/eval-max-sat.hpp"
 #include "exception.hpp"
 
 
 namespace lincs {
 
 template<typename V>
@@ -27,15 +28,15 @@
   create_variables();
   add_structural_constraints();
   add_learning_set_constraints();
 
   std::optional<std::vector<bool>> solution = sat.solve();
 
   if (!solution) {
-    throw LearningFailureException();
+    throw LearningFailureException("MaxSatCoalitions failed to find a solution.");
   }
 
   return decode(*solution);
 }
 
 template<typename MaxSatProblem>
 void MaxSatCoalitionsUcncsLearning<MaxSatProblem>::create_all_coalitions() {
@@ -232,13 +233,23 @@
         profile_ranks[criterion_index] = learning_set.values_counts[criterion_index];
       }
     }
 
     boundaries.emplace_back(profile_ranks, SufficientCoalitions(SufficientCoalitions::Roots(Internal(), roots)));
   }
 
-  return learning_set.post_process(boundaries);
+  const Model model = learning_set.post_process(boundaries);
+  #ifndef NDEBUG
+  unsigned expected_correct_count = 0;
+  for (unsigned alternative_index = 0; alternative_index != learning_set.alternatives_count; ++alternative_index) {
+    if (solution[correct[alternative_index]]) {
+      ++expected_correct_count;
+    }
+  }
+  assert(count_correctly_classified_alternatives(input_problem, model, input_learning_set) == expected_correct_count);
+  #endif
+  return model;
 }
 
 template class MaxSatCoalitionsUcncsLearning<EvalmaxsatMaxSatProblem>;
 
 }  // namespace lincs
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-coalitions.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 namespace lincs {
 
 template<typename MaxSatProblem>
 class MaxSatCoalitionsUcncsLearning {
  public:
   template<class... U>
   MaxSatCoalitionsUcncsLearning(const Problem& problem, const Alternatives& learning_set_, U&&... u) :
+    #ifndef NDEBUG
+    input_problem(problem),
+    input_learning_set(learning_set_),
+    #endif
     learning_set(problem, learning_set_),
     coalitions_count(1 << learning_set.criteria_count),
     goal_weight(1),
     better(),
     sufficient(),
     sat(std::forward<U>(u)...)
   {}
@@ -36,14 +40,18 @@
   void create_all_coalitions();
   void create_variables();
   void add_structural_constraints();
   void add_learning_set_constraints();
   Model decode(const std::vector<bool>& solution);
 
  private:
+  #ifndef NDEBUG
+  const Problem& input_problem;
+  const Alternatives& input_learning_set;
+  #endif
   PreProcessedLearningSet learning_set;
   const unsigned coalitions_count;
   typedef boost::dynamic_bitset<> Coalition;
   std::vector<Coalition> all_coalitions;
   const typename MaxSatProblem::weight_type goal_weight;
   // better[criterion_index][boundary_index][value_rank]: value is better than profile on criterion
   std::vector<std::vector<std::vector<typename MaxSatProblem::variable_type>>> better;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 #include <algorithm>
 #include <map>
 #include <set>
 #include <type_traits>
 
 #include "../chrones.hpp"
+#include "../classification.hpp"
 #include "../sat/eval-max-sat.hpp"
 #include "exception.hpp"
 
 
 namespace lincs {
 
 template<typename V>
@@ -28,15 +29,15 @@
   create_variables();
   add_structural_constraints();
   add_learning_set_constraints();
 
   std::optional<std::vector<bool>> solution = sat.solve();
 
   if (!solution) {
-    throw LearningFailureException();
+    throw LearningFailureException("MaxSatSeparation failed to find a solution.");
   }
 
   return decode(*solution);
 }
 
 template<typename MaxSatProblem>
 void MaxSatSeparationUcncsLearning<MaxSatProblem>::partition_alternatives() {
@@ -284,13 +285,23 @@
 
   std::vector<PreProcessedBoundary> boundaries;
   boundaries.reserve(learning_set.boundaries_count);
   for (unsigned boundary_index = 0; boundary_index != learning_set.boundaries_count; ++boundary_index) {
     boundaries.emplace_back(profile_ranks[boundary_index], SufficientCoalitions(SufficientCoalitions::Roots(Internal(), roots)));
   }
 
-  return learning_set.post_process(boundaries);
+  const Model model = learning_set.post_process(boundaries);
+  #ifndef NDEBUG
+  unsigned expected_correct_count = 0;
+  for (unsigned alternative_index = 0; alternative_index != learning_set.alternatives_count; ++alternative_index) {
+    if (solution[correct[alternative_index]]) {
+      ++expected_correct_count;
+    }
+  }
+  assert(count_correctly_classified_alternatives(input_problem, model, input_learning_set) == expected_correct_count);
+  #endif
+  return model;
 }
 
 template class MaxSatSeparationUcncsLearning<EvalmaxsatMaxSatProblem>;
 
 }  // namespace lincs
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-max-sat-by-separation.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 namespace lincs {
 
 template<typename MaxSatProblem>
 class MaxSatSeparationUcncsLearning {
  public:
   template<class... U>
   MaxSatSeparationUcncsLearning(const Problem& problem, const Alternatives& learning_set_, U&&... u) :
+    #ifndef NDEBUG
+    input_problem(problem),
+    input_learning_set(learning_set_),
+    #endif
     learning_set(problem, learning_set_),
     subgoal_weight(1),
     goal_weight(learning_set.boundaries_count * learning_set.alternatives_count),
     better_alternative_indexes(),
     worse_alternative_indexes(),
     better(),
     separates(),
@@ -32,22 +36,26 @@
   void partition_alternatives();
   void create_variables();
   void add_structural_constraints();
   void add_learning_set_constraints();
   Model decode(const std::vector<bool>& solution);
 
  private:
+  #ifndef NDEBUG
+  const Problem& input_problem;
+  const Alternatives& input_learning_set;
+  #endif
   PreProcessedLearningSet learning_set;
   const typename MaxSatProblem::weight_type subgoal_weight;
   const typename MaxSatProblem::weight_type goal_weight;
   // Alternatives better than category k
   std::vector<std::vector<unsigned>> better_alternative_indexes;
   // Alternatives in category k or worse
   std::vector<std::vector<unsigned>> worse_alternative_indexes;
-  // better[criterion_index][boundary_index][value_rank]: value is better profile on criterion
+  // better[criterion_index][boundary_index][value_rank]: value is better than profile on criterion
   std::vector<std::vector<std::vector<typename MaxSatProblem::variable_type>>> better;
   // separates[criterion_index][boundary_index_a][boundary_index_b][good_alternative_index][bad_alternative_index]:
   // criterion separates alternatives 'good' and 'bad' with regards to profiles 'a' and 'b'
   std::vector<std::vector<std::vector<std::vector<std::vector<typename MaxSatProblem::variable_type>>>>> separates;
   // correct[alternative_index]: alternative is correctly classified
   std::vector<typename MaxSatProblem::variable_type> correct;
   // proper[alternative_index][boundary_index]: alternative is properly classified by the 2-categories model defined by the boundary
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #include "ucncs-by-sat-by-coalitions.hpp"
 
 #include <algorithm>
 #include <map>
 #include <type_traits>
 
 #include "../chrones.hpp"
+#include "../classification.hpp"
 #include "../sat/minisat.hpp"
 #include "exception.hpp"
 
 
 namespace lincs {
 
 // @todo(Project management, v1.2) Factorize common parts of all SAT approaches (when we implement single-peaked criteria)
@@ -38,15 +39,15 @@
   create_variables();
   add_structural_constraints();
   add_learning_set_constraints();
 
   std::optional<std::vector<bool>> solution = sat.solve();
 
   if (!solution) {
-    throw LearningFailureException();
+    throw LearningFailureException("SatCoalitions failed to find a solution.");
   }
 
   return decode(*solution);
 }
 
 template<typename SatProblem>
 void SatCoalitionsUcncsLearning<SatProblem>::create_all_coalitions() {
@@ -239,13 +240,15 @@
         profile_ranks[criterion_index] = learning_set.values_counts[criterion_index];
       }
     }
 
     boundaries.emplace_back(profile_ranks, SufficientCoalitions(SufficientCoalitions::Roots(Internal(), roots)));
   }
 
-  return learning_set.post_process(boundaries);
+  const Model model = learning_set.post_process(boundaries);
+  assert(count_correctly_classified_alternatives(input_problem, model, input_learning_set) == learning_set.alternatives_count);
+  return model;
 }
 
 template class SatCoalitionsUcncsLearning<MinisatSatProblem>;
 
 }  // namespace lincs
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 namespace lincs {
 
 template<typename SatProblem>
 class SatCoalitionsUcncsLearning {
  public:
   template<class... U>
   SatCoalitionsUcncsLearning(const Problem& problem, const Alternatives& learning_set_, U&&... u) :
+    #ifndef NDEBUG
+    input_problem(problem),
+    input_learning_set(learning_set_),
+    #endif
     learning_set(problem, learning_set_),
     coalitions_count(1 << learning_set.criteria_count),
     better(),
     sufficient(),
     sat(std::forward<U>(u)...)
   {}
 
@@ -35,14 +39,18 @@
   void create_all_coalitions();
   void create_variables();
   void add_structural_constraints();
   void add_learning_set_constraints();
   Model decode(const std::vector<bool>& solution);
 
  private:
+  #ifndef NDEBUG
+  const Problem& input_problem;
+  const Alternatives& input_learning_set;
+  #endif
   PreProcessedLearningSet learning_set;
   const unsigned coalitions_count;
   // @todo(Performance, later) Dematerialize 'all_coalitions':
   // use a more abstract class that can be used in place of the current std::vector<boost::dynamic_bitset<>>
   // Same in "max-SAT by coalitions"
   typedef boost::dynamic_bitset<> Coalition;
   std::vector<Coalition> all_coalitions;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-separation.cpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-separation.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 #include <algorithm>
 #include <map>
 #include <set>
 #include <type_traits>
 
 #include "../chrones.hpp"
+#include "../classification.hpp"
 #include "../sat/minisat.hpp"
 #include "exception.hpp"
 
 
 namespace lincs {
 
 template<typename V>
@@ -28,15 +29,15 @@
   create_variables();
   add_structural_constraints();
   add_learning_set_constraints();
 
   std::optional<std::vector<bool>> solution = sat.solve();
 
   if (!solution) {
-    throw LearningFailureException();
+    throw LearningFailureException("SatSeparation failed to find a solution.");
   }
 
   return decode(*solution);
 }
 
 template<typename SatProblem>
 void SatSeparationUcncsLearning<SatProblem>::partition_alternatives() {
@@ -242,13 +243,15 @@
 
   std::vector<PreProcessedBoundary> boundaries;
   boundaries.reserve(learning_set.boundaries_count);
   for (unsigned boundary_index = 0; boundary_index != learning_set.boundaries_count; ++boundary_index) {
     boundaries.emplace_back(profile_ranks[boundary_index], SufficientCoalitions(SufficientCoalitions::Roots(Internal(), roots)));
   }
 
-  return learning_set.post_process(boundaries);
+  const Model model = learning_set.post_process(boundaries);
+  assert(count_correctly_classified_alternatives(input_problem, model, input_learning_set) == learning_set.alternatives_count);
+  return model;
 }
 
 template class SatSeparationUcncsLearning<MinisatSatProblem>;
 
 }  // namespace lincs
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning/ucncs-by-sat-by-separation.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 namespace lincs {
 
 template<typename SatProblem>
 class SatSeparationUcncsLearning {
  public:
   template<class... U>
   SatSeparationUcncsLearning(const Problem& problem, const Alternatives& learning_set_, U&&... u) :
+    #ifndef NDEBUG
+    input_problem(problem),
+    input_learning_set(learning_set_),
+    #endif
     learning_set(problem, learning_set_),
     better_alternative_indexes(),
     worse_alternative_indexes(),
     better(),
     separates(),
     sat(std::forward<U>(u)...)
   {}
@@ -29,14 +33,18 @@
   void partition_alternatives();
   void create_variables();
   void add_structural_constraints();
   void add_learning_set_constraints();
   Model decode(const std::vector<bool>& solution);
 
  private:
+  #ifndef NDEBUG
+  const Problem& input_problem;
+  const Alternatives& input_learning_set;
+  #endif
   PreProcessedLearningSet learning_set;
   // Alternatives better than category k
   std::vector<std::vector<unsigned>> better_alternative_indexes;
   // Alternatives in category k or worse
   std::vector<std::vector<unsigned>> worse_alternative_indexes;
   // better[criterion_index][boundary_index][value_rank]: value is better than profile on criterion
   std::vector<std::vector<std::vector<typename SatProblem::variable_type>>> better;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/learning.hpp` & `lincs-2.0.0a0/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/liblincs-module/converters.cpp` & `lincs-2.0.0a0/lincs/liblincs/liblincs-module/converters.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -95,14 +95,58 @@
       &std_vector_converter<std::vector<T>>::construct,
       bp::type_id<std::vector<std::vector<T>>>()
     );
   }
 };
 
 template<typename T>
+struct std_vector_converter<std::optional<T>> {
+  static PyObject* convert(const std::vector<std::optional<T>>& xs) {
+    bp::list result;
+    for (const std::optional<T>& x : xs) {
+      if (x) {
+        result.append(*x);
+      } else {
+        result.append(bp::object());
+      }
+    }
+    return bp::incref(result.ptr());
+  }
+
+  static void* convertible(PyObject* obj) {
+    if (PyObject_GetIter(obj)) {
+      return obj;
+    } else {
+      return nullptr;
+    }
+  }
+
+  static void construct(PyObject* obj, bp::converter::rvalue_from_python_stage1_data* data) {
+    bp::handle<> handle(bp::borrowed(obj));
+
+    typedef bp::converter::rvalue_from_python_storage<std::vector<std::optional<T>>> storage_type;
+    void* storage = reinterpret_cast<storage_type*>(data)->storage.bytes;
+
+    typedef bp::stl_input_iterator<typename std::vector<std::optional<T>>::value_type> iterator;
+
+    new (storage) std::vector<std::optional<T>>(iterator(bp::object(handle)), iterator());
+    data->convertible = storage;
+  }
+
+  static void enroll() {
+    bp::to_python_converter<std::vector<std::optional<T>>, std_vector_converter<std::optional<T>>>();
+    bp::converter::registry::push_back(
+      &std_vector_converter<std::optional<T>>::convertible,
+      &std_vector_converter<std::optional<T>>::construct,
+      bp::type_id<std::vector<std::optional<T>>>()
+    );
+  }
+};
+
+template<typename T>
 struct std_optional_converter {
   static PyObject* convert(const std::optional<T>& value) {
     if (value) {
       return bp::incref(bp::object(*value).ptr());
     } else {
       return bp::incref(bp::object().ptr());
     }
@@ -147,14 +191,20 @@
 
   std_vector_converter<unsigned>::enroll();
   bp::class_<std::vector<unsigned>>("Iterable[uint]").def(bp::vector_indexing_suite<std::vector<unsigned>>());
 
   std_vector_converter<std::string>::enroll();
   bp::class_<std::vector<std::string>>("Iterable[str]").def(bp::vector_indexing_suite<std::vector<std::string>>());
 
+  std_vector_converter<std::optional<float>>::enroll();
+
+  std_vector_converter<std::optional<int>>::enroll();
+
+  std_vector_converter<std::optional<std::string>>::enroll();
+
   std_vector_converter<std::vector<unsigned>>::enroll();
 
   std_vector_converter<lincs::Category>::enroll();
   bp::class_<std::vector<lincs::Category>>("Iterable[Category]").def(bp::vector_indexing_suite<std::vector<lincs::Category>>());
 
   std_vector_converter<lincs::Criterion>::enroll();
   bp::class_<std::vector<lincs::Criterion>>("Iterable[Criterion]").def(bp::vector_indexing_suite<std::vector<lincs::Criterion>>());
@@ -179,20 +229,27 @@
 
   std_vector_converter<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy*>::enroll();
   bp::class_<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy*>>("Iterable[TerminationStrategy]").def(bp::vector_indexing_suite<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy*>>());
 
   std_vector_converter<lincs::LearnMrsortByWeightsProfilesBreed::Observer*>::enroll();
   bp::class_<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::Observer*>>("Iterable[Observer]").def(bp::vector_indexing_suite<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::Observer*>>());
 
-  bp::class_<std::mt19937>("UniformRandomBitsGenerator", "@todo(Documentation, v1.1) Add a docstring.", bp::no_init)
-    .def("__call__", &std::mt19937::operator(), "@todo(Documentation, v1.1) Add a docstring.")
+  bp::class_<std::mt19937>("UniformRandomBitsGenerator", "Random number generator.", bp::no_init)
+    .def(
+      "__call__",
+      &std::mt19937::operator(),
+      (bp::arg("self")),
+      "Generate the next pseudo-random integer."
+    )
   ;
   bp::class_<std::vector<std::mt19937>>("Iterable[UniformRandomBitsGenerator]").def(bp::vector_indexing_suite<std::vector<std::mt19937>>());
 
   std_optional_converter<float>::enroll();
+  std_optional_converter<int>::enroll();
+  std_optional_converter<std::string>::enroll();
   std_optional_converter<unsigned>::enroll();
 }
 
 }  // namespace lincs
 
 namespace {
 
@@ -231,14 +288,15 @@
 
  public:
   template<typename Class>
   static void visit(Class& cl) {
     cl
       .def("__len__", &len)
       .def("__getitem__", &getitem)
+      .def("__setitem__", &setitem)
     ;
   }
 
  private:
   static unsigned len(const Container& c) {
     return c.s0();
   }
@@ -246,14 +304,22 @@
   static T getitem(const Container& c, unsigned i) {
     if (i < 0 || i >= c.s0()) {
       PyErr_SetString(PyExc_IndexError, "index out of range");
       bp::throw_error_already_set();
     }
     return c[i];
   }
+
+  static void setitem(Container& c, unsigned i, T v) {
+    if (i < 0 || i >= c.s0()) {
+      PyErr_SetString(PyExc_IndexError, "index out of range");
+      bp::throw_error_already_set();
+    }
+    c[i] = v;
+  }
 };
 
 template<typename T>
 class HostArray2DIndexingSuite : public bp::def_visitor<HostArray2DIndexingSuite<T>> {
  private:
   typedef Array2D<Host, T> Container;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/liblincs-module/generation-functions.cpp` & `lincs-2.0.0a0/lincs/liblincs/liblincs-module/generation-functions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/liblincs-module/io-classes.cpp` & `lincs-2.0.0a0/lincs/liblincs/liblincs-module/io-classes.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
   };
 
   accepted_values_class.attr("RealThresholds") = bp::class_<lincs::AcceptedValues::RealThresholds>(
     "RealThresholds",
     "Descriptor for thresholds for an real-valued criterion.",
     bp::no_init
   )
-    .def(bp::init<const std::vector<float>&>(
+    .def(bp::init<const std::vector<std::optional<float>>&>(
       (bp::arg("self"), "thresholds"),
       "Parameters map exactly to attributes with identical names."
     ))
     .add_property("thresholds", bp::make_function(&lincs::AcceptedValues::RealThresholds::get_thresholds, bp::return_value_policy<bp::return_by_value>()), "The thresholds for this descriptor.")
     .def_pickle(RealThresholdsPickleSuite())
   ;
 
@@ -332,15 +332,15 @@
   };
 
   accepted_values_class.attr("IntegerThresholds") = bp::class_<lincs::AcceptedValues::IntegerThresholds>(
     "IntegerThresholds",
     "Descriptor for thresholds for an integer-valued criterion.",
     bp::no_init
   )
-    .def(bp::init<const std::vector<int>&>(
+    .def(bp::init<const std::vector<std::optional<int>>&>(
       (bp::arg("self"), "thresholds"),
       "Parameters map exactly to attributes with identical names."
     ))
     .add_property("thresholds", bp::make_function(&lincs::AcceptedValues::IntegerThresholds::get_thresholds, bp::return_value_policy<bp::return_by_value>()), "The thresholds for this descriptor.")
     .def_pickle(IntegerThresholdsPickleSuite())
   ;
 
@@ -351,15 +351,15 @@
   };
 
   accepted_values_class.attr("EnumeratedThresholds") = bp::class_<lincs::AcceptedValues::EnumeratedThresholds>(
     "EnumeratedThresholds",
     "Descriptor for thresholds for a criterion taking enumerated values.",
     bp::no_init
   )
-    .def(bp::init<const std::vector<std::string>&>(
+    .def(bp::init<const std::vector<std::optional<std::string>>&>(
       (bp::arg("self"), "thresholds"),
       "Parameters map exactly to attributes with identical names."
     ))
     .add_property("thresholds", bp::make_function(&lincs::AcceptedValues::EnumeratedThresholds::get_thresholds, bp::return_value_policy<bp::return_by_value>()), "The thresholds for this descriptor.")
     .def_pickle(EnumeratedThresholdsPickleSuite())
   ;
```

### Comparing `lincs-1.1.0a6/lincs/liblincs/liblincs-module/main.cpp` & `lincs-2.0.0a0/lincs/liblincs/liblincs-module/main.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-2.0.0a0/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/linear-programming/glop.cpp` & `lincs-2.0.0a0/lincs/liblincs/linear-programming/glop.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/linear-programming/glop.hpp` & `lincs-2.0.0a0/lincs/liblincs/linear-programming/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/linear-programming/test.cpp` & `lincs-2.0.0a0/lincs/liblincs/linear-programming/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/randomness-utils.cpp` & `lincs-2.0.0a0/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/randomness-utils.hpp` & `lincs-2.0.0a0/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/sat/eval-max-sat.hpp` & `lincs-2.0.0a0/lincs/liblincs/sat/eval-max-sat.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/sat/minisat.cpp` & `lincs-2.0.0a0/lincs/liblincs/sat/minisat.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/sat/minisat.hpp` & `lincs-2.0.0a0/lincs/liblincs/sat/minisat.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/sat/test.cpp` & `lincs-2.0.0a0/lincs/liblincs/sat/test.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/variant-dispatch.hpp` & `lincs-2.0.0a0/lincs/liblincs/variant-dispatch.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibinternal.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibinternal.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibinternal.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibinternal.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibmisc.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibmisc.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/alglibmisc.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/alglibmisc.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/ap.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/ap.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/ap.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/ap.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/dataanalysis.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/dataanalysis.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/dataanalysis.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/dataanalysis.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/diffequations.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/diffequations.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/diffequations.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/diffequations.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/fasttransforms.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/fasttransforms.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/fasttransforms.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/fasttransforms.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/integration.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/integration.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/integration.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/integration.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/interpolation.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/interpolation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/interpolation.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/interpolation.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_avx2.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_avx2.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_avx2.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_fma.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_fma.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_fma.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_fma.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_sse2.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/kernels_sse2.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/kernels_sse2.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/linalg.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/linalg.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/linalg.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/linalg.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/optimization.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/optimization.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/optimization.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/optimization.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/solvers.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/solvers.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/solvers.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/solvers.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/specialfunctions.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/specialfunctions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/specialfunctions.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/specialfunctions.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/statistics.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/statistics.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/alglib/statistics.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/alglib/statistics.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/doctest.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/doctest.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/analyze.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/analyze.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/arena.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/arena.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/arena.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/assume.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/assume.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/averages.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/averages.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/averages.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/backtrack.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/backtrack.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/backward.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/backward.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/block.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/block.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/block.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/block.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cadical.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/checker.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/checker.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/checker.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/clause.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/clause.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/clause.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/collect.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/collect.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/compact.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/compact.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/condition.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/condition.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/config.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/config.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/constrain.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/constrain.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/contract.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/contract.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/contract.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cover.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/cover.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/cover.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/decide.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/decide.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/decompose.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/decompose.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/deduplicate.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/deduplicate.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/elim.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/elim.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/elim.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ema.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ema.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/extend.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/extend.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/external.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/external.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/external.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/external.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/flags.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/flags.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/flags.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/format.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/format.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/format.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/format.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/gates.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/gates.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/heap.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/heap.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/instantiate.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/internal.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/internal.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/internal.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/inttypes.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/inttypes.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ipasir.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/level.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/level.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/limit.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/limit.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/limit.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/logging.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/logging.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/logging.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/lookahead.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/lookahead.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/lucky.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/lucky.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/message.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/message.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/message.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/message.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/minimize.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/minimize.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/observer.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/observer.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/occs.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/occs.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/occs.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/options.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/options.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/options.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/options.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/parse.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/parse.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/phases.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/phases.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/probe.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/probe.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/profile.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/profile.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/profile.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/propagate.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/propagate.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/queue.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/queue.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/queue.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/radix.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/radix.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/random.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/random.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/random.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/random.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/range.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/range.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/reduce.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/reduce.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/reluctant.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/reluctant.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/rephase.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/rephase.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/report.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/report.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/resources.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/resources.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/restart.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/restart.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/restore.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/restore.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/score.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/score.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/shrink.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/shrink.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/signal.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/signal.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/solution.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/solution.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/solver.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/solver.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/stats.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/stats.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/stats.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/subsume.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/ternary.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/ternary.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/tracer.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/transred.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/transred.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/util.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/util.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/util.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/util.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/var.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/var.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/version.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/version.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/vivify.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/walk.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/walk.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/watch.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadical/watch.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadical/watch.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cadicalinterface.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cadicalinterface.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/card_oe.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/card_oe.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/cardincremental.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/mcqd.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/mcqd.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualcard.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/eval-max-sat/virtualsat.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/lov-e.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/lov-e.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/magic_enum.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/magic_enum.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/Solver.cc` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/Solver.cc`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/Solver.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/Solver.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/core/SolverTypes.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/core/SolverTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Alg.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Alg.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Alloc.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Alloc.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Heap.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Heap.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/IntMap.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/IntMap.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/IntTypes.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Map.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Map.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Queue.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Queue.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Sort.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Sort.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/Vec.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/Vec.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/mtl/XAlloc.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/minisat/simp/SimpSolver.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/rapidcsv.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/rapidcsv.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/compat/optional.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/compat/optional.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/constraint.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/exceptions.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/adapter.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/debug.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/debug.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/json_reference.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/internal/uri.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/internal/uri.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/schema.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/schema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/schema_parser.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/schema_parser.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/subschema.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/subschema.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/utils/file_utils.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validation_results.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validation_results.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validation_visitor.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validation_visitor.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/valijson/validator.hpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/valijson/validator.hpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/binary.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/binary.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/binary.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/binary.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/collectionstack.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/collectionstack.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/convert.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/convert.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/depthguard.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/depthguard.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/directives.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/directives.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/dll.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/dll.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emit.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emit.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitfromevents.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitfromevents.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitfromevents.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitfromevents.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitter.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitter.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitter.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitter.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterdef.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterdef.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emittermanip.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emittermanip.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterstate.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterstate.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterstate.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterstate.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterutils.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterutils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/emitterutils.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/emitterutils.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/eventhandler.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/eventhandler.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exceptions.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exceptions.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exceptions.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exp.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exp.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/exp.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/exp.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/indentation.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/indentation.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/mark.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/mark.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/memory.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/memory.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/convert.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/convert.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/impl.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/impl.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator_fwd.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/iterator_fwd.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/memory.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/memory.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_data.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_data.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_iterator.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_iterator.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/detail/node_ref.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/detail/node_ref.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/emit.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/emit.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/impl.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/impl.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/iterator.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/iterator.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/node.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/node.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/parse.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/parse.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node/ptr.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node/ptr.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/node_data.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/node_data.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodebuilder.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodebuilder.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodebuilder.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodebuilder.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodeevents.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodeevents.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/nodeevents.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/nodeevents.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/noexcept.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/noexcept.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/null.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/null.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ostream_wrapper.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parse.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parse.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parser.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parser.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/parser.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/parser.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/ptr_vector.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/ptr_vector.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regex_yaml.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regex_yaml.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regex_yaml.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regex_yaml.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/regeximpl.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/regeximpl.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanner.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanner.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanner.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanner.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanscalar.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanscalar.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scanscalar.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scanscalar.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantag.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantag.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantag.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantag.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/scantoken.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/scantoken.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/setting.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/setting.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/simplekey.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/simplekey.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/singledocparser.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/singledocparser.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/singledocparser.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/singledocparser.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stlemitter.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stlemitter.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stream.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stream.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stream.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stream.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/streamcharsource.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/streamcharsource.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/stringsource.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/stringsource.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/tag.cpp` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/tag.cpp`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/tag.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/tag.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/token.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/token.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/traits.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/traits.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs/vendored/yaml-cpp/yaml.h` & `lincs-2.0.0a0/lincs/liblincs/vendored/yaml-cpp/yaml.h`

 * *Files identical despite different names*

### Comparing `lincs-1.1.0a6/lincs/liblincs_module_tests.py` & `lincs-2.0.0a0/lincs/liblincs_module_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2023-2024 Vincent Jacques
 
 import copy
+import io
 import pickle
+import textwrap
 import unittest
 import os
 
 from . import DataValidationException, LearningFailureException
 from .classification import *
 
 
@@ -1071,27 +1073,27 @@
 
         class MyWeightsOptimizationStrategy(LearnMrsortByWeightsProfilesBreed.WeightsOptimizationStrategy):
             def __init__(self, learning_data):
                 super().__init__()
                 self.strategy = OptimizeWeightsUsingGlop(learning_data)
                 self.called_count = 0
 
-            def optimize_weights(self):
+            def optimize_weights(self, begin, end):
                 self.called_count += 1
-                return self.strategy.optimize_weights()
+                return self.strategy.optimize_weights(begin, end)
 
         class MyProfilesImprovementStrategy(LearnMrsortByWeightsProfilesBreed.ProfilesImprovementStrategy):
             def __init__(self, learning_data):
                 super().__init__()
                 self.strategy = ImproveProfilesWithAccuracyHeuristicOnCpu(learning_data)
                 self.called_count = 0
 
-            def improve_profiles(self):
+            def improve_profiles(self, begin, end):
                 self.called_count += 1
-                return self.strategy.improve_profiles()
+                return self.strategy.improve_profiles(begin, end)
 
         class MyBreedingStrategy(LearnMrsortByWeightsProfilesBreed.BreedingStrategy):
             def __init__(self, learning_data, profiles_initialization_strategy, count):
                 super().__init__()
                 self.strategy = ReinitializeLeastAccurate(learning_data, profiles_initialization_strategy, count)
                 self.called_count = 0
 
@@ -1135,14 +1137,135 @@
         self.assertEqual(result.unchanged, 192)
 
         testing_set = generate_alternatives(problem, model, 1000, 44)
         result = classify_alternatives(problem, learned_model, testing_set)
         self.assertEqual(result.changed, 68)
         self.assertEqual(result.unchanged, 932)
 
+    def test_silly_strategies(self):
+        class SillyProfilesInitializationStrategy(LearnMrsortByWeightsProfilesBreed.ProfilesInitializationStrategy):
+            def __init__(self, log, learning_data):
+                super().__init__()
+                self.log = log
+                self.learning_data = learning_data
+
+            def initialize_profiles(self, model_indexes_begin, model_indexes_end):
+                self.log.append(("initialize_profiles", model_indexes_begin, model_indexes_end))
+                for model_index_index in range(model_indexes_begin, model_indexes_end):
+                    model_index = learning_data.model_indexes[model_index_index]
+                    for boundary_index in range(self.learning_data.boundaries_count):
+                        for criterion_index in range(self.learning_data.criteria_count):
+                            self.learning_data.profile_ranks[model_index][boundary_index][criterion_index] = 0
+
+        class SillyWeightsOptimizationStrategy(LearnMrsortByWeightsProfilesBreed.WeightsOptimizationStrategy):
+            def __init__(self, log, learning_data):
+                super().__init__()
+                self.log = log
+                self.learning_data = learning_data
+
+            def optimize_weights(self, model_indexes_begin, model_indexes_end):
+                self.log.append(("optimize_weights", model_indexes_begin, model_indexes_end))
+                for model_index_index in range(model_indexes_begin, model_indexes_end):
+                    model_index = learning_data.model_indexes[model_index_index]
+                    for criterion_index in range(self.learning_data.criteria_count):
+                        self.learning_data.weights[model_index][criterion_index] = 1.1 / self.learning_data.criteria_count
+
+        class SillyProfilesImprovementStrategy(LearnMrsortByWeightsProfilesBreed.ProfilesImprovementStrategy):
+            def __init__(self, log, learning_data):
+                super().__init__()
+                self.log = log
+                self.learning_data = learning_data
+
+            def improve_profiles(self, model_indexes_begin, model_indexes_end):
+                self.log.append(("improve_profiles", model_indexes_begin, model_indexes_end))
+                for model_index_index in range(model_indexes_begin, model_indexes_end):
+                    model_index = learning_data.model_indexes[model_index_index]
+                    for boundary_index in range(self.learning_data.boundaries_count):
+                        for criterion_index in range(self.learning_data.criteria_count):
+                            rank = (boundary_index + 1) * (self.learning_data.values_counts[criterion_index] // (self.learning_data.boundaries_count + 1))
+                            self.learning_data.profile_ranks[model_index][boundary_index][criterion_index] = rank
+
+        class SillyBreedingStrategy(LearnMrsortByWeightsProfilesBreed.BreedingStrategy):
+            def __init__(self, log, learning_data):
+                super().__init__()
+                self.log = log
+                self.learning_data = learning_data
+
+            def breed(self):
+                self.log.append(("breed",))
+
+        class SillyTerminationStrategy(LearnMrsortByWeightsProfilesBreed.TerminationStrategy):
+            def __init__(self, log, learning_data):
+                super().__init__()
+                self.log = log
+                self.learning_data = learning_data
+
+            def terminate(self):
+                self.log.append(("terminate",))
+                return self.learning_data.iteration_index == 3
+
+        problem = Problem(
+            [
+                Criterion("Criterion 1", Criterion.RealValues(Criterion.PreferenceDirection.decreasing, 0, 10)),
+                Criterion("Criterion 2", Criterion.IntegerValues(Criterion.PreferenceDirection.increasing, 0, 100)),
+                Criterion("Criterion 3", Criterion.EnumeratedValues(["F", "E", "D", "C", "B", "A"])),
+            ],
+            [Category("Bad"), Category("Medium"), Category("Good")],
+        )
+        learning_set = generate_alternatives(problem, generate_mrsort_model(problem, random_seed=42), alternatives_count=1000, random_seed=43)
+
+        log = []
+        learning_data = LearnMrsortByWeightsProfilesBreed.LearningData(problem, learning_set, models_count=9, random_seed=43)
+        profiles_initialization_strategy = SillyProfilesInitializationStrategy(log, learning_data)
+        weights_optimization_strategy = SillyWeightsOptimizationStrategy(log, learning_data)
+        profiles_improvement_strategy = SillyProfilesImprovementStrategy(log, learning_data)
+        breeding_strategy = SillyBreedingStrategy(log, learning_data)
+        termination_strategy = SillyTerminationStrategy(log, learning_data)
+
+        learned_model = LearnMrsortByWeightsProfilesBreed(
+            learning_data,
+            profiles_initialization_strategy,
+            weights_optimization_strategy,
+            profiles_improvement_strategy,
+            breeding_strategy,
+            termination_strategy,
+        ).perform()
+
+        self.assertEqual(log, [
+            ("initialize_profiles", 0, 9),
+            ("optimize_weights", 0, 9),
+            ("improve_profiles", 0, 9),
+            ("terminate",),
+            ("breed",),
+            ("optimize_weights", 0, 9),
+            ("improve_profiles", 0, 9),
+            ("terminate",),
+            ("breed",),
+            ("optimize_weights", 0, 9),
+            ("improve_profiles", 0, 9),
+            ("terminate",),
+            ("breed",),
+            ("optimize_weights", 0, 9),
+            ("improve_profiles", 0, 9),
+            ("terminate",),
+        ])
+
+        self.assertAlmostEqual(learned_model.accepted_values[0].real_thresholds.thresholds[0], 6.9493637)
+        self.assertAlmostEqual(learned_model.accepted_values[0].real_thresholds.thresholds[1], 3.2469211)
+        self.assertEqual(learned_model.accepted_values[1].integer_thresholds.thresholds[0], 33)
+        self.assertEqual(learned_model.accepted_values[1].integer_thresholds.thresholds[1], 66)
+        self.assertEqual(learned_model.accepted_values[2].enumerated_thresholds.thresholds[0], "D")
+        self.assertEqual(learned_model.accepted_values[2].enumerated_thresholds.thresholds[1], "B")
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[0].weights.criterion_weights[0], 1.1 / 3)
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[0].weights.criterion_weights[1], 1.1 / 3)
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[0].weights.criterion_weights[2], 1.1 / 3)
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[1].weights.criterion_weights[0], 1.1 / 3)
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[1].weights.criterion_weights[1], 1.1 / 3)
+        self.assertAlmostEqual(learned_model.sufficient_coalitions[1].weights.criterion_weights[2], 1.1 / 3)
+
     def test_observers(self):
         problem = generate_problem(5, 3, 41)
         model = generate_mrsort_model(problem, 42)
         learning_set = generate_alternatives(problem, model, 200, 43)
 
         class MyObserver(LearnMrsortByWeightsProfilesBreed.Observer):
             def __init__(self, learning_data):
@@ -1306,7 +1429,318 @@
         learning_set = generate_alternatives(problem, model, 100, 42)
         misclassify_alternatives(problem, learning_set, 10, 42 + 27)
 
         learning = LearnUcncsBySatByCoalitionsUsingMinisat(problem, learning_set)
 
         with self.assertRaises(LearningFailureException):
             learned_model = learning.perform()
+
+    def test_bug_found_by_laurent_cabaret_in_real_life_data(self):
+        # Previously, in (max-)SAT learning methods, when the SAT solver returned a solution where no value was accepted
+        # for a given criterion, we used the maximum value for that criterion (as configured in the problem) as the threshold.
+        # This was incorrect, and would in rare occasions cause the resulting model to classify alternatives in a higher
+        # category that expected. To solve this issue, we had to allow "unreachable thresholds", materialized by None in
+        # Python, and null in YAML. That change broke the public interface of the library, so it required releasing a
+        # major version.
+
+        problem = Problem.load(io.StringIO(textwrap.dedent("""\
+            kind: classification-problem
+            format_version: 1
+            criteria:
+              - name: a
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 1
+              - name: b
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 1
+              - name: c
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 1  # Setting to 2 improves accuracy. Why?
+              - name: d
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 1  # Setting to 2 improves accuracy. Why?
+              - name: e
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 4  # Setting to 5 improves accuracy. Why?
+              - name: f
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 15  # Setting to 16 improves accuracy. Why?
+              - name: g
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 15
+              - name: h
+                value_type: integer
+                preference_direction: increasing
+                min_value: 0
+                max_value: 10
+            ordered_categories:
+              - name: 4
+              - name: 3
+              - name: 2
+              - name: 1
+        """)))
+
+        learning_set = Alternatives.load(problem, io.StringIO(textwrap.dedent("""\
+            name,a,b,c,d,e,f,g,h,category
+            01,1,1,1,1,4,12,10,7,1
+            02,1,1,1,1,0,15,9,9,1
+            03,1,1,1,1,4,13,8,7,1
+            04,1,1,1,1,4,12,6,5,1
+            05,1,1,1,1,1,15,10,5,1
+            06,1,1,1,1,4,12,1,5,1
+            07,1,1,1,1,4,13,12,10,1
+            08,1,1,1,1,4,14,14,10,1
+            09,1,1,1,1,0,15,14,10,1
+            10,1,1,1,1,4,6,5,6,1
+            11,0,1,1,1,3,15,4,5,2
+            12,1,1,1,1,4,8,12,10,1
+            13,0,1,1,1,4,4,6,7,3
+            14,1,1,1,1,3,15,14,10,1
+            15,1,0,1,1,4,12,2,0,3
+            16,1,1,1,1,4,12,13,4,1
+            17,1,1,1,1,0,15,14,7,1
+            18,1,1,1,1,4,7,11,7,1
+            19,1,1,1,1,4,10,5,5,1
+            20,0,1,1,1,4,2,15,7,3
+            21,1,1,1,1,4,12,7,7,1
+            22,1,1,1,1,0,15,7,7,1
+            23,1,1,1,1,4,12,5,8,1
+            24,1,0,1,1,2,15,3,1,3
+            25,1,0,1,1,4,12,2,2,3
+            26,0,1,1,1,4,12,9,9,2
+            27,0,1,1,1,4,12,12,10,2
+            28,1,1,1,1,3,15,10,9,1
+            29,0,1,1,1,4,12,11,9,2
+            30,0,1,1,1,4,3,4,7,3
+            31,1,1,1,1,0,15,13,5,1
+            32,0,1,1,1,4,12,11,4,2
+            33,1,1,1,1,3,15,5,8,1
+            34,0,1,1,1,4,11,7,7,2
+            35,1,0,1,1,2,15,2,5,3
+            36,1,1,1,1,4,11,7,7,1
+            37,0,1,0,0,4,5,6,5,4
+            38,1,1,1,1,4,6,13,8,1
+            39,0,0,0,1,2,15,4,7,4
+            40,1,0,1,1,2,15,2,1,3
+            41,1,1,1,1,4,12,7,8,1
+            42,0,1,1,1,4,1,4,4,3
+            43,1,0,1,1,4,9,10,9,2
+            44,1,0,1,1,4,12,2,7,3
+            45,0,1,1,1,4,0,7,5,3
+            46,0,1,1,1,3,15,11,3,2
+            47,1,1,1,1,4,7,8,4,1
+            48,1,0,1,1,4,11,4,1,3
+            49,1,0,1,1,4,12,0,0,3
+            50,1,0,1,1,3,15,4,1,3
+        """)))
+
+        learning_data = LearnMrsortByWeightsProfilesBreed.LearningData(problem, learning_set, models_count=9, random_seed=43)
+        profiles_initialization_strategy = InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(learning_data)
+        weights_optimization_strategy = OptimizeWeightsUsingGlop(learning_data)
+        profiles_improvement_strategy = ImproveProfilesWithAccuracyHeuristicOnCpu(learning_data)
+        breeding_strategy = ReinitializeLeastAccurate(learning_data, profiles_initialization_strategy=profiles_initialization_strategy, count=4)
+        termination_strategy = TerminateAtAccuracy(learning_data, target_accuracy=len(learning_set.alternatives))
+        model = LearnMrsortByWeightsProfilesBreed(learning_data, profiles_initialization_strategy, weights_optimization_strategy, profiles_improvement_strategy, breeding_strategy, termination_strategy).perform()
+        model_dump = io.StringIO()
+        model.dump(problem, model_dump)
+        self.assertEqual(model_dump.getvalue(), textwrap.dedent("""\
+            kind: ncs-classification-model
+            format_version: 1
+            accepted_values:
+              - kind: thresholds
+                thresholds: [0, 1, 1]
+              - kind: thresholds
+                thresholds: [0, 1, 1]
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [3, 3, 4]
+              - kind: thresholds
+                thresholds: [5, 5, 14]
+              - kind: thresholds
+                thresholds: [3, 9, 9]
+              - kind: thresholds
+                thresholds: [0, 1, 5]
+            sufficient_coalitions:
+              - &coalitions
+                kind: weights
+                criterion_weights: [0.166666836, 0.333332658, 0.166666836, 0.166666836, 0.166666836, 0.166666836, 0.166665822, 0]
+              - *coalitions
+              - *coalitions
+        """))
+        learning_set_copy = copy.deepcopy(learning_set)
+        classification_result = classify_alternatives(problem, model, learning_set_copy)
+        self.assertEqual(classification_result.unchanged, 50)
+
+        model = LearnUcncsBySatBySeparationUsingMinisat(problem, learning_set).perform()
+        model_dump = io.StringIO()
+        model.dump(problem, model_dump)
+        self.assertEqual(model_dump.getvalue(), textwrap.dedent("""\
+            kind: ncs-classification-model
+            format_version: 1
+            accepted_values:
+              - kind: thresholds
+                thresholds: [0, 0, 1]
+              - kind: thresholds
+                thresholds: [0, 1, 1]
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [1, null, null]
+              - kind: thresholds
+                thresholds: [0, 3, 3]
+              - kind: thresholds
+                thresholds: [0, 6, 6]
+              - kind: thresholds
+                thresholds: [5, 5, 5]
+              - kind: thresholds
+                thresholds: [0, 8, 10]
+            sufficient_coalitions:
+              - &coalitions
+                kind: roots
+                upset_roots:
+                  - [0, 1, 2, 4, 5]
+                  - [0, 1, 2, 5, 6]
+                  - [0, 2, 4, 5, 6, 7]
+              - *coalitions
+              - *coalitions
+        """))
+        learning_set_copy = copy.deepcopy(learning_set)
+        classification_result = classify_alternatives(problem, model, learning_set_copy)
+        self.assertEqual(classification_result.unchanged, 50)
+
+        model = LearnUcncsBySatByCoalitionsUsingMinisat(problem, learning_set).perform()
+        model_dump = io.StringIO()
+        model.dump(problem, model_dump)
+        self.assertEqual(model_dump.getvalue(), textwrap.dedent("""\
+            kind: ncs-classification-model
+            format_version: 1
+            accepted_values:
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [0, 1, 1]
+              - kind: thresholds
+                thresholds: [1, null, null]
+              - kind: thresholds
+                thresholds: [1, 1, null]
+              - kind: thresholds
+                thresholds: [3, 3, null]
+              - kind: thresholds
+                thresholds: [6, 9, null]
+              - kind: thresholds
+                thresholds: [0, 4, 13]
+              - kind: thresholds
+                thresholds: [0, 8, null]
+            sufficient_coalitions:
+              - &coalitions
+                kind: roots
+                upset_roots:
+                  - [0, 1]
+                  - [1, 2, 6]
+                  - [1, 4, 5, 6]
+                  - [1, 2, 4, 5, 7]
+                  - [1, 3, 4, 6, 7]
+                  - [0, 3, 4, 5, 6, 7]
+              - *coalitions
+              - *coalitions
+        """))
+        learning_set_copy = copy.deepcopy(learning_set)
+        classification_result = classify_alternatives(problem, model, learning_set_copy)
+        self.assertEqual(classification_result.unchanged, 50)
+
+        model = LearnUcncsByMaxSatBySeparationUsingEvalmaxsat(problem, learning_set).perform()
+        model_dump = io.StringIO()
+        model.dump(problem, model_dump)
+        self.assertEqual(model_dump.getvalue(), textwrap.dedent("""\
+            kind: ncs-classification-model
+            format_version: 1
+            accepted_values:
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [0, 1, 1]
+              - kind: thresholds
+                thresholds: [1, 1, null]
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [0, 3, 4]
+              - kind: thresholds
+                thresholds: [0, 6, 10]
+              - kind: thresholds
+                thresholds: [0, 3, 8]
+              - kind: thresholds
+                thresholds: [0, 3, 4]
+            sufficient_coalitions:
+              - &coalitions
+                kind: roots
+                upset_roots:
+                  - [0, 1, 3, 4, 7]
+                  - [0, 1, 3, 5, 7]
+                  - [0, 2, 3, 4, 5, 6, 7]
+                  - [1, 2, 3, 4, 5, 6, 7]
+              - *coalitions
+              - *coalitions
+        """))
+        learning_set_copy = copy.deepcopy(learning_set)
+        classification_result = classify_alternatives(problem, model, learning_set_copy)
+        self.assertEqual(classification_result.unchanged, 50)
+
+        model = LearnUcncsByMaxSatByCoalitionsUsingEvalmaxsat(problem, learning_set).perform()
+        model_dump = io.StringIO()
+        model.dump(problem, model_dump)
+        self.assertEqual(model_dump.getvalue(), textwrap.dedent("""\
+            kind: ncs-classification-model
+            format_version: 1
+            accepted_values:
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [1, 1, 1]
+              - kind: thresholds
+                thresholds: [1, null, null]
+              - kind: thresholds
+                thresholds: [null, null, null]
+              - kind: thresholds
+                thresholds: [3, null, null]
+              - kind: thresholds
+                thresholds: [11, 11, null]
+              - kind: thresholds
+                thresholds: [7, null, null]
+              - kind: thresholds
+                thresholds: [8, 8, null]
+            sufficient_coalitions:
+              - &coalitions
+                kind: roots
+                upset_roots:
+                  - [0, 1]
+                  - [1, 2, 4]
+                  - [1, 3, 4]
+                  - [1, 5]
+                  - [2, 5]
+                  - [3, 5]
+                  - [4, 5]
+                  - [6]
+                  - [7]
+              - *coalitions
+              - *coalitions
+        """))
+        learning_set_copy = copy.deepcopy(learning_set)
+        classification_result = classify_alternatives(problem, model, learning_set_copy)
+        self.assertEqual(classification_result.unchanged, 50)
```

### Comparing `lincs-1.1.0a6/lincs/visualization.py` & `lincs-2.0.0a0/lincs/visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright 2023-2024 Vincent Jacques
 
 from typing import Iterable
 import unittest
 
-import matplotlib.pyplot as plt
+import matplotlib.pyplot
 
 from .classification import Problem, Model, Alternative
 
 
-def visualize_classification_model(problem: Problem, model: Model, alternatives: Iterable[Alternative], axes: plt.Axes):
+def visualize_classification_model(problem: Problem, model: Model, alternatives: Iterable[Alternative], axes: matplotlib.pyplot.Axes):
     """
     Create a visual representation of a classification model and classified alternatives, using Matplotlib.
     """
 
     # @todo(Feature, v1.2) Visualize single-peaked criteria.
     # See the possible solutions in e-mail "Visualisation des critères single-peaked" 2023-11-24
 
@@ -65,39 +65,39 @@
     unstacked_ys = [ys[0]]
     for ys1, ys2 in zip(ys[1:], ys[:-1]):
         unstacked_ys.append([y1 - y2 for y1, y2 in zip(ys1, ys2)])
     collections = axes.stackplot([0] + xs + [1], unstacked_ys, alpha=0.4)
     colors = [collection.get_facecolor()[0] for collection in collections]
 
     for (x, criterion) in zip(xs, problem.criteria):
-        secondary_ax = axes.secondary_yaxis(x)
+        criterion_axis = axes.secondary_yaxis(x)
         if criterion.is_real:
             values = criterion.real_values
-            ticks = [0, 0.5, 1]
-            labels = [f"{values.min_value:.1f}", f"{(values.min_value + values.max_value) / 2:.1f}", f"{values.max_value:.1f}"]
+            ticks = [0, 0.25, 0.5, 0.75, 1]
+            labels = [f"{values.min_value + tick * (values.max_value - values.min_value):.1f}" for tick in ticks]
             if values.is_increasing:
-                secondary_ax.set_yticks(ticks, labels)
+                criterion_axis.set_yticks(ticks, labels)
             else:
                 assert values.is_decreasing
-                secondary_ax.set_yticks(ticks, reversed(labels))
+                criterion_axis.set_yticks(ticks, reversed(labels))
         elif criterion.is_integer:
             values = criterion.integer_values
             labels = list(make_integer_labels(values.min_value, values.max_value))
             ticks = [(label - values.min_value) / (values.max_value - values.min_value) for label in labels]
             if values.is_increasing:
-                secondary_ax.set_yticks(ticks, labels)
+                criterion_axis.set_yticks(ticks, labels)
             else:
                 assert values.is_decreasing
-                secondary_ax.set_yticks(ticks, reversed(labels))
+                criterion_axis.set_yticks(ticks, reversed(labels))
         else:
             assert criterion.is_enumerated
             values = criterion.enumerated_values
             ticks_count = len(values.ordered_values)
             ticks = [n / (ticks_count - 1) for n in range(ticks_count)]
-            secondary_ax.set_yticks(ticks, values.ordered_values)
+            criterion_axis.set_yticks(ticks, values.ordered_values)
 
     for (category_index, category) in enumerate(problem.ordered_categories):
         if category_index == 0:
             low_y = 0
         else:
             low_y = normalize_value(problem.criteria[0], boundary_profiles[category_index - 1][0])
         if category_index == len(problem.ordered_categories) - 1:
@@ -145,19 +145,14 @@
     if intervals_count == 1:
         yield min_value
         yield max_value
     elif intervals_count == 2:
         yield min_value
         yield min_value + 1
         yield max_value
-    elif intervals_count == 3:
-        yield min_value
-        yield min_value + 1
-        yield min_value + 2
-        yield max_value
     elif intervals_count % 2 == 0:
         yield min_value
         yield min_value + intervals_count // 4
         yield (min_value + max_value) // 2
         yield max_value - intervals_count // 4
         yield max_value
     else:
```

### Comparing `lincs-1.1.0a6/lincs.egg-info/PKG-INFO` & `lincs-2.0.0a0/lincs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 1.1.0a6
+Version: 2.0.0a0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -15,30 +15,31 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.LESSER
 Requires-Dist: click~=8.1
-Requires-Dist: matplotlib~=3.5
+Requires-Dist: matplotlib~=3.7
+Requires-Dist: six~=1.16
 
 .. Copyright 2023-2024 Vincent Jacques
 
 .. This README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* (Learn and Infer Non Compensatory Sortings) is a collection of `MCDA <https://en.wikipedia.org/wiki/Multiple-criteria_decision_analysis>`_ algorithms, usable as a command-line utility and through a Python (3.8+) API.
 
 *lincs* supports Linux, macOS and Windows, with the exception that GPU-based algorithms are not available on macOS, because CUDA itself is not available there.
 On these 3 OSes, *lincs* only support x86_64 CPUs.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v1.1.0a6/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v1.1.0a6/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v2.0.0a0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v2.0.0a0/COPYING.LESSER>`_.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
 
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 You should probably take a look at `our roadmap <https://mics-lab.github.io/lincs/roadmap.html>`_ first.
@@ -88,15 +89,15 @@
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Versioning
 ==========
 
-Starting with version 1.0.0, *lincs* uses `semantic versioning <https://semver.org/>`_.
+*lincs* uses `semantic versioning <https://semver.org/>`_.
 
 *lincs*' public API (that "must be declared" according to SemVer) is constituted exclusively by its `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_,
 **at a code level**: we consider a change as backward compatible if the client code doesn't need to be modified to keep working,
 even if that change requires recompiling the client code in some cases.
 
 Future backward compatible changes might change *lincs*' behavior, especially with regards to pseudo-random behavior.
 
@@ -109,22 +110,22 @@
 
 Default values
 ^^^^^^^^^^^^^^
 
 Default values of optional arguments are not considered part of the public API.
 They might change in future releases if we find values that perform better for most use-cases.
 
-We advice you write your scripts in an explicit way where it matters to you,
+We advice you write your code in an explicit way where it matters to you,
 and rely on implicit default values only where you want the potential future improvements.
 
 File formats
 ^^^^^^^^^^^^
 
 The same specification applies to files read and produced by *lincs*.
-This leads to an issue about backward compatibility:
+This leads to an issue with regard to backward compatibility:
 if we allow more flexibility in input files, new versions of *lincs* will be able to read both the old and the new format, in a backward-compatible way.
 But if *lincs* produces a file in the new format, existing client scripts might not be able to read it, making this change backward-incompatible.
 
 To solve this issue, we impose an additional constraint to *lincs*' public API:
 *lincs* will produce files in a new format only when the client uses the new feature that motivated the new format.
 
 That way, we know that the client already needs to modify their scripts, so they can adapt to the new format.
```

### Comparing `lincs-1.1.0a6/lincs.egg-info/SOURCES.txt` & `lincs-2.0.0a0/lincs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 lincs/liblincs/lincs.hpp
 lincs/liblincs/randomness-utils.cpp
 lincs/liblincs/randomness-utils.hpp
 lincs/liblincs/unreachable.hpp
 lincs/liblincs/variant-dispatch.hpp
 lincs/liblincs/io/alternatives.cpp
 lincs/liblincs/io/alternatives.hpp
+lincs/liblincs/io/exception.cpp
+lincs/liblincs/io/exception.hpp
 lincs/liblincs/io/model.cpp
 lincs/liblincs/io/model.hpp
 lincs/liblincs/io/problem.cpp
 lincs/liblincs/io/problem.hpp
 lincs/liblincs/io/validation.cpp
 lincs/liblincs/io/validation.hpp
 lincs/liblincs/learning/exception.cpp
```

### Comparing `lincs-1.1.0a6/setup.py` & `lincs-2.0.0a0/setup.py`

 * *Files identical despite different names*

